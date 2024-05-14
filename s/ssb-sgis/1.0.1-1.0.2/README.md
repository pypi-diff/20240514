# Comparing `tmp/ssb_sgis-1.0.1.tar.gz` & `tmp/ssb_sgis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-1.0.1.tar", max compression
+gzip compressed data, was "ssb_sgis-1.0.2.tar", max compression
```

## Comparing `ssb_sgis-1.0.1.tar` & `ssb_sgis-1.0.2.tar`

### file list

```diff
@@ -1,63 +1,61 @@
--rw-r--r--   0        0        0     1074 2024-04-22 11:27:43.960336 ssb_sgis-1.0.1/LICENSE
--rw-r--r--   0        0        0     7557 2024-04-22 11:27:43.960336 ssb_sgis-1.0.1/README.md
--rw-r--r--   0        0        0     2743 2024-04-22 11:27:56.192429 ssb_sgis-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4018 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/__init__.py
--rw-r--r--   0        0        0      576 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0    22565 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/bounds.py
--rw-r--r--   0        0        0    17930 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    14142 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/centerlines.py
--rw-r--r--   0        0        0    23889 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/cleaning.py
--rw-r--r--   0        0        0    21903 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/conversion.py
--rw-r--r--   0        0        0    13124 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/duplicates.py
--rw-r--r--   0        0        0    24999 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0      691 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/geocoding.py
--rw-r--r--   0        0        0     7167 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    15895 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    23426 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6897 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    36718 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0    11184 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/polygons_as_rings.py
--rw-r--r--   0        0        0     8531 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/geopandas_tools/sfilter.py
--rw-r--r--   0        0        0     6190 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/helpers.py
--rw-r--r--   0        0        0      431 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/io/_is_dapla.py
--rw-r--r--   0        0        0     7987 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/io/dapla_functions.py
--rw-r--r--   0        0        0      610 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/io/opener.py
--rw-r--r--   0        0        0     3774 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/io/read_parquet.py
--rw-r--r--   0        0        0        0 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0     8110 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/examine.py
--rw-r--r--   0        0        0    30785 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1902 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20680 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    23688 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/map.py
--rw-r--r--   0        0        0    20331 2024-04-22 11:27:43.992336 ssb_sgis-1.0.1/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0     2733 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/maps/tilesources.py
--rw-r--r--   0        0        0        0 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6308 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2151 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     5336 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    13329 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    14267 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0    11217 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3370 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    67276 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12607 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6844 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0     5558 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/networkanalysis/traveling_salesman.py
--rw-r--r--   0        0        0    26997 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/parallel/parallel.py
--rw-r--r--   0        0        0        0 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/py.typed
--rw-r--r--   0        0        0        0 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/__init__.py
--rw-r--r--   0        0        0     1015 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/bands.py
--rw-r--r--   0        0        0      942 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/base.py
--rw-r--r--   0        0        0    34854 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/cube.py
--rw-r--r--   0        0        0      735 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/cubebase.py
--rw-r--r--   0        0        0     2352 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/gradient.py
--rw-r--r--   0        0        0     2782 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/indices.py
--rw-r--r--   0        0        0     2789 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/methods_as_functions.py
--rw-r--r--   0        0        0    45375 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/raster.py
--rw-r--r--   0        0        0     3898 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/torchgeo.py
--rw-r--r--   0        0        0     3259 2024-04-22 11:27:43.996336 ssb_sgis-1.0.1/src/sgis/raster/zonal.py
--rw-r--r--   0        0        0     9068 1970-01-01 00:00:00.000000 ssb_sgis-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/LICENSE
+-rw-r--r--   0        0        0     9387 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/README.md
+-rw-r--r--   0        0        0     7162 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6519 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/src/sgis/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/src/sgis/exceptions.py
+-rw-r--r--   0        0        0       28 2024-05-14 10:54:24.391094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0    23846 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/bounds.py
+-rw-r--r--   0        0        0    18303 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    14435 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/centerlines.py
+-rw-r--r--   0        0        0    23772 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/cleaning.py
+-rw-r--r--   0        0        0    24062 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/conversion.py
+-rw-r--r--   0        0        0    13596 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/duplicates.py
+-rw-r--r--   0        0        0    25944 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0      691 2024-05-14 10:54:14.855183 ssb_sgis-1.0.2/src/sgis/geopandas_tools/geocoding.py
+-rw-r--r--   0        0        0     7586 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    16363 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    25509 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6959 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    37224 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0    13558 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/polygons_as_rings.py
+-rw-r--r--   0        0        0     8653 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/geopandas_tools/sfilter.py
+-rw-r--r--   0        0        0     8294 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/helpers.py
+-rw-r--r--   0        0        0      431 2024-05-14 10:54:14.855183 ssb_sgis-1.0.2/src/sgis/io/_is_dapla.py
+-rw-r--r--   0        0        0     8807 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/io/dapla_functions.py
+-rw-r--r--   0        0        0      862 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/io/opener.py
+-rw-r--r--   0        0        0     3775 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/io/read_parquet.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:54:14.855183 ssb_sgis-1.0.2/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0     8708 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/examine.py
+-rw-r--r--   0        0        0    33284 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1982 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    24329 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    25234 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    20582 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14764 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0     2772 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/maps/tilesources.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:54:14.855183 ssb_sgis-1.0.2/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6368 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     3434 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4481 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     5385 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12093 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    15191 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0    11412 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3382 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7847 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    68444 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12955 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6863 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0     5654 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/networkanalysis/traveling_salesman.py
+-rw-r--r--   0        0        0    36002 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/parallel/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:54:14.859183 ssb_sgis-1.0.2/src/sgis/py.typed
+-rw-r--r--   0        0        0      175 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/__init__.py
+-rw-r--r--   0        0        0     1192 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/base.py
+-rw-r--r--   0        0        0    40419 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/cube.py
+-rw-r--r--   0        0        0      639 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/cubebase.py
+-rw-r--r--   0        0        0     2703 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/indices.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/methods_as_functions.py
+-rw-r--r--   0        0        0    53765 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/raster.py
+-rw-r--r--   0        0        0     4523 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/torchgeo.py
+-rw-r--r--   0        0        0     3862 2024-05-14 10:54:24.395094 ssb_sgis-1.0.2/src/sgis/raster/zonal.py
+-rw-r--r--   0        0        0    11780 1970-01-01 00:00:00.000000 ssb_sgis-1.0.2/PKG-INFO
```

### Comparing `ssb_sgis-1.0.1/LICENSE` & `ssb_sgis-1.0.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Statistics Norway
+Copyright © 2024 Statistics Norway
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ssb_sgis-1.0.1/README.md` & `ssb_sgis-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 # ssb-sgis
 
 GIS Python tools used in [Statistics Norway](https://www.ssb.no/en).
 
 See documentation [here](https://statisticsnorway.github.io/ssb-sgis/reference/index.html).
 
-[![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
+[![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][pypi status]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
-[![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
-[![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
+[![Documentation](https://github.com/statisticsnorway/ssb-sgis/actions/workflows/docs.yml/badge.svg)][documentation]
+[![Tests](https://github.com/statisticsnorway/ssb-sgis/actions/workflows/tests.yml/badge.svg)][tests]
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=coverage)][sonarcov]
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=alert_status)][sonarquality]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
-[pypi_]: https://pypi.org/project/ssb-sgis/
-[status]: https://pypi.org/project/ssb-sgis/
-[python version]: https://pypi.org/project/ssb-sgis
-[read the docs]: https://ssb-sgis.readthedocs.io/
+[pypi status]: https://pypi.org/project/ssb-sgis/
+[documentation]: https://statisticsnorway.github.io/ssb-sgis
 [tests]: https://github.com/statisticsnorway/ssb-sgis/actions?workflow=Tests
-[coverage]: https://sonarcloud.io/component_measures?metric=coverage&id=statisticsnorway_ssb-sgis
+[sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-sgis
+[sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-sgis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
+[poetry]: https://python-poetry.org/
 
 sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
 To install, use one of:
 
 ```shell
 poetry add ssb-sgis
 pip install ssb-sgis
 ```
 
+The sgis package has the following optional dependencies:
+
+- bucket: For working with files stored in GCP buckets
+- torch: Use functionality from PyTorch and torchgeo
+- xarray: Use functionality from xarray and rioxarray
+- test: Packages needed for running pytest
+- all: All optional dependencies
+
+The optional dependencies can be installed by adding them in
+brackets when installing, like this:
+
+```shell
+poetry add ssb-sgis[all]
+pip install ssb-sgis[all]
+```
+
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
 
@@ -160,15 +180,15 @@
 
 ### Dependencies
 
 [Poetry](https://python-poetry.org/) is used for dependency management. Install
 poetry and run the command below from the root directory to install the dependencies.
 
 ```shell
-poetry install --no-root
+poetry install -E test --no-root
 ```
 
 ### Tests
 
 Use the following command from the root directory to run the tests:
 
 ```shell
@@ -187,14 +207,22 @@
 poetry run jupter lab
 ```
 
 For VS Code there are extensions for opening a python script as Jupyter Notebook,
 for example:
 [Jupytext for Notebooks](https://marketplace.visualstudio.com/items?itemName=donjayamanne.vscode-jupytext).
 
+### Code quality
+
+Run 'ruff' on all files with safe fixes:
+
+```shell
+poetry run ruff check --fix .
+```
+
 ### Formatting
 
 Format the code with `black` and `isort` by running the following command from the
 root directory:
 
 ```shell
 poetry run black .
@@ -231,11 +259,37 @@
 
 To check and run the docstrings examples, run this command:
 
 ```shell
 poetry run xdoctest --command=all ./src/sgis
 ```
 
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_SSB sgis_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [Statistics Norway]'s [SSB PyPI Template].
+
+[statistics norway]: https://www.ssb.no/en
+[pypi]: https://pypi.org/
+[ssb pypi template]: https://github.com/statisticsnorway/ssb-pypitemplate
+[file an issue]: https://github.com/statisticsnorway/ssb-sgis/issues
+[pip]: https://pip.pypa.io/
+
 <!-- github-only -->
 
 [license]: https://github.com/statisticsnorway/ssb-sgis/blob/main/LICENSE
 [contributor guide]: https://github.com/statisticsnorway/ssb-sgis/blob/main/CONTRIBUTING.md
+[reference guide]: https://statisticsnorway.github.io/ssb-sgis/reference.html
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/bounds.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/bounds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import functools
-import numbers
-from collections.abc import Callable, Collection, Mapping
+from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
-from pandas.api.types import is_dict_like
-from shapely import Geometry, box, extract_unique_points
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from pyproj import CRS
+from shapely import Geometry
+from shapely import box
+from shapely import extract_unique_points
 from shapely.geometry import Polygon
 
 from ..parallel.parallel import Parallel
-from .conversion import to_bbox, to_gdf
-from .general import clean_clip, is_bbox_like
+from .conversion import to_bbox
+from .conversion import to_gdf
+from .general import clean_clip
+from .general import is_bbox_like
 
 
 @dataclass
 class Gridlooper:
     """Run functions in a loop cellwise based on a grid.
 
     Args:
@@ -28,29 +32,28 @@
             Defaults to 0.
         clip: If True (default) geometries are clipped by the grid cells.
             If False, all geometries that intersect will be selected in each iteration.
         verbose: Whether to print progress. Defaults to False.
         keep_geom_type: Whether to keep only the input geometry types after clipping.
             Defaults to True.
 
-    Examples
+    Examples:
     --------
-
     Get some points and some polygons.
 
     >>> import sgis as sg
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
     >>> points["idx"] = points.index
     >>> buffered = sg.buff(points, 100)
     >>> buffered
         idx                                           geometry
     0      0  POLYGON ((263222.700 6651184.900, 263222.651 6...
     1      1  POLYGON ((272556.100 6653369.500, 272556.051 6...
     2      2  POLYGON ((270182.300 6653032.700, 270182.251 6...
-    3      3  POLYGON ((259904.800 6650339.700, 259904.751 6...
+        3      3  POLYGON ((259904.800 6650339.700, 259904.751 6...
     4      4  POLYGON ((272976.200 6652889.100, 272976.151 6...
     ..   ...                                                ...
     995  995  POLYGON ((266901.700 6647844.500, 266901.651 6...
     996  996  POLYGON ((261374.000 6653593.400, 261373.951 6...
     997  997  POLYGON ((263642.900 6645427.000, 263642.851 6...
     998  998  POLYGON ((269326.700 6650628.000, 269326.651 6...
     999  999  POLYGON ((264670.300 6644239.500, 264670.251 6...
@@ -91,24 +94,32 @@
     gridbuffer: int = 0
     parallelizer: Parallel | None = None
     concat: bool = False
     clip: bool = True
     keep_geom_type: bool = True
     verbose: bool = False
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
+        """Fix types."""
         if not isinstance(self.mask, GeoDataFrame):
             self.mask = to_gdf(self.mask)
 
-    def run(self, func: Callable, *args, **kwargs):
-        def intersects_mask(df):
+    def run(self, func: Callable, *args, **kwargs) -> Any | list[Any]:
+        """Run a function for each grid cell in a loop.
+
+        Returns a list of the return values from the function,
+        or a (Geo)DataFrame if self.concat is True.
+
+        """
+
+        def _intersects_mask(df: GeoDataFrame) -> pd.Series:
             return df.index.isin(df.sjoin(self.mask).index)
 
         grid: GeoSeries = (
-            make_grid(self.mask, gridsize=self.gridsize).loc[intersects_mask].geometry
+            make_grid(self.mask, gridsize=self.gridsize).loc[_intersects_mask].geometry
         )
 
         n = len(grid)
 
         buffered_grid = grid.buffer(self.gridbuffer, resolution=1, join_style=2)
 
         if self.parallelizer is not None:
@@ -133,15 +144,17 @@
                     _clip_back_to_unbuffered_grid(
                         cell_res, unbuffered, self.keep_geom_type
                     )
                 )
             return out if not self.concat else pd.concat(out, ignore_index=True)
 
         results = []
-        for i, (unbuffered, buffered) in enumerate(zip(grid, buffered_grid)):
+        for i, (unbuffered, buffered) in enumerate(
+            zip(grid, buffered_grid, strict=False)
+        ):
             cell_kwargs = {
                 key: _clip_if_isinstance(
                     value, buffered, self.keep_geom_type, self.clip
                 )
                 for key, value in kwargs.items()
             }
             cell_args = tuple(
@@ -196,21 +209,24 @@
             Defaults to True.
         args: Positional arguments to pass to the function. Arguments
             of type GeoDataFrame or GeoSeries will be clipped by the grid cells in
             a loop.
         kwargs: Keyword arguments to pass to the function. Arguments
             of type GeoDataFrame or GeoSeries will be clipped by the grid cells in
             a loop.
+        parallelizer: Optional instance of sgis.Parallel, to run the function in parallel.
 
     Returns:
         List of results with the same length as number of grid cells.
 
-    Examples
-    --------
+    Raises:
+        TypeError: If args or kwargs has a wrong type
 
+    Examples:
+    --------
     Get some points and some polygons.
 
     >>> import sgis as sg
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
     >>> points["idx"] = points.index
     >>> buffered = sg.buff(points, 100)
     >>> buffered
@@ -270,16 +286,18 @@
         args = ()
     elif not isinstance(args, tuple):
         raise TypeError("args should be a tuple")
 
     if not isinstance(mask, GeoDataFrame):
         mask = to_gdf(mask)
 
-    intersects_mask = lambda df: df.index.isin(df.sjoin(mask).index)
-    grid: GeoSeries = make_grid(mask, gridsize=gridsize).loc[intersects_mask].geometry
+    def _intersects_mask(df: GeoDataFrame) -> pd.Series:
+        return df.index.isin(df.sjoin(mask).index)
+
+    grid: GeoSeries = make_grid(mask, gridsize=gridsize).loc[_intersects_mask].geometry
 
     n = len(grid)
 
     buffered_grid = grid.buffer(gridbuffer, resolution=1, join_style=2)
 
     if parallelizer is not None:
         func_with_clip = functools.partial(
@@ -297,15 +315,15 @@
         for cell_res, unbuffered in zip(results, grid, strict=True):
             out.append(
                 _clip_back_to_unbuffered_grid(cell_res, unbuffered, keep_geom_type)
             )
         return out
 
     results = []
-    for i, (unbuffered, buffered) in enumerate(zip(grid, buffered_grid)):
+    for i, (unbuffered, buffered) in enumerate(zip(grid, buffered_grid, strict=False)):
         cell_kwargs = {
             key: _clip_if_isinstance(value, buffered, keep_geom_type, clip)
             for key, value in kwargs.items()
         }
         cell_args = tuple(
             _clip_if_isinstance(value, buffered, keep_geom_type, clip) for value in args
         )
@@ -329,42 +347,46 @@
 def _clip_and_run_func(
     grid_cell: Polygon,
     func: Callable,
     args: tuple,
     kwargs: dict,
     keep_geom_type: bool,
     clip: bool,
-):
+) -> Any:
     cell_args = tuple(
         _clip_if_isinstance(value, grid_cell, keep_geom_type, clip) for value in args
     )
     cell_kwargs = {
         key: _clip_if_isinstance(value, grid_cell, keep_geom_type, clip)
         for key, value in kwargs.items()
     }
 
     return func(*cell_args, **cell_kwargs)
 
 
-def _clip_if_isinstance(value, cell, keep_geom_type, clip: bool):
-    if not isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
+def _clip_if_isinstance(
+    value: Any, cell: Geometry, keep_geom_type: bool, clip: bool
+) -> Any:
+    if not isinstance(value, (gpd.GeoDataFrame | gpd.GeoSeries | Geometry)):
         return value
 
-    if isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries)):
+    if isinstance(value, (gpd.GeoDataFrame | gpd.GeoSeries)):
         if clip:
             return clean_clip(value, cell, keep_geom_type=keep_geom_type)
         return value.loc[value.intersects(cell)]
 
     return value.intersection(cell).make_valid()
 
 
-def _clip_back_to_unbuffered_grid(results, mask, keep_geom_type):
-    if isinstance(results, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
+def _clip_back_to_unbuffered_grid(
+    results: Any, mask: GeoDataFrame, keep_geom_type: bool
+) -> Any:
+    if isinstance(results, (gpd.GeoDataFrame | gpd.GeoSeries | Geometry)):
         return _clip_if_isinstance(results, mask, keep_geom_type, clip=True)
-    elif isinstance(results, (pd.DataFrame, pd.Series, np.ndarray)):
+    elif isinstance(results, (pd.DataFrame | pd.Series | np.ndarray)):
         return results
     try:
         for key, value in results.items():
             results[key] = _clip_if_isinstance(value, mask, keep_geom_type, clip=True)
     except AttributeError:
         try:
             return [
@@ -379,15 +401,15 @@
 def make_grid_from_bbox(
     minx: int | float,
     miny: int | float,
     maxx: int | float,
     maxy: int | float,
     *_,
     gridsize: int | float,
-    crs,
+    crs: CRS | int | str,
 ) -> GeoDataFrame:
     """Creates a polygon grid from a bounding box.
 
     Creates a GeoDataFrame of grid cells of a given size within the given
     maxumum and mimimum x and y values.
 
     Args:
@@ -416,15 +438,15 @@
     return gpd.GeoDataFrame(grid_cells, columns=["geometry"], crs=crs)
 
 
 def make_grid(
     obj: GeoDataFrame | GeoSeries | Geometry | tuple,
     gridsize: int | float,
     *,
-    crs=None,
+    crs: CRS = None,
     clip_to_bounds: bool = False,
 ) -> GeoDataFrame:
     """Create a polygon grid around geometries.
 
     Creates a GeoDataFrame of grid cells of a given size around the bounds of
     a given GeoDataFrame. The corners are rounded to the nearest integer.
 
@@ -435,16 +457,19 @@
         crs: Coordinate reference system if 'obj' is not GeoDataFrame or GeoSeries.
         clip_to_bounds: Whether to clip the grid to the total bounds of the geometries.
             Defaults to False.
 
     Returns:
         GeoDataFrame with grid polygons.
 
+    Raises:
+        ValueError: crs can only be None if obj is GeoDataFrame/GeoSeries.
+
     """
-    if isinstance(obj, (GeoDataFrame, GeoSeries)):
+    if isinstance(obj, (GeoDataFrame | GeoSeries)):
         crs = obj.crs or crs
     elif not crs:
         raise ValueError(
             "'crs' cannot be None when 'obj' is not GeoDataFrame/GeoSeries."
         )
     if hasattr(obj, "__len__") and not len(obj):
         return GeoDataFrame({"geometry": []}, crs=crs)
@@ -471,22 +496,25 @@
     The GeoDataFrame must have 25833 as crs (UTM 33 N).
 
     Courtesy https://gis.stackexchange.com/questions/269243/creating-polygon-grid-using-geopandas
 
     Args:
         gdf: A GeoDataFrame.
         gridsize: Size of the grid in meters.
+        add: Number of grid cells to add on each side,
+            to make sure all data is covered by the grid.
 
     Returns:
         GeoDataFrame with grid geometries and a column 'SSBID'.
 
     Raises:
         ValueError: If the GeoDataFrame does not have 25833 as crs.
+        TypeError: if gdf has wrong type.
     """
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+    if not isinstance(gdf, (GeoDataFrame | GeoSeries)):
         raise TypeError("gdf must be GeoDataFrame og GeoSeries.")
 
     if not gdf.crs.equals(25833):
         raise ValueError(
             "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
             "projection or df.to_crs(25833) for transforming."
         )
@@ -547,14 +575,15 @@
     """Adds an SSB grid ID column to a GeoDataFrame of points.
 
     The GeoDataFrame must have 25833 as crs (UTM 33 N).
 
     Args:
         gdf: A GeoDataFrame.
         gridsize: Size of the grid in meters.
+        out_column: Name of column for the grid id.
 
     Returns:
         The input GeoDataFrame with a new grid id column.
 
     Raises:
         ValueError: If the GeoDataFrame does not have 25833 as crs.
     """
@@ -583,17 +612,17 @@
     Args:
         gdf: The GeoDataFrame.
         copy: Defaults to True.
 
     Returns:
         GeoDataFrame of box polygons with length and index of 'gdf'.
 
-    Examples
+    Examples:
     --------
-
+    >>> import sgis as sg
     >>> gdf = sg.to_gdf([MultiPoint([(0, 0), (1, 1)]), Point(0, 0)])
     >>> gdf
                                             geometry
     0  MULTIPOINT (0.00000 0.00000, 1.00000 1.00000)
     1                        POINT (0.00000 0.00000)
 
     >>> sg.bounds_to_polygon(gdf)
@@ -618,16 +647,17 @@
     Args:
         gdf: The GeoDataFrame.
         copy: Defaults to True.
 
     Returns:
         GeoDataFrame of multipoints with same length and index as 'gdf'.
 
-    Examples
+    Examples:
     --------
+    >>> import sgis as sg
     >>> gdf = sg.to_gdf([MultiPoint([(0, 0), (1, 1)]), Point(0, 0)])
     >>> gdf
                                             geometry
     0  MULTIPOINT (0.00000 0.00000, 1.00000 1.00000)
     1                        POINT (0.00000 0.00000)
 
     >>> sg.bounds_to_points(gdf)
@@ -639,27 +669,34 @@
     if isinstance(gdf, GeoSeries):
         return GeoSeries(extract_unique_points(as_bounds), index=gdf.index)
     gdf.geometry = extract_unique_points(as_bounds.geometry)
     return gdf
 
 
 def get_total_bounds(
-    *geometries: GeoDataFrame | GeoSeries | Geometry,
+    *geometries: GeoDataFrame | GeoSeries | Geometry, strict: bool = False
 ) -> tuple[float, float, float, float]:
     """Get a combined total bounds of multiple geometry objects."""
     xs, ys = [], []
     for obj in geometries:
-        minx, miny, maxx, maxy = to_bbox(obj)
+        try:
+            minx, miny, maxx, maxy = to_bbox(obj)
+        except Exception as e:
+            if strict:
+                raise e
+            else:
+                continue
         xs += [minx, maxx]
         ys += [miny, maxy]
     return min(xs), min(ys), max(xs), max(ys)
 
 
-def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int):
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)) and is_bbox_like(gdf):
+def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int) -> GeoDataFrame:
+    """Get a GeoDataFrame of points within the bounds of the GeoDataFrame."""
+    if not isinstance(gdf, (GeoDataFrame | GeoSeries)) and is_bbox_like(gdf):
         minx, miny, maxx, maxy = gdf
     else:
         minx, miny, maxx, maxy = gdf.total_bounds
     xs = np.linspace(minx, maxx, num=n2)
     ys = np.linspace(miny, maxy, num=n2)
     x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
     coords = np.concatenate((x_coords.reshape(-1, 1), y_coords.reshape(-1, 1)), axis=1)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 - If 'by' is not specified, the index will be labeled 0, 1, …, n - 1 after exploded, instead of 0, 0, …, 0 as it will with the geopandas defaults.
 
 - index_parts is set to False, which will be the default in a future version of geopandas.
 
 - The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
 """
 
-from typing import Callable
+from collections.abc import Callable
+from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 
-from .general import merge_geometries, parallel_unary_union
+from .general import _merge_geometries
+from .general import _parallel_unary_union
 from .geometry_types import make_all_singlepart
-from .polygon_operations import get_cluster_mapper, get_grouped_centroids
+from .polygon_operations import get_cluster_mapper
+from .polygon_operations import get_grouped_centroids
 
 
 def _decide_ignore_index(kwargs: dict) -> tuple[dict, bool]:
     if "ignore_index" in kwargs:
         ignore_index = kwargs.pop("ignore_index")
         return kwargs, ignore_index
 
@@ -61,14 +65,16 @@
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
         copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
+        grid_size: Rounding of the coordinates. Defaults to None.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
     """
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
@@ -105,20 +111,21 @@
         gdf: the GeoDataFrame that will be
             buffered and dissolved.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
         copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where geometries are dissolved.
 
-    Examples
+    Examples:
     --------
     Create some random points.
 
     >>> import sgis as sg
     >>> import numpy as np
     >>> points = sg.read_parquet_url(
     ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
@@ -163,15 +170,21 @@
     2     d  MULTIPOLYGON (((258180.258 6647935.731, 258179...  0.580157
     """
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
 
     return _dissolve(buffered, n_jobs=n_jobs, **dissolve_kwargs)
 
 
-def _dissolve(gdf, aggfunc="first", grid_size=None, n_jobs=1, **dissolve_kwargs):
+def _dissolve(
+    gdf: GeoDataFrame,
+    aggfunc: str = "first",
+    grid_size: None | float = None,
+    n_jobs: int = 1,
+    **dissolve_kwargs,
+) -> GeoDataFrame:
 
     if not len(gdf):
         return gdf
 
     geom_col = gdf._geometry_column_name
 
     by = dissolve_kwargs.pop("by", None)
@@ -216,25 +229,25 @@
 
     dissolved = many_hits.groupby(by, **dissolve_kwargs)[other_cols].agg(aggfunc)
 
     # dissolved = gdf.groupby(by, **dissolve_kwargs)[other_cols].agg(aggfunc)
 
     if n_jobs > 1:
         try:
-            agged = parallel_unary_union(
+            agged = _parallel_unary_union(
                 many_hits, n_jobs=n_jobs, by=by, grid_size=grid_size, **dissolve_kwargs
             )
             dissolved[geom_col] = agged
             return GeoDataFrame(dissolved, geometry=geom_col, crs=gdf.crs)
         except Exception as e:
             print(e, dissolved, agged, many_hits)
             raise e
 
     geoms_agged = many_hits.groupby(by, **dissolve_kwargs)[geom_col].agg(
-        lambda x: merge_geometries(x, grid_size=grid_size)
+        lambda x: _merge_geometries(x, grid_size=grid_size)
     )
 
     if not dissolve_kwargs.get("as_index"):
         try:
             geoms_agged = geoms_agged[geom_col]
         except KeyError:
             pass
@@ -244,31 +257,33 @@
     return GeoDataFrame(
         pd.concat([dissolved, one_hit]).sort_index(), geometry=geom_col, crs=gdf.crs
     )
 
 
 def diss(
     gdf: GeoDataFrame,
-    by=None,
-    aggfunc="first",
+    by: str | Sequence[str] | None = None,
+    aggfunc: str | Callable | dict[str, str | Callable] = "first",
     as_index: bool = True,
     grid_size: float | int | None = None,
     n_jobs: int = 1,
     **dissolve_kwargs,
-):
+) -> GeoDataFrame:
     """Dissolves geometries.
 
     It takes a GeoDataFrame and dissolves and fixes geometries.
 
     Args:
         gdf: the GeoDataFrame that will be dissolved and exploded.
         by: Columns to dissolve by.
         aggfunc: How to aggregate the non-geometry colums not in "by".
         as_index: Whether the 'by' columns should be returned as index. Defaults to
             True to be consistent with geopandas.
+        grid_size: Rounding of the coordinates. Defaults to None.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame with dissolved geometries.
     """
     if not len(gdf):
         if as_index:
@@ -288,34 +303,36 @@
         as_index=as_index,
         **dissolve_kwargs,
     )
 
 
 def dissexp(
     gdf: GeoDataFrame,
-    by=None,
-    aggfunc="first",
+    by: str | Sequence[str] | None = None,
+    aggfunc: str | Callable | dict[str, str | Callable] = "first",
     as_index: bool = True,
     index_parts: bool = False,
     grid_size: float | int | None = None,
     n_jobs: int = 1,
     **dissolve_kwargs,
-):
+) -> GeoDataFrame:
     """Dissolves overlapping geometries.
 
     It takes a GeoDataFrame and dissolves, fixes and explodes geometries.
 
     Args:
         gdf: the GeoDataFrame that will be dissolved and exploded.
         by: Columns to dissolve by.
         aggfunc: How to aggregate the non-geometry colums not in "by".
         as_index: Whether the 'by' columns should be returned as index. Defaults to
             True to be consistent with geopandas.
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
+        grid_size: Rounding of the coordinates. Defaults to None.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
     dissolve_kwargs = dissolve_kwargs | {
         "by": by,
@@ -330,28 +347,30 @@
 
     return make_all_singlepart(
         dissolved, ignore_index=ignore_index, index_parts=index_parts
     )
 
 
 def dissexp_by_cluster(
-    gdf: GeoDataFrame, predicate=None, n_jobs: int = 1, **dissolve_kwargs
+    gdf: GeoDataFrame, predicate: str | None = None, n_jobs: int = 1, **dissolve_kwargs
 ) -> GeoDataFrame:
     """Dissolves overlapping geometries through clustering with sjoin and networkx.
 
     Works exactly like dissexp, but, before dissolving, the geometries are divided
     into clusters based on overlap (uses the function sgis.get_polygon_clusters).
     The geometries are then dissolved based on this column (and optionally other
     columns).
 
     This might be many times faster than a regular dissexp, if there are many
     non-overlapping geometries.
 
     Args:
         gdf: the GeoDataFrame that will be dissolved and exploded.
+        predicate: Spatial predicate to use.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
     return _run_func_by_cluster(
         dissexp, gdf, predicate=predicate, n_jobs=n_jobs, **dissolve_kwargs
@@ -369,48 +388,33 @@
     columns).
 
     This might be many times faster than a regular dissexp, if there are many
     non-overlapping geometries.
 
     Args:
         gdf: the GeoDataFrame that will be dissolved and exploded.
+        predicate: Spatial predicate to use.
+        n_jobs: Number of threads to use. Defaults to 1.
         **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
     return _run_func_by_cluster(
         diss, gdf, predicate=predicate, n_jobs=n_jobs, **dissolve_kwargs
     )
 
 
 def _run_func_by_cluster(
     func: Callable,
     gdf: GeoDataFrame,
-    predicate=None,
+    predicate: str | None = None,
     n_jobs: int = 1,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
-    """Dissolves overlapping geometries through clustering with sjoin and networkx.
-
-    Works exactly like dissexp, but, before dissolving, the geometries are divided
-    into clusters based on overlap (uses the function sgis.get_polygon_clusters).
-    The geometries are then dissolved based on this column (and optionally other
-    columns).
-
-    This might be many times faster than a regular dissexp, if there are many
-    non-overlapping geometries.
-
-    Args:
-        gdf: the GeoDataFrame that will be dissolved and exploded.
-        **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
-
-    Returns:
-        A GeoDataFrame where overlapping geometries are dissolved.
-    """
     is_geoseries = isinstance(gdf, GeoSeries)
 
     by = dissolve_kwargs.pop("by", [])
     if isinstance(by, str):
         by = [by]
     elif by:
         by = list(by)
@@ -473,14 +477,15 @@
     Args:
         gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
         copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
+        n_jobs: int = 1,
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
     """
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
     return dissexp_by_cluster(buffered, n_jobs=n_jobs, **dissolve_kwargs)
@@ -503,15 +508,14 @@
             Here defaults to 50, as opposed to the default 16 in geopandas.
         copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
         **buffer_kwargs: additional keyword arguments passed to geopandas' buffer.
 
     Returns:
         A buffered GeoDataFrame.
     """
-
     if isinstance(gdf, GeoSeries):
         return gdf.buffer(distance, resolution=resolution, **buffer_kwargs).make_valid()
 
     if copy:
         gdf = gdf.copy()
 
     gdf[gdf._geometry_column_name] = gdf.buffer(
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/centerlines.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/centerlines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import functools
+import itertools
 import warnings
 
 import numpy as np
 import pandas as pd
 import shapely
-from geopandas import GeoDataFrame, GeoSeries
-from geopandas.array import GeometryArray
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from numpy.typing import NDArray
-from shapely import (
-    STRtree,
-    distance,
-    extract_unique_points,
-    get_parts,
-    get_rings,
-    line_merge,
-    make_valid,
-    segmentize,
-    unary_union,
-    voronoi_polygons,
-)
+from shapely import STRtree
+from shapely import distance
+from shapely import extract_unique_points
+from shapely import get_rings
+from shapely import line_merge
+from shapely import make_valid
+from shapely import segmentize
+from shapely import unary_union
+from shapely import voronoi_polygons
 from shapely.errors import GEOSException
 from shapely.geometry import LineString
 from shapely.ops import nearest_points
 
-from ..maps.maps import explore, explore_locals
+from ..maps.maps import explore
 from ..networkanalysis.traveling_salesman import traveling_salesman_problem
-from .conversion import to_gdf, to_geoseries
-from .general import clean_geoms, make_lines_between_points, sort_long_first
+from .conversion import to_gdf
+from .conversion import to_geoseries
+from .general import clean_geoms
+from .general import make_lines_between_points
+from .general import sort_long_first
 from .geometry_types import make_all_singlepart
-from .sfilter import sfilter_inverse, sfilter_split
-
+from .sfilter import sfilter_inverse
+from .sfilter import sfilter_split
 
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
-def get_traveling_salesman_lines(df, return_to_start=False):
+def get_traveling_salesman_lines(
+    df: GeoDataFrame, return_to_start: bool = False
+) -> list[LineString]:
     path = traveling_salesman_problem(df, return_to_start=return_to_start)
 
     try:
-        return [LineString([p1, p2]) for p1, p2 in zip(path[:-1], path[1:])]
+        return [LineString([p1, p2]) for p1, p2 in itertools.pairwise(path)]
     except IndexError as e:
         if len(path) == 1:
             return path
         raise e
 
 
-def remove_longest_if_not_intersecting(centerlines, geoms):
+def _remove_longest_if_not_intersecting(
+    centerlines: GeoDataFrame, geoms: GeoDataFrame
+) -> GeoDataFrame:
     centerlines = sort_long_first(make_all_singlepart(centerlines))
 
     has_only_one_line = centerlines.groupby(level=0).size() == 1
     only_one_line = centerlines[has_only_one_line]
     centerlines = centerlines[~has_only_one_line]
 
     longest = centerlines.loc[lambda x: ~x.index.duplicated()]
@@ -79,33 +84,32 @@
     should start and end at the polygons' "endpoints".
 
     The function is meant for getting centerlines from slivers in coverage_clean and
     snap_polygons. It will give weird results and be extremely slow for
     complext polygons like (buffered) road networks.
 
     """
-
-    PRECISION = 0.01
+    precision = 0.01
 
     if not len(gdf):
         return gdf
 
     if not gdf.index.is_unique:
         raise ValueError("Index must be unique")
 
     geoms: GeoSeries = to_geoseries(gdf).explode(index_parts=False)
 
     segmentized: GeoSeries = segmentize(geoms, max_segment_length=max_segment_length)
 
-    points: GeoSeries = get_points_in_polygons(segmentized, PRECISION)
+    points: GeoSeries = _get_points_in_polygons(segmentized, precision)
 
     has_no_points = geoms.loc[(~geoms.index.isin(points.index))]
 
-    more_points: GeoSeries = get_points_in_polygons(
-        has_no_points.buffer(PRECISION), PRECISION
+    more_points: GeoSeries = _get_points_in_polygons(
+        has_no_points.buffer(precision), precision
     )
 
     # Geometries that have no lines inside, might be perfect circles.
     # These can get the centroid as centerline
     still_has_no_points = has_no_points.loc[
         (~has_no_points.index.isin(more_points.index))
     ]
@@ -127,15 +131,15 @@
         )
     else:
         segmentized = segmentized.loc[
             ~segmentized.index.isin(still_has_no_points.index)
         ]
 
     # make sure to include the endpoints
-    endpoints = get_approximate_polygon_endpoints(segmentized)
+    endpoints = _get_approximate_polygon_endpoints(segmentized)
 
     geoms = geoms.loc[~geoms.index.isin(still_has_no_points.index)]
 
     # check if line between endpoints make up a decent centerline
     has_two = endpoints.groupby(level=0).size() == 2
     endpoint1 = endpoints.loc[has_two].groupby(level=0).first()
     endpoint2 = endpoints.loc[has_two].groupby(level=0).last()
@@ -144,24 +148,24 @@
     end_to_end = GeoSeries(
         make_lines_between_points(endpoint1, endpoint2), index=endpoint1.index
     )
 
     # keep lines 90 percent intersecting the polygon
     length_now = end_to_end.length
     end_to_end = (
-        end_to_end.intersection(geoms.buffer(PRECISION))
+        end_to_end.intersection(geoms.buffer(precision))
         .dropna()
         .loc[lambda x: x.length > length_now * 0.9]
     )
 
     # straight end buffer to remove all in between ends
     to_be_erased = points.index.isin(end_to_end.index)
 
     dont_intersect = sfilter_inverse(
-        points.iloc[to_be_erased], end_to_end.buffer(PRECISION, cap_style=2)
+        points.iloc[to_be_erased], end_to_end.buffer(precision, cap_style=2)
     )
 
     points = (
         clean_geoms(
             pd.concat(
                 [
                     points.iloc[~to_be_erased],
@@ -180,15 +184,15 @@
             points,
             endpoints,
         ]
     )
 
     explore(points=to_gdf(points, 25833), gdf=gdf)
 
-    remove_longest = functools.partial(remove_longest_if_not_intersecting, geoms=geoms)
+    remove_longest = functools.partial(_remove_longest_if_not_intersecting, geoms=geoms)
 
     centerlines = GeoSeries(
         points.groupby(level=0).apply(get_traveling_salesman_lines).explode()
     ).pipe(remove_longest)
 
     # centerlines = sort_long_first(centerlines).loc[lambda x: x.index.duplicated()]
 
@@ -231,15 +235,15 @@
 
     centerlines = GeoDataFrame(
         {"geometry": pd.concat([centerlines, still_has_no_points])}, crs=gdf.crs
     )
     return centerlines
 
 
-def get_points_in_polygons(geometries: GeoSeries, precision: float) -> GeoSeries:
+def _get_points_in_polygons(geometries: GeoSeries, precision: float) -> GeoSeries:
     # voronoi can cause problems if coordinates are nearly identical
     # buffering solves it
     try:
         voronoi_lines = voronoi_polygons(geometries, only_edges=True)
     except GEOSException:
         try:
             geometries = make_valid(geometries)
@@ -263,15 +267,15 @@
         == "MultiPoint"
     )
     not_within_but_relevant = not_within.loc[intersect_polys_at_two_places]
 
     return pd.concat([within_polygons, not_within_but_relevant]).centroid
 
 
-def get_approximate_polygon_endpoints(geoms: GeoSeries) -> GeoSeries:
+def _get_approximate_polygon_endpoints(geoms: GeoSeries) -> GeoSeries:
     out_geoms = []
 
     are_thin = geoms.buffer(-1e-2).is_empty
     not_thin = geoms.loc[~are_thin]
     thin = geoms.loc[are_thin].buffer(1e-2)
 
     rectangles = pd.concat([not_thin, thin]).minimum_rotated_rectangle()
@@ -328,15 +332,15 @@
         )
 
         nearest_rectangle_points = nearest_points(by_rectangle, rectangles)[1]
         nearest_geom_points = nearest_points(nearest_rectangle_points, geoms)[1]
 
         out_geoms.append(nearest_geom_points)
 
-    lines_around_geometries = multipoints_to_line_segments(
+    lines_around_geometries = _multipoints_to_line_segments(
         extract_unique_points(rectangles)
     )
 
     distance_to_rect = distance(
         two_nearest.values, rectangles.loc[two_nearest.index].values
     )
 
@@ -366,83 +370,88 @@
             index=to_be_moved.index,
         )
         out_geoms.append(points_moved)
 
     return pd.concat(out_geoms)
 
 
-def multipoints_to_line_segments(
+def _multipoints_to_line_segments(
     multipoints: GeoSeries | GeoDataFrame, to_next: bool = True, cycle: bool = True
 ) -> GeoSeries | GeoDataFrame:
     if not len(multipoints):
         return multipoints
 
     multipoints = to_geoseries(multipoints)
 
     if isinstance(multipoints.index, pd.MultiIndex):
         index = [
             multipoints.index.get_level_values(i)
             for i in range(multipoints.index.nlevels)
         ]
         multipoints.index = pd.MultiIndex.from_arrays(
-            [list(range(len(multipoints)))] + index,
-            names=["range_idx"] + multipoints.index.names,
+            [list(range(len(multipoints))), *index],
+            names=["range_idx", *multipoints.index.names],
         )
     else:
         multipoints.index = pd.MultiIndex.from_arrays(
             [np.arange(0, len(multipoints)), multipoints.index],
-            names=["range_idx"] + [multipoints.index.name],
+            names=["range_idx", multipoints.index.name],
         )
 
     try:
         crs = multipoints.crs
     except AttributeError:
         crs = None
 
     point_df = multipoints.explode(index_parts=False).to_frame("geometry")
 
     if to_next:
         shift = -1
-        filt = lambda x: ~x.index.get_level_values(0).duplicated(keep="first")
+        keep = "first"
     else:
         shift = 1
-        filt = lambda x: ~x.index.get_level_values(0).duplicated(keep="last")
+        keep = "last"
 
     point_df["next"] = point_df.groupby(level=0)["geometry"].shift(shift)
 
     if cycle:
-        first_points = point_df.loc[filt, "geometry"]
+        first_points: GeoSeries = point_df.loc[
+            lambda x: ~x.index.get_level_values(0).duplicated(keep=keep), "geometry"
+        ]
         is_last_point = point_df["next"].isna()
 
         point_df.loc[is_last_point, "next"] = first_points
         assert point_df["next"].notna().all()
     else:
         point_df = point_df[point_df["next"].notna()]
 
     point_df["geometry"] = [
-        LineString([x1, x2]) for x1, x2 in zip(point_df["geometry"], point_df["next"])
+        LineString([x1, x2])
+        for x1, x2 in zip(point_df["geometry"], point_df["next"], strict=False)
     ]
     if isinstance(multipoints.index, pd.MultiIndex):
         point_df.index = point_df.index.droplevel(0)
 
     if isinstance(multipoints, GeoDataFrame):
         return GeoDataFrame(
             point_df.drop(columns=["next"]), geometry="geometry", crs=crs
         )
     return GeoSeries(point_df["geometry"], crs=crs)
 
 
-def get_line_segments(lines, extract_unique: bool = False, cycle=False) -> GeoDataFrame:
+def get_line_segments(
+    lines: GeoDataFrame | GeoSeries, extract_unique: bool = False, cycle=False
+) -> GeoDataFrame:
     try:
         assert lines.index.is_unique
     except AttributeError:
         pass
 
     lines = to_geoseries(lines)
 
     if extract_unique:
         points = extract_unique_points(lines.values)
     else:
         coords, indices = shapely.get_coordinates(lines, return_index=True)
         points = GeoSeries(shapely.points(coords), index=indices)
 
-    return multipoints_to_line_segments(points, cycle=cycle)
+    return _multipoints_to_line_segments(points, cycle=cycle)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/cleaning.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/cleaning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,61 @@
 import re
 import warnings
-from typing import Callable
+from collections.abc import Callable
+from typing import Any
 
-import networkx as nx
 import numpy as np
 import pandas as pd
 import shapely
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from geopandas.array import GeometryArray
 from numpy.typing import NDArray
-from shapely import (
-    Geometry,
-    STRtree,
-    extract_unique_points,
-    force_2d,
-    get_coordinates,
-    get_exterior_ring,
-    get_parts,
-    linearrings,
-    linestrings,
-    make_valid,
-    multipoints,
-    polygons,
-    reverse,
-    segmentize,
-    simplify,
-    unary_union,
-)
+from shapely import extract_unique_points
+from shapely import get_coordinates
+from shapely import get_parts
+from shapely import linestrings
 from shapely.errors import GEOSException
-from shapely.geometry import LinearRing, LineString, MultiLineString, MultiPoint, Point
-from shapely.ops import nearest_points
+from shapely.geometry import LineString
+from shapely.geometry import Point
 
-from ..networkanalysis.closing_network_holes import get_angle
-from ..networkanalysis.cutting_lines import split_lines_by_nearest_point
-from .buffer_dissolve_explode import buff, buffdissexp, dissexp, dissexp_by_cluster
-from .conversion import coordinate_array, to_gdf, to_geoseries
-from .duplicates import get_intersections, update_geometries
+from .buffer_dissolve_explode import buff
+from .buffer_dissolve_explode import dissexp
+from .conversion import coordinate_array
+from .conversion import to_gdf
+from .duplicates import get_intersections
+from .duplicates import update_geometries
 
 # from .general import sort_large_first as _sort_large_first
-from .general import (
-    clean_clip,
-    clean_geoms,
-    sort_large_first,
-    sort_long_first,
-    sort_small_first,
-    to_lines,
-)
-from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
-from .neighbors import get_k_nearest_neighbors, get_neighbor_indices
+from .general import clean_geoms
+from .general import sort_large_first
+from .general import sort_small_first
+from .general import to_lines
+from .geometry_types import make_all_singlepart
+from .geometry_types import to_single_geom_type
 from .overlay import clean_overlay
-from .polygon_operations import (
-    close_all_holes,
-    close_small_holes,
-    close_thin_holes,
-    eliminate_by_longest,
-    get_cluster_mapper,
-    get_gaps,
-)
-from .polygons_as_rings import PolygonsAsRings
-from .sfilter import sfilter, sfilter_inverse, sfilter_split
-
+from .polygon_operations import eliminate_by_longest
+from .polygon_operations import get_cluster_mapper
+from .polygon_operations import get_gaps
+from .sfilter import sfilter_inverse
+from .sfilter import sfilter_split
 
 warnings.simplefilter(action="ignore", category=UserWarning)
 warnings.simplefilter(action="ignore", category=RuntimeWarning)
 
 
 PRECISION = 1e-3
 BUFFER_RES = 50
 
 
 def coverage_clean(
     gdf: GeoDataFrame,
     tolerance: int | float,
     duplicate_action: str = "fix",
     grid_sizes: tuple[None | int] = (None,),
-    logger=None,
-    mask=None,
     n_jobs: int = 1,
 ) -> GeoDataFrame:
     """Fix thin gaps, holes, slivers and double surfaces.
 
     The operations might raise GEOSExceptions, so it might be nessecary to set
     the 'grid_sizes' argument, it might also be a good idea to run coverage_clean
     twice to fill gaps resulting from these GEOSExceptions.
@@ -98,66 +74,41 @@
 
     Args:
         gdf: GeoDataFrame to be cleaned.
         tolerance: distance (usually meters) used as the minimum thickness
             for polygons to be eliminated. Any gap, hole, sliver or double
             surface that are empty after a negative buffer of tolerance / 2
             are eliminated into the neighbor with the longest shared border.
-        duplicate action: Either "fix", "error" or "ignore".
+        duplicate_action: Either "fix", "error" or "ignore".
             If "fix" (default), double surfaces thicker than the
             tolerance will be updated from top to bottom (function update_geometries)
             and then dissolved into the neighbor polygon with the longest shared border.
             If "error", an Exception is raised if there are any double surfaces thicker
             than the tolerance. If "ignore", double surfaces are kept as is.
         grid_sizes: One or more grid_sizes used in overlay and dissolve operations that
             might raise a GEOSException. Defaults to (None,), meaning no grid_sizes.
+        n_jobs: Number of threads.
 
     Returns:
         A GeoDataFrame with cleaned polygons.
-
-    Examples
-    --------
-
-    >>> cleaned = coverage_clean(
-    ...     gdf,
-    ...     0.1,
-    ...     grid_sizes=[None, 1e-6, 1e-5, 1e-4, 1e-3],
-    ... )
-
-    If you have a known mask for your coverage, e.g. municipality polygons,
-    it might be a good idea to buffer the gaps, slivers and double surfaces
-    before elimination to make sure the polygons are properly dissolved.
-
-    >>> def _small_buffer(df):
-    ...     df.geometry = df.buffer(0.001)
-    ...     return df
-    ...
-    >>> cleaned = coverage_clean(
-    ...     gdf,
-    ...     0.1,
-    ...     grid_sizes=[None, 1e-6, 1e-5, 1e-4, 1e-3],
-    ...     pre_dissolve_func=_small_buffer,
-    ... ).pipe(sg.clean_clip, your_mask, geom_type="polygon")
-
     """
-
     if not len(gdf):
         return gdf
 
     _cleaning_checks(gdf, tolerance, duplicate_action)
 
     if not gdf.index.is_unique:
         gdf = gdf.reset_index(drop=True)
 
     gdf = make_all_singlepart(gdf).loc[
         lambda x: x.geom_type.isin(["Polygon", "MultiPolygon"])
     ]
 
     try:
-        gdf = safe_simplify(gdf, PRECISION)
+        gdf = _safe_simplify(gdf, PRECISION)
     except GEOSException:
         pass
 
     gdf = (
         clean_geoms(gdf)
         .pipe(make_all_singlepart)
         .loc[lambda x: x.geom_type.isin(["Polygon", "MultiPolygon"])]
@@ -171,15 +122,15 @@
                 gaps = get_gaps(gdf, include_interiors=True, grid_size=grid_size)
                 if grid_size:
                     # in order to not get more gaps
                     gaps.geometry = gaps.buffer(grid_size)
                 break
             except GEOSException as e:
                 if i == len(grid_sizes) - 1:
-                    explore_geosexception(e, gdf, logger=logger)
+                    explore_geosexception(e, gdf)
                     raise e
 
     gaps["_was_gap"] = 1
 
     if duplicate_action == "ignore":
         double = GeoDataFrame({"geometry": []}, crs=gdf.crs)
         double["_double_idx"] = None
@@ -258,15 +209,15 @@
                 geom_type="polygon",
                 grid_size=grid_size,
                 n_jobs=n_jobs,
             ).drop(columns=["_eliminate_idx", "_double_idx"])
             break
         except GEOSException as e:
             if i == len(grid_sizes) - 1:
-                explore_geosexception(e, gdf, intersecting, isolated, logger=logger)
+                explore_geosexception(e, gdf, intersecting, isolated)
                 raise e
 
     not_really_isolated = isolated[["geometry", "_eliminate_idx", "_cluster"]].merge(
         without_double.drop(columns=["geometry"]),
         on="_cluster",
         how="inner",
     )
@@ -329,43 +280,41 @@
                 )
                 .sort_index()
                 .reset_index(drop=True)
             )
             break
         except GEOSException as e:
             if i == len(grid_sizes) - 1:
-                explore_geosexception(
-                    e, gdf, without_double, isolated, really_isolated, logger=logger
-                )
+                explore_geosexception(e, gdf, without_double, isolated, really_isolated)
                 raise e
 
     cleaned = pd.concat([many_hits, one_hit], ignore_index=True)
 
     gdf = gdf.drop(columns="_poly_idx")
 
     for i, grid_size in enumerate(grid_sizes):
         try:
             cleaned = clean_overlay(
                 gdf,
                 cleaned,
                 how="update",
                 geom_type="polygon",
+                grid_size=grid_size,
                 n_jobs=n_jobs,
             )
             break
         except GEOSException as e:
             if i == len(grid_sizes) - 1:
                 explore_geosexception(
                     e,
                     gdf,
                     cleaned,
                     without_double,
                     isolated,
                     really_isolated,
-                    logger=logger,
                 )
                 raise e
 
     cleaned = sort_large_first(cleaned)
 
     # slivers on bottom
     cleaned = pd.concat(split_out_slivers(cleaned, tolerance))
@@ -384,29 +333,28 @@
                 explore_geosexception(
                     e,
                     gdf,
                     cleaned,
                     without_double,
                     isolated,
                     really_isolated,
-                    logger=logger,
                 )
                 raise e
 
-    # cleaned = safe_simplify(cleaned, PRECISION)
+    # cleaned = _safe_simplify(cleaned, PRECISION)
     # cleaned.geometry = shapely.make_valid(cleaned.geometry)
 
     # TODO check why polygons dissappear in rare cases. For now, just add back the missing
     dissapeared_polygons = sfilter_inverse(gdf, cleaned.buffer(-PRECISION))
     cleaned = pd.concat([cleaned, dissapeared_polygons])
 
     return to_single_geom_type(cleaned, "polygon")
 
 
-def safe_simplify(gdf, tolerance: float | int, **kwargs):
+def _safe_simplify(gdf: GeoDataFrame, tolerance: float | int, **kwargs) -> GeoDataFrame:
     """Simplify only if the resulting area is no more than 1 percent larger.
 
     Because simplifying can result in holes being filled.
     """
     length_then = gdf.length
     copied = gdf.copy()
     copied.geometry = shapely.make_valid(
@@ -416,15 +364,15 @@
     copied.loc[filt, copied._geometry_column_name] = gdf.loc[
         filt, copied._geometry_column_name
     ]
 
     return copied
 
 
-def remove_interior_slivers(gdf, tolerance):
+def _remove_interior_slivers(gdf: GeoDataFrame, tolerance: int | float) -> GeoDataFrame:
     gdf, slivers = split_out_slivers(gdf, tolerance)
     slivers["_idx"] = range(len(slivers))
     without_thick = clean_overlay(
         to_lines(slivers), buff(gdf, PRECISION), how="difference"
     )
     return pd.concat(
         [
@@ -435,22 +383,37 @@
         ]
     )
 
 
 def remove_spikes(
     gdf: GeoDataFrame, tolerance: int | float, n_jobs: int = 1
 ) -> GeoDataFrame:
+    """Remove thin spikes from polygons.
+
+    Args:
+        gdf: A GeoDataFrame.
+        tolerance: Spike tolerance.
+        n_jobs: Number of threads.
+
+    Returns:
+        A GeoDataFrame.
+    """
     return clean_overlay(
         gdf, gdf[["geometry"]], how="intersection", grid_size=tolerance, n_jobs=n_jobs
     )
 
 
 def _properly_fix_duplicates(
-    gdf, double, slivers, thin_gaps_and_double, tolerance, n_jobs
-):
+    gdf: GeoDataFrame,
+    double: GeoDataFrame,
+    slivers: GeoDataFrame,
+    thin_gaps_and_double: GeoDataFrame,
+    tolerance: int | float,
+    n_jobs: int,
+) -> GeoDataFrame:
     gdf = _dissolve_thick_double_and_update(gdf, double, thin_gaps_and_double, n_jobs)
     gdf, more_slivers = split_out_slivers(gdf, tolerance)
     slivers = pd.concat([slivers, more_slivers], ignore_index=True)
     gaps = get_gaps(gdf, include_interiors=True)
     gaps["_was_gap"] = 1
     assert "_double_idx" not in gaps
     double = get_intersections(gdf)
@@ -458,15 +421,17 @@
     thin_gaps_and_double = pd.concat([gaps, double], ignore_index=True).loc[
         lambda x: x.buffer(-tolerance / 2).is_empty
     ]
 
     return gdf, thin_gaps_and_double, slivers
 
 
-def _dissolve_thick_double_and_update(gdf, double, thin_double, n_jobs):
+def _dissolve_thick_double_and_update(
+    gdf: GeoDataFrame, double: GeoDataFrame, thin_double: GeoDataFrame, n_jobs: int
+) -> GeoDataFrame:
     large = (
         double.loc[~double["_double_idx"].isin(thin_double["_double_idx"])].drop(
             columns="_double_idx"
         )
         # .pipe(sort_large_first)
         # .sort_values("_poly_idx")
         .pipe(update_geometries, geom_type="polygon", n_jobs=n_jobs)
@@ -475,15 +440,17 @@
         clean_overlay(gdf, large, how="update", geom_type="polygon", n_jobs=n_jobs)
         # .pipe(sort_large_first)
         # .sort_values("_poly_idx")
         .pipe(update_geometries, geom_type="polygon", n_jobs=n_jobs)
     )
 
 
-def _cleaning_checks(gdf, tolerance, duplicate_action):  # , spike_action):
+def _cleaning_checks(
+    gdf: GeoDataFrame, tolerance: int | float, duplicate_action: bool
+) -> GeoDataFrame:  # , spike_action):
     if not len(gdf) or not tolerance:
         return gdf
     if tolerance < PRECISION:
         raise ValueError(
             f"'tolerance' must be larger than {PRECISION} to avoid "
             "problems with floating point precision."
         )
@@ -499,19 +466,19 @@
     gdf = gdf.loc[~is_sliver]
     slivers, isolated = sfilter_split(slivers, gdf.buffer(PRECISION))
     gdf = pd.concat([gdf, isolated])
     return gdf, slivers
 
 
 def try_for_grid_size(
-    func,
+    func: Callable,
     grid_sizes: tuple[None, float | int],
     args: tuple | None = None,
     kwargs: dict | None = None,
-):
+) -> Any:
     args = args or ()
     kwargs = kwargs or {}
     for i, grid_size in enumerate(grid_sizes):
         try:
             return func(*args, grid_size=grid_size, **kwargs)
         except GEOSException as e:
             if i == len(grid_sizes) - 1:
@@ -519,15 +486,14 @@
 
 
 def split_and_eliminate_by_longest(
     gdf: GeoDataFrame | list[GeoDataFrame],
     to_eliminate: GeoDataFrame,
     tolerance: int | float,
     grid_sizes: tuple[None | float | int] = (None,),
-    logger=None,
     n_jobs: int = 1,
     **kwargs,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     if not len(to_eliminate):
         return gdf
 
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
@@ -581,15 +547,20 @@
         eliminate_by_longest,
         grid_sizes=grid_sizes,
         args=(gdf, missing),
         kwargs=kwargs | {"n_jobs": n_jobs},
     )
 
 
-def split_by_neighbors(df, split_by, tolerance, grid_size=None):
+def split_by_neighbors(
+    df: GeoDataFrame,
+    split_by: GeoDataFrame,
+    tolerance: int | float,
+    grid_size: float | int | None = None,
+) -> GeoDataFrame:
     if not len(df):
         return df
 
     split_by = split_by.copy()
     split_by.geometry = shapely.simplify(split_by.geometry, tolerance)
 
     intersecting_lines = (
@@ -617,15 +588,15 @@
     )
 
     buffered = buff(extended_lines, tolerance, single_sided=True)
 
     return clean_overlay(df, buffered, how="identity", grid_size=grid_size)
 
 
-def extend_lines(arr1, arr2, distance):
+def extend_lines(arr1, arr2, distance) -> NDArray[LineString]:
     if len(arr1) != len(arr2):
         raise ValueError
     if not len(arr1):
         return arr1
 
     arr1, arr2 = arr2, arr1  # TODO fix
 
@@ -660,15 +631,15 @@
             pd.DataFrame(get_coordinates(arr2), columns=["x", "y"]),
         ]
     ).sort_index()
 
     return linestrings(coords.values, indices=coords.index)
 
 
-def get_line_segments(lines) -> GeoDataFrame:
+def get_line_segments(lines: GeoDataFrame | GeoSeries) -> GeoDataFrame:
     assert lines.index.is_unique
     if isinstance(lines, GeoDataFrame):
         geom_col = lines._geometry_column_name
         multipoints = lines.assign(
             **{geom_col: extract_unique_points(lines.geometry.values)}
         )
         segments = multipoints_to_line_segments(multipoints.geometry)
@@ -707,15 +678,16 @@
     first_points = point_df.loc[lambda x: ~x.index.duplicated(), "geometry"]
     is_last_point = point_df["next"].isna()
 
     point_df.loc[is_last_point, "next"] = first_points
     assert point_df["next"].notna().all()
 
     point_df["geometry"] = [
-        LineString([x1, x2]) for x1, x2 in zip(point_df["geometry"], point_df["next"])
+        LineString([x1, x2])
+        for x1, x2 in zip(point_df["geometry"], point_df["next"], strict=False)
     ]
     return GeoDataFrame(point_df.drop(columns=["next"]), geometry="geometry", crs=crs)
 
 
 def points_to_line_segments(points: GeoDataFrame) -> GeoDataFrame:
     points = points.copy()
     points["next"] = points.groupby(level=0)["geometry"].shift(-1)
@@ -723,24 +695,35 @@
     first_points = points.loc[lambda x: ~x.index.duplicated(), "geometry"]
     is_last_point = points["next"].isna()
 
     points.loc[is_last_point, "next"] = first_points
     assert points["next"].notna().all()
 
     points["geometry"] = [
-        LineString([x1, x2]) for x1, x2 in zip(points["geometry"], points["next"])
+        LineString([x1, x2])
+        for x1, x2 in zip(points["geometry"], points["next"], strict=False)
     ]
     return GeoDataFrame(
         points.drop(columns=["next"]), geometry="geometry", crs=points.crs
     )
 
 
-def explore_geosexception(e: GEOSException, *gdfs, logger=None):
-    from ..maps.maps import Explore, explore
-    from .conversion import to_gdf
+def explore_geosexception(
+    e: GEOSException, *gdfs: GeoDataFrame, logger: Any | None = None
+) -> None:
+    """Extract the coordinates of a GEOSException and show in map.
+
+    Args:
+        e: The exception thrown by a GEOS operation, which potentially contains coordinates information.
+        *gdfs: One or more GeoDataFrames to display for context in the map.
+        logger: An optional logger to log the error with visualization. If None, uses standard output.
+
+    """
+    from ..maps.maps import Explore
+    from ..maps.maps import explore
 
     pattern = r"(\d+\.\d+)\s+(\d+\.\d+)"
 
     matches = re.findall(pattern, str(e))
     coords_in_error_message = [(float(match[0]), float(match[1])) for match in matches]
     exception_point = to_gdf(coords_in_error_message, crs=gdfs[0].crs)
     if len(exception_point):
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/conversion.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 import numbers
 import re
-from collections.abc import Collection, Iterator, Mapping, Sized
+from collections.abc import Callable
+from collections.abc import Collection
+from collections.abc import Iterable
+from collections.abc import Iterator
+from collections.abc import Mapping
+from collections.abc import Sized
 from typing import Any
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio
 import shapely
 from affine import Affine
-from geopandas import GeoDataFrame, GeoSeries
-from pandas.api.types import is_array_like, is_dict_like, is_list_like
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from numpy.typing import NDArray
+from pandas.api.types import is_array_like
+from pandas.api.types import is_dict_like
+from pandas.api.types import is_list_like
 from pyproj import CRS
 from rasterio import features
-from shapely import Geometry, box, wkb, wkt
+from shapely import Geometry
+from shapely import box
+from shapely import wkb
+from shapely import wkt
 from shapely.errors import GEOSException
-from shapely.geometry import Point, shape
+from shapely.geometry import Point
+from shapely.geometry import shape
 from shapely.ops import unary_union
 
-
 try:
     from torchgeo.datasets.geo import RasterDataset
 except ImportError:
 
-    class RasterDataset:
-        """Placeholder"""
+    class RasterDataset:  # type: ignore
+        """Placeholder."""
 
 
-@staticmethod
-def crs_to_string(crs):
+def crs_to_string(crs: Any) -> str:
+    """Extract the string of a CRS-like object."""
     if crs is None:
         return "None"
     crs = pyproj.CRS(crs)
     crs_str = str(crs.to_json_dict()["name"])
     pattern = r"\d{4,5}"
-    try:
-        return re.search(pattern, crs_str).group()
-    except AttributeError:
-        return crs_str
+    match = re.search(pattern, crs_str)
+    return match.group() if match else crs_str
 
 
 def to_geoseries(obj: Any, crs: Any | None = None) -> GeoSeries:
+    """Convert an object to GeoSeries."""
     if crs is None:
         try:
             crs = obj.crs
         except AttributeError:
             pass
 
     try:
@@ -69,27 +80,38 @@
             # geoseries will raise an Exception for non-geometry objects,
             # so we can safely pass here
             pass
 
     return GeoSeries(obj, index=index, crs=crs)
 
 
-def to_shapely(obj) -> Geometry:
+def to_shapely(obj: Any) -> Geometry:
+    """Convert a geometry object or bounding box to a shapely Geometry."""
     if isinstance(obj, Geometry):
         return obj
     if not hasattr(obj, "__iter__"):
         raise TypeError(type(obj))
     if hasattr(obj, "unary_union"):
         return obj.unary_union
-    # if is_bbox_like(obj):
-    #     return box(*obj)
     try:
         return Point(*obj)
     except TypeError:
+        pass
+    try:
         return box(*to_bbox(obj))
+    except TypeError:
+        pass
+    try:
+        return shapely.wkt.loads(obj)
+    except TypeError:
+        pass
+    try:
+        return shapely.wkb.loads(obj)
+    except TypeError:
+        pass
 
 
 def to_bbox(
     obj: GeoDataFrame | GeoSeries | Geometry | Collection | Mapping,
 ) -> tuple[float, float, float, float]:
     """Returns 4-length tuple of bounds if possible, else raises ValueError.
 
@@ -101,32 +123,32 @@
     """
     if isinstance(obj, (GeoDataFrame, GeoSeries)):
         return tuple(obj.total_bounds)
     if isinstance(obj, Geometry):
         return tuple(obj.bounds)
 
     try:
-        minx = int(np.min(obj["minx"]))
-        miny = int(np.min(obj["miny"]))
-        maxx = int(np.max(obj["maxx"]))
-        maxy = int(np.max(obj["maxy"]))
+        minx = int(np.min(obj["minx"]))  # type: ignore [index]
+        miny = int(np.min(obj["miny"]))  # type: ignore [index]
+        maxx = int(np.max(obj["maxx"]))  # type: ignore [index]
+        maxy = int(np.max(obj["maxy"]))  # type: ignore [index]
         return minx, miny, maxx, maxy
     except Exception:
         try:
-            minx = int(np.min(obj.minx))
-            miny = int(np.min(obj.miny))
-            maxx = int(np.max(obj.maxx))
-            maxy = int(np.max(obj.maxy))
+            minx = int(np.min(obj.minx))  # type: ignore [union-attr]
+            miny = int(np.min(obj.miny))  # type: ignore [union-attr]
+            maxx = int(np.max(obj.maxx))  # type: ignore [union-attr]
+            maxy = int(np.max(obj.maxy))  # type: ignore [union-attr]
             return minx, miny, maxx, maxy
         except Exception:
             pass
 
     if hasattr(obj, "geometry"):
         try:
-            return tuple(GeoSeries(obj["geometry"]).total_bounds)
+            return tuple(GeoSeries(obj["geometry"]).total_bounds)  # type: ignore [index]
         except Exception:
             return tuple(GeoSeries(obj.geometry).total_bounds)
 
     if (
         hasattr(obj, "__len__")
         and len(obj) == 4
         and all(isinstance(x, numbers.Number) for x in obj)
@@ -136,73 +158,87 @@
     try:
         of_length = f" of length {len(obj)}"
     except TypeError:
         of_length = ""
     raise TypeError(f"Cannot convert type {obj.__class__.__name__}{of_length} to bbox")
 
 
-def from_4326(lon: float, lat: float, crs=25833):
+def from_4326(lon: float, lat: float, crs=25833) -> tuple[float, float]:
     """Get utm 33 N coordinates from lonlat (4326)."""
     transformer = pyproj.Transformer.from_crs(
         "EPSG:4326", f"EPSG:{crs}", always_xy=True
     )
     return transformer.transform(lon, lat)
 
 
-def to_4326(lon: float, lat: float, crs=25833):
+def to_4326(lon: float, lat: float, crs=25833) -> tuple[float, float]:
     """Get degree coordinates  33 N coordinates from lonlat (4326)."""
     transformer = pyproj.Transformer.from_crs(
         f"EPSG:{crs}", "EPSG:4326", always_xy=True
     )
     return transformer.transform(lon, lat)
 
 
 def coordinate_array(
     gdf: GeoDataFrame | GeoSeries,
-    strict=False,
-) -> np.ndarray[np.ndarray[float], np.ndarray[float]]:
+    strict: bool = False,
+    include_z: bool = False,
+) -> NDArray[np.float64]:
     """Creates a 2d ndarray of coordinates from point geometries.
 
     Args:
         gdf: GeoDataFrame or GeoSeries of point geometries.
+        strict: If False (default), geometries without coordinates
+            are given the value None.
+        include_z: Whether to include z-coordinates. Defaults to False.
 
     Returns:
         np.ndarray of np.ndarrays of coordinates.
 
-    Examples
+    Examples:
     --------
-    >>> from sgis import coordinate_array, random_points
-    >>> points = random_points(5)
+    >>> import sgis as sg
+    >>> points = sg.to_gdf(
+    ...     [
+    ...         (0, 1),
+    ...         (1, 0),
+    ...         (1, 1),
+    ...         (0, 0),
+    ...         (0.5, 0.5),
+    ...         (0.5, 0.25),
+    ...         (0.25, 0.25),
+    ...         (0.75, 0.75),
+    ...         (0.25, 0.75),
+    ...         (0.75, 0.25),
+    ...     ]
+    ... )
     >>> points
                     geometry
     0  POINT (0.59376 0.92577)
     1  POINT (0.34075 0.91650)
     2  POINT (0.74841 0.10627)
     3  POINT (0.00966 0.87868)
     4  POINT (0.38046 0.87879)
-    >>> coordinate_array(points)
+    >>> sg.coordinate_array(points)
     array([[0.59376221, 0.92577159],
         [0.34074678, 0.91650446],
         [0.74840912, 0.10626954],
         [0.00965935, 0.87867915],
         [0.38045827, 0.87878816]])
-    >>> coordinate_array(points.geometry)
+    >>> sg.coordinate_array(points.geometry)
     array([[0.59376221, 0.92577159],
         [0.34074678, 0.91650446],
         [0.74840912, 0.10626954],
         [0.00965935, 0.87867915],
         [0.38045827, 0.87878816]])
     """
-    if isinstance(gdf, GeoDataFrame):
-        gdf = gdf.geometry
-    if strict:
-        return np.array([(geom.x, geom.y) for geom in gdf])
-    return np.array(
-        [(geom.x, geom.y) if hasattr(geom, "x") else (None, None) for geom in gdf]
-    )
+    try:
+        return shapely.get_coordinates(gdf.geometry.values, include_z=include_z)
+    except AttributeError:
+        return shapely.get_coordinates(gdf, include_z=include_z)
 
 
 def to_gdf(
     obj: (
         Geometry
         | str
         | bytes
@@ -238,82 +274,82 @@
             If not specified, the key/column 'geometry' will be used if it
             exists. If multiple columns, can be given as e.g. "xyz" or ["x", "y"].
         **kwargs: additional keyword arguments taken by the GeoDataFrame constructor.
 
     Returns:
         A GeoDataFrame with one column, the geometry column.
 
-    Examples
+    Examples:
     --------
-    >>> from sgis import to_gdf
+    >>> import sgis as sg
     >>> coords = (10, 60)
-    >>> to_gdf(coords, crs=4326)
+    >>> sg.to_gdf(coords, crs=4326)
                         geometry
     0  POINT (10.00000 60.00000)
 
     From wkt.
 
     >>> wkt = "POINT (10 60)"
-    >>> to_gdf(wkt, crs=4326)
+    >>> sg.to_gdf(wkt, crs=4326)
                         geometry
     0  POINT (10.00000 60.00000)
 
     From DataFrame with x, y (optionally z) coordinate columns. Index and
     columns are preserved.
 
     >>> df = pd.DataFrame({"x": [10, 11], "y": [60, 59]}, index=[1,3])
         x   y
     1  10  60
     3  11  59
-    >>> gdf = to_gdf(df, geometry=["x", "y"], crs=4326)
+    >>> gdf = sg.to_gdf(df, geometry=["x", "y"], crs=4326)
     >>> gdf
         x   y                   geometry
     1  10  60  POINT (10.00000 60.00000)
     3  11  59  POINT (11.00000 59.00000)
 
     For DataFrame/dict with a geometry-like column named "geometry". If the column has
     another name, it must be set with the geometry parameter.
 
     >>> df = pd.DataFrame({"col": [1, 2], "geometry": ["point (10 60)", (11, 59)]})
     >>> df
        col       geometry
     0    1  point (10 60)
     1    2       (11, 59)
-    >>> gdf = to_gdf(df, crs=4326)
+    >>> gdf = sg.to_gdf(df, crs=4326)
     >>> gdf
        col                   geometry
     0    1  POINT (10.00000 60.00000)
     1    2  POINT (11.00000 59.00000)
 
     From Series.
 
     >>> series = Series({1: (10, 60), 3: (11, 59)})
-    >>> to_gdf(series)
+    >>> sg.to_gdf(series)
                         geometry
     1  POINT (10.00000 60.00000)
     3  POINT (11.00000 59.00000)
 
     Multiple coordinates will be converted to points, unless a line or polygon geometry
     is constructed beforehand.
 
     >>> coordslist = [(10, 60), (11, 59)]
-    >>> to_gdf(coordslist, crs=4326)
+    >>> sg.to_gdf(coordslist, crs=4326)
                         geometry
     0  POINT (10.00000 60.00000)
     1  POINT (11.00000 59.00000)
 
     >>> from shapely.geometry import LineString
-    >>> to_gdf(LineString(coordslist), crs=4326)
+    >>> sg.to_gdf(LineString(coordslist), crs=4326)
                                                 geometry
     0  LINESTRING (10.00000 60.00000, 11.00000 59.00000)
 
     From 2 or 3 dimensional array.
 
     >>> arr = np.random.randint(100, size=(5, 3))
-    >>> to_gdf(arr)
+    >>> sg.to_gdf(arr)
                              geometry
     0  POINT Z (82.000 88.000 82.000)
     1  POINT Z (70.000 92.000 20.000)
     2   POINT Z (91.000 34.000 3.000)
     3   POINT Z (1.000 50.000 77.000)
     4  POINT Z (58.000 49.000 46.000)
     """
@@ -329,25 +365,33 @@
 
     if isinstance(obj, GeoSeries):
         geom_col = geometry or "geometry"
         return _geoseries_to_gdf(obj, geom_col, crs, **kwargs)
 
     if crs is None:
         try:
-            crs = obj.crs
+            crs = obj.crs  # type: ignore
         except AttributeError:
             try:
-                matches = re.search(r"SRID=(\d+);", obj)
+                matches = re.search(r"SRID=(\d+);", obj)  # type: ignore
             except TypeError:
                 try:
-                    matches = re.search(r"SRID=(\d+);", obj[0])
+                    matches = re.search(r"SRID=(\d+);", obj[0])  # type: ignore
                 except Exception:
                     pass
             try:
-                crs = CRS(int("".join(x for x in matches.group(0) if x.isnumeric())))
+                crs = CRS(
+                    int(
+                        "".join(
+                            x
+                            for x in matches.group(0)  # type:ignore
+                            if x.isnumeric()
+                        )
+                    )
+                )
             except Exception:
                 pass
 
     if isinstance(obj, RasterDataset):
         # read the entire dataset
         obj = obj[obj.bounds]
         crs = obj["crs"]
@@ -358,21 +402,21 @@
                 _array_to_geojson(array, transform),
                 columns=["value", "geometry"],
             ),
             geometry="geometry",
             crs=crs,
         )
 
-    if is_array_like(geometry) and len(geometry) == len(obj):
+    if is_array_like(geometry) and len(geometry) == len(obj):  # type: ignore
         geometry = GeoSeries(
-            _make_one_shapely_geom(g) for g in geometry if g is not None
+            _make_one_shapely_geom(g) for g in geometry if g is not None  # type: ignore
         )
         return GeoDataFrame(obj, geometry=geometry, crs=crs, **kwargs)
 
-    geom_col: str = find_geometry_column(obj, geometry)
+    geom_col: str = _find_geometry_column(obj, geometry)  # type: ignore[no-redef]
     index = kwargs.pop("index", None)
 
     # get done with iterators that get consumed by 'all'
     if isinstance(obj, Iterator) and not isinstance(obj, Sized):
         obj = GeoSeries(
             (_make_one_shapely_geom(g) for g in obj if g is not None), index=index
         )
@@ -389,68 +433,68 @@
             return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
         elif all(hasattr(obj, attr) for attr in ["minx", "miny", "maxx", "maxy"]):
             obj = GeoSeries(shapely.box(*to_bbox(obj)), index=index)
             return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
         if is_nested_geojson(obj):
             # crs = crs or get_crs_from_dict(obj)
             obj = pd.concat(
-                (GeoSeries(_from_json(g)) for g in obj if g is not None),
+                (GeoSeries(_from_json(g)) for g in obj if g is not None),  # type: ignore
                 ignore_index=True,
             )
             if index is not None:
                 obj.index = index
             return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
         # list etc.
         else:
-            obj = GeoSeries(make_shapely_geoms(obj), index=index)
+            obj = GeoSeries(_make_shapely_geoms(obj), index=index)
             return GeoDataFrame(
                 {geom_col: obj}, geometry=geom_col, index=index, crs=crs, **kwargs
             )
 
     # now we have dict, Series or DataFrame
 
-    obj = obj.copy()
+    obj = obj.copy()  # type: ignore [union-attr]
 
     # preserve Series/DataFrame index
     index = obj.index if hasattr(obj, "index") and index is None else index
 
     if geom_col in obj.keys():
         if isinstance(obj, pd.DataFrame):
             notna = obj[geom_col].notna()
             obj.loc[notna, geom_col] = list(
-                make_shapely_geoms(obj.loc[notna, geom_col])
+                _make_shapely_geoms(obj.loc[notna, geom_col])
             )
             obj[geom_col] = GeoSeries(obj[geom_col])
             return GeoDataFrame(obj, geometry=geom_col, crs=crs, **kwargs)
         if isinstance(obj[geom_col], Geometry):
             return GeoDataFrame(
                 dict(obj), geometry=geom_col, crs=crs, index=[0], **kwargs
             )
         if not hasattr(obj[geom_col], "__iter__") or len(obj[geom_col]) == 1:
-            obj[geom_col] = make_shapely_geoms(obj[geom_col])
+            obj[geom_col] = _make_shapely_geoms(obj[geom_col])
             return GeoDataFrame(
                 dict(obj), geometry=geom_col, crs=crs, index=index, **kwargs
             )
-        obj[geom_col] = GeoSeries(make_shapely_geoms(obj[geom_col]), index=index)
+        obj[geom_col] = GeoSeries(_make_shapely_geoms(obj[geom_col]), index=index)
         return GeoDataFrame(dict(obj), geometry=geom_col, crs=crs, **kwargs)
 
-    if geometry and all(g in obj for g in geometry):
+    if geometry and all(g in obj for g in geometry):  # type: ignore [union-attr]
         obj[geom_col] = _geoseries_from_xyz(obj, geometry, index=index)
         return GeoDataFrame(obj, geometry=geom_col, crs=crs, **kwargs)
 
     if len(obj.keys()) == 1:
-        key = list(obj.keys())[0]
+        key = next(iter(obj.keys()))
         if isinstance(obj, dict):
             geoseries = GeoSeries(
-                make_shapely_geoms(list(obj.values())[0]), index=index
+                _make_shapely_geoms(next(iter(obj.values()))), index=index
             )
         elif isinstance(obj, pd.Series):
-            geoseries = GeoSeries(make_shapely_geoms(obj), index=index)
+            geoseries = GeoSeries(_make_shapely_geoms(obj), index=index)
         else:
-            geoseries = GeoSeries(make_shapely_geoms(obj.iloc[:, 0]), index=index)
+            geoseries = GeoSeries(_make_shapely_geoms(obj.iloc[:, 0]), index=index)
         return GeoDataFrame({key: geoseries}, geometry=key, crs=crs, **kwargs)
 
     if geometry and geom_col not in obj or isinstance(obj, pd.DataFrame):
         raise ValueError("Cannot find geometry column(s)", geometry)
 
     # geojson, __geo_interface__
     if (
@@ -467,15 +511,17 @@
     try:
         geoseries = _series_like_to_geoseries(obj, index=index)
     except ValueError:
         geoseries = _series_like_to_geoseries(obj.dropna(), index=obj.dropna().index)
     return GeoDataFrame(geometry=geoseries, crs=crs, **kwargs)
 
 
-def _array_to_geojson(array: np.ndarray, transform: Affine):
+def _array_to_geojson(
+    array: np.ndarray, transform: Affine
+) -> list[tuple[dict, Geometry]]:
     try:
         return [
             (value, shape(geom))
             for geom, value in features.shapes(array, transform=transform)
         ]
     except ValueError:
         array = array.astype(np.float32)
@@ -494,54 +540,51 @@
     elif len(shape) == 3:
         _, width, height = shape
     else:
         raise ValueError
     return rasterio.transform.from_bounds(minx, miny, maxx, maxy, width, height)
 
 
-def make_shapely_geoms(obj):
+def _make_shapely_geoms(obj: Any) -> Geometry | Any:
     if _is_one_geometry(obj):
         return _make_one_shapely_geom(obj)
     if isinstance(obj, dict) and "coordinates" in obj:
         return _from_json(obj)
     return (_make_one_shapely_geom(g) for g in obj)
 
 
-"""def is_boundingbox(obj) -> bool:
-    if not hasattr(obj, "__iter__"):
-        return False
+def is_bbox_like(obj: Any) -> bool:
+    """Returns True if the object is an iterable of 4 numbers.
 
-    classname = obj.__class__.__name__.lower()
-    if "bounding" not in classname and "box" not in classname:
-        return False
-
-    if len(obj) == 4 and all(isinstance(x, numbers.Number) for x in obj):
-        return True
-
-    return False"""
-
-
-def is_bbox_like(obj) -> bool:
+    Args:
+        obj: Any object.
+    """
     if (
         hasattr(obj, "__len__")
         and len(obj) == 4
         and hasattr(obj, "__iter__")
         and all(isinstance(x, numbers.Number) for x in obj)
     ):
         return True
     return False
 
 
-def is_nested_geojson(obj) -> bool:
+def is_nested_geojson(obj: Any) -> bool:
+    """Returns True if the object is an iterable of all dicts.
+
+    Args:
+        obj: Any object.
+    """
     if hasattr(obj, "__iter__") and all(isinstance(g, dict) for g in obj):
         return True
     return False
 
 
-def get_crs_from_dict(obj):
+def get_crs_from_dict(obj: Any) -> CRS | None | Any:
+    """Try to extract the 'crs' attribute of the object or an object in the object."""
     if (
         not hasattr(obj, "__iter__")
         or not is_dict_like(obj)
         and not is_dict_like(obj[0])
     ):
         return None
 
@@ -562,50 +605,52 @@
             else:
                 return None
         return obj
 
     return None
 
 
-def _from_json(obj: dict):
+def _from_json(obj: dict | list[dict]) -> Geometry:
     if not isinstance(obj, dict) and isinstance(obj[0], dict):
         return [_from_json(g) for g in obj]
     if "geometry" in obj:
         return _from_json(obj["geometry"])
     if "features" in obj:
         return _from_json(obj["features"])
     coords = obj["coordinates"]
-    constructor = eval("shapely.geometry." + obj.get("type", Point))
+    constructor: Callable = eval("shapely.geometry." + obj.get("type", Point))
     try:
         return constructor(coords)
     except TypeError:
         while len(coords) == 1:
             coords = coords[0]
         return constructor(coords)
 
 
-def _series_like_to_geoseries(obj, index):
+def _series_like_to_geoseries(obj: Iterable, index: Iterable) -> GeoSeries:
     if index is None:
         index = obj.keys()
     if isinstance(obj, dict):
-        return GeoSeries(make_shapely_geoms(list(obj.values())), index=index)
+        return GeoSeries(_make_shapely_geoms(list(obj.values())), index=index)
     else:
-        return GeoSeries(make_shapely_geoms(obj.values), index=index)
+        return GeoSeries(_make_shapely_geoms(obj.values), index=index)
 
 
-def _geoseries_to_gdf(obj: GeoSeries, geometry, crs, **kwargs) -> GeoDataFrame:
+def _geoseries_to_gdf(
+    obj: GeoSeries, geometry: str | GeoSeries | Iterable, crs: CRS | Any, **kwargs
+) -> GeoDataFrame:
     if not crs:
         crs = obj.crs
     else:
         obj = obj.to_crs(crs) if obj.crs else obj.set_crs(crs)
 
     return GeoDataFrame({geometry: obj}, geometry=geometry, crs=crs, **kwargs)
 
 
-def find_geometry_column(obj, geometry) -> str:
+def _find_geometry_column(obj: Any, geometry: GeoSeries | Iterable | None) -> str:
     if geometry is None:
         return "geometry"
 
     # dict key
     if not is_list_like(geometry) and geometry in obj:
         return geometry
 
@@ -617,17 +662,20 @@
         return "geometry"
 
     raise ValueError(
         "geometry should be a geometry column or x, y (z) coordinate columns."
     )
 
 
-def _geoseries_from_xyz(obj, geometry, index) -> GeoSeries:
+def _geoseries_from_xyz(
+    obj: Any,
+    geometry: Iterable[float, float] | Iterable[float, float, float],
+    index: Iterable | None,
+) -> GeoSeries:
     """Make geoseries from the geometry column or columns (x y (z))."""
-
     if len(geometry) == 2:
         x, y = geometry
         z = None
 
     elif len(geometry) == 3:
         x, y, z = geometry
         z = obj[z]
@@ -636,25 +684,25 @@
         raise ValueError(
             "geometry should be a geometry column or x, y (z) coordinate columns."
         )
 
     return gpd.GeoSeries.from_xy(x=obj[x], y=obj[y], z=z, index=index)
 
 
-def _is_one_geometry(obj) -> bool:
+def _is_one_geometry(obj: Any) -> bool:
     if (
-        isinstance(obj, (str, bytes, Geometry))
+        isinstance(obj, (str, bytes, Geometry))  # type: ignore [unreachable]
         or all(isinstance(i, numbers.Number) for i in obj)
         or not hasattr(obj, "__iter__")
     ):
         return True
-    return False
+    return False  # type: ignore [unreachable]
 
 
-def _make_one_shapely_geom(obj):
+def _make_one_shapely_geom(obj: Any) -> Geometry:
     """Create shapely geometry from wkt, wkb or coordinate tuple.
 
     Works recursively if the object is a nested iterable.
     """
     if isinstance(obj, str):
         try:
             return wkt.loads(obj)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/duplicates.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/duplicates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from collections.abc import Iterable
 
 import networkx as nx
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
-from shapely import STRtree, difference, make_valid, simplify, unary_union
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from shapely import STRtree
+from shapely import difference
+from shapely import make_valid
+from shapely import simplify
+from shapely import unary_union
 from shapely.errors import GEOSException
 
-from .general import (
-    _determine_geom_type_args,
-    _push_geom_col,
-    clean_geoms,
-    parallel_unary_union_geoseries,
-)
-from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
-from .overlay import _run_overlay_dask, clean_overlay, make_valid_and_keep_geom_type
-from .sfilter import sfilter_inverse, sfilter_split
-
+from .general import _determine_geom_type_args
+from .general import _parallel_unary_union_geoseries
+from .general import _push_geom_col
+from .general import clean_geoms
+from .geometry_types import get_geom_type
+from .geometry_types import make_all_singlepart
+from .geometry_types import to_single_geom_type
+from .overlay import _run_overlay_dask
+from .overlay import clean_overlay
+from .overlay import make_valid_and_keep_geom_type
+from .sfilter import sfilter_inverse
 
 PRECISION = 1e-3
 
 
 def update_geometries(
     gdf: GeoDataFrame,
     geom_type: str | None = None,
@@ -40,16 +46,18 @@
             GeometryCollections. If False, return all resulting geometries
             (potentially mixed types).
         geom_type: Optionally specify what geometry type to keep.,
             if there are mixed geometry types. Must be either "polygon",
             "line" or "point".
         grid_size: Precision grid size to round the geometries. Will use the highest
             precision of the inputs by default.
+        n_jobs: Number of threads.
+        predicate: Spatial predicate for the spatial tree.
 
-    Example
+    Example:
     ------
     Create two circles and get the overlap.
 
     >>> import sgis as sg
     >>> circles = sg.to_gdf([(0, 0), (1, 1)]).pipe(sg.buff, 1)
     >>> duplicates = sg.get_intersections(circles)
     >>> duplicates
@@ -103,15 +111,15 @@
     tree = STRtree(copied.geometry.values)
     left, right = tree.query(copied.geometry.values, predicate=predicate)
     indices = pd.Series(right, index=left).loc[lambda x: x.index > x.values]
 
     # select geometries from 'right', index from 'left', dissolve by 'left'
     erasers = pd.Series(copied.geometry.loc[indices.values].values, index=indices.index)
     if n_jobs > 1:
-        erasers = parallel_unary_union_geoseries(
+        erasers = _parallel_unary_union_geoseries(
             erasers,
             level=0,
             n_jobs=n_jobs,
             grid_size=grid_size,
         )
         erasers = pd.Series(erasers, index=indices.index.unique())
     else:
@@ -194,19 +202,21 @@
     Args:
         gdf: GeoDataFrame of polygons.
         geom_type: Optionally specify which geometry type to keep.
             Either "polygon", "line" or "point".
         keep_geom_type: Whether to keep the original geometry type.
             If mixed geometry types and keep_geom_type=True,
             an exception is raised.
+        n_jobs: Number of threads.
+        predicate: Spatial predicate for the spatial tree.
 
     Returns:
         A GeoDataFrame of the overlapping polygons.
 
-    Examples
+    Examples:
     --------
     Create three partially overlapping polygons.
 
     >>> import sgis as sg
     >>> circles = sg.to_gdf([(0, 0), (1, 0), (2, 0)]).pipe(sg.buff, 1.2)
     >>> circles.area
     0    4.523149
@@ -280,15 +290,19 @@
     if was_geoseries:
         return duplicated_geoms.geometry
 
     return duplicated_geoms.drop(columns="orig_idx")
 
 
 def _get_intersecting_geometries(
-    gdf: GeoDataFrame, geom_type, keep_geom_type, n_jobs, predicate
+    gdf: GeoDataFrame,
+    geom_type: str | None,
+    keep_geom_type: bool,
+    n_jobs: int,
+    predicate: str | None,
 ) -> GeoDataFrame:
     right = gdf[[gdf._geometry_column_name]]
     right["idx_right"] = right.index
 
     left = (
         gdf
         if not any("index_" in str(col) for col in gdf)
@@ -372,15 +386,15 @@
     idx_name = gdf.index.name
 
     gdf = gdf.reset_index(drop=True)
 
     tree = STRtree(gdf.geometry.values)
     left, right = tree.query(gdf.geometry.values, predicate="within")
 
-    edges = list(zip(left, right))
+    edges = list(zip(left, right, strict=False))
 
     graph = nx.Graph()
     graph.add_edges_from(edges)
 
     component_mapper = {
         j: i
         for i, component in enumerate(nx.connected_components(graph))
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/general.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import numbers
 import warnings
-from collections.abc import Hashable, Iterable
+from collections.abc import Hashable
+from collections.abc import Iterable
 from typing import Any
 
+import dask_geopandas
 import joblib
 import numpy as np
 import pandas as pd
 import pyproj
-from geopandas import GeoDataFrame, GeoSeries
-from geopandas.array import GeometryArray, GeometryDtype
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from geopandas.array import GeometryArray
+from geopandas.array import GeometryDtype
 from numpy.typing import NDArray
-from shapely import (
-    Geometry,
-    get_coordinates,
-    get_exterior_ring,
-    get_interior_ring,
-    get_num_interior_rings,
-    get_parts,
-    linestrings,
-    make_valid,
-)
+from shapely import Geometry
+from shapely import get_coordinates
+from shapely import get_exterior_ring
+from shapely import get_interior_ring
+from shapely import get_num_interior_rings
+from shapely import get_parts
+from shapely import linestrings
+from shapely import make_valid
 from shapely import points as shapely_points
 from shapely import unary_union
-from shapely.geometry import LineString, Point
+from shapely.geometry import LineString
+from shapely.geometry import Point
 
-from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
+from .geometry_types import get_geom_type
+from .geometry_types import make_all_singlepart
+from .geometry_types import to_single_geom_type
 
 
 def split_geom_types(gdf: GeoDataFrame | GeoSeries) -> tuple[GeoDataFrame | GeoSeries]:
     return tuple(
         gdf.loc[gdf.geom_type == geom_type] for geom_type in gdf.geom_type.unique()
     )
 
@@ -75,21 +80,21 @@
         actually_different = set()
         for x in truthy_crs:
             if x.to_string() in {j.to_string() for j in actually_different}:
                 continue
             actually_different.add(x)
 
         if len(actually_different) == 1:
-            return list(actually_different)[0]
+            return next(iter(actually_different))
         raise ValueError("'crs' mismatch.", truthy_crs)
 
     return pyproj.CRS(truthy_crs[0])
 
 
-def is_bbox_like(obj) -> bool:
+def is_bbox_like(obj: Any) -> bool:
     if (
         hasattr(obj, "__iter__")
         and len(obj) == 4
         and all(isinstance(x, numbers.Number) for x in obj)
     ):
         return True
     return False
@@ -110,24 +115,25 @@
         The GeoDataFrame with the geometry column pushed all the way to the right.
     """
     geom_col = gdf._geometry_column_name
     return gdf.reindex(columns=[c for c in gdf.columns if c != geom_col] + [geom_col])
 
 
 def drop_inactive_geometry_columns(gdf: GeoDataFrame) -> GeoDataFrame:
+    """Removes geometry columns in a GeoDataFrame if they are not active."""
     for col in gdf.columns:
         if (
             isinstance(gdf[col].dtype, GeometryDtype)
             and col != gdf._geometry_column_name
         ):
             gdf = gdf.drop(col, axis=1)
     return gdf
 
 
-def rename_geometry_if(gdf: GeoDataFrame) -> GeoDataFrame:
+def _rename_geometry_if(gdf: GeoDataFrame) -> GeoDataFrame:
     geom_col = gdf._geometry_column_name
     if geom_col == "geometry" and geom_col in gdf.columns:
         return gdf
     elif geom_col in gdf.columns:
         return gdf.rename_geometry("geometry")
 
     geom_cols = list(
@@ -153,15 +159,15 @@
         ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
             Defaults to False
 
     Returns:
         GeoDataFrame or GeoSeries with fixed geometries and only the rows with valid,
         non-empty and not-NaN/-None geometries.
 
-    Examples
+    Examples:
     --------
     >>> import sgis as sg
     >>> import pandas as pd
     >>> from shapely import wkt
     >>> gdf = sg.to_gdf([
     ...         "POINT (0 0)",
     ...         "LINESTRING (1 1, 2 2)",
@@ -227,47 +233,71 @@
     if ignore_index:
         gdf = gdf.reset_index(drop=True)
 
     return gdf
 
 
 def get_grouped_centroids(
-    gdf: GeoDataFrame, groupby: str, as_string: bool = True
+    gdf: GeoDataFrame, groupby: str | list[str], as_string: bool = True
 ) -> pd.Series:
+    """Get the centerpoint of the geometries within a group.
+
+    Args:
+        gdf: GeoDataFrame.
+        groupby: column to group by.
+        as_string: If True (default), coordinates are returned in
+            the format "{x}_{y}". If False, coordinates are returned
+            as Points.
+
+    Returns:
+        A pandas.Series of grouped centroids with the index of 'gdf'.
+    """
     centerpoints = gdf.assign(geometry=lambda x: x.centroid)
 
     grouped_centerpoints = centerpoints.dissolve(by=groupby).assign(
         geometry=lambda x: x.centroid
     )
     xs = grouped_centerpoints.geometry.x
     ys = grouped_centerpoints.geometry.y
 
     if as_string:
-        grouped_centerpoints["wkt"] = [f"{int(x)}_{int(y)}" for x, y in zip(xs, ys)]
+        grouped_centerpoints["wkt"] = [
+            f"{int(x)}_{int(y)}" for x, y in zip(xs, ys, strict=False)
+        ]
     else:
-        grouped_centerpoints["wkt"] = [Point(x, y) for x, y in zip(xs, ys)]
+        grouped_centerpoints["wkt"] = [
+            Point(x, y) for x, y in zip(xs, ys, strict=False)
+        ]
 
     return gdf[groupby].map(grouped_centerpoints["wkt"])
 
 
 def sort_large_first(gdf: GeoDataFrame | GeoSeries) -> GeoDataFrame | GeoSeries:
     """Sort GeoDataFrame by area in decending order.
 
     Args:
         gdf: A GeoDataFrame or GeoSeries.
 
     Returns:
         A GeoDataFrame or GeoSeries sorted from large to small in area.
 
-    Examples
+    Examples:
     --------
     Create GeoDataFrame with NaN values.
 
     >>> import sgis as sg
-    >>> df = sg.random_points(5)
+    >>> df = sg.to_gdf(
+    ...     [
+    ...         (0, 1),
+    ...         (1, 0),
+    ...         (1, 1),
+    ...         (0, 0),
+    ...         (0.5, 0.5),
+    ...     ]
+    ... )
     >>> df.geometry = df.buffer([4, 1, 2, 3, 5])
     >>> df["col"] = [None, 1, 2, None, 1]
     >>> df["col2"] = [None, 1, 2, 3, None]
     >>> df["area"] = df.area
     >>> df
                                                 geometry  col  col2       area
     0  POLYGON ((4.56136 0.53436, 4.54210 0.14229, 4....  NaN   NaN  50.184776
@@ -295,24 +325,14 @@
     # using enumerate, then iloc on the sorted dict keys.
     # to avoid creating a temporary area column (which doesn't work for GeoSeries).
     area_mapper = dict(enumerate(gdf.area.values))
     sorted_areas = dict(reversed(sorted(area_mapper.items(), key=lambda item: item[1])))
     return gdf.iloc[list(sorted_areas)]
 
 
-def sort_df(
-    df: pd.DataFrame | GeoDataFrame, sort_col: pd.Series
-) -> pd.DataFrame | GeoDataFrame:
-    value_mapper: dict[int, Any] = dict(enumerate(sort_col.values))
-    sorted_indices = dict(
-        reversed(sorted(value_mapper.items(), key=lambda item: item[1]))
-    )
-    return df.iloc[list(sorted_indices)]
-
-
 def sort_long_first(gdf: GeoDataFrame | GeoSeries) -> GeoDataFrame | GeoSeries:
     """Sort GeoDataFrame by length in decending order.
 
     Args:
         gdf: A GeoDataFrame or GeoSeries.
 
     Returns:
@@ -398,15 +418,15 @@
     Args:
         n: Number of points/rows to create.
         loc: Mean ('centre') of the distribution.
 
     Returns:
         A GeoDataFrame of points with n rows.
 
-    Examples
+    Examples:
     --------
     >>> import sgis as sg
     >>> points = sg.random_points(10_000)
     >>> points
                          geometry
     0     POINT (0.62044 0.22805)
     1     POINT (0.31885 0.38109)
@@ -447,14 +467,24 @@
 
     return GeoDataFrame(
         (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
     )
 
 
 def random_points_in_polygons(gdf: GeoDataFrame, n: int, seed=None) -> GeoDataFrame:
+    """Creates a GeoDataFrame with n random points within the geometries of 'gdf'.
+
+    Args:
+        gdf: A GeoDataFrame.
+        n: Number of points/rows to create.
+        seed: Optional random seet.
+
+    Returns:
+        A GeoDataFrame of points with n rows.
+    """
     all_points = []
 
     rng = np.random.default_rng(seed)
 
     for i, geom in enumerate(gdf.geometry):
         minx, miny, maxx, maxy = geom.bounds
 
@@ -488,15 +518,15 @@
             GeoDataFrames.
 
     Note:
         The index is preserved if only one GeoDataFrame is given, but otherwise
         ignored. This is because the union overlay used if multiple GeoDataFrames
         always ignores the index.
 
-    Examples
+    Examples:
     --------
     Convert single polygon to linestring.
 
     >>> import sgis as sg
     >>> from shapely.geometry import Polygon
     >>> poly1 = sg.to_gdf(Polygon([(0, 0), (0, 1), (1, 1), (1, 0)]))
     >>> poly1["poly1"] = 1
@@ -521,24 +551,22 @@
 
     Plot before and after.
 
     >>> sg.qtm(poly1, poly2)
     >>> lines["l"] = lines.length
     >>> sg.qtm(lines, "l")
     """
-
     if not all(isinstance(gdf, (GeoSeries, GeoDataFrame)) for gdf in gdfs):
         raise TypeError("gdf must be GeoDataFrame or GeoSeries")
 
     if any(gdf.geom_type.isin(["Point", "MultiPoint"]).any() for gdf in gdfs):
         raise ValueError("Cannot convert points to lines.")
 
     def _shapely_geometry_to_lines(geom):
         """Get all lines from the exterior and interiors of a Polygon."""
-
         # if lines (points are not allowed in this function)
         if geom.area == 0:
             return geom
 
         singlepart = get_parts(geom)
         lines = []
         for part in singlepart:
@@ -660,19 +688,19 @@
     elif keep_geom_type:
         geom_type = get_geom_type(gdf)
         if geom_type == "mixed":
             raise ValueError("Cannot set keep_geom_type=True with mixed geometries")
     return gdf, geom_type, keep_geom_type
 
 
-def merge_geometries(geoms: GeoSeries, grid_size=None) -> Geometry:
+def _merge_geometries(geoms: GeoSeries, grid_size=None) -> Geometry:
     return make_valid(unary_union(geoms, grid_size=grid_size))
 
 
-def parallel_unary_union(
+def _parallel_unary_union(
     gdf: GeoDataFrame, n_jobs: int = 1, by=None, grid_size=None, **kwargs
 ) -> list[Geometry]:
     try:
         geom_col = gdf._geometry_column_name
     except AttributeError:
         geom_col = "geometry"
 
@@ -698,15 +726,15 @@
     )
     if _was_none:
         dissolved.crs = None
 
     return dissolved.geometry
 
 
-def parallel_unary_union_geoseries(
+def _parallel_unary_union_geoseries(
     ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
 ) -> list[Geometry]:
     if ser.crs is None:
         ser.crs = 25833
         _was_none = True
     else:
         _was_none = False
@@ -721,61 +749,61 @@
     )
     if _was_none:
         dissolved.crs = None
 
     return dissolved.geometry
 
 
-def parallel_unary_union(
+def _parallel_unary_union(
     gdf: GeoDataFrame, n_jobs: int = 1, by=None, grid_size=None, **kwargs
 ) -> list[Geometry]:
     try:
         geom_col = gdf._geometry_column_name
     except AttributeError:
         geom_col = "geometry"
 
     with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
         delayed_operations = []
         for _, geoms in gdf.groupby(by, **kwargs)[geom_col]:
             delayed_operations.append(
-                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+                joblib.delayed(_merge_geometries)(geoms, grid_size=grid_size)
             )
 
         return parallel(delayed_operations)
 
 
-def parallel_unary_union_geoseries(
+def _parallel_unary_union_geoseries(
     ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
 ) -> list[Geometry]:
 
     is_one_hit = ser.groupby(**kwargs).transform("size") == 1
 
     one_hit = ser.loc[is_one_hit]
     many_hits = ser.loc[~is_one_hit]
 
     with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
         delayed_operations = []
         for _, geoms in many_hits.groupby(**kwargs):
             delayed_operations.append(
-                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+                joblib.delayed(_merge_geometries)(geoms, grid_size=grid_size)
             )
 
         dissolved = pd.Series(
             parallel(delayed_operations),
-            index=is_one_hit[lambda x: x == False].index.unique(),
+            index=is_one_hit[lambda x: x is False].index.unique(),
         )
 
     return pd.concat([dissolved, one_hit]).sort_index().values
 
 
-def parallel_unary_union_geoseries(
+def _parallel_unary_union_geoseries(
     ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
 ) -> list[Geometry]:
 
     with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
         delayed_operations = []
         for _, geoms in ser.groupby(**kwargs):
             delayed_operations.append(
-                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+                joblib.delayed(_merge_geometries)(geoms, grid_size=grid_size)
             )
 
         return parallel(delayed_operations)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/geocoding.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/geocoding.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/geometry_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 """Check and set geometry type."""
+
 import numpy as np
 import pandas as pd
 import shapely
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from geopandas.array import GeometryArray
 from shapely import Geometry
 
 
 def make_all_singlepart(
     gdf: GeoDataFrame | GeoSeries, index_parts: bool = False, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
+    """Make all geometries single part.
+
+    This means doing either 0, 1 or 2 calls to the explode method.
+
+    Args:
+        gdf: GeoDataFrame
+        index_parts: Defaults to False.
+        ignore_index: Defaults to False.
+
+    Returns:
+        A GeoDataFrame of singlepart geometries.
+    """
     # only explode if nessecary
     if (
         index_parts or ignore_index
     ):  # and not gdf.index.equals(pd.Index(range(len(gdf)))):
         gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
 
     while not gdf.geom_type.isin(
@@ -21,15 +35,15 @@
     ).all():
         gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
 
     return gdf
 
 
 def to_single_geom_type(
-    gdf: GeoDataFrame | GeoSeries,
+    gdf: GeoDataFrame | GeoSeries | Geometry | GeometryArray | np.ndarray,
     geom_type: str,
     ignore_index: bool = False,
 ) -> GeoDataFrame | GeoSeries:
     """Returns only the specified geometry type in a GeoDataFrame or GeoSeries.
 
     GeometryCollections are first exploded, then only the rows with the given
     geometry_type is kept. Both multipart and singlepart geometries are kept.
@@ -45,15 +59,15 @@
     Returns:
         A GeoDataFrame with a single geometry type.
 
     Raises:
         TypeError: If incorrect gdf type.
         ValueError: If 'geom_type' is neither 'polygon', 'line' or 'point'.
 
-    Examples
+    Examples:
     --------
     First create a GeoDataFrame of mixed geometries.
 
     >>> from sgis import to_gdf, to_single_geom_type
     >>> from shapely.geometry import LineString, Polygon
     >>> gdf = to_gdf([
     ...     (0, 0),
@@ -92,15 +106,15 @@
     if isinstance(gdf, Geometry):
         return _shapely_to_single_geom_type(gdf, geom_type)
 
     if isinstance(gdf, (np.ndarray, GeometryArray)):
         arr = np.vectorize(_shapely_to_single_geom_type)(gdf, geom_type)
         return arr[~shapely.is_empty(arr)]
 
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):  # type: ignore [unreachable]
         raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
 
     # explode collections to single-typed geometries
     collections = gdf.geom_type == "GeometryCollection"
     if collections.any():
         collections = make_all_singlepart(gdf[collections], ignore_index=ignore_index)
 
@@ -118,15 +132,15 @@
         is_point = gdf.geom_type.isin(["Point", "MultiPoint"])
         if not is_point.all():
             gdf = gdf.loc[is_point]
 
     return gdf.reset_index(drop=True) if ignore_index else gdf
 
 
-def _shapely_to_single_geom_type(geom, geom_type):
+def _shapely_to_single_geom_type(geom: Geometry, geom_type: str) -> Geometry:
     parts = shapely.get_parts(geom)
     return shapely.unary_union(
         [part for part in parts if geom_type.lower() in part.geom_type.lower()]
     )
 
 
 def get_geom_type(gdf: GeoDataFrame | GeoSeries) -> str:
@@ -137,15 +151,15 @@
 
     Returns:
         A string that is either "polygon", "line", "point", or "mixed".
 
     Raises:
         TypeError: If 'gdf' is not of type GeoDataFrame or GeoSeries.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import to_gdf, get_geom_type
     >>> gdf = to_gdf([0, 0])
     >>> gdf
                       geometry
     0  POINT (0.00000 0.00000)
     >>> get_geom_type(gdf)
@@ -185,15 +199,15 @@
 
     Returns:
         True if all geometries are the same type, False if not.
 
     Raises:
         TypeError: If 'gdf' is not of type GeoDataFrame or GeoSeries.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import to_gdf, get_geom_type
     >>> gdf = to_gdf([0, 0])
     >>> gdf
                                                 geometry
     0                            POINT (0.00000 0.00000)
     >>> is_single_geom_type(gdf)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 The results of all functions will be identical with GeoDataFrame and GeoSeries as input
 types.
 """
 
 import numpy as np
 import shapely
-from geopandas import GeoDataFrame, GeoSeries
-from pandas import DataFrame, Series, concat
-from shapely import STRtree
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from pandas import DataFrame
+from pandas import Series
 from sklearn.neighbors import NearestNeighbors
 
 from .conversion import coordinate_array
 from .geometry_types import get_geom_type
 
 
 def get_neighbor_indices(
@@ -44,15 +45,15 @@
         A pandas Series with values of the intersecting 'neighbors' indices.
         The Series' index will follow the index of 'gdf'.
 
     Raises:
         ValueError: If gdf and neighbors do not have the same coordinate reference
             system.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import get_neighbor_indices, to_gdf
     >>> points = to_gdf([(0, 0), (0.5, 0.5)])
     >>> points
                     geometry
     0  POINT (0.00000 0.00000)
     1  POINT (0.50000 0.50000)
@@ -92,15 +93,14 @@
     >>> neighbor_indices.index
     Int64Index([0, 1, 0, 1], dtype='int64')
 
     >>> neighbor_indices.values
     ['a' 'a' 'b' 'b']
 
     """
-
     if gdf.crs != neighbors.crs:
         raise ValueError(f"'crs' mismatch. Got {gdf.crs} and {neighbors.crs}")
 
     if isinstance(neighbors, GeoSeries):
         neighbors = neighbors.to_frame()
 
     # buffer and keep only geometry column
@@ -148,15 +148,15 @@
         DataFrame with the columns 'neighbor_index' and 'distance'. The index follows
         the index of 'gdf'.
 
     Raises:
         ValueError: If the coordinate reference system of 'gdf' and 'neighbors' are
             not the same.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import get_all_distances, random_points
     >>> points = random_points(100)
     >>> neighbors = random_points(100)
 
     >>> distances = get_all_distances(points, neighbors)
     >>> distances
@@ -244,15 +244,14 @@
     gdf: GeoDataFrame | GeoSeries,
     neighbors: GeoDataFrame | GeoSeries,
     distance: int | float,
     distance_col: str = "distance",
     **kwargs,
 ) -> GeoDataFrame:
     """Sjoin with a buffer on the right GeoDataFrame and adds a distance column."""
-
     new_neighbor_cols = {"__left_range_idx": range(len(neighbors))}
     if distance:
         new_neighbor_cols[neighbors._geometry_column_name] = lambda x: x.buffer(
             distance
         )
 
     # using assign to get a copy
@@ -293,15 +292,15 @@
         DataFrame with the columns 'neighbor_index' and 'distance'. The index follows
         the index of 'gdf'.
 
     Raises:
         ValueError: If the coordinate reference system of 'gdf' and 'neighbors' are
             not the same.
 
-    Examples
+    Examples:
     --------
     Make some random points.
 
     >>> from sgis import get_k_nearest_neighbors, random_points
     >>> points = random_points(100)
     >>> neighbors = random_points(100)
 
@@ -426,14 +425,27 @@
 
 def k_nearest_neighbors(
     from_array: np.ndarray[np.ndarray[float]],
     to_array: np.ndarray[np.ndarray[float]],
     k: int | None = None,
     strict: bool = False,
 ) -> tuple[np.ndarray[float], np.ndarray[int]]:
+    """Finds nearest neighbors for an array of coordinates to another array of coordinates.
+
+    Args:
+        from_array: Numpy array of coordinates.
+        to_array: Numpy array of coordinates.
+        k: Number of neighbors to find.
+        strict: If True (not default), an exception is raised
+            if k is larger than the length of 'to_array'.
+
+    Returns a tuple of arrays, one with distances and one with indices
+        of the neighbors.
+
+    """
     if not len(to_array) or not len(from_array):
         return np.array([]), np.array([])
 
     if k is None:
         k = len(to_array)
 
     if not strict:
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/overlay.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,38 @@
 version of the solution from GH 2792.
 
 'clean_overlay' also includes the overlay type "update", which can be specified in the
 "how" parameter, in addition to the five native geopandas how-s.
 """
 
 import functools
+from collections.abc import Callable
 
-import dask
 import dask.array as da
 import geopandas as gpd
 import joblib
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from pandas import DataFrame
-from shapely import (
-    Geometry,
-    STRtree,
-    box,
-    difference,
-    get_parts,
-    intersection,
-    make_valid,
-    unary_union,
-)
+from shapely import Geometry
+from shapely import STRtree
+from shapely import box
+from shapely import difference
+from shapely import intersection
+from shapely import make_valid
+from shapely import unary_union
 from shapely.errors import GEOSException
 
-from .general import (
-    _determine_geom_type_args,
-    clean_geoms,
-    merge_geometries,
-    parallel_unary_union,
-)
-from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
-
+from .general import _determine_geom_type_args
+from .general import clean_geoms
+from .geometry_types import get_geom_type
+from .geometry_types import make_all_singlepart
+from .geometry_types import to_single_geom_type
 
 DEFAULT_GRID_SIZE = None
 DEFAULT_LSUFFIX = "_1"
 DEFAULT_RSUFFIX = "_2"
 
 
 def clean_overlay(
@@ -71,14 +66,18 @@
         keep_geom_type: If True (default), return only geometries of the same
             geometry type as df1 has, if False, return all resulting geometries.
         geom_type: optionally specify what geometry type to keep before the overlay,
             if there are mixed geometry types. Must be either "polygon", "line" or
             "point".
         grid_size: Precision grid size to round the geometries. Will use the highest
             precision of the inputs by default.
+        n_jobs: number of threads.
+        predicate: Spatial predicate in the spatial tree.
+        lsuffix: Suffix of columns in df1 that are also in df2.
+        rsuffix: Suffix of columns in df2 that are also in df1.
 
     Returns:
         GeoDataFrame with overlayed and fixed geometries and columns from both
         GeoDataFrames.
 
     Raises:
         ValueError: If 'how' is not one of 'intersection', 'union', 'identity',
@@ -186,17 +185,18 @@
     return GeoDataFrame(
         pd.DataFrame(columns=cols_with_suffix + [geom_col]),
         geometry=geom_col,
         crs=df1.crs,
     )
 
 
-def _no_intersections_return(df1, df2, how, lsuffix, rsuffix):
-    """Return with no overlay if no intersecting bounding box"""
-
+def _no_intersections_return(
+    df1: GeoDataFrame, df2: GeoDataFrame, how: str, lsuffix, rsuffix: str
+) -> GeoDataFrame:
+    """Return with no overlay if no intersecting bounding box."""
     if how == "intersection":
         return _join_and_get_no_rows(df1, df2, lsuffix, rsuffix)
 
     if how == "difference":
         return df1.reset_index(drop=True)
 
     if how == "identity":
@@ -222,17 +222,17 @@
 
 def _shapely_pd_overlay(
     df1: DataFrame,
     df2: DataFrame,
     how: str,
     grid_size: float = DEFAULT_GRID_SIZE,
     predicate: str = "intersects",
-    lsuffix=DEFAULT_LSUFFIX,
-    rsuffix=DEFAULT_RSUFFIX,
-    geom_type=None,
+    lsuffix: str = DEFAULT_LSUFFIX,
+    rsuffix: str = DEFAULT_RSUFFIX,
+    geom_type: str | None = None,
     n_jobs: int = 1,
 ) -> DataFrame:
     if not grid_size and not len(df1) or not len(df2):
         return _no_intersections_return(df1, df2, how, lsuffix, rsuffix)
 
     tree = STRtree(df2.geometry.values)
     left, right = tree.query(df1.geometry.values, predicate=predicate)
@@ -312,48 +312,73 @@
     overlayed["geometry"] = make_valid(overlayed["geometry"])
     # None and empty are falsy
     overlayed = overlayed.loc[lambda x: x["geometry"].notna()]
 
     return overlayed
 
 
-def _update(pairs, df1, df2, left, grid_size, geom_type, n_jobs) -> GeoDataFrame:
+def _update(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    df2: pd.DataFrame,
+    left: np.ndarray,
+    grid_size: float | None | int,
+    geom_type: str | None,
+    n_jobs: int,
+) -> GeoDataFrame:
     overlayed = _difference(
         pairs, df1, left, grid_size=grid_size, geom_type=geom_type, n_jobs=n_jobs
     )
 
     return overlayed + [df2]
 
 
-def _run_overlay_dask(arr1, arr2, func, n_jobs, grid_size):
+def _run_overlay_dask(
+    arr1: np.ndarray,
+    arr2: np.ndarray,
+    func: Callable,
+    n_jobs: int,
+    grid_size: float | int | None,
+) -> np.ndarray:
     if len(arr1) // n_jobs <= 1:
         try:
             return func(arr1, arr2, grid_size=grid_size)
         except TypeError as e:
-            raise TypeError(e, {type(x) for x in arr1}, {type(x) for x in arr2})
+            raise TypeError(e, {type(x) for x in arr1}, {type(x) for x in arr2}) from e
     arr1 = da.from_array(arr1, chunks=len(arr1) // n_jobs)
     arr2 = da.from_array(arr2, chunks=len(arr2) // n_jobs)
     res = arr1.map_blocks(func, arr2, grid_size=grid_size, dtype=float)
     return res.compute(scheduler="threads", optimize_graph=False, num_workers=n_jobs)
 
 
-def _run_overlay_joblib_threading(arr1, arr2, func, n_jobs, grid_size):
+def _run_overlay_joblib_threading(
+    arr1: np.ndarray,
+    arr2: np.ndarray,
+    func: Callable,
+    n_jobs: int,
+    grid_size: int | float | None,
+) -> list[Geometry]:
     if len(arr1) // n_jobs <= 1:
         try:
             return func(arr1, arr2, grid_size=grid_size)
         except TypeError as e:
-            raise TypeError(e, {type(x) for x in arr1}, {type(x) for x in arr2})
+            raise TypeError(e, {type(x) for x in arr1}, {type(x) for x in arr2}) from e
     with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
         return parallel(
             joblib.delayed(func)(g1, g2, grid_size=grid_size)
             for g1, g2 in zip(arr1, arr2, strict=True)
         )
 
 
-def _intersection(pairs, grid_size, geom_type, n_jobs=1) -> GeoDataFrame:
+def _intersection(
+    pairs: pd.DataFrame,
+    grid_size: None | float | int,
+    geom_type: str | None,
+    n_jobs: int = 1,
+) -> GeoDataFrame:
     if not len(pairs):
         return pairs.drop(columns="geom_right")
 
     intersections = pairs.copy()
 
     arr1 = intersections["geometry"].to_numpy()
     arr2 = intersections["geom_right"].to_numpy()
@@ -406,15 +431,25 @@
         intersections["geometry"] = intersection(
             left.to_numpy(), right.to_numpy(), grid_size=grid_size
         )
 
     return intersections.drop(columns="geom_right")
 
 
-def _union(pairs, df1, df2, left, right, grid_size, rsuffix, geom_type, n_jobs=1):
+def _union(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    df2: pd.DataFrame,
+    left: np.ndarray,
+    right: np.ndarray,
+    grid_size: int | float | None,
+    rsuffix: str,
+    geom_type: str | None,
+    n_jobs: int = 1,
+) -> list[GeoDataFrame]:
     merged = []
     if len(left):
         intersections = _intersection(
             pairs, grid_size=grid_size, geom_type=geom_type, n_jobs=n_jobs
         )
         merged.append(intersections)
     symmdiff = _symmetric_difference(
@@ -428,29 +463,44 @@
         geom_type=geom_type,
         n_jobs=n_jobs,
     )
     merged += symmdiff
     return merged
 
 
-def _identity(pairs, df1, left, grid_size, geom_type, n_jobs=1):
+def _identity(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    left: np.ndarray,
+    grid_size: int | float | None,
+    geom_type: str | None,
+    n_jobs: int = 1,
+) -> list[GeoDataFrame]:
     merged = []
     if len(left):
         intersections = _intersection(
             pairs, grid_size=grid_size, geom_type=geom_type, n_jobs=n_jobs
         )
         merged.append(intersections)
     diff = _difference(pairs, df1, left, grid_size=grid_size, n_jobs=n_jobs)
     merged += diff
     return merged
 
 
 def _symmetric_difference(
-    pairs, df1, df2, left, right, grid_size, rsuffix, geom_type, n_jobs=1
-) -> list:
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    df2: pd.DataFrame,
+    left: np.ndarray,
+    right: np.ndarray,
+    grid_size: int | float | None,
+    rsuffix: str,
+    geom_type: str | None,
+    n_jobs: int = 1,
+) -> list[GeoDataFrame]:
     merged = []
 
     difference_left = _difference(
         pairs, df1, left, grid_size=grid_size, geom_type=geom_type, n_jobs=n_jobs
     )
     merged += difference_left
 
@@ -468,15 +518,22 @@
 
     diff_right = _add_from_right(df1, df2, right, rsuffix)
     merged.append(diff_right)
 
     return merged
 
 
-def _difference(pairs, df1, left, grid_size=None, geom_type=None, n_jobs=1) -> list:
+def _difference(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    left: np.ndarray,
+    grid_size: int | float | None = None,
+    geom_type: str | None = None,
+    n_jobs: int = 1,
+) -> list[GeoDataFrame]:
     merged = []
     if len(left):
         clip_left = _shapely_diffclip_left(
             pairs=pairs,
             df1=df1,
             grid_size=grid_size,
             geom_type=geom_type,
@@ -489,15 +546,15 @@
 
 
 def _get_intersects_pairs(
     df1: GeoDataFrame,
     df2: GeoDataFrame,
     left: np.ndarray,
     right: np.ndarray,
-    rsuffix,
+    rsuffix: str,
 ) -> DataFrame:
     return pd.concat(
         [
             df1.take(left),
             (
                 DataFrame(
                     {"_overlay_index_right": right}, index=df1.index.values.take(left)
@@ -508,50 +565,56 @@
     ).join(
         df2.rename(columns={"geometry": "geom_right"}, errors="raise"),
         on="_overlay_index_right",
         rsuffix=rsuffix,
     )
 
 
-def _add_suffix_left(overlayed, df1, df2, lsuffix):
+def _add_suffix_left(
+    overlayed: pd.DataFrame, df1: pd.DataFrame, df2: pd.DataFrame, lsuffix: str
+):
     """Separating this from _add_indices_from_left, since this suffix is not needed in difference."""
     return overlayed.rename(
         columns={
             c: (
                 f"{c}{lsuffix}"
                 if c in df1.columns and c in df2.columns and c != "geometry"
                 else c
             )
             for c in overlayed.columns
         }
     )
 
 
-def _add_indices_from_left(df1, left):
+def _add_indices_from_left(df1: pd.DataFrame, left: np.ndarray) -> pd.DataFrame:
     return df1.take(np.setdiff1d(np.arange(len(df1)), left))
 
 
 def _add_from_right(
-    df1: GeoDataFrame, df2: GeoDataFrame, right: np.ndarray, rsuffix
+    df1: GeoDataFrame, df2: GeoDataFrame, right: np.ndarray, rsuffix: str
 ) -> GeoDataFrame:
     return df2.take(np.setdiff1d(np.arange(len(df2)), right)).rename(
         columns={
             c: f"{c}{rsuffix}" if c in df1.columns and c != "geometry" else c
             for c in df2.columns
         }
     )
 
 
-def _shapely_diffclip_left(pairs, df1, grid_size, geom_type, n_jobs):
-    """Aggregate areas in right by unique values of left, then use those to clip
-    areas out of left"""
-
+def _shapely_diffclip_left(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    grid_size: int | float | None,
+    geom_type: str | None,
+    n_jobs: int,
+) -> pd.DataFrame:
+    """Aggregate areas in right by unique values from left, then erases those from left."""
     keep_cols = list(df1.columns.difference({"_overlay_index_right"})) + ["geom_right"]
 
-    agg_geoms_partial = functools.partial(agg_geoms, grid_size=grid_size)
+    agg_geoms_partial = functools.partial(_agg_geoms, grid_size=grid_size)
 
     try:
         only_one = pairs.groupby(level=0).transform("size") == 1
         one_hit = pairs.loc[only_one, list(keep_cols)]
         many_hits = pairs.loc[~only_one, list(keep_cols) + ["_overlay_index_right"]]
         # keep first in non-geom-cols, agg only geom col bacause of speed
         many_hits_agged = many_hits.loc[
@@ -588,15 +651,17 @@
             .explode()
             .to_frame("_overlay_index_right")
         )
         agger["geom_right"] = agger["_overlay_index_right"].map(
             {
                 i: g
                 for i, g in zip(
-                    many_hits["_overlay_index_right"], many_hits["geom_right"]
+                    many_hits["_overlay_index_right"],
+                    many_hits["geom_right"],
+                    strict=False,
                 )
             }
         )
 
         agged = pd.Series(
             {
                 i: agg_geoms_partial(geoms)
@@ -620,16 +685,24 @@
         geom_type=geom_type,
         n_jobs=n_jobs,
     )
 
     return clip_left.drop(columns="geom_right")
 
 
-def _shapely_diffclip_right(pairs, df1, df2, grid_size, rsuffix, geom_type, n_jobs):
-    agg_geoms_partial = functools.partial(agg_geoms, grid_size=grid_size)
+def _shapely_diffclip_right(
+    pairs: pd.DataFrame,
+    df1: pd.DataFrame,
+    df2: pd.DataFrame,
+    grid_size: int | float | None,
+    rsuffix: str,
+    geom_type: str | None,
+    n_jobs: int,
+) -> pd.DataFrame:
+    agg_geoms_partial = functools.partial(_agg_geoms, grid_size=grid_size)
 
     pairs = pairs.rename(columns={"geometry": "geom_left", "geom_right": "geometry"})
 
     try:
         only_one = pairs.groupby("_overlay_index_right").transform("size") == 1
         one_hit = pairs[only_one].set_index("_overlay_index_right")[
             ["geom_left", "geometry"]
@@ -671,15 +744,21 @@
         grid_size=grid_size,
         geom_type=geom_type,
     )
 
     return clip_right.drop(columns="geom_left")
 
 
-def _try_difference(left, right, grid_size, geom_type, n_jobs=1):
+def _try_difference(
+    left: np.ndarray,
+    right: np.ndarray,
+    grid_size: int | float | None,
+    geom_type: str | None,
+    n_jobs: int = 1,
+) -> np.ndarray:
     """Try difference overlay, then make_valid and retry."""
     if n_jobs > 1 and len(left) / n_jobs > 10:
         try:
             return _run_overlay_joblib_threading(
                 left,
                 right,
                 func=difference,
@@ -718,31 +797,35 @@
         try:
             return difference(
                 left.to_numpy(),
                 right.to_numpy(),
                 grid_size=grid_size,
             )
         except GEOSException as e:
-            raise e.__class__(e, f"{grid_size=}", f"{left=}", f"{right=}")
+            raise e.__class__(e, f"{grid_size=}", f"{left=}", f"{right=}") from e
 
 
 def make_valid_and_keep_geom_type(
-    geoms: np.ndarray, geom_type: str, n_jobs
+    geoms: np.ndarray, geom_type: str, n_jobs: int
 ) -> GeoSeries:
     """Make GeometryCollections into (Multi)Polygons, (Multi)LineStrings or (Multi)Points.
 
     Because GeometryCollections might appear after dissolving (unary_union).
     And this makes shapely difference/intersection fail.
 
+    Args:
+        geoms: Array of geometries.
+        geom_type: geometry type to be kept.
+        n_jobs: Number of treads.
     """
     geoms = GeoSeries(geoms)
     geoms.index = range(len(geoms))
     geoms.loc[:] = make_valid(geoms.to_numpy())
     geoms = geoms.explode(index_parts=False).pipe(to_single_geom_type, geom_type)
     only_one = geoms.groupby(level=0).transform("size") == 1
     one_hit = geoms[only_one]
     many_hits = geoms[~only_one].groupby(level=0).agg(unary_union)
     return pd.concat([one_hit, many_hits]).sort_index()
 
 
-def agg_geoms(g, grid_size=None):
+def _agg_geoms(g: np.ndarray, grid_size: int | float | None = None) -> Geometry:
     return make_valid(unary_union(g, grid_size=grid_size))
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/point_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Functions for point geometries."""
 
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
-from shapely import distance, snap, unary_union
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from shapely import distance
+from shapely import unary_union
 from shapely.ops import nearest_points
 
-from ..geopandas_tools.general import to_lines
-from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
+from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.geometry_types import to_single_geom_type
 from ..geopandas_tools.polygon_operations import PolygonsAsRings
 
 
 def snap_within_distance(
     points: GeoDataFrame | GeoSeries,
     to: GeoDataFrame | GeoSeries,
     max_distance: int | float,
@@ -41,15 +43,15 @@
         chosen as the snap geometry. This will usually only happen with constructed
         data like grids or in the examples below.
 
         The snap point might be in between vertices of lines and polygons. Convert the
         'to' geometries to multipoint before snapping if the snap points should be
         vertices.
 
-    Examples
+    Examples:
     --------
     Create som points.
 
     >>> from sgis import snap_within_distance, to_gdf
     >>> points = to_gdf([(0, 0), (1, 1)])
     >>> points
                     geometry
@@ -72,15 +74,14 @@
     0  POINT (0.00000 0.00000)          <NA>
     1  POINT (2.00000 2.00000)      1.414214
     >>> snap_within_distance(points, to, 3)
                     geometry snap_distance
     0  POINT (2.00000 2.00000)      2.828427
     1  POINT (2.00000 2.00000)      1.414214
     """
-
     to = _polygons_to_rings(to)
 
     if not distance_col and not isinstance(points, GeoDataFrame):
         return _shapely_snap(
             points=points,
             to=to,
             max_distance=max_distance,
@@ -130,15 +131,15 @@
         chosen as the snap geometry. This will usually only happen with constructed
         data like grids or in the examples below.
 
         The snap point might be in between vertices of lines and polygons. Convert the
         'to' geometries to multipoint before snapping if the snap points should be
         vertices.
 
-    Examples
+    Examples:
     --------
     Create som points.
 
     >>> from sgis import snap_all, to_gdf
     >>> points = to_gdf([(0, 0), (1, 1)])
     >>> points
                     geometry
@@ -179,15 +180,15 @@
         copied[distance_col] = copied.distance(points)
         copied[distance_col] = np.where(
             copied[distance_col] == 0, pd.NA, copied[distance_col]
         )
     return copied
 
 
-def _polygons_to_rings(gdf):
+def _polygons_to_rings(gdf: GeoDataFrame) -> GeoDataFrame:
     if get_geom_type(gdf) == "polygon":
         return PolygonsAsRings(gdf).get_rings()
     if get_geom_type(gdf) != "mixed":
         return gdf
     gdf_points = to_single_geom_type(gdf, "point")
     gdf_lines = to_single_geom_type(gdf, "line")
     gdf_polys = PolygonsAsRings(to_single_geom_type(gdf, "polygon")).get_rings()
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 """Functions for polygon geometries."""
 
 import networkx as nx
 import numpy as np
 import pandas as pd
-import shapely
-from geopandas import GeoDataFrame, GeoSeries
-from geopandas.array import GeometryArray
-from shapely import (
-    STRtree,
-    area,
-    box,
-    buffer,
-    difference,
-    get_exterior_ring,
-    get_interior_ring,
-    get_num_interior_rings,
-    get_parts,
-    is_empty,
-    make_valid,
-    polygons,
-    unary_union,
-)
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from shapely import STRtree
+from shapely import area
+from shapely import box
+from shapely import buffer
+from shapely import difference
+from shapely import get_exterior_ring
+from shapely import get_interior_ring
+from shapely import get_num_interior_rings
+from shapely import get_parts
+from shapely import is_empty
+from shapely import make_valid
+from shapely import polygons
+from shapely import unary_union
 from shapely.errors import GEOSException
 
-from .duplicates import get_intersections
-from .general import (
-    _push_geom_col,
-    clean_geoms,
-    get_grouped_centroids,
-    parallel_unary_union,
-    parallel_unary_union_geoseries,
-    to_lines,
-)
-from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
+from .general import _parallel_unary_union
+from .general import _parallel_unary_union_geoseries
+from .general import _push_geom_col
+from .general import clean_geoms
+from .general import get_grouped_centroids
+from .general import to_lines
+from .geometry_types import get_geom_type
+from .geometry_types import make_all_singlepart
+from .geometry_types import to_single_geom_type
 from .neighbors import get_neighbor_indices
-from .overlay import _try_difference, clean_overlay
+from .overlay import _try_difference
+from .overlay import clean_overlay
 from .polygons_as_rings import PolygonsAsRings
-from .sfilter import sfilter, sfilter_inverse
+from .sfilter import sfilter
+from .sfilter import sfilter_inverse
 
 
 def get_polygon_clusters(
     *gdfs: GeoDataFrame | GeoSeries,
     cluster_col: str = "cluster",
     allow_multipart: bool = False,
     predicate: str | None = "intersects",
@@ -59,24 +57,24 @@
     polygons overlap.
 
     Args:
         gdfs: One or more GeoDataFrames of polygons.
         cluster_col: Name of the resulting cluster column.
         allow_multipart: Whether to allow mutipart geometries in the gdfs.
             Defaults to False to avoid confusing results.
+        predicate: Spatial predicate. Defaults to "intersects".
         as_string: Whether to return the cluster column values as a string with x and y
             coordinates. Convinient to always get unique ids.
             Defaults to False because of speed.
 
     Returns:
         One or more GeoDataFrames (same amount as was given) with a new cluster column.
 
-    Examples
+    Examples:
     --------
-
     Create geometries with three clusters of overlapping polygons.
 
     >>> import sgis as sg
     >>> gdf = sg.to_gdf([(0, 0), (1, 1), (0, 1), (4, 4), (4, 3), (7, 7)])
     >>> buffered = sg.buff(gdf, 1)
     >>> gdf
                                                 geometry
@@ -182,15 +180,17 @@
         gdf.index = orig_indices[i]
         gdf = gdf.drop(["i__"], axis=1)
         unconcated = unconcated + (gdf,)
 
     return unconcated
 
 
-def get_cluster_mapper(gdf, predicate="intersects"):
+def get_cluster_mapper(
+    gdf: GeoDataFrame | GeoSeries, predicate: str = "intersects"
+) -> dict[int, int]:
     if not gdf.index.is_unique:
         raise ValueError("Index must be unique")
     neighbors = get_neighbor_indices(gdf, gdf, predicate=predicate)
 
     edges = [(source, target) for source, target in neighbors.items()]
 
     graph = nx.Graph()
@@ -237,23 +237,24 @@
             0, 1, …, n - 1.
         aggfunc: Aggregation function(s) to use when dissolving/eliminating.
             Defaults to None, meaning the values of 'gdf' is used. Otherwise,
             aggfunc will be passed to pandas groupby.agg. note: The geometries of
             'gdf' are sorted first, but if 'gdf' has missing values, the resulting
             polygons might get values from the polygons to be eliminated
             (if aggfunc="first").
-        kwargs: Keyword arguments passed to the dissolve method.
+        grid_size: Rounding of the coordinates. Defaults to None.
+        n_jobs: Number of threads to use. Defaults to 1.
+        **kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame (gdf) with the geometries of 'to_eliminate' dissolved in.
         If multiple GeoDataFrame are passed as 'gdf', they are returned as a tuple.
 
-    Examples
+    Examples:
     --------
-
     Create two polygons with a sliver in between:
 
     >>> sliver = sg.to_gdf(Polygon([(0, 0), (0.1, 1), (0, 2), (-0.1, 1)]))
     >>> small_poly = sg.to_gdf(
     ...     Polygon([(0, 0), (-0.1, 1), (0, 2), (-1, 2), (-2, 2), (-1, 1)])
     ... )
     >>> large_poly = sg.to_gdf(
@@ -394,14 +395,16 @@
     Eliminates selected geometries by dissolving them with the neighboring
     polygon with the largest area. The index and column values of the
     large polygons will be kept, unless else is specified.
 
     Args:
         gdf: GeoDataFrame with polygon geometries, or a list of GeoDataFrames.
         to_eliminate: The geometries to be eliminated by 'gdf'.
+        max_distance: Max distance to search for neighbors. Defaults to None, meaning
+            0.
         remove_isolated: If False (default), polygons in 'to_eliminate' that share
             no border with any polygon in 'gdf' will be kept. If True, the isolated
             polygons will be removed.
         fix_double: If True, geometries to be eliminated will be erased by overlapping
             geometries to not get double surfaces if the geometries in 'to_eliminate'
             overlaps with multiple geometries in 'gdf'.
         ignore_index: If False (default), the resulting GeoDataFrame will keep the
@@ -410,23 +413,24 @@
         aggfunc: Aggregation function(s) to use when dissolving/eliminating.
             Defaults to None, meaning the values of 'gdf' is used. Otherwise,
             aggfunc will be passed to pandas groupby.agg. note: The geometries of
             'gdf' are sorted first, but if 'gdf' has missing values, the resulting
             polygons might get values from the polygons to be eliminated
             (if aggfunc="first").
         predicate: Binary predicate passed to sjoin. Defaults to "intersects".
-        kwargs: Keyword arguments passed to the dissolve method.
+        grid_size: Rounding of the coordinates. Defaults to None.
+        n_jobs: Number of threads to use. Defaults to 1.
+        **kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame (gdf) with the geometries of 'to_eliminate' dissolved in.
         If multiple GeoDataFrame are passed as 'gdf', they are returned as a tuple.
 
-    Examples
+    Examples:
     --------
-
     Create two polygons with a sliver in between:
 
     >>> sliver = sg.to_gdf(Polygon([(0, 0), (0.1, 1), (0, 2), (-0.1, 1)]))
     >>> small_poly = sg.to_gdf(
     ...     Polygon([(0, 0), (-0.1, 1), (0, 2), (-1, 2), (-2, 2), (-1, 1)])
     ... )
     >>> large_poly = sg.to_gdf(
@@ -696,15 +700,15 @@
             grid_size=grid_size,
             n_jobs=n_jobs,
             geom_type="polygon",
         )
 
         if n_jobs > 1:
             eliminated["geometry"] = GeoSeries(
-                parallel_unary_union_geoseries(
+                _parallel_unary_union_geoseries(
                     pd.concat([eliminators, soon_erased, missing]),
                     level=0,
                     grid_size=grid_size,
                     n_jobs=n_jobs,
                 ),
                 index=eliminated.index,
             )
@@ -717,15 +721,15 @@
                         unary_union(x.dropna().values, grid_size=grid_size)
                     )
                 )
             )
 
     else:
         if n_jobs > 1:
-            eliminated["geometry"] = parallel_unary_union(
+            eliminated["geometry"] = _parallel_unary_union(
                 many_hits, by="_dissolve_idx", grid_size=grid_size, n_jobs=n_jobs
             )
         else:
             eliminated["geometry"] = many_hits.groupby("_dissolve_idx")["geometry"].agg(
                 lambda x: make_valid(unary_union(x.values, grid_size=grid_size))
             )
 
@@ -769,24 +773,14 @@
 
     if not (gdf.geom_type == "Polygon").all():
         raise ValueError(gdf.geom_type.value_counts())
 
     return PolygonsAsRings(gdf).apply_numpy_func_to_interiors(to_none_if_thin).to_gdf()
 
 
-def return_correct_geometry_object(in_obj, out_obj):
-    if isinstance(in_obj, GeoDataFrame):
-        in_obj.geometry = out_obj
-        return in_obj
-    elif isinstance(in_obj, GeoSeries):
-        return GeoSeries(out_obj, crs=in_obj.crs)
-    else:
-        return out_obj
-
-
 def close_all_holes(
     gdf: GeoDataFrame | GeoSeries,
     *,
     ignore_islands: bool = False,
     copy: bool = True,
 ) -> GeoDataFrame | GeoSeries:
     """Closes all holes in polygons.
@@ -804,15 +798,15 @@
             duplicate surfaces in the resulting geometries.
             Note that ignoring islands is a lot faster.
 
     Returns:
         A GeoDataFrame or GeoSeries of polygons with closed holes in the geometry
         column.
 
-    Examples
+    Examples:
     --------
     Let's create a circle with a hole in it.
 
     >>> point = sg.to_gdf([260000, 6650000], crs=25833)
     >>> point
                             geometry
     0  POINT (260000.000 6650000.000)
@@ -893,17 +887,16 @@
         column.
 
     Raises:
         ValueError: If the coordinate reference system of the GeoDataFrame is not in
             meter units.
         ValueError: If both 'max_m2' and 'max_km2' is given.
 
-    Examples
+    Examples:
     --------
-
     Let's create a circle with a hole in it.
 
     >>> point = sg.to_gdf([260000, 6650000], crs=25833)
     >>> point
                             geometry
     0  POINT (260000.000 6650000.000)
     >>> circle = sg.buff(point, 1000)
@@ -980,15 +973,14 @@
             return gdf
         else:
             return GeoSeries(results, crs=gdf.crs)
 
 
 def _close_small_holes_no_islands(poly, max_area, all_geoms):
     """Closes small holes within one shapely geometry of polygons."""
-
     # start with a list containing the polygon,
     # then append all holes smaller than 'max_km2' to the list.
     holes_closed = [poly]
     singlepart = get_parts(poly)
     for part in singlepart:
         n_interior_rings = get_num_interior_rings(part)
 
@@ -1006,15 +998,14 @@
                 holes_closed.append(no_islands)
 
     return make_valid(unary_union(holes_closed))
 
 
 def _close_all_holes_no_islands(poly, all_geoms):
     """Closes all holes within one shapely geometry of polygons."""
-
     # start with a list containing the polygon,
     # then append all holes smaller than 'max_km2' to the list.
     holes_closed = [poly]
     singlepart = get_parts(poly)
     for part in singlepart:
         n_interior_rings = get_num_interior_rings(part)
 
@@ -1037,14 +1028,15 @@
 ) -> GeoDataFrame:
     """Get the gaps between polygons.
 
     Args:
         gdf: GeoDataFrame of polygons.
         include_interiors: If False (default), the holes inside individual polygons
             will not be included as gaps.
+        grid_size: Rounding of the coordinates.
 
     Note:
         See get_holes to find holes inside singlepart polygons.
 
     Returns:
         GeoDataFrame of polygons with only a geometry column.
     """
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/polygons_as_rings.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/polygons_as_rings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,50 @@
-from typing import Any, Callable, Iterable
+from collections.abc import Callable
+from typing import Any
 
-import geopandas as gpd
-import igraph
-import networkx as nx
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from geopandas.array import GeometryArray
-from IPython.display import display
-from networkx.algorithms import approximation as approx
-from numpy import ndarray
 from numpy.typing import NDArray
-from pandas import Index
-from shapely import (
-    Geometry,
-    STRtree,
-    area,
-    box,
-    buffer,
-    centroid,
-    difference,
-    distance,
-    extract_unique_points,
-    get_coordinates,
-    get_exterior_ring,
-    get_interior_ring,
-    get_num_interior_rings,
-    get_parts,
-    intersection,
-    intersects,
-    is_empty,
-    is_ring,
-    length,
-    line_merge,
-    linearrings,
-    linestrings,
-    make_valid,
-    points,
-    polygons,
-    segmentize,
-    simplify,
-    unary_union,
-    voronoi_polygons,
-)
-from shapely.errors import GEOSException
-from shapely.geometry import (
-    LinearRing,
-    LineString,
-    MultiLineString,
-    MultiPoint,
-    Point,
-    Polygon,
-)
+from pyproj import CRS
+from shapely import get_coordinates
+from shapely import get_exterior_ring
+from shapely import get_interior_ring
+from shapely import get_num_interior_rings
+from shapely import linearrings
+from shapely import make_valid
+from shapely import polygons
+from shapely import unary_union
+from shapely.geometry import LinearRing
+from shapely.geometry import Polygon
 
-from .conversion import to_gdf, to_geoseries
+from .conversion import to_gdf
+from .conversion import to_geoseries
 
 
 class PolygonsAsRings:
     """Convert polygons to linearrings, apply linestring functions, then convert back to polygons."""
 
     def __init__(
         self,
         polys: GeoDataFrame | GeoSeries | GeometryArray,
-        crs=None,
+        crs: CRS | Any | None = None,
         allow_multipart: bool = False,
         gridsize: int | None = None,
-    ):
+    ) -> None:
+        """Initialize the PolygonsAsRings object with polygons and optional CRS information.
+
+        Args:
+            polys: GeoDataFrame, GeoSeries, or GeometryArray containing polygon geometries.
+            crs: Coordinate Reference System to be used, defaults to None.
+            allow_multipart: Allow multipart polygons if True, defaults to False.
+            gridsize: Size of the grid for any grid operations, defaults to None.
+        """
         if not isinstance(polys, (pd.DataFrame, pd.Series, GeometryArray)):
             raise TypeError(type(polys))
 
         self.polyclass = polys.__class__
 
         if not isinstance(polys, pd.DataFrame):
             polys = to_gdf(polys, crs)
@@ -121,15 +96,24 @@
 
         interiors.index = self._interiors_index
 
         interiors = interiors.dropna()
 
         self.rings = pd.concat([exterior, interiors])
 
-    def get_rings(self, agg: bool = False):
+    def get_rings(self, agg: bool = False) -> GeoDataFrame | GeoSeries | np.ndarray:
+        """Retrieve rings from the polygons, optionally aggregating them.
+
+        Args:
+            agg: If True, aggregate the rings into single geometries.
+
+        Returns:
+            The rings either aggregated or separated, in the type of
+                the input polygons.
+        """
         gdf = self.gdf.copy()
         rings = self.rings.copy()
         if not len(rings):
             return GeoSeries()
         if agg:
             gdf.geometry = rings.groupby(level=1).agg(unary_union)
         else:
@@ -140,102 +124,152 @@
         if issubclass(self.polyclass, pd.DataFrame):
             return GeoDataFrame(gdf, crs=self.crs)
         if issubclass(self.polyclass, pd.Series):
             return GeoSeries(gdf.geometry)
         return self.polyclass(gdf.geometry.values)
 
     def apply_numpy_func_to_interiors(
-        self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
-    ):
-        """Run an array function on only the interior rings of the polygons."""
+        self,
+        func: Callable,
+        args: tuple | None = None,
+        kwargs: dict | None = None,
+    ) -> "PolygonsAsRings":
+        """Apply a numpy function specifically to the interior rings of the polygons.
+
+        Args:
+            func: Numpy function to apply.
+            args: Tuple of positional arguments for the function.
+            kwargs: Dictionary of keyword arguments for the function.
+
+        Returns:
+            PolygonsAsRings: The instance itself after applying the function.
+        """
         kwargs = kwargs or {}
         args = args or ()
         arr: NDArray[LinearRing] = self.rings.loc[self.is_interior].values
         index: pd.Index = self.rings.loc[self.is_interior].index
         results = pd.Series(
             np.array(func(arr, *args, **kwargs)),
             index=index,
         )
         self.rings.loc[self.is_interior] = results
         return self
 
     def apply_numpy_func(
-        self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
-    ):
-        """Run a function that takes an array of lines/rings and returns an array of lines/rings."""
+        self,
+        func: Callable,
+        args: tuple | None = None,
+        kwargs: dict | None = None,
+    ) -> "PolygonsAsRings":
+        """Apply a numpy function to all rings of the polygons.
+
+        Args:
+            func: Numpy function to apply.
+            args: Tuple of positional arguments for the function.
+            kwargs: Dictionary of keyword arguments for the function.
+
+        Returns:
+            PolygonsAsRings: The instance itself after applying the function.
+        """
         kwargs = kwargs or {}
         args = args or ()
 
         results = np.array(func(self.rings.values, *args, **kwargs))
 
         if len(results) != len(self.rings):
             raise ValueError(
                 f"Different length of results. Got {len(results)} and {len(self.rings)} original rings"
             )
 
-        self.rings.loc[:] = results
+        self.rings.loc[:] = results  # type: ignore [call-overload]
 
         return self
 
     def apply_geoseries_func(
-        self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
-    ):
-        """Run a function that takes a GeoSeries and returns a GeoSeries."""
+        self,
+        func: Callable,
+        args: tuple | None = None,
+        kwargs: dict | None = None,
+    ) -> "PolygonsAsRings":
+        """Apply a function that operates on a GeoSeries to the rings.
+
+        Args:
+            func: Function to apply that expects a GeoSeries.
+            args: Tuple of positional arguments for the function.
+            kwargs: Dictionary of keyword arguments for the function.
+
+        Returns:
+            PolygonsAsRings: The instance itself after applying the function.
+        """
         kwargs = kwargs or {}
         args = args or ()
 
-        self.rings.loc[:] = np.array(
+        self.rings.loc[:] = np.array(  # type: ignore [call-overload]
             func(
                 GeoSeries(
                     self.rings.values,
                     crs=self.crs,
                     index=self.rings.index.get_level_values(1).map(self._index_mapper),
                 ),
                 *args,
                 **kwargs,
             )
         )
 
         return self
 
     def apply_gdf_func(
-        self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
-    ):
-        """Run a function that takes a GeoDataFrame and returns a GeoDataFrame."""
+        self,
+        func: Callable,
+        args: tuple | None = None,
+        kwargs: dict | None = None,
+    ) -> "PolygonsAsRings":
+        """Apply a function that operates on a GeoDataFrame to the rings.
+
+        Args:
+            func: Function to apply that expects a GeoDataFrame.
+            args: Tuple of positional arguments for the function.
+            kwargs: Dictionary of keyword arguments for the function.
+
+        Returns:
+            PolygonsAsRings: The instance itself after applying the function.
+        """
         kwargs = kwargs or {}
         args = args or ()
 
         gdf = GeoDataFrame(
             {"geometry": self.rings.values},
             crs=self.crs,
             index=self.rings.index.get_level_values(1).map(self._index_mapper),
         ).join(self.gdf.drop(columns="geometry"))
 
         assert len(gdf) == len(self.rings)
 
         gdf.index = self.rings.index
 
-        self.rings.loc[:] = func(
+        self.rings.loc[:] = func(  # type: ignore [call-overload]
             gdf,
             *args,
             **kwargs,
         ).geometry.values
 
         return self
 
     @property
-    def is_interior(self):
+    def is_interior(self) -> bool:
+        """Returns a boolean Series of whether the row is an interior ring."""
         return self.rings.index.get_level_values(0) == 1
 
     @property
-    def is_exterior(self):
+    def is_exterior(self) -> bool:
+        """Returns a boolean Series of whether the row is an exterior ring."""
         return self.rings.index.get_level_values(0) == 0
 
     @property
-    def _interiors_index(self):
+    def _interiors_index(self) -> pd.MultiIndex:
         """A three-leveled MultiIndex.
 
         Used to separate interior and exterior and sort the interior in
         the 'to_numpy' method.
 
         level 0: all 1s, indicating "is interior".
         level 1: gdf index repeated *self.max_rings* times.
@@ -250,15 +284,15 @@
         one_for_interior = np.repeat(1, n_potential_interiors)
 
         return pd.MultiIndex.from_arrays(
             [one_for_interior, gdf_index, interior_number_index]
         )
 
     @property
-    def _exterior_index(self):
+    def _exterior_index(self) -> pd.MultiIndex:
         """A three-leveled MultiIndex.
 
         Used to separate interior and exterior in the 'to_numpy' method.
         Only leve 1 is used for the exterior.
 
         level 0: all 0s, indicating "not interior".
         level 1: gdf index.
@@ -270,16 +304,16 @@
         )
 
     def to_gdf(self) -> GeoDataFrame:
         """Return the GeoDataFrame with polygons."""
         self.gdf.geometry = self.to_numpy()
         return self.gdf
 
-    def to_geoseries(self) -> GeoDataFrame:
-        """Return the GeoDataFrame with polygons."""
+    def to_geoseries(self) -> GeoSeries:
+        """Return the GeoSeries with polygons."""
         self.gdf.geometry = self.to_numpy()
         return self.gdf.geometry
 
     def to_numpy(self) -> NDArray[Polygon]:
         """Return a numpy array of polygons."""
         if not len(self.rings):
             return np.array([])
@@ -289,15 +323,15 @@
 
         nonempty_interiors = self.rings.loc[self.is_interior]
 
         if not len(nonempty_interiors):
             try:
                 return make_valid(polygons(exterior.values))
             except Exception:
-                return _geoms_to_linearrings_fallback(exterior)
+                return _geoms_to_linearrings_fallback(exterior).values
 
         empty_interiors = pd.Series(
             [None for _ in range(len(self.gdf) * self.max_rings)],
             index=self._interiors_index,
         ).loc[lambda x: ~x.index.isin(nonempty_interiors.index)]
 
         interiors = (
@@ -308,27 +342,36 @@
             .sort_index()
         )
         assert interiors.shape == (len(self.gdf), self.max_rings), interiors.shape
 
         try:
             return make_valid(polygons(exterior.values, interiors.values))
         except Exception:
-            return _geoms_to_linearrings_fallback(exterior, interiors)
+            return _geoms_to_linearrings_fallback(exterior, interiors).values
+
+
+def get_linearring_series(geoms: GeoDataFrame | GeoSeries) -> pd.Series:
+    """Convert geometries into a series of LinearRings.
 
+    Args:
+        geoms: GeoDataFrame or GeoSeries from which to extract LinearRings.
 
-def get_linearring_series(geoms: Any) -> pd.Series:
+    Returns:
+        pd.Series: A series containing LinearRings.
+    """
     geoms = to_geoseries(geoms).explode(index_parts=False)
     coords, indices = get_coordinates(geoms, return_index=True)
     return pd.Series(linearrings(coords, indices=indices), index=geoms.index)
 
 
 def _geoms_to_linearrings_fallback(
     exterior: pd.Series, interiors: pd.Series | None = None
 ) -> pd.Series:
     exterior.index = exterior.index.get_level_values(1)
+    assert exterior.index.is_monotonic_increasing
 
     exterior = get_linearring_series(exterior)
 
     if interiors is None:
         return (
             pd.Series(
                 make_valid(polygons(exterior.values)),
```

### Comparing `ssb_sgis-1.0.1/src/sgis/geopandas_tools/sfilter.py` & `ssb_sgis-1.0.2/src/sgis/geopandas_tools/sfilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import warnings
 
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from shapely import Geometry
 
 from .conversion import to_gdf
 
-
 gdf_type_error_message = "'gdf' should be of type GeoDataFrame or GeoSeries."
 
 
 def sfilter(
     gdf: GeoDataFrame | GeoSeries,
     other: GeoDataFrame | GeoSeries | Geometry,
     predicate: str = "intersects",
@@ -30,17 +30,17 @@
         other: The geometry object to filter 'gdf' by.
         predicate: Spatial predicate to use. Defaults to 'intersects'.
 
     Returns:
         A copy of 'gdf' with only the rows matching the
         spatial predicate with 'other'.
 
-    Examples
+    Examples:
     --------
-
+    >>> import sgis as sg
     >>> df1 = sg.to_gdf([(0, 0), (0, 1)])
     >>> df1
                       geometry
     0  POINT (0.00000 0.00000)
     1  POINT (0.00000 1.00000)
     >>> df2 = sg.to_gdf([(0, 0), (1, 2)])
     >>> df2
@@ -67,15 +67,15 @@
     is often a lot slower since df2 must be dissolved:
 
     >>> df1.loc[df1.intersects(df2.unary_union)]
                       geometry
     0  POINT (0.00000 0.00000)
 
     """
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+    if not isinstance(gdf, (GeoDataFrame | GeoSeries)):
         raise TypeError(gdf_type_error_message)
 
     other = _sfilter_checks(other, crs=gdf.crs)
 
     indices = _get_sfilter_indices(gdf, other, predicate)
 
     return gdf.iloc[indices]
@@ -96,17 +96,17 @@
         other: The geometry object to filter 'gdf' by.
         predicate: Spatial predicate to use. Defaults to 'intersects'.
 
     Returns:
         A tuple of GeoDataFrames, one with the rows that match the spatial predicate
         and one with the rows that do not.
 
-    Examples
+    Examples:
     --------
-
+    >>> import sgis as sg
     >>> df1 = sg.to_gdf([(0, 0), (0, 1)])
     >>> df1
                       geometry
     0  POINT (0.00000 0.00000)
     1  POINT (0.00000 1.00000)
     >>> df2 = sg.to_gdf([(0, 0), (1, 2)])
     >>> df2
@@ -136,24 +136,24 @@
     is often slower since df2 must be dissolved:
 
     >>> filt = df1.intersects(df2.unary_union)
     >>> intersecting = df1.loc[filt]
     >>> not_intersecting = df1.loc[~filt]
 
     """
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+    if not isinstance(gdf, (GeoDataFrame | GeoSeries)):
         raise TypeError(gdf_type_error_message)
 
     other = _sfilter_checks(other, crs=gdf.crs)
 
     indices = _get_sfilter_indices(gdf, other, predicate)
 
     return (
         gdf.iloc[indices],
-        gdf.iloc[pd.Index(range(len(gdf))).difference(indices)],
+        gdf.iloc[pd.Index(range(len(gdf))).difference(pd.Index(indices))],
     )
 
 
 def sfilter_inverse(
     gdf: GeoDataFrame | GeoSeries,
     other: GeoDataFrame | GeoSeries | Geometry,
     predicate: str = "intersects",
@@ -167,17 +167,17 @@
         other: The geometry object to filter 'gdf' by.
         predicate: Spatial predicate to use. Defaults to 'intersects'.
 
     Returns:
         A copy of 'gdf' with only the rows that do not match the
         spatial predicate with 'other'.
 
-    Examples
+    Examples:
     --------
-
+    >>> import sgis as sg
     >>> df1 = sg.to_gdf([(0, 0), (0, 1)])
     >>> df1
                       geometry
     0  POINT (0.00000 0.00000)
     1  POINT (0.00000 1.00000)
     >>> df2 = sg.to_gdf([(0, 0), (1, 2)])
     >>> df2
@@ -201,22 +201,22 @@
 
     Also equivelent to using the intersects method, which
     is often slower since df2 must be dissolved:
 
     >>> not_intersecting = df1.loc[~df1.intersects(df2.unary_union)]
 
     """
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
+    if not isinstance(gdf, (GeoDataFrame | GeoSeries)):
         raise TypeError(gdf_type_error_message)
 
     other = _sfilter_checks(other, crs=gdf.crs)
 
     indices = _get_sfilter_indices(gdf, other, predicate)
 
-    return gdf.iloc[pd.Index(range(len(gdf))).difference(indices)]
+    return gdf.iloc[pd.Index(range(len(gdf))).difference(pd.Index(indices))]
 
 
 def _sfilter_checks(other, crs):
     """Allow 'other' to be any geometry object."""
     if isinstance(other, GeoSeries):
         return other
 
@@ -252,15 +252,15 @@
     Parameters
     ----------
     left : GeoDataFrame
     right : GeoDataFrame
     predicate : string
         Binary predicate to query.
 
-    Returns
+    Returns:
     -------
     DataFrame
         DataFrame with matching indices in
         columns named `_key_left` and `_key_right`.
     """
     original_predicate = predicate
```

### Comparing `ssb_sgis-1.0.1/src/sgis/io/dapla_functions.py` & `ssb_sgis-1.0.2/src/sgis/io/dapla_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-"""Functions for reading and writing GeoDataFrames in Statistics Norway's GCS Dapla.
-"""
+"""Functions for reading and writing GeoDataFrames in Statistics Norway's GCS Dapla."""
 
 from pathlib import Path
-from typing import Optional
 
 import dapla as dp
 import geopandas as gpd
+import joblib
 import pandas as pd
 from geopandas import GeoDataFrame
 from geopandas.io.arrow import _geopandas_to_arrow
 from pandas import DataFrame
 from pyarrow import parquet
 
 
 def read_geopandas(
-    gcs_path: str | Path,
+    gcs_path: str | Path | list[str | Path],
     pandas_fallback: bool = False,
-    file_system: Optional[dp.gcs.GCSFileSystem] = None,
+    file_system: dp.gcs.GCSFileSystem | None = None,
     **kwargs,
 ) -> GeoDataFrame | DataFrame:
     """Reads geoparquet or other geodata from a file on GCS.
 
     If the file has 0 rows, the contents will be returned as a pandas.DataFrame,
     since geopandas does not read and write empty tables.
 
     Note:
         Does not currently read shapefiles or filegeodatabases.
 
     Args:
-        gcs_path: path to a file on Google Cloud Storage.
+        gcs_path: path to one or more files on Google Cloud Storage.
+            Multiple paths are read with threading.
         pandas_fallback: If False (default), an exception is raised if the file can
             not be read with geopandas and the number of rows is more than 0. If True,
-            the file will be read as
+            the file will be read with pandas if geopandas fails.
+        file_system: Optional file system.
         **kwargs: Additional keyword arguments passed to geopandas' read_parquet
             or read_file, depending on the file type.
 
-     Returns:
+    Returns:
          A GeoDataFrame if it has rows. If zero rows, a pandas DataFrame is returned.
     """
+    if file_system is None:
+        file_system = dp.FileClient.get_gcs_file_system()
+
+    if isinstance(gcs_path, (list, tuple)):
+        kwargs |= {"file_system": file_system, "pandas_fallback": pandas_fallback}
+        # recursive read with threads
+        with joblib.Parallel(n_jobs=len(gcs_path), backend="threading") as parallel:
+            dfs: list[GeoDataFrame] = parallel(
+                joblib.delayed(read_geopandas)(x, **kwargs) for x in gcs_path
+            )
+        return pd.concat(dfs)
 
     if not isinstance(gcs_path, str):
         try:
             gcs_path = str(gcs_path)
-        except TypeError:
-            raise TypeError(f"Unexpected type {type(gcs_path)}.")
-
-    if file_system is None:
-        file_system = dp.FileClient.get_gcs_file_system()
+        except TypeError as e:
+            raise TypeError(f"Unexpected type {type(gcs_path)}.") from e
 
     if "parquet" in gcs_path or "prqt" in gcs_path:
         with file_system.open(gcs_path, mode="rb") as file:
             try:
                 return gpd.read_parquet(file, **kwargs)
             except ValueError as e:
                 if "Missing geo metadata" not in str(e) and "geometry" not in str(e):
@@ -73,47 +82,51 @@
                 if pandas_fallback or not len(df):
                     return df
                 else:
                     raise e
 
 
 def write_geopandas(
-    df: gpd.GeoDataFrame,
+    df: GeoDataFrame,
     gcs_path: str | Path,
     overwrite: bool = True,
     pandas_fallback: bool = False,
-    file_system: Optional[dp.gcs.GCSFileSystem] = None,
+    file_system: dp.gcs.GCSFileSystem | None = None,
     **kwargs,
 ) -> None:
     """Writes a GeoDataFrame to the speficied format.
 
     Note:
         Does not currently write to shapelfile or filegeodatabase.
 
     Args:
         df: The GeoDataFrame to write.
         gcs_path: The path to the file you want to write to.
         overwrite: Whether to overwrite the file if it exists. Defaults to True.
+        pandas_fallback: If False (default), an exception is raised if the file can
+            not be written with geopandas and the number of rows is more than 0. If True,
+            the file will be written without geo-metadata if >0 rows.
+        file_system: Optional file sustem.
         **kwargs: Additional keyword arguments passed to parquet.write_table
             (for parquet) or geopandas' to_file method (if not parquet).
     """
-
     if not isinstance(gcs_path, str):
         try:
             gcs_path = str(gcs_path)
         except TypeError as e:
             raise TypeError(f"Unexpected type {type(gcs_path)}.") from e
 
     if not overwrite and exists(gcs_path):
         raise ValueError("File already exists.")
 
     if file_system is None:
         file_system = dp.FileClient.get_gcs_file_system()
 
-    pd.io.parquet.BaseImpl.validate_dataframe(df)
+    if not isinstance(df, GeoDataFrame):
+        raise ValueError("DataFrame must be GeoDataFrame.")
 
     if not len(df):
         if pandas_fallback:
             df.geometry = df.geometry.astype(str)
             df = pd.DataFrame(df)
         dp.write_pandas(df, gcs_path, **kwargs)
         return
@@ -148,15 +161,14 @@
 
     Args:
         path (str): The path to the file or directory.
 
     Returns:
         True if the path exists, False if not.
     """
-
     file_system = dp.FileClient.get_gcs_file_system()
     return file_system.exists(path)
 
 
 def check_files(
     folder: str,
     contains: str | None = None,
@@ -181,15 +193,15 @@
     fileinfo = [
         (x["name"], x["size"], x["updated"])
         for x in info
         if x["storageClass"] != "DIRECTORY"
     ]
     folderinfo = [x["name"] for x in info if x["storageClass"] == "DIRECTORY"]
 
-    fileinfo += get_files_in_subfolders(folderinfo)
+    fileinfo += _get_files_in_subfolders(folderinfo)
 
     df = pd.DataFrame(fileinfo, columns=["path", "kb", "updated"])
 
     if contains:
         try:
             df = df.loc[df["path"].str.contains(contains)]
         except TypeError:
@@ -220,20 +232,17 @@
     if not within_minutes:
         return df[["kb", "mb", "name", "child", "path"]]
 
     the_time = pd.Timestamp.now() - pd.Timedelta(minutes=within_minutes)
     return df.loc[lambda x: x.index > the_time, ["kb", "mb", "name", "child", "path"]]
 
 
-def get_files_in_subfolders(folderinfo: list[dict]) -> list[dict]:
+def _get_files_in_subfolders(folderinfo: list[dict]) -> list[tuple]:
     file_system = dp.FileClient.get_gcs_file_system()
 
-    if isinstance(folderinfo, (str, Path)):
-        folderinfo = [folderinfo]
-
     fileinfo = []
 
     while folderinfo:
         new_folderinfo = []
         for m in folderinfo:
             more_info = file_system.ls(m, detail=True, recursive=True)
             if not more_info:
```

### Comparing `ssb_sgis-1.0.1/src/sgis/io/read_parquet.py` & `ssb_sgis-1.0.2/src/sgis/io/read_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Args:
         url: URL containing a geoparquet file.
 
     Returns:
         A GeoDataFrame.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url
     >>> url = "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
     >>> points = read_parquet_url(url)
     >>> points
           idx                        geometry
     0       1  POINT (263122.700 6651184.900)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/examine.py` & `ssb_sgis-1.0.2/src/sgis/maps/examine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 import geopandas as gpd
 import numpy as np
 
 from ..geopandas_tools.bounds import get_total_bounds
 from ..helpers import unit_is_degrees
 from .map import Map
-from .maps import clipmap, explore, samplemap
+from .maps import clipmap
+from .maps import explore
+from .maps import samplemap
 
 
 class Examine:
     """Explore geometries one row at a time.
 
     It takes one or more GeoDataFrames and shows an interactive map
     of one area at the time with the 'next' method or random areas with
     the 'sample' method.
 
     After creating the examiner object, the 'next' method will create a map
     showing all geometries within a given radius (the size parameter) of the
     first geometry in 'mask_gdf' (or the first speficied gdf). The 'next' method
     can then be repeated.
 
-    Args:
-        *gdfs: One or more GeoDataFrames. The rows of the first GeoDataFrame
-            will be used as masks, unless 'mask_gdf' is specified.
-        column: Column to use as colors.
-        mask_gdf: Optional GeoDataFrame to use as mask iterator. The geometries
-            of mask_gdf will not be shown.
-        size: Number of meters (or other crs unit) to buffer the mask geometry
-            before clipping.
-        sort_values: Optional sorting column(s) of the mask GeoDataFrame. Rows
-            will be iterated through from the top.
-        **kwargs: Additional keyword arguments passed to sgis.clipmap.
-
-    Examples
+    Examples:
     --------
     Create the examiner.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
     >>> e = sg.Examine(points, roads)
@@ -74,24 +64,43 @@
         *gdfs: gpd.GeoDataFrame,
         column: str | None = None,
         mask_gdf: gpd.GeoDataFrame | None = None,
         sort_values: str | None = None,
         size: int | float = 1000,
         only_show_mask: bool = True,
         **kwargs,
-    ):
+    ) -> None:
+        """Initialiser.
+
+        Args:
+            *gdfs: One or more GeoDataFrames. The rows of the first GeoDataFrame
+                will be used as masks, unless 'mask_gdf' is specified.
+            column: Column to use as colors.
+            mask_gdf: Optional GeoDataFrame to use as mask iterator. The geometries
+                of mask_gdf will not be shown.
+            size: Number of meters (or other crs unit) to buffer the mask geometry
+                before clipping.
+            sort_values: Optional sorting column(s) of the mask GeoDataFrame. Rows
+                will be iterated through from the top.
+            only_show_mask: If True (default), show only the mask GeoDataFrame by default.
+                The other layers can be toggled on.
+            **kwargs: Additional keyword arguments passed to sgis.clipmap.
+
+        """
         gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
         if mask_gdf is None:
             self.mask_gdf = gdfs[0]
         else:
             self.mask_gdf = mask_gdf
 
         m = Map(*gdfs, column=column, **kwargs)
-        self._gdfs: dict[str, gpd.GeoDataFrame] = dict(zip(m.labels, m.gdfs))
+        self._gdfs: dict[str, gpd.GeoDataFrame] = dict(
+            zip(m.labels, m.gdfs, strict=False)
+        )
 
         self.indices = list(range(len(self.mask_gdf)))
         self.i = 0
         self.column = column
         self.size = size
         self.kwargs = {
             key: value for key, value in kwargs.items() if key not in self._gdfs
@@ -117,15 +126,15 @@
             self.mask_gdf = self.mask_gdf.sort_values(sort_values)
 
         if only_show_mask:
             self.kwargs["show"] = [True] + [False] * (len(self._gdfs) - 1)
         elif not kwargs.get("show", True):
             self.kwargs["show"] = [False] * len(self._gdfs)
 
-    def next(self, i: int | None = None, **kwargs):
+    def next(self, i: int | None = None, **kwargs) -> None:
         """Displays a map of geometries within the next row of the mask gdf.
 
         Args:
             i: Index to display.
             **kwargs: Additional keyword arguments passed to sgis.clipmap.
 
         """
@@ -147,15 +156,15 @@
             self.column,
             **self._gdfs,
             mask=self.mask_gdf.iloc[[self.i]].buffer(self.size),
             **self.kwargs,
         )
         self.i += 1
 
-    def sample(self, **kwargs):
+    def sample(self, **kwargs) -> None:
         """Takes a sample index of the mask and displays a map of this area.
 
         Args:
             **kwargs: Additional keyword arguments passed to sgis.clipmap.
         """
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
@@ -167,15 +176,15 @@
         clipmap(
             self.column,
             **self._gdfs,
             mask=self.mask_gdf.iloc[[i]].buffer(self.size),
             **self.kwargs,
         )
 
-    def current(self, i: int | None = None, **kwargs):
+    def current(self, i: int | None = None, **kwargs) -> None:
         """Repeat the last shown map."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         if i and i < 0:
             self.i -= i
@@ -186,39 +195,39 @@
         clipmap(
             self.column,
             **self._gdfs,
             mask=self.mask_gdf.iloc[[self.i]].buffer(self.size),
             **self.kwargs,
         )
 
-    def explore(self, **kwargs):
+    def explore(self, **kwargs) -> None:
         """Show all rows like the function explore."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         explore(
             **self._gdfs,
             column=self.column,
             **self.kwargs,
         )
 
-    def clipmap(self, **kwargs):
+    def clipmap(self, **kwargs) -> None:
         """Show all rows like the function clipmap."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         clipmap(
             **self._gdfs,
             column=self.column,
             **self.kwargs,
         )
 
-    def samplemap(self, **kwargs):
+    def samplemap(self, **kwargs) -> None:
         """Show all rows like the function samplemap."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         samplemap(
             **self._gdfs,
@@ -237,25 +246,29 @@
         mask = self.mask_gdf.iloc[[self.i]]
         gdfs = {}
         for label, gdf in self._gdfs.items():
             gdfs[label] = gdf.clip(mask.buffer(self.size))
         return gdfs
 
     @property
-    def bounds(self):
+    def bounds(self) -> tuple[float, float, float, float]:
+        """Total bounds of all GeoDataFrames."""
         return get_total_bounds(*list(self.gdfs.values()))
 
-    def _fix_kwargs(self, kwargs) -> dict:
+    def _fix_kwargs(self, kwargs: dict) -> dict:
         self.size = kwargs.pop("size", self.size)
         self.column = kwargs.pop("column", self.column)
         return kwargs
 
     def __repr__(self) -> str:
+        """Representation."""
         return f"{self.__class__.__name__}(indices={len(self.indices)}, current={self.i}, n_gdfs={len(self._gdfs)})"
 
-    def __add__(self, scalar):
+    def __add__(self, scalar: int) -> "Examine":
+        """Add a number to the index."""
         self.i += scalar
         return self
 
-    def __sub__(self, scalar):
+    def __sub__(self, scalar: int) -> "Examine":
+        """Subtract a number from the index."""
         self.i -= scalar
         return self
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/explore.py` & `ssb_sgis-1.0.2/src/sgis/maps/explore.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,48 @@
 """
 
 import os
 import warnings
 from collections.abc import Iterable
 from numbers import Number
 from statistics import mean
+from typing import Any
+from typing import ClassVar
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
 import xyzservices
 from folium import plugins
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from IPython.display import display
 from jinja2 import Template
 from pandas.api.types import is_datetime64_any_dtype
 from shapely import Geometry
 from shapely.geometry import LineString
 
-from ..geopandas_tools.conversion import from_4326, to_gdf
-from ..geopandas_tools.general import clean_geoms, make_all_singlepart
-from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
+from ..geopandas_tools.conversion import to_gdf
+from ..geopandas_tools.general import clean_geoms
+from ..geopandas_tools.general import make_all_singlepart
+from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.geometry_types import to_single_geom_type
 from .httpserver import run_html_server
 from .map import Map
-from .tilesources import kartverket, xyz
-
+from .tilesources import kartverket
+from .tilesources import xyz
 
 try:
     from torchgeo.datasets.geo import RasterDataset
 except ImportError:
 
     class RasterDataset:
-        """Placeholder"""
+        """Placeholder."""
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
@@ -92,15 +97,18 @@
         {{ this.options|tojson }});
     {{this._parent.get_name()}}.addControl({{this.get_name()}});
 
 {% endmacro %}
     """
     )
 
-    def __init__(self, active_color="red", completed_color="red", **kwargs):
+    def __init__(
+        self, active_color: str = "red", completed_color: str = "red", **kwargs
+    ) -> None:
+        """Run super __init__ after the new _template class attribute is made."""
         super().__init__(
             active_color=active_color, completed_color=completed_color, **kwargs
         )
 
 
 def to_tile(tile: str | xyzservices.TileProvider, max_zoom: int) -> folium.TileLayer:
     common_bgmaps = {
@@ -142,40 +150,66 @@
         except (AttributeError, TypeError):
             attr = None
 
     return folium.TileLayer(provider, name=name, attr=attr, max_zoom=max_zoom)
 
 
 class Explore(Map):
+    """Class for displaying and saving html maps of multiple GeoDataFrames."""
+
     # class attribute that can be overridden locally
-    tiles = (
+    tiles: ClassVar[tuple[str]] = (
         "grunnkart",
         "norge_i_bilder",
         "dark",
         "OpenStreetMap",
     )
 
     def __init__(
         self,
         *gdfs,
         mask=None,
         column: str | None = None,
         popup: bool = True,
         max_zoom: int = 40,
-        smooth_factor: float = 1.5,
+        smooth_factor: float = 1.1,
         browser: bool = False,
         prefer_canvas: bool = True,
         measure_control: bool = True,
         geocoder: bool = False,
-        save=None,
+        save: str | None = None,
         show: bool | Iterable[bool] | None = None,
         text: str | None = None,
         decimals: int = 6,
         **kwargs,
-    ):
+    ) -> None:
+        """Initialiser.
+
+        Args:
+            *gdfs: One or more GeoDataFrames.
+            mask: Optional mask to clip to.
+            column: Optional column to color the data by.
+            popup: Whether to make the data popups clickable.
+            max_zoom: Max levels of zoom.
+            smooth_factor: Float of 1 or higher, 1 meaning no smoothing
+                of lines.
+            browser: Whether to open the map in a browser tab.
+            prefer_canvas: Option.
+            measure_control: Whether to include measurement box.
+            geocoder: Whether to include search bar for addresses.
+            save: Optional file path to an html file. The map will then
+                be saved instead of displayed.
+            show: Whether to show or hide the data upon creating the map.
+                If False, the data can be toggled on later. 'show' can also be
+                a sequence of boolean values the same length as the number of
+                GeoDataFrames.
+            text: Optional text for a text box in the map.
+            decimals: Number of decimals in the coordinates.
+            **kwargs: Additional keyword arguments passed to
+        """
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
         self.prefer_canvas = prefer_canvas
         self.measure_control = measure_control
         self.geocoder = geocoder
         self.save = save
@@ -191,20 +225,20 @@
 
         if show is None:
             show_was_none = True
             show = True
         else:
             show_was_none = False
 
-        self.raster_datasets = tuple(
-            raster_dataset_to_background_map(x)
-            for x in gdfs
-            if isinstance(x, RasterDataset)
-        )
-        self.tiles  # += self.raster_datasets
+        self.raster_datasets = []  # tuple(
+        #     raster_dataset_to_background_map(x)
+        #     for x in gdfs
+        #     if isinstance(x, RasterDataset)
+        # )
+        # self.tiles  # += self.raster_datasets
 
         super().__init__(*gdfs, column=column, show=show, **kwargs)
 
         if self.gdfs is None:
             return
 
         # stringify or remove columns not renerable by leaflet (list, geometry etc.)
@@ -258,22 +292,28 @@
             self.cmap_stop = kwargs.pop("cmap_stop", 256)
 
         if self._gdf.crs is None:
             self.kwargs["crs"] = "Simple"
 
         self.original_crs = self.gdf.crs
 
-    def __repr__(self):
+    def __repr__(self) -> str:
+        """Representation."""
         return f"{self.__class__.__name__}()"
 
     def explore(
-        self, column: str | None = None, center=None, size=None, **kwargs
+        self,
+        column: str | None = None,
+        center: Any | None = None,
+        size: int | None = None,
+        **kwargs,
     ) -> None:
+        """Explore all the data."""
         if not any(len(gdf) for gdf in self._gdfs) and not len(self.raster_datasets):
-            warnings.warn("None of the GeoDataFrames have rows.")
+            warnings.warn("None of the GeoDataFrames have rows.", stacklevel=1)
             return
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
 
         if self.mask is not None:
@@ -307,14 +347,15 @@
     def samplemap(
         self,
         size: int = 1000,
         column: str | None = None,
         sample_from_first: bool = True,
         **kwargs,
     ) -> None:
+        """Explore a sample of the data."""
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
 
         if sample_from_first:
             sample = self._gdfs[0].sample(1)
@@ -343,18 +384,19 @@
         self._gdf = pd.concat(gdfs, ignore_index=True)
 
         self._get_unique_values()
         self._explore(**kwargs)
 
     def clipmap(
         self,
-        mask,
+        mask: Any,
         column: str | None = None,
         **kwargs,
     ) -> None:
+        """Explore the data within a mask extent."""
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
 
         gdfs: tuple[GeoDataFrame] = ()
         for gdf in self._gdfs:
@@ -364,15 +406,15 @@
                 collections = make_all_singlepart(collections)
                 gdf = pd.concat([gdf, collections], ignore_index=False)
             gdfs = gdfs + (gdf,)
         self._gdfs = gdfs
         self._gdf = pd.concat(gdfs, ignore_index=True)
         self._explore(**kwargs)
 
-    def _explore(self, **kwargs):
+    def _explore(self, **kwargs) -> None:
         self.kwargs = self.kwargs | kwargs
 
         if self._is_categorical:
             self._create_categorical_map()
         else:
             self._create_continous_map()
 
@@ -380,27 +422,27 @@
             with open(os.getcwd() + "/" + self.save.strip(".html") + ".html", "w") as f:
                 f.write(self.map._repr_html_())
         elif self.browser:
             run_html_server(self.map._repr_html_())
         else:
             display(self.map)
 
-    def _split_categories(self):
+    def _split_categories(self) -> None:
         new_gdfs, new_labels, new_shows = [], [], []
         for cat in self._unique_values:
             gdf = self.gdf.loc[self.gdf[self.column] == cat]
             new_gdfs.append(gdf)
             new_labels.append(cat)
             new_shows.append(self.show[0])
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self.labels = new_labels
         self.show = new_shows
 
-    def _to_single_geom_type(self, gdf) -> GeoDataFrame:
+    def _to_single_geom_type(self, gdf: GeoDataFrame) -> GeoDataFrame:
         gdf = clean_geoms(gdf)
 
         if get_geom_type(gdf) != "mixed":
             return gdf
 
         geom_types = gdf.geom_type.str.lower()
         mess = "Leaflet cannot render mixed geometry types well. "
@@ -416,24 +458,24 @@
 
         elif geom_types.str.contains("lin").any():
             mess += "Keeping only lines."
             gdf = to_single_geom_type(gdf, geom_type="line")
 
         assert get_geom_type(gdf) != "mixed", gdf.geom_type.value_counts()
 
-        warnings.warn(mess)
+        warnings.warn(mess, stacklevel=1)
 
         return gdf
 
-    def _update_column(self):
+    def _update_column(self) -> None:
         self._is_categorical = self._check_if_categorical()
         self._fillna_if_col_is_missing()
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
-    def _create_categorical_map(self):
+    def _create_categorical_map(self) -> None:
         self._get_categorical_colors()
 
         gdf = self._prepare_gdf_for_map(self._gdf)
         self.map = self._make_folium_map(
             bounds=gdf.total_bounds,
             max_zoom=self.max_zoom,
             popup=self.popup,
@@ -474,15 +516,15 @@
             self._categories_colors_dict.values(),
         )
 
         self.map.add_child(folium.LayerControl())
 
     def _add_tiles(
         self, mapobj: folium.Map, tiles: list[str, xyzservices.TileProvider]
-    ):
+    ) -> None:
         for tile in tiles:
             to_tile(tile, max_zoom=self.max_zoom).add_to(mapobj)
 
     def _create_continous_map(self):
         self._prepare_continous_map()
         if self.scheme:
             classified = self._classify_from_bins(self._gdf, bins=self.bins)
@@ -545,15 +587,15 @@
     def _tooltip_cols(self, gdf: GeoDataFrame) -> list:
         if "tooltip" in self.kwargs:
             tooltip = self.kwargs.pop("tooltip")
             return tooltip
         return [col for col in gdf.columns if col not in COLS_TO_DROP]
 
     @staticmethod
-    def _prepare_gdf_for_map(gdf):
+    def _prepare_gdf_for_map(gdf: GeoDataFrame) -> GeoDataFrame:
         if isinstance(gdf, GeoSeries):
             gdf = gdf.to_frame("geometry")
 
         # convert LinearRing to LineString
         rings_mask = gdf.geom_type == "LinearRing"
         if rings_mask.any():
             gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
@@ -563,21 +605,21 @@
         if gdf.crs is not None and not gdf.crs.equals(4326):
             gdf = gdf.to_crs(4326)
 
         return gdf
 
     def _make_folium_map(
         self,
-        bounds,
-        attr=None,
-        tiles=None,
-        width="100%",
-        height="100%",
-        control_scale=True,
-        map_kwds=None,
+        bounds: tuple[float, float, float, float],
+        attr: Any = None,
+        tiles: Any = None,
+        width: str = "100%",
+        height: str = "100%",
+        control_scale: bool = True,
+        map_kwds: dict | None = None,
         **kwargs,
     ):
         if not map_kwds:
             map_kwds = {}
 
         if tiles is None:
             tiles = self.tiles
@@ -675,29 +717,37 @@
             m.get_root().add_child(style)
             # folium.LayerControl(collapsed=False).add_to(m)
 
         return m
 
     def _make_geojson(
         self,
-        df,
+        df: GeoDataFrame,
         show: bool,
-        color=None,
-        tooltip=True,
-        popup=False,
-        highlight=True,
-        marker_type=None,
-        marker_kwds={},
-        style_kwds={},
-        highlight_kwds={},
-        tooltip_kwds={},
-        popup_kwds={},
-        map_kwds={},
+        color: str | None = None,
+        tooltip: bool = True,
+        popup: bool = False,
+        highlight: bool = True,
+        marker_type: str | None = None,
+        marker_kwds: dict | None = None,
+        style_kwds: dict | None = None,
+        highlight_kwds: dict | None = None,
+        tooltip_kwds: dict | None = None,
+        popup_kwds: dict | None = None,
+        map_kwds: dict | None = None,
         **kwargs,
-    ):
+    ) -> folium.GeoJson:
+
+        marker_kwds = marker_kwds or {}
+        style_kwds = style_kwds or {}
+        highlight_kwds = highlight_kwds or {}
+        tooltip_kwds = tooltip_kwds or {}
+        popup_kwds = popup_kwds or {}
+        map_kwds = map_kwds or {}
+
         gdf = df.copy()
 
         # convert LinearRing to LineString
         rings_mask = gdf.geom_type == "LinearRing"
         if rings_mask.any():
             gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
                 lambda g: LineString(g)
@@ -812,17 +862,18 @@
             highlight_function=highlight_function,
             smooth_factor=self.smooth_factor,
             show=show,
             **kwargs,
         )
 
 
-def _tooltip_popup(type, fields, gdf, **kwds):
-    """get tooltip or popup"""
-
+def _tooltip_popup(
+    type_: str, fields: Any, gdf: GeoDataFrame, **kwargs
+) -> folium.GeoJsonTooltip | folium.GeoJsonPopup:
+    """Get tooltip or popup."""
     # specify fields to show in the tooltip
     if fields is False or fields is None or fields == 0:
         return None
     else:
         if fields is True:
             fields = gdf.columns.drop(gdf.geometry.name).to_list()
         elif isinstance(fields, int):
@@ -832,28 +883,24 @@
 
     for field in ["__plottable_column", "__folium_color"]:
         if field in fields:
             fields.remove(field)
 
     # Cast fields to str
     fields = list(map(str, fields))
-    if type == "tooltip":
-        return folium.GeoJsonTooltip(fields, **kwds)
-    elif type == "popup":
-        return folium.GeoJsonPopup(fields, **kwds)
-
+    if type_ == "tooltip":
+        return folium.GeoJsonTooltip(fields, **kwargs)
+    elif type_ == "popup":
+        return folium.GeoJsonPopup(fields, **kwargs)
 
-def raster_dataset_to_background_map(dataset: RasterDataset):
-    crs = dataset.crs
-    bbox = dataset.bounds
 
-
-def _categorical_legend(m, title, categories, colors):
-    """
-    Add categorical legend to a map
+def _categorical_legend(
+    m: folium.Map, title: str, categories: list[str], colors: list[str]
+) -> None:
+    """Add categorical legend to a map.
 
     The implementation is using the code originally written by Michel Metran
     (@michelmetran) and released on GitHub
     (https://github.com/michelmetran/package_folium) under MIT license.
 
     Copyright (c) 2020 Michel Metran
 
@@ -864,15 +911,14 @@
     title : str
         title of the legend (e.g. column name)
     categories : list-like
         list of categories
     colors : list-like
         list of colors (in the same order as categories)
     """
-
     # Header to Add
     head = """
     {% macro header(this, kwargs) %}
     <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
     <script>$( function() {
         $( ".maplegend" ).draggable({
             start: function (event, ui) {
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/httpserver.py` & `ssb_sgis-1.0.2/src/sgis/maps/httpserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 import webbrowser
-from http.server import BaseHTTPRequestHandler, HTTPServer
+from http.server import BaseHTTPRequestHandler
+from http.server import HTTPServer
 
-from IPython.display import HTML, display
+from IPython.display import HTML
+from IPython.display import display
 
 
-def run_html_server(contents: str | None = None, port: int = 3000):
+def run_html_server(contents: str | None = None, port: int = 3000) -> None:
     """Run a simple, temporary http web server for serving static HTML content."""
     if "JUPYTERHUB_SERVICE_PREFIX" in os.environ:
         # Create a link using the https://github.com/jupyterhub/jupyter-server-proxy
-        display_address = os.environ["JUPYTERHUB_SERVICE_PREFIX"] + "proxy/{}/".format(
-            port
-        )
+        display_address = os.environ["JUPYTERHUB_SERVICE_PREFIX"] + f"proxy/{port}/"
         display_content = HTML(
             f"""
         <p>Click <a href='{display_address}'>here</a> to open in browser.</p>
         <p>Click <a href='{display_address}/stop'>here</a> to stop.</p>
         """
         )
     else:
         display_address = f"http://localhost:{port}"
-        display_content = (
-            f"Server started at http://localhost:{port}. "
-            f"Click http://localhost:{port}/stop to stop server."
+        display_content = HTML(
+            f"""
+        <p>Click <a href='http://localhost:{port}'>here</a> to open in browser.</p>
+        <p>Click <a href='http://localhost:{port}/stop'>here</a> to stop.<p>"
+        """
         )
 
     class HTTPServerRequestHandler(BaseHTTPRequestHandler):
-        """
-        A handler of request for the server, hosting static content.
-        """
+        """A handler of request for the server, hosting static content."""
 
         allow_reuse_address = True
 
         def do_GET(self):
             """Handle GET requests."""
             self.send_response(200)
             self.send_header("Content-type", "text/html")
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/legend.py` & `ssb_sgis-1.0.2/src/sgis/maps/legend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Attributes of the legend of the ThematicMap class.
 
 The Legend class is best accessed through the 'legend' attribute of the ThematicMap
 class.
 
 """
+
+import itertools
 import warnings
+from typing import Any
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from geopandas import GeoDataFrame
 from matplotlib.lines import Line2D
 from pandas import Series
 
 from ..geopandas_tools.bounds import points_in_bounds
 
-
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
@@ -48,33 +51,46 @@
         framealpha: Transparency of the legend background.
         edgecolor: Color of the legend border. Defaults to #0f0f0f (almost black).
         kwargs: Stores additional keyword arguments taken by the matplotlib legend
             method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
             'm' is the name of the ThematicMap instance. See here:
             https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
 
-    Examples
+    Examples:
     --------
-    Create ten random points with a numeric column from 0 to 9.
+    Create ten points with a numeric column from 0 to 9.
 
     >>> import sgis as sg
-    >>> points = sg.random_points(10)
+    >>> points = sg.to_gdf(
+    ...     [
+    ...         (0, 1),
+    ...         (1, 0),
+    ...         (1, 1),
+    ...         (0, 0),
+    ...         (0.5, 0.5),
+    ...         (0.5, 0.25),
+    ...         (0.25, 0.25),
+    ...         (0.75, 0.75),
+    ...         (0.25, 0.75),
+    ...         (0.75, 0.25),
+    ...     ]
+    ... )
     >>> points["number"] = range(10)
     >>> points
-                    geometry  number
-    0  POINT (0.59780 0.50425)       0
-    1  POINT (0.07019 0.26167)       1
-    2  POINT (0.56475 0.15422)       2
-    3  POINT (0.87293 0.60316)       3
-    4  POINT (0.47373 0.20040)       4
-    5  POINT (0.98661 0.15614)       5
-    6  POINT (0.30951 0.77057)       6
-    7  POINT (0.47802 0.52824)       7
-    8  POINT (0.12215 0.96588)       8
-    9  POINT (0.02938 0.93467)       9
+                      geometry  number
+    0  POINT (0.00000 1.00000)       0
+    1  POINT (1.00000 0.00000)       1
+    2  POINT (1.00000 1.00000)       2
+    3  POINT (0.00000 0.00000)       3
+    4  POINT (0.50000 0.50000)       4
+    5  POINT (0.50000 0.25000)       5
+    6  POINT (0.25000 0.25000)       6
+    7  POINT (0.75000 0.75000)       7
+    8  POINT (0.25000 0.75000)       8
+    9  POINT (0.75000 0.25000)       9
 
     Creating the ThematicMap instance will also create the legend. Since we
     specify a numeric column, a ContinousLegend instance is created.
 
     >>> m = sg.ThematicMap(points, column="number")
     >>> m.legend
     <sgis.maps.legend.ContinousLegend object at 0x00000222206738D0>
@@ -109,15 +125,38 @@
         position: tuple[float] | None = None,
         markersize: int | None = None,
         fontsize: int | None = None,
         title_fontsize: int | None = None,
         framealpha: float = 1.0,
         edgecolor: str = "#0f0f0f",
         **kwargs,
-    ):
+    ) -> None:
+        """Initialiser.
+
+        Args:
+            title: Legend title. Defaults to the column name if used in the
+                ThematicMap class.
+            labels: Labels of the categories.
+            position: The legend's x and y position in the plot, specified as a tuple of
+                x and y position between 0 and 1. E.g. position=(0.8, 0.2) for a position
+                in the bottom right corner, (0.2, 0.8) for the upper left corner.
+            fontsize: Text size of the legend labels. Defaults to the size of
+                the ThematicMap class.
+            title_fontsize: Text size of the legend title. Defaults to the
+                size * 1.2 of the ThematicMap class.
+            markersize: Size of the color circles in the legend. Defaults to the size of
+                the ThematicMap class.
+            framealpha: Transparency of the legend background.
+            edgecolor: Color of the legend border. Defaults to #0f0f0f (almost black).
+            kwargs: Stores additional keyword arguments taken by the matplotlib legend
+                method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
+                'm' is the name of the ThematicMap instance. See here:
+                https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
+
+        """
         self.title = title
 
         if "size" in kwargs:
             size = kwargs.pop("size")
             self._get_legend_sizes(size, kwargs)
         else:
             self._title_fontsize = title_fontsize
@@ -132,17 +171,16 @@
         self.labelspacing = kwargs.pop("labelspacing", 0.8)
 
         self.labels = labels
         self._position = position
         self.kwargs = kwargs
         self._position_has_been_set = True if position else False
 
-    def _get_legend_sizes(self, size, kwargs):
+    def _get_legend_sizes(self, size: int | float, kwargs: dict) -> None:
         """Adjust fontsize and markersize to size kwarg."""
-
         if "title_fontsize" in kwargs:
             self._title_fontsize = kwargs["title_fontsize"]
             self._title_fontsize_has_been_set = True
         else:
             self._title_fontsize = size * 1.2
 
         if "fontsize" in kwargs:
@@ -153,15 +191,17 @@
 
         if "markersize" in kwargs:
             self._markersize = kwargs["markersize"]
             self._markersize_has_been_set = True
         else:
             self._markersize = size
 
-    def _prepare_categorical_legend(self, categories_colors: dict, nan_label: str):
+    def _prepare_categorical_legend(
+        self, categories_colors: dict, nan_label: str
+    ) -> None:
         for attr in self.__dict__.keys():
             if attr in self.kwargs:
                 self[attr] = self.kwargs.pop(attr)
 
         # swap column values with label values if labels is dict
         if self.labels and isinstance(self.labels, dict):
             categories_colors = {
@@ -191,15 +231,15 @@
                     alpha=self.kwargs.get("alpha", 1),
                     markersize=self._markersize,
                     markerfacecolor=color,
                     markeredgewidth=0,
                 )
             )
 
-    def _actually_add_legend(self, ax):
+    def _actually_add_legend(self, ax: matplotlib.axes.Axes) -> matplotlib.axes.Axes:
         legend = ax.legend(
             self._patches,
             self._categories,
             fontsize=self._fontsize,
             title=self.title,
             title_fontsize=self._title_fontsize,
             bbox_to_anchor=self._position + (self.width, self.height),
@@ -211,15 +251,17 @@
         )
 
         if self.title_color:
             plt.setp(legend.get_title(), color=self.title_color)
 
         return ax
 
-    def _get_best_legend_position(self, gdf, k: int):
+    def _get_best_legend_position(
+        self, gdf: GeoDataFrame, k: int
+    ) -> tuple[float, float]:
         minx, miny, maxx, maxy = gdf.total_bounds
         diffx = maxx - minx
         diffy = maxy - miny
 
         points = points_in_bounds(gdf, 30)
         gdf = gdf.loc[:, ~gdf.columns.str.contains("index|level_")]
         joined = points.sjoin_nearest(gdf, distance_col="nearest")
@@ -239,59 +281,66 @@
         besty_01 = (besty - miny) / (diffy)
 
         bestx_01 = 0.1 if bestx_01 < 0.5 else 0.90
         besty_01 = 0.0375 * k if besty_01 < 0.5 else 1
 
         return bestx_01, besty_01
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str) -> Any:
+        """Get attribute with square brackets."""
         return getattr(self, item)
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Any) -> None:
+        """Set attribute with square brackets."""
         setattr(self, key, value)
 
-    def get(self, key, default=None):
+    def get(self, key: Any, default: Any = None) -> Any:
+        """Get value of an attribute of the Legend."""
         try:
             return self[key]
         except (KeyError, ValueError, IndexError, AttributeError):
             return default
 
     @property
-    def position(self):
+    def position(self) -> tuple[float, float]:
+        """Legend position in x, y."""
         return self._position
 
     @position.setter
-    def position(self, new_value: bool):
+    def position(self, new_value: tuple[float, float]) -> None:
         self._position = new_value
         self._position_has_been_set = True
 
     @property
-    def title_fontsize(self):
+    def title_fontsize(self) -> int:
+        """Legend title fontsize."""
         return self._title_fontsize
 
     @title_fontsize.setter
-    def title_fontsize(self, new_value: bool):
+    def title_fontsize(self, new_value: int) -> None:
         self._title_fontsize = new_value
         self._title_fontsize_has_been_set = True
 
     @property
-    def fontsize(self):
+    def fontsize(self) -> int:
+        """Legend fontsize."""
         return self._fontsize
 
     @fontsize.setter
-    def fontsize(self, new_value: bool):
+    def fontsize(self, new_value: int) -> None:
         self._fontsize = new_value
         self._fontsize_has_been_set = True
 
     @property
-    def markersize(self):
+    def markersize(self) -> int:
+        """Legend markersize."""
         return self._markersize
 
     @markersize.setter
-    def markersize(self, new_value: bool):
+    def markersize(self, new_value: int) -> None:
         self._markersize = new_value
         self._markersize_has_been_set = True
 
 
 class ContinousLegend(Legend):
     """Holds the legend attributes specific to numeric columns.
 
@@ -317,15 +366,15 @@
             if not bins are set manually.
         thousand_sep: Separator between each thousand for large numbers. Defaults to
             None, meaning no separator.
         decimal_mark: Text to use as decimal point. Defaults to None, meaning '.' (dot)
             unless 'thousand_sep' is '.'. In this case, ',' (comma) will be used as
             decimal mark.
 
-    Examples
+    Examples:
     --------
     Create ten random points with a numeric column from 0 to 9.
 
     >>> import sgis as sg
     >>> points = sg.random_points(10)
     >>> points["number"] = range(10)
     >>> points
@@ -382,15 +431,44 @@
         pretty_labels: bool = False,
         label_suffix: str | None = None,
         label_sep: str = "-",
         rounding: int | None = None,
         thousand_sep: str | None = None,
         decimal_mark: str | None = None,
         **kwargs,
-    ):
+    ) -> None:
+        """Initialiser.
+
+        Args:
+            labels: To manually set labels. If set, all other labeling attributes are
+                ignored. Should be given as a list of strings with the same length as
+                the number of color groups.
+            pretty_labels: If False (default), the minimum and maximum values of each
+                color group will be used as legend labels. If True, the labels will end
+                with the maximum value, but start at 1 + the maximum value of the previous
+                group. The labels will be correct but inaccurate.
+            label_suffix: The text to put after each number in the legend labels.
+                Defaults to None.
+            label_sep: Text to put in between the two numbers in each color group in
+                the legend. Defaults to '-'.
+            rounding: Number of decimals in the labels. By default, the rounding
+                depends on the column's maximum value and standard deviation.
+                OBS: The bins will not be rounded, meaning the labels might be wrong
+                if not bins are set manually.
+            thousand_sep: Separator between each thousand for large numbers. Defaults to
+                None, meaning no separator.
+            decimal_mark: Text to use as decimal point. Defaults to None, meaning '.' (dot)
+                unless 'thousand_sep' is '.'. In this case, ',' (comma) will be used as
+                decimal mark.
+            kwargs: Stores additional keyword arguments taken by the matplotlib legend
+                method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
+                'm' is the name of the ThematicMap instance. See here:
+                https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
+
+        """
         super().__init__(**kwargs)
 
         self.pretty_labels = pretty_labels
         self.thousand_sep = thousand_sep
         self.decimal_mark = decimal_mark
 
         self.label_sep = label_sep
@@ -419,31 +497,31 @@
         if max_ > 5 and std_ > 1:
             return 1
         if max_ > 1 and std_ > 0.1:
             return 2
         return int(abs(np.log10(std_))) + 1
 
     @staticmethod
-    def _set_rounding(bins, rounding: int | float):
+    def _set_rounding(bins, rounding: int | float) -> list[int | float]:
         if rounding == 0:
-            return [int(round(bin, 0)) for bin in bins]
+            return [int(round(bin_, 0)) for bin_ in bins]
         else:
-            return [round(bin, rounding) for bin in bins]
+            return [round(bin_, rounding) for bin_ in bins]
 
-    def _remove_max_legend_value(self):
+    def _remove_max_legend_value(self) -> None:
         if not self._legend:
             raise ValueError("Cannot modify legend before it is created.")
 
     def _prepare_continous_legend(
         self,
         bins: list[float],
         colors: list[str],
         nan_label: str,
         bin_values: dict,
-    ):
+    ) -> None:
         # TODO: clean up this messy method
 
         for attr in self.__dict__.keys():
             if attr in self.kwargs:
                 self[attr] = self.kwargs.pop(attr)
 
         self._patches, self._categories = [], []
@@ -487,15 +565,15 @@
                 else:
                     self._categories.append(
                         f"{min_rounded} {self.label_suffix} {self.label_sep} "
                         f"{max_rounded} {self.label_suffix}"
                     )
 
         else:
-            for i, (cat1, cat2) in enumerate(zip(bins[:-1], bins[1:], strict=True)):
+            for i, (cat1, cat2) in enumerate(itertools.pairwise(bins)):
                 if nan_label in str(cat1) or nan_label in str(cat2):
                     self._categories.append(nan_label)
                     continue
 
                 min_ = np.min(bin_values[i])
                 max_ = np.max(bin_values[i])
                 min_rounded = self._set_rounding([min_], self._rounding)[0]
@@ -523,44 +601,24 @@
                     self._categories.append(label)
                 else:
                     min_rounded = self._format_number(min_rounded)
                     max_rounded = self._format_number(max_rounded)
                     label = self._two_value_label(min_rounded, max_rounded)
                     self._categories.append(label)
 
-    def _actually_add_legend(self, ax):
-        legend = ax.legend(
-            self._patches,
-            self._categories,
-            fontsize=self._fontsize,
-            title=self.title,
-            title_fontsize=self._title_fontsize,
-            bbox_to_anchor=self._position + (self.width, self.height),
-            fancybox=False,
-            framealpha=self.framealpha,
-            edgecolor=self.edgecolor,
-            labelspacing=self.labelspacing,
-            **self.kwargs,
-        )
-
-        if self.title_color:
-            plt.setp(legend.get_title(), color=self.title_color)
-
-        return ax
-
-    def _two_value_label(self, value1, value2):
+    def _two_value_label(self, value1: int | float, value2: int | float) -> str:
         return (
             f"{value1} {self.label_suffix} {self.label_sep} "
             f"{value2} {self.label_suffix}"
         )
 
-    def _one_value_label(self, value1):
+    def _one_value_label(self, value1: int | float) -> str:
         return f"{value1} {self.label_suffix}"
 
-    def _format_number(self, number):
+    def _format_number(self, number: int | float) -> int | float:
         if not self.thousand_sep and not self.decimal_mark:
             return number
 
         if self.thousand_sep:
             number = f"{number:,}".replace(",", "*temp_thousand*")
 
         if self.decimal_mark:
@@ -577,14 +635,15 @@
         else:
             number = number.replace("*temp_thousand*", self.thousand_sep).replace(
                 "*temp_decimal*", self.decimal_mark
             )
         return number
 
     @property
-    def rounding(self):
+    def rounding(self) -> int:
+        """Number rounding."""
         return self._rounding
 
     @rounding.setter
-    def rounding(self, new_value: bool):
+    def rounding(self, new_value: int) -> None:
         self._rounding = new_value
         self._rounding_has_been_set = True
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/map.py` & `ssb_sgis-1.0.2/src/sgis/maps/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """Interactive or static map of one or more GeoDataFrames.
 
 This module holds the Map class, which is the basis for the Explore class.
 """
 
 import warnings
+from typing import Any
 
 import matplotlib
 import matplotlib.colors as colors
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from jenkspy import jenks_breaks
 from mapclassify import classify
 from shapely import Geometry
 
 from ..geopandas_tools.conversion import to_gdf
-from ..geopandas_tools.general import (
-    clean_geoms,
-    drop_inactive_geometry_columns,
-    get_common_crs,
-    rename_geometry_if,
-)
+from ..geopandas_tools.general import _rename_geometry_if
+from ..geopandas_tools.general import clean_geoms
+from ..geopandas_tools.general import drop_inactive_geometry_columns
+from ..geopandas_tools.general import get_common_crs
 from ..helpers import get_object_name
 
-
 try:
     from torchgeo.datasets.geo import RasterDataset
 except ImportError:
 
     class RasterDataset:
-        """Placeholder"""
+        """Placeholder."""
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
@@ -56,16 +55,24 @@
     10: "#750000",
     11: "#1c6b00",
 }
 
 DEFAULT_SCHEME = "quantiles"
 
 
-def proper_fillna(val, fill_val):
-    """fillna doesn't always work. So doing it manually."""
+def proper_fillna(val: Any, fill_val: Any) -> Any:
+    """Manually handle missing values when fillna doesn't work as expected.
+
+    Args:
+        val: The value to check and fill.
+        fill_val: The value to fill in.
+
+    Returns:
+        The original value or the filled value if conditions are met.
+    """
     try:
         if "NAType" in val.__class__.__name__:
             return fill_val
     except Exception:
         if fill_val is None:
             return fill_val
         if fill_val != fill_val:
@@ -87,16 +94,28 @@
         labels: tuple[str] | None = None,
         k: int = 5,
         bins: tuple[float] | None = None,
         nan_label: str = "Missing",
         nan_color="#c2c2c2",
         scheme: str = DEFAULT_SCHEME,
         **kwargs,
-    ):
+    ) -> None:
+        """Initialiser.
 
+        Args:
+            *gdfs: Variable length GeoDataFrame list.
+            column: The column name to work with.
+            labels: Tuple of labels for each GeoDataFrame.
+            k: Number of bins or classes for classification (default: 5).
+            bins: Predefined bins for data classification.
+            nan_label: Label for missing data.
+            nan_color: Color for missing data.
+            scheme: Classification scheme to be used.
+            **kwargs: Arbitrary keyword arguments.
+        """
         gdfs, column, kwargs = self._separate_args(gdfs, column, kwargs)
 
         self._column = column
         self.bins = bins
         self._k = k
         self.nan_label = nan_label
         self.nan_color = nan_color
@@ -134,15 +153,15 @@
             show_temp = show
 
         show_args = show_temp[: len(gdfs)]
         show_kwargs = show_temp[len(gdfs) :]
         self._gdfs = []
         new_labels = []
         self.show = []
-        for label, gdf, show in zip(self.labels, gdfs, show_args):
+        for label, gdf, show in zip(self.labels, gdfs, show_args, strict=False):
             if not len(gdf):
                 continue
 
             gdf = clean_geoms(gdf).reset_index(drop=True)
             if not len(gdf):
                 continue
 
@@ -185,15 +204,15 @@
         if hasattr(self.show, "__iter__") and len(self.show) != len(self._gdfs):
             raise ValueError(
                 "'show' must be boolean or an iterable of boleans same "
                 f"length as gdfs ({len(gdfs)}). Got len {len(show)}"
             )
 
         if not any(len(gdf) for gdf in self._gdfs):
-            warnings.warn("None of the GeoDataFrames have rows.")
+            warnings.warn("None of the GeoDataFrames have rows.", stacklevel=1)
             self._gdfs = None
             self._is_categorical = True
             self._unique_values = []
             return
 
         if not self.labels:
             self._set_labels()
@@ -218,15 +237,15 @@
             for gdf in self._gdfs:
                 gdf.crs = crs
             self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
         self._nan_idx = self._gdf[self._column].isna()
         self._get_unique_values()
 
-    def _get_unique_values(self):
+    def _get_unique_values(self) -> None:
         if not self._is_categorical:
             self._unique_values = self._get_unique_floats()
         else:
             unique = list(self._gdf[self._column].unique())
             try:
                 self._unique_values = sorted(unique)
             except TypeError:
@@ -250,29 +269,28 @@
 
         unique = array.reset_index(drop=True).drop_duplicates()
         as_int = self._array_to_large_int(unique)
         no_duplicates = as_int.drop_duplicates()
 
         return np.sort(np.array(unique.loc[no_duplicates.index]))
 
-    def _array_to_large_int(self, array):
+    def _array_to_large_int(self, array: np.ndarray | pd.Series) -> pd.Series:
         """Multiply values in float array, then convert to integer."""
         if not isinstance(array, pd.Series):
             array = pd.Series(array)
 
         notna = array[array.notna()]
         isna = array[array.isna()]
 
         unique_multiplied = (notna * self._multiplier).astype(np.int64)
 
         return pd.concat([unique_multiplied, isna]).sort_index()
 
-    def _get_multiplier(self, array: np.ndarray):
-        """Find the number of zeros needed to push the max value of the array above
-        +-1_000_000.
+    def _get_multiplier(self, array: np.ndarray) -> None:
+        """Find the number of zeros needed to push the max value of the array above +-1_000_000.
 
         Adding this as an attribute to use later in _classify_from_bins.
         """
         if np.max(array) == 0:
             self._multiplier: int = 1
             return
 
@@ -289,15 +307,15 @@
                 max_ = np.max(array * multiplier)
 
         self._multiplier: int = multiplier
 
     def _add_minmax_to_bins(self, bins: list[float | int]) -> list[float | int]:
         """If values are outside the bin range, add max and/or min values of array."""
         # make sure they are lists
-        bins = [bin for bin in bins]
+        bins = [bin_ for bin_ in bins]
 
         if min(bins) > 0 and min(self._gdf.loc[~self._nan_idx, self._column]) < min(
             bins
         ):
             bins = [min(self._gdf.loc[~self._nan_idx, self._column])] + bins
 
         if min(bins) < 0 and min(self._gdf.loc[~self._nan_idx, self._column]) < min(
@@ -367,17 +385,16 @@
                             # no need to raise here
                             pass
 
                 kwargs |= more_gdfs
 
         return gdfs, column, kwargs
 
-    def _prepare_continous_map(self):
+    def _prepare_continous_map(self) -> None:
         """Create bins if not already done and adjust k if needed."""
-
         if self.scheme is None:
             return
 
         if not self.bins:
             self.bins = self._create_bins(self._gdf, self._column)
             if len(self.bins) <= self._k and len(self.bins) != len(self._unique_values):
                 self._k = len(self.bins)
@@ -404,23 +421,25 @@
         """Setting the labels after copying the gdfs."""
         gdfs = []
         for i, gdf in enumerate(self._gdfs):
             gdf["label"] = self.labels[i]
             gdfs.append(gdf)
         self._gdfs = gdfs
 
-    def _to_common_crs_and_one_geom_col(self, gdfs: list[GeoDataFrame]):
+    def _to_common_crs_and_one_geom_col(
+        self, gdfs: list[GeoDataFrame]
+    ) -> list[GeoDataFrame]:
         """Need common crs and max one geometry column."""
         crs_list = list({gdf.crs for gdf in gdfs if gdf.crs is not None})
         if crs_list:
             self.crs = crs_list[0]
         new_gdfs = []
         for gdf in gdfs:
             gdf = gdf.reset_index(drop=True)
-            gdf = drop_inactive_geometry_columns(gdf).pipe(rename_geometry_if)
+            gdf = drop_inactive_geometry_columns(gdf).pipe(_rename_geometry_if)
             if crs_list:
                 try:
                     gdf = gdf.to_crs(self.crs)
                 except ValueError:
                     gdf = gdf.set_crs(self.crs)
             new_gdfs.append(gdf)
         return new_gdfs
@@ -526,15 +545,14 @@
         """Make bin list of length k + 1, or length of unique values.
 
         The returned bins sometimes have two almost identical
 
         If 'scheme' is not specified, the jenks_breaks function is used, which is
         much faster than the one from Mapclassifier.
         """
-
         if not len(gdf.loc[~self._nan_idx, column]):
             return np.array([0])
 
         n_classes = (
             self._k if len(self._unique_values) > self._k else len(self._unique_values)
         )
 
@@ -559,29 +577,29 @@
                 np.asarray(gdf.loc[~self._nan_idx, column]),
                 scheme=self.scheme,
                 k=self._k,
             )
             bins = binning.bins
             bins = self._add_minmax_to_bins(bins)
 
-        unique_bins = list({round(bin, 5) for bin in bins})
+        unique_bins = list({round(bin_, 5) for bin_ in bins})
         unique_bins.sort()
 
         if self._k == len(self._unique_values) - 1:
             return np.array(unique_bins)
 
         if len(unique_bins) == len(self._unique_values):
             return np.array(unique_bins)
 
         if len(unique_bins) == len(bins) - 1:
             self._k -= 1
 
         return np.array(bins)
 
-    def change_cmap(self, cmap: str, start: int = 0, stop: int = 256):
+    def change_cmap(self, cmap: str, start: int = 0, stop: int = 256) -> "Map":
         """Change the color palette of the plot.
 
         Args:
             cmap: The colormap.
                 https://matplotlib.org/stable/tutorials/colors/colormaps.html
             start: Start position for the color palette. Defaults to 0.
             stop: End position for the color palette. Defaults to 256, which
@@ -602,15 +620,14 @@
         ]
         if any(self._nan_idx):
             colors_ = colors_ + [self.nan_color]
         return np.array(colors_)
 
     def _classify_from_bins(self, gdf: GeoDataFrame, bins: np.ndarray) -> np.ndarray:
         """Place the column values into groups."""
-
         # if equal lenght, convert to integer and check for equality
         if len(bins) == len(self._unique_values):
             if gdf[self._column].isna().all():
                 return np.repeat(len(bins), len(gdf))
 
             gdf["col_as_int"] = self._array_to_large_int(gdf[self._column])
             bins = self._array_to_large_int(self._unique_values)
@@ -643,73 +660,81 @@
         Otherwise, will get index error when classifying colors.
         """
         rank_dict = {val: rank for rank, val in enumerate(np.unique(classified))}
 
         return np.array([rank_dict[val] for val in classified])
 
     @property
-    def k(self):
+    def k(self) -> int:
+        """Number of bins."""
         return self._k
 
     @k.setter
-    def k(self, new_value: bool):
+    def k(self, new_value: int) -> None:
         if not self._is_categorical and new_value > len(self._unique_values):
             raise ValueError(
                 "'k' cannot be greater than the number of unique values in the column.'"
                 f"Got new k={new_value} and previous k={len(self._unique_values)}.'"
                 #  f"{''.join(self._unique_values)}"
             )
         self._k = int(new_value)
 
     @property
-    def cmap(self):
+    def cmap(self) -> str:
+        """Colormap."""
         return self._cmap
 
     @cmap.setter
-    def cmap(self, new_value: bool):
+    def cmap(self, new_value: str) -> None:
         self._cmap = new_value
         self.change_cmap(cmap=new_value, start=self.cmap_start, stop=self.cmap_stop)
 
     @property
-    def gdf(self):
+    def gdf(self) -> GeoDataFrame:
+        """All GeoDataFrames concated."""
         return self._gdf
 
     @gdf.setter
-    def gdf(self, _):
+    def gdf(self, _) -> None:
         raise ValueError(
             "Cannot change 'gdf' after init. Put the GeoDataFrames into "
             "the class initialiser."
         )
 
     @property
-    def gdfs(self):
+    def gdfs(self) -> list[GeoDataFrame]:
+        """All GeoDataFrames as a list."""
         return self._gdfs
 
     @gdfs.setter
-    def gdfs(self, _):
+    def gdfs(self, _) -> None:
         raise ValueError(
             "Cannot change 'gdfs' after init. Put the GeoDataFrames into "
             "the class initialiser."
         )
 
     @property
-    def column(self):
+    def column(self) -> str | None:
+        """Column to use as colormap."""
         return self._column
 
     @column.setter
-    def column(self, _):
+    def column(self, _) -> None:
         raise ValueError(
             "Cannot change 'column' after init. Specify 'column' in the "
             "class initialiser."
         )
 
-    def __setitem__(self, item, new_item):
+    def __setitem__(self, item: Any, new_item: Any) -> None:
+        """Set an attribute with square brackets."""
         return setattr(self, item, new_item)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: Any) -> Any:
+        """Get an attribute with square brackets."""
         return getattr(self, item)
 
-    def get(self, key, default=None):
+    def get(self, key: Any, default: Any | None = None) -> Any:
+        """Get an attribute with default value if not present."""
         try:
             return self[key]
         except (KeyError, ValueError, IndexError, AttributeError):
             return default
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/maps.py` & `ssb_sgis-1.0.2/src/sgis/maps/maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,33 +7,38 @@
 The 'qtm' function shows a simple static map of one or more GeoDataFrames.
 """
 
 import inspect
 from numbers import Number
 from typing import Any
 
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from pyproj import CRS
 from shapely import Geometry
+from shapely import box
+from shapely.geometry import Polygon
 
+from ..geopandas_tools.bounds import get_total_bounds
 from ..geopandas_tools.conversion import to_gdf as to_gdf_func
-from ..geopandas_tools.general import clean_geoms, get_common_crs, is_wkt
+from ..geopandas_tools.general import clean_geoms
+from ..geopandas_tools.general import get_common_crs
+from ..geopandas_tools.general import is_wkt
 from ..geopandas_tools.geocoding import address_to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
 from .explore import Explore
 from .map import Map
 from .thematicmap import ThematicMap
 
-
 try:
     from torchgeo.datasets.geo import RasterDataset
 except ImportError:
 
     class RasterDataset:
-        """Placeholder"""
+        """Placeholder."""
 
 
 def _get_location_mask(kwargs: dict, gdfs) -> tuple[GeoDataFrame | None, dict]:
     try:
         crs = get_common_crs(gdfs)
     except IndexError:
         for x in kwargs.values():
@@ -68,15 +73,14 @@
     return None, kwargs
 
 
 def explore(
     *gdfs: GeoDataFrame | dict[str, GeoDataFrame],
     column: str | None = None,
     center: Any | None = None,
-    center_4326: Any | None = None,
     labels: tuple[str] | None = None,
     max_zoom: int = 40,
     browser: bool = False,
     smooth_factor: int | float = 1.5,
     size: int | None = None,
     **kwargs,
 ) -> None:
@@ -90,18 +94,17 @@
     'center' can be a string of a city or address, a coordinate tuple or a
     geometry-like object.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
             each GeoDataFrame will get a unique color.
-        center: Either an address string to be geocoded or a geometry like object
-            (coordinate pair (x, y), GeoDataFrame, bbox, etc.). If the geometry is a
-            point (or line), it will be buffered by 1000 (can be changed with the)
-            size parameter. If a polygon is given, it will not be buffered.
+        center: Geometry-like object to center the map on. If a three-length tuple
+            is given, the first two should be x and y coordinates and the third
+            should be a number of meters to buffer the centerpoint by.
         labels: By default, the GeoDataFrames will be labeled by their object names.
             Alternatively, labels can be specified as a tuple of strings with the same
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
         browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
@@ -109,20 +112,20 @@
             5 is quite a lot of simplification.
         size: The buffer distance. Only used when center is given. It then defaults to
             1000.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    See also
+    See Also:
     --------
     samplemap: same functionality, but shows only a random area of a given size.
     clipmap: same functionality, but shows only the areas clipped by a given mask.
 
-    Examples
+    Examples:
     --------
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
     Explore the area 500 meter around a given point. Coordinates are in UTM 33 format (25833).
 
@@ -134,15 +137,14 @@
 
     With additional arguments.
 
     >>> roads["meters"] = roads.length
     >>> points["meters"] = points.length
     >>> sg.explore(roads, points, column="meters", cmap="plasma", max_zoom=60, center_4326=(10.7463, 59.92, 500))
     """
-
     gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
     loc_mask, kwargs = _get_location_mask(kwargs | {"size": size}, gdfs)
 
     kwargs.pop("size", None)
 
     mask = kwargs.pop("mask", loc_mask)
@@ -158,22 +160,19 @@
             **kwargs,
         )
 
     try:
         to_crs = gdfs[0].crs
     except IndexError:
         try:
-            to_crs = [x for x in kwargs.values() if hasattr(x, "crs")][0].crs
+            to_crs = next(x for x in kwargs.values() if hasattr(x, "crs")).crs
         except IndexError:
             to_crs = None
 
-    if center_4326 is not None:
-        from_crs = 4326
-        center = center_4326
-    elif "crs" in kwargs:
+    if "crs" in kwargs:
         from_crs = kwargs.pop("crs")
     else:
         from_crs = to_crs
 
     if center is not None:
         size = size or 1000
         if isinstance(center, str) and not is_wkt(center):
@@ -181,14 +180,18 @@
         elif isinstance(center, (GeoDataFrame, GeoSeries)):
             mask = center
         else:
             if isinstance(center, (tuple, list)) and len(center) == 3:
                 *center, size = center
             mask = to_gdf_func(center, crs=from_crs)
 
+        bounds: Polygon = box(*get_total_bounds(*gdfs, *list(kwargs.values())))
+        if not mask.intersects(bounds).any():
+            mask = mask.set_crs(4326, allow_override=True)
+
         try:
             mask = mask.to_crs(to_crs)
         except ValueError:
             pass
 
         if get_geom_type(mask) in ["point", "line"]:
             mask = mask.buffer(size)
@@ -266,35 +269,34 @@
             or not in Jupyter, a static plot will be shown.
         browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    See also
+    See Also:
     --------
     explore: Same functionality, but shows the entire area of the geometries.
     clipmap: Same functionality, but shows only the areas clipped by a given mask.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url, samplemap
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
     >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
 
     With default sample size. To get a new sample area, simply re-run the line.
 
     >>> samplemap(roads, points)
 
     Sample area with a radius of 5 kilometers.
 
     >>> samplemap(roads, points, size=5_000, column="meters")
 
     """
-
     if gdfs and isinstance(gdfs[-1], (float, int)):
         *gdfs, size = gdfs
 
     gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
     mask, kwargs = _get_location_mask(kwargs | {"size": size}, gdfs)
     kwargs.pop("size")
@@ -389,20 +391,19 @@
             or not in Jupyter, a static plot will be shown.
         browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    See also
+    See Also:
     --------
     explore: same functionality, but shows the entire area of the geometries.
     samplemap: same functionality, but shows only a random area of a given size.
     """
-
     gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
     if mask is None and len(gdfs) > 1:
         mask = gdfs[-1]
         gdfs = gdfs[:-1]
 
     center = kwargs.pop("center", None)
@@ -440,15 +441,15 @@
         m._gdf = m._gdf.clip(mask)
         m._nan_idx = m._gdf[m._column].isna()
         m._get_unique_values()
 
         qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
 
-def explore_locals(*gdfs, convert: bool = True, **kwargs):
+def explore_locals(*gdfs: GeoDataFrame, convert: bool = True, **kwargs) -> None:
     """Displays all local variables with geometries (GeoDataFrame etc.).
 
     Local means inside a function or file/notebook.
 
     Args:
         *gdfs: Additional GeoDataFrames.
         convert: If True (default), non-GeoDataFrames will be converted
@@ -474,23 +475,23 @@
                 local_gdfs[name] = value
                 continue
             if not convert:
                 continue
 
             if isinstance(value, dict) or hasattr(value, "__dict__"):
                 # add dicts or classes with GeoDataFrames to kwargs
-                for key, value in as_dict(value).items():
-                    if isinstance(value, allowed_types):
-                        gdf = clean_geoms(to_gdf_func(value))
+                for key, val in as_dict(value).items():
+                    if isinstance(val, allowed_types):
+                        gdf = clean_geoms(to_gdf_func(val))
                         if len(gdf):
                             local_gdfs[key] = gdf
 
-                    elif isinstance(value, dict) or hasattr(value, "__dict__"):
+                    elif isinstance(val, dict) or hasattr(val, "__dict__"):
                         try:
-                            for k, v in value.items():
+                            for k, v in val.items():
                                 if isinstance(v, allowed_types):
                                     gdf = clean_geoms(to_gdf_func(v))
                                     if len(gdf):
                                         local_gdfs[k] = gdf
                         except Exception:
                             # no need to raise here
                             pass
@@ -539,20 +540,21 @@
             GeoDataFrame is given a unique color.
         title: Text to use as the map's heading.
         black: If True (default), the background color will be black and the title
             white. If False, it will be the opposite. The colormap will also be
             'viridis' when black, and 'RdPu' when white.
         size: Size of the plot. Defaults to 10.
         title_fontsize: Size of the title.
+        legend: Whether to add legend. Defaults to True.
         cmap: Color palette of the map. See:
             https://matplotlib.org/stable/tutorials/colors/colormaps.html
         k: Number of color groups.
         **kwargs: Additional keyword arguments taken by the geopandas plot method.
 
-    See also:
+    See Also:
         ThematicMap: Class with more options for customising the plot.
     """
     gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
     new_kwargs = {}
     for key, value in kwargs.items():
         if isinstance(value, GeoDataFrame):
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/thematicmap.py` & `ssb_sgis-1.0.2/src/sgis/maps/thematicmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 """Make static maps with geopandas and matplotlib."""
+
 import warnings
+from typing import Any
 
 import matplotlib
+import matplotlib.figure
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 
-from .legend import ContinousLegend, Legend
+from .legend import ContinousLegend
+from .legend import Legend
 from .map import Map
 
-
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
 class ThematicMap(Map):
     """Class for creating static maps with geopandas and matplotlib.
 
     The class takes one or more GeoDataFrames and a column name. The class attributes
     can then be set to customise the map before plotting.
 
-    Args:
-        *gdfs: One or more GeoDataFrames.
-        column: The name of the column to plot.
-        size: Width and height of the plot in inches. Fontsize of title and legend is
-            adjusted accordingly. Defaults to 25.
-        black: If False (default), the background will be white and the text black. If
-            True, the background will be black and the text white. When True, the
-            default cmap is "viridis", and when False, the default is red to purple
-            (RdPu).
-
     Attributes:
         size (int): Width and height of the plot in inches.
         k (int): Number of color groups.
         legend (Legend): The legend object of the map. The legend holds its own set of
             attributes. See the Legend class for details.
         title (str): Title of the plot.
         title_color (str): Color of the title font.
@@ -46,15 +39,15 @@
             maximum value for the color groups.
         cmap (str): Colormap of the plot. See:
             https://matplotlib.org/stable/tutorials/colors/colormaps.html
         cmap_start (int): Start position for the color palette.
         cmap_stop (int): End position for the color palette.
         facecolor (str): Background color.
 
-    Examples
+    Examples:
     --------
     >>> import sgis as sg
     >>> points = sg.random_points(100).pipe(sg.buff, np.random.rand(100))
     >>> points2 = sg.random_points(100).pipe(sg.buff, np.random.rand(100))
 
     Simple plot with legend and title.
 
@@ -86,15 +79,28 @@
 
     def __init__(
         self,
         *gdfs: GeoDataFrame,
         column: str | None = None,
         size: int = 25,
         black: bool = False,
-    ):
+    ) -> None:
+        """Initialiser.
+
+        Args:
+            *gdfs: One or more GeoDataFrames.
+            column: The name of the column to plot.
+            size: Width and height of the plot in inches. Fontsize of title and legend is
+                adjusted accordingly. Defaults to 25.
+            black: If False (default), the background will be white and the text black. If
+                True, the background will be black and the text white. When True, the
+                default cmap is "viridis", and when False, the default is red to purple
+                (RdPu).
+
+        """
         super().__init__(*gdfs, column=column)
 
         self._size = size
         self._black = black
         self.background_gdfs = []
 
         self._title_fontsize = self._size * 2
@@ -102,28 +108,30 @@
         self.black = black
 
         if not self._is_categorical:
             self._choose_cmap()
 
         self._create_legend()
 
-    def change_cmap(self, cmap: str, start: int = 0, stop: int = 256):
+    def change_cmap(self, cmap: str, start: int = 0, stop: int = 256) -> "ThematicMap":
         """Change the color palette of the plot.
 
         Args:
             cmap: The colormap.
                 https://matplotlib.org/stable/tutorials/colors/colormaps.html
             start: Start position for the color palette. Defaults to 0.
             stop: End position for the color palette. Defaults to 256, which
                 is the end of the color range.
         """
         super().change_cmap(cmap, start, stop)
         return self
 
-    def add_background(self, gdf, color: str | None = None):
+    def add_background(
+        self, gdf: GeoDataFrame, color: str | None = None
+    ) -> "ThematicMap":
         """Add a GeoDataFrame as a background layer.
 
         Args:
             gdf: a GeoDataFrame.
             color: Single color. Defaults to gray (shade depends on whether the map
                 facecolor is black or white).
         """
@@ -141,15 +149,14 @@
         return self
 
     def plot(self, **kwargs) -> None:
         """Creates the final plot.
 
         This method should be run after customising the map, but before saving.
         """
-
         __test = kwargs.pop("__test", False)
         include_legend = bool(kwargs.pop("legend", self.legend))
 
         if "color" in kwargs:
             kwargs.pop("column", None)
             self.legend = None
             include_legend = False
@@ -210,15 +217,15 @@
         except FileNotFoundError:
             from dapla import FileClient
 
             fs = FileClient.get_gcs_file_system()
             with fs.open(path, "wb") as file:
                 plt.savefig(file)
 
-    def _prepare_plot(self, **kwargs):
+    def _prepare_plot(self, **kwargs) -> None:
         """Add figure and axis, title and background gdf."""
         for attr in self.__dict__.keys():
             if attr in self.kwargs:
                 self[attr] = self.kwargs.pop(attr)
             if attr in kwargs:
                 self[attr] = kwargs.pop(attr)
 
@@ -232,15 +239,15 @@
             self._actually_add_background()
 
         if hasattr(self, "title") and self.title:
             self.ax.set_title(
                 self.title, fontsize=self.title_fontsize, color=self.title_color
             )
 
-    def _prepare_continous_plot(self, kwargs) -> dict:
+    def _prepare_continous_plot(self, kwargs: dict) -> dict:
         """Create bins and colors."""
         self._prepare_continous_map()
 
         if self.scheme is None:
             self.legend = None
             kwargs["column"] = self.column
             return kwargs
@@ -266,15 +273,15 @@
             )
 
             if any(self._nan_idx):
                 self.bins = self.bins + [self.nan_label]
 
         return kwargs
 
-    def _prepare_categorical_plot(self, kwargs) -> dict:
+    def _prepare_categorical_plot(self, kwargs: dict) -> dict:
         """Map values to colors."""
         self._get_categorical_colors()
         colorarray = self._gdf["color"]
 
         kwargs["color"] = colorarray
         return kwargs
 
@@ -296,58 +303,60 @@
                 ax=self.ax,
                 bins=self.bins,
                 colors=self._unique_colors,
                 nan_label=self.nan_label,
                 bin_values=self._bins_unique_values,
             )
 
-    def _create_legend(self):
+    def _create_legend(self) -> None:
         """Instantiate the Legend class."""
         kwargs = {}
         if self._black:
             kwargs["facecolor"] = "#0f0f0f"
             kwargs["labelcolor"] = "#fefefe"
             kwargs["title_color"] = "#fefefe"
 
         if self._is_categorical:
             self.legend = Legend(title=self._column, size=self._size, **kwargs)
         else:
             self.legend = ContinousLegend(title=self._column, size=self._size, **kwargs)
 
-    def _choose_cmap(self):
-        """kwargs is to catch start and stop points for the cmap in __init__."""
+    def _choose_cmap(self) -> None:
+        """Kwargs is to catch start and stop points for the cmap in __init__."""
         if self._black:
             self._cmap = "viridis"
             self.cmap_start = 0
             self.cmap_stop = 256
         else:
             self._cmap = "RdPu"
             self.cmap_start = 23
             self.cmap_stop = 256
 
-    def _make_bin_value_dict(self, gdf, classified) -> dict:
+    def _make_bin_value_dict(self, gdf: GeoDataFrame, classified: np.ndarray) -> dict:
         """Dict with unique values of all bins. Used in labels in ContinousLegend."""
         bins_unique_values = {
             i: list(set(gdf.loc[classified == i, self._column]))
             for i, _ in enumerate(np.unique(classified))
         }
         return bins_unique_values
 
-    def _actually_add_background(self):
+    def _actually_add_background(self) -> None:
         self.ax.set_xlim([self.minx - self.diffx * 0.03, self.maxx + self.diffx * 0.03])
         self.ax.set_ylim([self.miny - self.diffy * 0.03, self.maxy + self.diffy * 0.03])
         self._background_gdfs.plot(ax=self.ax, color=self.bg_gdf_color)
 
     @staticmethod
-    def _get_matplotlib_figure_and_axix(figsize: tuple[int, int]):
+    def _get_matplotlib_figure_and_axix(
+        figsize: tuple[int, int]
+    ) -> tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
         fig = plt.figure(figsize=figsize)
         ax = fig.add_subplot(1, 1, 1)
         return fig, ax
 
-    def _black_or_white(self):
+    def _black_or_white(self) -> None:
         if self._black:
             self.facecolor, self.title_color, self.bg_gdf_color = (
                 "#0f0f0f",
                 "#fefefe",
                 "#383836",
             )
             self.nan_color = "#666666"
@@ -363,50 +372,54 @@
             self.nan_color = "#c2c2c2"
             if not self._is_categorical:
                 self.change_cmap("RdPu", start=23)
 
         self._create_legend()
 
     @property
-    def black(self):
+    def black(self) -> bool:
+        """Whether to use dark background and light text colors."""
         return self._black
 
     @black.setter
     def black(self, new_value: bool):
         self._black = new_value
         self._black_or_white()
 
     @property
-    def title_fontsize(self):
+    def title_fontsize(self) -> int:
+        """Title fontsize, not to be confused with legend.title_fontsize."""
         return self._title_fontsize
 
     @title_fontsize.setter
-    def title_fontsize(self, new_value: bool):
+    def title_fontsize(self, new_value: int) -> None:
         self._title_fontsize = new_value
         self._title_fontsize_has_been_set = True
 
     @property
-    def size(self):
+    def size(self) -> int:
+        """Size of the image."""
         return self._size
 
     @size.setter
-    def size(self, new_value: bool):
+    def size(self, new_value: bool) -> None:
         """Adjust font and marker size if not actively set."""
         self._size = new_value
         if not hasattr(self, "_title_fontsize_has_been_set"):
             self._title_fontsize = self._size * 2
         if not hasattr(self, "legend"):
             return
         if not hasattr(self.legend, "_title_fontsize_has_been_set"):
             self.legend._title_fontsize = self._size * 1.2
         if not hasattr(self.legend, "_fontsize_has_been_set"):
             self.legend._fontsize = self._size
         if not hasattr(self.legend, "_markersize_has_been_set"):
             self.legend._markersize = self._size
 
-    def __setattr__(self, __name: str, __value) -> None:
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        """Set an attribute with square brackets."""
         if "legend_" in __name:
             last_part = __name.split("legend_")[-1]
             raise AttributeError(
                 f"Invalid attribute {__name!r}. Did you mean 'legend.{last_part}'?"
             )
         return super().__setattr__(__name, __value)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/maps/tilesources.py` & `ssb_sgis-1.0.2/src/sgis/maps/tilesources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-from xyzservices import TileProvider, Bunch, providers
+from xyzservices import Bunch
+from xyzservices import TileProvider
+from xyzservices import providers
 
 kartverket = Bunch(
     norgeskart=TileProvider(
         name="Norgeskart",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=norgeskart_bakgrunn&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     bakgrunnskart_forenklet=TileProvider(
         name="Norgeskart forenklet",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=bakgrunnskart_forenklet&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     norges_grunnkart=TileProvider(
         name="Norges grunnkart",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=norges_grunnkart&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     norges_grunnkart_gråtone=TileProvider(
         name="Norges grunnkart gråtone",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=norges_grunnkart_graatone&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     n50=TileProvider(
         name="N5 til N50 kartdata",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=kartdata3&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     topogråtone=TileProvider(
         name="Topografisk norgeskart gråtone",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=topo4graatone&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     toporaster=TileProvider(
         name="Topografisk raster",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_gmaps?layers=toporaster4&zoom={z}&x={x}&y={y}",
         attribution="© Kartverket",
         html_attribution='&copy; <a href="https://kartverket.no">Kartverket</a>',
     ),
-
     norge_i_bilder=TileProvider(
         name="Norge i bilder",
         url="https://opencache.statkart.no/gatekeeper/gk/gk.open_nib_web_mercator_wmts_v2?SERVICE=WMTS&REQUEST=GetTile&VERSION=1.0.0&LAYER=Nibcache_web_mercator_v2&STYLE=default&FORMAT=image/jpgpng&tileMatrixSet=default028mm&tileMatrix={z}&tileRow={y}&tileCol={x}",
         max_zoom=19,
         attribution="© Geovekst",
     ),
 )
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-from xyzservices import TileProvider, Bunch, providers kartverket = Bunch
-( norgeskart=TileProvider( name="Norgeskart", url="https://
-opencache.statkart.no/gatekeeper/gk/
+from xyzservices import Bunch from xyzservices import TileProvider from
+xyzservices import providers kartverket = Bunch( norgeskart=TileProvider
+( name="Norgeskart", url="https://opencache.statkart.no/gatekeeper/gk/
 gk.open_gmaps?layers=norgeskart_bakgrunn&zoom={z}&x={x}&y={y}", attribution="Â©
 Kartverket", html_attribution='© _K_a_r_t_v_e_r_k_e_t', ),
 bakgrunnskart_forenklet=TileProvider( name="Norgeskart forenklet", url="https:/
 /opencache.statkart.no/gatekeeper/gk/
 gk.open_gmaps?layers=bakgrunnskart_forenklet&zoom={z}&x={x}&y={y}",
 attribution="Â© Kartverket", html_attribution='© _K_a_r_t_v_e_r_k_e_t', ),
 norges_grunnkart=TileProvider( name="Norges grunnkart", url="https://
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/_get_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
 from pandas import DataFrame
 
 
 def _get_route_frequencies(
-    graph,
+    graph: Graph,
     roads: GeoDataFrame,
     weight_df: DataFrame,
 ) -> GeoDataFrame:
     """Function used in the get_route_frequencies method of NetworkAnalysis."""
     warnings.filterwarnings("ignore", category=RuntimeWarning)
 
     resultlist: list[DataFrame] = []
@@ -56,15 +56,14 @@
 def _get_route(
     graph: Graph,
     weight: str,
     roads: GeoDataFrame,
     od_pairs: pd.MultiIndex,
 ) -> GeoDataFrame:
     """Function used in the get_route method of NetworkAnalysis."""
-
     warnings.filterwarnings("ignore", category=RuntimeWarning)
 
     resultlist: list[DataFrame] = []
 
     for ori_id in od_pairs.get_level_values(0).unique():
         relevant_pairs = od_pairs[od_pairs.get_level_values(0) == ori_id]
         destinations = relevant_pairs.get_level_values(1)
@@ -82,15 +81,16 @@
             line_ids = _create_line_id_df(indices["src_tgt_wt"], ori_id, des_id)
 
             resultlist.append(line_ids)
 
     if not resultlist:
         warnings.warn(
             "No paths were found. Try larger search_tolerance or search_factor. "
-            "Or close_network_holes() or remove_isolated()."
+            "Or close_network_holes() or remove_isolated().",
+            stacklevel=1,
         )
         return pd.DataFrame(columns=["origin", "destination", weight, "geometry"])
 
     results: DataFrame = pd.concat(resultlist)
     assert list(results.columns) == ["origin", "destination"], list(results.columns)
     lines: GeoDataFrame = _get_line_geometries(results, roads, weight)
     lines = lines.dissolve(by=["origin", "destination"], aggfunc="sum", as_index=False)
@@ -117,15 +117,16 @@
         )
         if k_lines is not None:
             resultlist.append(k_lines)
 
     if not resultlist:
         warnings.warn(
             "No paths were found. Try larger search_tolerance or search_factor. "
-            "Or close_network_holes() or remove_isolated()."
+            "Or close_network_holes() or remove_isolated().",
+            stacklevel=1,
         )
         return pd.DataFrame(columns=["origin", "destination", weight, "geometry"])
 
     results: DataFrame = pd.concat(resultlist)
 
     assert list(results.columns) == ["origin", "destination", "k"], list(
         results.columns
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         results = gpd.GeoDataFrame(results, geometry="geometry", crs=25833)
 
     results = results.drop(["wkt_ori", "wkt_des"], axis=1, errors="ignore")
 
     return results.reset_index(drop=True)
 
 
-def _get_od_df(graph, origins, destinations, weight_col):
+def _get_od_df(
+    graph: Graph, origins: GeoDataFrame, destinations: GeoDataFrame, weight_col: str
+) -> pd.DataFrame:
     distances: list[list[float]] = graph.distances(
         weights="weight",
         source=origins,
         target=destinations,
     )
 
     ori_idx, des_idx, costs = [], [], []
@@ -64,7 +66,48 @@
     return (
         pd.DataFrame(
             data={"origin": ori_idx, "destination": des_idx, weight_col: costs}
         )
         .replace([np.inf, -np.inf], np.nan)
         .reset_index(drop=True)
     )
+
+
+def _get_one_od_df(
+    graph: Graph, origins: GeoDataFrame, destinations: GeoDataFrame, weight_col: str
+) -> pd.DataFrame:
+    distances: list[list[float]] = graph.distances(
+        weights="weight",
+        source=origins,
+        target=destinations,
+    )
+
+    ori_idx, des_idx, costs = [], [], []
+    for i, f_idx in enumerate(origins):
+        for j, t_idx in enumerate(destinations):
+            ori_idx.append(f_idx)
+            des_idx.append(t_idx)
+            costs.append(distances[i][j])
+
+    return (
+        pd.DataFrame(
+            data={"origin": ori_idx, "destination": des_idx, weight_col: costs}
+        )
+        .replace([np.inf, -np.inf], np.nan)
+        .reset_index(drop=True)
+    )
+
+
+# def _get_od_df(
+#     graph: Graph,
+#     origins: GeoDataFrame,
+#     destinations: GeoDataFrame,
+#     weight_col: str,
+# ) -> pd.DataFrame:
+#     from ..parallel.parallel import Parallel
+
+#     results: list[pd.DataFrame] = Parallel(40, backend="loky").map(
+#         _get_one_od_df,
+#         [origins[origins.index == i] for i in origins.index.unique()],
+#         kwargs=dict(graph=graph, destinations=destinations, weight_col=weight_col),
+#     )
+#     return pd.concat(results, ignore_index=True)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/_points.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from collections.abc import Sequence
+
 import numpy as np
+import pandas as pd
 from geopandas import GeoDataFrame
 
 from ..geopandas_tools.neighbors import get_k_nearest_neighbors
 from .networkanalysisrules import NetworkAnalysisRules
 
-
 """
 These are internal classes used in the NetworkAnalysis class. The classes used in
 NetworkAnalysis are Origins and Destinations, which are subclasses of Points. The
 Origins and Destinations classes are the same, except that the edges are in
 opposite directions.
 """
 
@@ -22,25 +24,26 @@
 
     def _make_temp_idx(self, start: int) -> None:
         """Make a temporary id column thad don't overlap with the node ids.
 
         The original indices are stored in a dict and mapped back to the results in the
         end.
         """
-
         self.gdf["temp_idx"] = np.arange(start=start, stop=start + len(self.gdf))
         self.gdf["temp_idx"] = self.gdf["temp_idx"].astype(str)
 
         self.idx_dict = {
             temp_idx: idx
             for temp_idx, idx in zip(self.gdf.temp_idx, self.gdf.index, strict=True)
         }
 
     @staticmethod
-    def _convert_distance_to_weight(distances, rules):
+    def _convert_distance_to_weight(
+        distances: Sequence, rules: NetworkAnalysisRules
+    ) -> list[float]:
         """Meters to minutes based on 'weight_to_nodes_' attribute of the rules."""
         if not rules.nodedist_multiplier and not rules.nodedist_kmh:
             return [0 for _ in distances]
 
         if rules.nodedist_multiplier and rules.nodedist_kmh:
             raise ValueError(
                 "Can only specify one of 'nodedist_multiplier' and 'nodedist_kmh'"
@@ -56,25 +59,28 @@
         if rules.nodedist_kmh and rules.weight != "minutes":
             raise ValueError(
                 "Can only specify 'nodedist_kmh' when the 'weight' is minutes"
             )
 
         return [x / (16.666667 * rules.nodedist_kmh) for x in distances]
 
-    def _make_edges(self, df, from_col, to_col):
+    def _make_edges(
+        self, df: GeoDataFrame | pd.DataFrame, from_col: str, to_col: str
+    ) -> list[tuple[int, int]]:
         return [(f, t) for f, t in zip(df[from_col], df[to_col], strict=True)]
 
     def _get_edges_and_weights(
         self,
         nodes: GeoDataFrame,
         rules: NetworkAnalysisRules,
         k: int,
         from_col: str,
         to_col: str,
     ):
+        """Make edges and weights between points and the nodes of a network."""
         distances = get_k_nearest_neighbors(
             gdf=self.gdf.set_index("temp_idx"),
             neighbors=nodes.set_index("node_id"),
             k=k,
         )
 
         distances["distance_min"] = distances.groupby(level=0)["distance"].min()
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/_service_area.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
-from shapely import force_2d, reverse, unary_union
-from shapely.geometry import MultiLineString, MultiPoint, Point
+from shapely import force_2d
+from shapely import reverse
+from shapely import unary_union
+from shapely.geometry import MultiPoint
+from shapely.geometry import Point
 from shapely.ops import nearest_points
 from shapely.wkt import loads
 
 from ..geopandas_tools.sfilter import sfilter
 from .cutting_lines import cut_lines_once
 from .nodes import make_edge_wkt_cols
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,29 @@
 """Functions for filling gaps in the network with straight lines."""
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from pandas import DataFrame
 from shapely import shortest_line
 
-from ..geopandas_tools.conversion import coordinate_array, to_geoseries
-from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.conversion import coordinate_array
 from ..geopandas_tools.neighbors import k_nearest_neighbors
-from .nodes import make_edge_wkt_cols, make_node_ids
-
-
-def close_network_holes_to(
-    lines: GeoDataFrame | GeoSeries,
-    extend_to: GeoDataFrame | GeoSeries,
-    max_distance: int | float,
-    max_angle: int | float,
-) -> GeoDataFrame | GeoSeries:
-    if isinstance(lines, GeoSeries):
-        lines = lines.to_frame("geometry")
-        was_geoseries = True
-    else:
-        was_geoseries = False
-
-    lines, _ = make_node_ids(lines)
-
-    if isinstance(extend_to, GeoSeries):
-        extend_to = extend_to.to_frame("geometry")
-
-    if not (extend_to.geom_type == "Point").all():
-        raise ValueError("'extend_to' must be singlepart point geometries")
-
-    extend_to["wkt"] = extend_to.geometry.to_wkt()
-    extend_to = extend_to.drop_duplicates("wkt")
-    extend_to["node_id"] = range(len(extend_to))
-
-    new_lines: GeoSeries = _close_holes_all_lines(
-        lines, extend_to, max_distance=max_distance, max_angle=max_angle, idx_start=0
-    )
-
-    if was_geoseries:
-        return pd.concat([lines.geometry, new_lines])
-
-    new_lines = gpd.GeoDataFrame(
-        {"geometry": new_lines}, geometry="geometry", crs=lines.crs
-    )
-
-    return pd.concat([lines, new_lines], ignore_index=True).drop(
-        columns=[
-            "source_wkt",
-            "target_wkt",
-            "source",
-            "target",
-            "n_source",
-            "n_target",
-        ]
-    )
+from .nodes import make_edge_wkt_cols
+from .nodes import make_node_ids
 
 
 def close_network_holes(
     gdf: GeoDataFrame,
     max_distance: int | float,
     max_angle: int,
     hole_col: str | None = "hole",
-):
+) -> GeoDataFrame:
     """Fills network gaps with straigt lines.
 
     Fills holes in the network by connecting deadends with the nodes that are
     within the 'max_distance' distance.
 
     Args:
         gdf: GeoDataFrame with lines.
@@ -85,15 +39,15 @@
     Returns:
         The input GeoDataFrame with new lines added.
 
     Note:
         The holes will have missing values in the weight column used in
         NetworkAnalysis. These values must be filled before analysis.
 
-    Examples
+    Examples:
     --------
     Read road data with small gaps.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
     Roads need to be singlepart linestrings for this to work.
@@ -101,18 +55,18 @@
     >>> from shapely import line_merge
     >>> roads.geometry = line_merge(roads.geometry)
 
     Fill gaps shorter than 1.1 meters.
 
     >>> filled = sg.close_network_holes(roads, max_distance=1.1, max_angle=180)
     >>> filled.hole.value_counts()
-    Name: connected, dtype: int64
+    hole
     0    93395
     1     7102
-    Name: hole, dtype: int64
+    Name: count, dtype: int64
 
     Compare the number of isolated lines before and after.
 
     >>> roads = sg.get_connected_components(roads)
     >>> roads.connected.value_counts()
     1.0    85638
     0.0     7757
@@ -124,23 +78,23 @@
     0.0       180
     Name: connected, dtype: int64
 
     Fill only gaps with an angle deviation between 0 and 30 compared to the prior line.
 
     >>> filled = sg.close_network_holes(roads, max_distance=1.1, max_angle=30)
     >>> filled.hole.value_counts()
+    hole
     0    93395
     1     7092
-    Name: hole, dtype: int64
+    Name: count, dtype: int64
 
     It's not always wise to fill gaps. In the case of this data, these small gaps are
     intentional. They are road blocks where most cars aren't allowed to pass. Fill the
     holes only if it makes the travel times/routes more realistic.
     """
-
     lines, nodes = make_node_ids(gdf)
 
     # remove duplicates of lines going both directions
     lines["sorted"] = [
         "_".join(sorted([s, t]))
         for s, t in zip(lines["source"], lines["target"], strict=True)
     ]
@@ -170,43 +124,43 @@
         lines[hole_col] = (
             0 if hole_col not in lines.columns else lines[hole_col].fillna(0)
         )
 
     return pd.concat([lines, new_lines], ignore_index=True)
 
 
-def get_angle(array_a, array_b):
+def get_angle(array_a: np.ndarray, array_b: np.ndarray) -> np.ndarray:
     dx = array_b[:, 0] - array_a[:, 0]
     dy = array_b[:, 1] - array_a[:, 1]
 
     angles_rad = np.arctan2(dx, dy)
     angles_degrees = np.degrees(angles_rad)
     return angles_degrees
 
 
 def close_network_holes_to_deadends(
     gdf: GeoDataFrame,
     max_distance: int | float,
     hole_col: str | None = "hole",
-):
+) -> GeoDataFrame:
     """Fills gaps between two deadends if the distance is less than 'max_distance'.
 
     Fills holes between deadends in the network with straight lines if the distance is
     less than 'max_distance'.
 
     Args:
         gdf: GeoDataFrame with lines
         max_distance: The maximum distance between two nodes to be considered a hole.
         hole_col: If you want to keep track of which lines were added, you can add a
             column with a value of 1. Defaults to 'hole'
 
     Returns:
         The input GeoDataFrame with new lines added.
 
-    Examples
+    Examples:
     --------
     Read road data with small gaps.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
     Roads need to be singlepart linestrings for this to work.
@@ -242,28 +196,32 @@
     if not len(new_lines):
         gdf[hole_col] = 0 if hole_col not in gdf.columns else gdf[hole_col].fillna(0)
         return gdf
 
     new_lines = make_edge_wkt_cols(new_lines)
 
     wkt_id_dict = {
-        wkt: id for wkt, id in zip(nodes["wkt"], nodes["node_id"], strict=True)
+        wkt: id_ for wkt, id_ in zip(nodes["wkt"], nodes["node_id"], strict=True)
     }
     new_lines["source"] = new_lines["source_wkt"].map(wkt_id_dict)
     new_lines["target"] = new_lines["target_wkt"].map(wkt_id_dict)
 
     if hole_col:
         new_lines[hole_col] = 1
         gdf[hole_col] = 0 if hole_col not in gdf.columns else gdf[hole_col].fillna(0)
 
     return pd.concat([gdf, new_lines], ignore_index=True)
 
 
 def _close_holes_all_lines(
-    lines, nodes, max_distance, max_angle, idx_start: int
+    lines: GeoDataFrame,
+    nodes: GeoDataFrame,
+    max_distance: int | None,
+    max_angle: int | None,
+    idx_start: int,
 ) -> GeoSeries:
     k = min(len(nodes), 50)
 
     # make point gdf for the deadends and the other endpoint of the deadend lines
     deadends_target = lines.loc[lines["n_target"] == 1].rename(
         columns={"target_wkt": "wkt", "source_wkt": "wkt_other_end"}
     )
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/cutting_lines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 """Cutting and splitting line geometries."""
+
 import warnings
 
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
-from pandas import DataFrame, Series
-from shapely import (
-    buffer,
-    extract_unique_points,
-    force_2d,
-    get_coordinates,
-    get_parts,
-    linestrings,
-    touches,
-    unary_union,
-)
-from shapely.geometry import LineString, Point
+from geopandas import GeoDataFrame
+from pandas import DataFrame
+from pandas import Series
+from shapely import extract_unique_points
+from shapely import force_2d
+from shapely.geometry import LineString
+from shapely.geometry import Point
 
 from ..geopandas_tools.buffer_dissolve_explode import buff
 from ..geopandas_tools.conversion import to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..geopandas_tools.neighbors import get_k_nearest_neighbors
-from ..geopandas_tools.point_operations import (
-    _shapely_snap,
-    snap_all,
-    snap_within_distance,
-)
+from ..geopandas_tools.point_operations import snap_all
+from ..geopandas_tools.point_operations import snap_within_distance
 from ..geopandas_tools.sfilter import sfilter_split
 from .nodes import make_edge_coords_cols
 
 
 def split_lines_by_nearest_point(
     gdf: GeoDataFrame,
     points: GeoDataFrame,
@@ -55,15 +47,15 @@
         A GeoDataFrame with the same columns as the input lines, but with the lines
         split at the closest point to the points. If no lines are within 'max_distance'
         from any points, 'gdf' is returned as it came.
 
     Raises:
         ValueError: If the crs of the input data differs.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url, split_lines_by_nearest_point
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
     >>> rows = len(roads)
     >>> rows
     93395
@@ -144,16 +136,16 @@
 
     # get line endpoints as columns (source_coords and target_coords)
     splitted = make_edge_coords_cols(splitted)
 
     splitted_source = to_gdf(splitted["source_coords"], crs=gdf.crs)
     splitted_target = to_gdf(splitted["target_coords"], crs=gdf.crs)
 
-    def get_nearest(splitted, snapped) -> pd.DataFrame:
-        """find the nearest snapped point for each source and target of the lines"""
+    def get_nearest(splitted: GeoDataFrame, snapped: GeoDataFrame) -> pd.DataFrame:
+        """Find the nearest snapped point for each source and target of the lines."""
         return get_k_nearest_neighbors(splitted, snapped, k=1).loc[
             lambda x: x["distance"] <= PRECISION * 2
         ]
 
     # snapped = snapped.set_index("point_coords")
     snapped.index = snapped.geometry
     dists_source = get_nearest(splitted_source, snapped)
@@ -162,91 +154,111 @@
     # neighbor_index: point coordinates as tuple
     pointmapper_source: pd.Series = dists_source["neighbor_index"]
     pointmapper_target: pd.Series = dists_target["neighbor_index"]
 
     # now, we can replace the source/target coordinate with the coordinates of
     # the snapped points.
 
-    splitted = change_line_endpoint(
+    splitted = _change_line_endpoint(
         splitted,
         indices=dists_source.index,
         pointmapper=pointmapper_source,
         change_what="first",
     )  # i=0)
 
     # same for the lines where the target was split, but change the last coordinate
-    splitted = change_line_endpoint(
+    splitted = _change_line_endpoint(
         splitted,
         indices=dists_target.index,
         pointmapper=pointmapper_target,
         change_what="last",
     )  # , i=-1)
 
     if splitted_col:
         splitted[splitted_col] = 1
 
     return pd.concat([the_other_lines, splitted, circles], ignore_index=True).drop(
         ["source_coords", "target_coords"], axis=1
     )
 
 
-def change_line_endpoint(
+def _change_line_endpoint(
     gdf: GeoDataFrame,
     indices: pd.Index,
     pointmapper: pd.Series,
     change_what: str | int,
 ) -> GeoDataFrame:
-    """
-    Loop for each line where the source is the endpoint that was split
-    change the first point of the line to the point it was split by
+    """Modify the endpoints of selected lines in a GeoDataFrame based on an index mapping.
+
+    This function updates the geometry of specified line features within a GeoDataFrame,
+    changing either the first or last point of each line to new coordinates provided by a mapping.
+    It is typically used in scenarios where line endpoints need to be adjusted to new locations,
+    such as in network adjustments or data corrections.
+
+    Args:
+        gdf: A GeoDataFrame containing line geometries.
+        indices: An Index object identifying the rows in the GeoDataFrame whose endpoints will be changed.
+        pointmapper: A Series mapping from the index of lines to new point geometries.
+        change_what: Specifies which endpoint of the line to change. Accepts 'first' or 0 for the
+            starting point, and 'last' or -1 for the ending point.
+
+    Returns:
+        A GeoDataFrame with the specified line endpoints updated according to the pointmapper.
+
+    Raises:
+        ValueError: If `change_what` is not one of the accepted values ('first', 'last', 0, -1).
     """
     assert gdf.index.is_unique
 
     if change_what == "first" or change_what == 0:
-        to_be_changed = lambda x: ~x.index.duplicated(keep="first")
+        keep = "first"
     elif change_what == "last" or change_what == -1:
-        to_be_changed = lambda x: ~x.index.duplicated(keep="last")
+        keep = "last"
     else:
         raise ValueError(
             f"change_what should be 'first' or 'last' or 0 or -1. Got {change_what}"
         )
 
     is_relevant = gdf.index.isin(indices)
     relevant_lines = gdf.loc[is_relevant]
 
     relevant_lines.geometry = extract_unique_points(relevant_lines.geometry)
     relevant_lines = relevant_lines.explode(index_parts=False)
 
-    relevant_lines.loc[to_be_changed, "geometry"] = (
-        relevant_lines.loc[to_be_changed].index.map(pointmapper).values
+    relevant_lines.loc[lambda x: ~x.index.duplicated(keep=keep), "geometry"] = (
+        relevant_lines.loc[lambda x: ~x.index.duplicated(keep=keep)]
+        .index.map(pointmapper)
+        .values
     )
 
     relevant_lines_mapped = relevant_lines.groupby(level=0)["geometry"].agg(LineString)
 
     gdf.loc[is_relevant, "geometry"] = relevant_lines_mapped
 
     return gdf
 
 
-def cut_lines(gdf: GeoDataFrame, max_length: int, ignore_index=False) -> GeoDataFrame:
+def cut_lines(
+    gdf: GeoDataFrame, max_length: int, ignore_index: bool = False
+) -> GeoDataFrame:
     """Cuts lines of a GeoDataFrame into pieces of a given length.
 
     Args:
         gdf: GeoDataFrame.
         max_length: The maximum length of the lines in the output GeoDataFrame.
         ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
             Defaults to False.
 
     Returns:
         A GeoDataFrame with lines cut to the maximum distance.
 
     Note:
         This method is time consuming for large networks and low 'max_length'.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url, cut_lines
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> roads.length.describe().round(1)
     count    93395.0
     mean        41.2
     std         78.5
@@ -310,15 +322,15 @@
     Args:
         gdf: GeoDataFrame.
         distances: The distance from the start of the lines to cut at. Either a number,
             the name of a column or array-like of same length as the line GeoDataFrame.
         ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
             Defaults to False.
 
-    Examples
+    Examples:
     --------
     >>> from sgis import cut_lines_once, to_gdf
     >>> import pandas as pd
     >>> from shapely.geometry import LineString
     >>> gdf = to_gdf(LineString([(0, 0), (1, 1), (2, 2)]))
     >>> gdf = pd.concat([gdf, gdf, gdf])
     >>> gdf
@@ -340,32 +352,32 @@
 
     Cut distance as column.
 
     >>> gdf["dist"] = [1, 2, 3]
     >>> cut_lines_once(gdf, "dist")
                                                 geometry  dist
     0      LINESTRING (0.00000 0.00000, 0.70711 0.70711)     1
-    1  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
-    2  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
-    3      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
-    4  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
+    0  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
+    0      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
 
     Cut distance as list (same result as above).
 
     >>> cut_lines_once(gdf, [1, 2, 3])
                                                 geometry  dist
     0      LINESTRING (0.00000 0.00000, 0.70711 0.70711)     1
-    1  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
-    2  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
-    3      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
-    4  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
+    0  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
+    0      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
     """
 
     def _cut(line: LineString, distance: int | float) -> list[LineString]:
-        """From the shapely docs"""
+        """From the shapely docs."""
         if distance <= 0.0 or distance >= line.length:
             return line
         coords = list(line.coords)
         for i, p in enumerate(coords):
             prd = line.project(Point(p))
             if prd == distance:
                 return [LineString(coords[: i + 1]), LineString(coords[i:])]
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/directednetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Prepare a GeoDataFrame of line geometries for directed network analysis."""
 
 import warnings
+from collections.abc import Sequence
 
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.constructive import reverse
 
-from ..helpers import return_two_vals, unit_is_meters
+from ..helpers import return_two_vals
+from ..helpers import unit_is_meters
 
 
 def make_directed_network_norway(gdf: GeoDataFrame, dropnegative: bool) -> GeoDataFrame:
     """Runs the method make_directed_network for Norwegian road data.
 
     The parameters in make_directed_network are set to the correct values for
     Norwegian road data as of 2023.
@@ -22,15 +24,15 @@
         gdf: Road GeoDataFrame.
         dropnegative: Whether to keep rows with negative minute values in both directions.
             These are mostly circles with no impact on the analyses, but there might be
             exceptions. Keeping negative values will result in an error when building the
             network graph. Recode these rows to a non-negative values if you want
             to keep them.
 
-    Examples
+    Examples:
     --------
     2022 data for the municipalities of Oslo and Eidskog can be read directly like this:
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url(
     ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
     ... )
@@ -43,33 +45,35 @@
     199733      FT      0.009097     -1.000000  MULTILINESTRING Z ((271877.373 6653214.697 141...
     ...        ...           ...           ...                                                ...
     1944129     FT      0.010482     -1.000000  MULTILINESTRING Z ((268649.503 6651869.320 111...
     1944392      B      0.135561      0.135561  MULTILINESTRING Z ((259501.570 6648459.580 3.2...
     1944398      B      0.068239      0.068239  MULTILINESTRING Z ((258292.600 6648313.440 18....
     1944409      B      0.023629      0.023629  MULTILINESTRING Z ((258291.452 6648289.258 19....
     1944415      B      0.175876      0.175876  MULTILINESTRING Z ((260762.830 6650240.620 43....
-    [93395 rows x 46 columns]
+    <BLANKLINE>
+    [93395 rows x 4 columns]
 
     And converted to a directed network like this:
 
-    >>> roads_directed = sg.make_directed_network_norway(roads)
+    >>> roads_directed = sg.make_directed_network_norway(roads, dropnegative=True)
     >>> roads_directed[["minutes", "geometry"]]
              minutes                                           geometry
     0       0.216611  MULTILINESTRING Z ((258028.440 6674249.890 413...
     1       0.028421  MULTILINESTRING Z ((266382.600 6639604.600 -99...
     2       0.047592  MULTILINESTRING Z ((266349.200 6639372.499 171...
     3       0.026180  MULTILINESTRING Z ((266360.515 6639120.493 172...
     4       0.023978  MULTILINESTRING Z ((266351.263 6639416.154 169...
     ...          ...                                                ...
     175620  0.007564  MULTILINESTRING Z ((268641.225 6651871.624 111...
     175621  0.020246  MULTILINESTRING Z ((268669.748 6651890.291 110...
     175622  0.036810  MULTILINESTRING Z ((268681.757 6651886.457 110...
     175623  0.003019  MULTILINESTRING Z ((268682.748 6651886.162 110...
     175624  0.036975  MULTILINESTRING Z ((268694.594 6651881.688 111...
-    [175541 rows x 45 columns]
+    <BLANKLINE>
+    [175541 rows x 2 columns]
     """
     if gdf["drivetime_fw"].isna().any():
         raise ValueError("Missing values in the columns 'drivetime_fw'")
     if gdf["drivetime_bw"].isna().any():
         raise ValueError("Missing values in the columns 'drivetime_bw'")
 
     return make_directed_network(
@@ -198,30 +202,34 @@
     if flat_speed_kmh:
         meters_per_min = (flat_speed_kmh / 60) * 1000
         gdf["minutes"] = gdf.length / meters_per_min
 
     return gdf
 
 
-def _validate_minute_args(minute_cols, speed_col_kmh, flat_speed_kmh):
+def _validate_minute_args(
+    minute_cols: Sequence[str], speed_col_kmh: str, flat_speed_kmh: str
+) -> None:
     if not minute_cols and not speed_col_kmh and not flat_speed_kmh:
         warnings.warn(
             "Minute column will not be calculated when both 'minute_cols', "
             "'speed_col_kmh' and 'flat_speed_kmh' is None",
             stacklevel=2,
         )
 
     if sum([bool(minute_cols), bool(speed_col_kmh), bool(flat_speed_kmh)]) > 1:
         raise ValueError(
             "Can only calculate minutes from either 'speed_col_kmh', "
             "'minute_cols' or 'flat_speed_kmh'."
         )
 
 
-def _validate_direction_args(gdf, direction_col, direction_vals_bft):
+def _validate_direction_args(
+    gdf: GeoDataFrame, direction_col: str, direction_vals_bft: Sequence[str]
+) -> None:
     if len(direction_vals_bft) != 3:
         raise ValueError(
             "'direction_vals_bft' should be tuple/list with values of directions "
             "both, from and to. E.g. ('B', 'F', 'T')"
         )
 
     b, f, t = direction_vals_bft
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     Args:
         gdf: A GeoDataFrame of lines.
 
     Returns:
         The GeoDataFrame with a new column "connected".
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url, get_connected_components
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
     >>> roads = get_connected_components(roads)
     >>> roads.connected.value_counts()
     1.0    85638
@@ -71,27 +71,28 @@
 
     Args:
         gdf: a GeoDataFrame of lines.
 
     Returns:
         A GeoDataFrame with a new column "component_size".
 
-    Examples
+    Examples:
     --------
     >>> from sgis import read_parquet_url, get_component_size
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
     >>> roads = get_component_size(roads)
     >>> roads.component_size.value_counts().head()
+    component_size
     79180    85638
     2         1601
     4          688
     6          406
     3          346
-    Name: component_size, dtype: int64
+    Name: count, dtype: int64
     """
     gdf, _ = make_node_ids(gdf)
 
     edges = [
         (str(source), str(target))
         for source, target in zip(gdf["source"], gdf["target"], strict=True)
     ]
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/network.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Network class with methods for manipulating line geometries.
 
 The module includes functions for cutting and splitting lines, filling holes in the
 network, finding and removing isolated network islands and creating unique node ids.
 """
 
 import warnings
-from copy import copy, deepcopy
+from copy import copy
+from copy import deepcopy
 
 import numpy as np
 from geopandas import GeoDataFrame
 from pandas import DataFrame
 from shapely import line_merge
 
 from ..exceptions import ZeroLinesError
@@ -17,17 +18,20 @@
 from ..geopandas_tools.geometry_types import to_single_geom_type
 from .nodes import make_node_ids
 
 
 class Network:
     """Class used in NetworkAnalysis."""
 
-    def __init__(self, gdf: GeoDataFrame):
+    def __init__(self, gdf: GeoDataFrame) -> None:
         """The lines are fixed, welded together rowwise and exploded. Creates node-ids.
 
+        Args:
+            gdf: GeoDataFrame of line geometries to make up the network.
+
         Raises:
             TypeError: If 'gdf' is not of type GeoDataFrame.
             ZeroLinesError: If 'gdf' has zero rows.
         """
         if not isinstance(gdf, GeoDataFrame):
             raise TypeError(f"'lines' should be GeoDataFrame, got {type(gdf)}")
 
@@ -148,45 +152,46 @@
 
         if any(removed):
             return False
 
         return True
 
     def get_edges(self) -> list[tuple[str, str]]:
+        """Get a list of edges in the network."""
         return [
             (str(source), str(target))
             for source, target in zip(
                 self.gdf["source"], self.gdf["target"], strict=True
             )
         ]
 
     @staticmethod
     def _create_edge_ids(
         edges: list[tuple[str, str]], weights: list[float]
     ) -> list[str]:
         """Edge identifiers represented with source and target ids and the weight."""
         return [f"{s}_{t}_{w}" for (s, t), w in zip(edges, weights, strict=True)]
 
-    def _update_nodes_if(self):
+    def _update_nodes_if(self) -> None:
         if not self._nodes_are_up_to_date():
             self._make_node_ids()
 
     @property
-    def nodes(self):
+    def nodes(self) -> GeoDataFrame:
         """GeoDataFrame with the network nodes (line endpoints).
 
         Upon instantiation of the class, a GeoDataFrame of points is created from the
         unique endpoints of the lines. The node ids are then used to make the 'source'
         and 'target' columns of the line gdf. The nodes are remade every time the
         geometries of the line gdf changes, since the 'source' and 'target' columns
         must be up to date with the actual line geometries when making the graph.
         """
         return self._nodes
 
-    def _warn_if_undirected(self):
+    def _warn_if_undirected(self) -> None:
         """Road data often have to be duplicated and flipped to make it directed."""
         if self.percent_bidirectional > 5:
             return
 
         mess = (
             "Your network is likely not directed. "
             f"Only {self.percent_bidirectional:.1f} percent of the lines go both ways."
@@ -198,31 +203,28 @@
             )
         else:
             mess = mess + "Try running 'make_directed_network'"
 
         warnings.warn(mess, stacklevel=2)
 
     @property
-    def percent_bidirectional(self):
+    def percent_bidirectional(self) -> float:
         """The percentage of lines that appear in both directions."""
         return self._percent_bidirectional
 
-    def copy(self):
+    def copy(self) -> "Network":
         """Returns a shallow copy of the class instance."""
         return copy(self)
 
-    def deepcopy(self):
+    def deepcopy(self) -> "Network":
         """Returns a deep copy of the class instance."""
         return deepcopy(self)
 
     def __repr__(self) -> str:
         """The print representation."""
         cl = self.__class__.__name__
         km = int(sum(self.gdf.length) / 1000)
         return f"{cl}({km} km, percent_bidirectional={self._percent_bidirectional})"
 
-    def __iter__(self):
-        """So the attributes can be iterated through."""
-        return iter(self.__dict__.items())
-
-    def __len__(self):
+    def __len__(self) -> int:
+        """Number og rows in the GeoDataFrame."""
         return len(self.gdf)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Contains the NetworkAnalysis class.
 
 The class has five analysis methods: od_cost_matrix, get_route, get_k_routes,
 get_route_frequencies and service_area.
 """
 
-
-from copy import copy, deepcopy
+from copy import copy
+from copy import deepcopy
 from datetime import datetime
 from time import perf_counter
+from typing import Any
 
 import igraph
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
-from pandas import DataFrame, MultiIndex
+from pandas import DataFrame
+from pandas import MultiIndex
 
 from ..geopandas_tools.general import _push_geom_col
-from ._get_route import _get_k_routes, _get_route, _get_route_frequencies
+from ._get_route import _get_k_routes
+from ._get_route import _get_route
+from ._get_route import _get_route_frequencies
 from ._od_cost_matrix import _od_cost_matrix
-from ._points import Destinations, Origins
+from ._points import Destinations
+from ._points import Origins
 from ._service_area import _service_area
 from .cutting_lines import split_lines_by_nearest_point
 from .network import Network
 from .networkanalysisrules import NetworkAnalysisRules
 
 
 class NetworkAnalysis:
@@ -42,32 +47,20 @@
     The service_area methods only take a set of origins, and return the lines that
     can be reached within one or more breaks.
 
     The 'get_route_frequencies' method is a bit different. It returns the individual
     line segments that were visited with an added column for how many times the
     segments were used.
 
-    Args:
-        network: A GeoDataFrame of line geometries.
-        rules: The rules for the analysis, either as an instance of
-            NetworkAnalysisRules or a dictionary with the parameters
-            as keys.
-        log: If True (default), a DataFrame with information about each
-            analysis run will be stored in the 'log' attribute.
-        detailed_log: If True, the log DataFrame will include columns for
-            all arguments passed to the analysis method, plus standard deviation and
-            percentiles (25th, 50th, 75th) of the weight column in the results.
-            Defaults to False.
-
     Attributes:
         network: A Network instance that holds the lines and nodes (points).
         rules: NetworkAnalysisRules instance.
         log: A DataFrame with information about each analysis run.
 
-    Examples
+    Examples:
     --------
     Read example data.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
     Preparing the lines for directed network analysis.
@@ -75,36 +68,53 @@
     >>> connected_roads = sg.get_connected_components(roads).query("connected == 1")
 
     >>> directed_roads = sg.make_directed_network(
     ...     connected_roads,
     ...     direction_col="oneway",
     ...     direction_vals_bft=("B", "FT", "TF"),
     ...     minute_cols=("drivetime_fw", "drivetime_bw"),
+    ...     dropnegative=True,
+    ...     dropna=True,
     ... )
 
-    >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+    >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
     >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
     >>> nwa
     NetworkAnalysis(
-        network=DirectedNetwork(6364 km, percent_bidirectional=87),
+        network=Network(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
     Now we're ready for network analysis.
 
     """
 
     def __init__(
         self,
         network: GeoDataFrame,
         rules: NetworkAnalysisRules | dict,
         log: bool = True,
         detailed_log: bool = False,
-    ):
+    ) -> None:
+        """Initialise NetworkAnalysis instance.
+
+        Args:
+            network: A GeoDataFrame of line geometries.
+            rules: The rules for the analysis, either as an instance of
+                NetworkAnalysisRules or a dictionary with the parameters
+                as keys.
+            log: If True (default), a DataFrame with information about each
+                analysis run will be stored in the 'log' attribute.
+            detailed_log: If True, the log DataFrame will include columns for
+                all arguments passed to the analysis method, plus standard deviation and
+                percentiles (25th, 50th, 75th) of the weight column in the results.
+                Defaults to False.
+
+        """
         if not isinstance(rules, NetworkAnalysisRules):
             rules = NetworkAnalysisRules(**rules)
 
         if not isinstance(network, Network):
             network = Network(network)
 
         self.network = network
@@ -121,30 +131,30 @@
 
         if log:
             self.log = DataFrame()
 
         self._graph_updated_count = 0
         self._k_nearest_points = 50
 
-    def _check_if_holes_are_nan(self):
-        HOLES_ARE_NAN = (
+    def _check_if_holes_are_nan(self) -> None:
+        holes_are_nan: str = (
             "Network holes have been filled by straigt lines, but the rows have "
             f"NaN values in the {self.rules.weight!r} column. Either remove NaNs "
             "or fill these values with a numeric value (e.g. 0)."
         )
         if (
             hasattr(self.network.gdf, "hole")
             and len(self.network.gdf.loc[lambda x: x["hole"] == 1])
             and (
                 self.network.gdf.loc[lambda x: x["hole"] == 1, self.rules.weight]
                 .isna()
                 .all()
             )
         ):
-            raise ValueError(HOLES_ARE_NAN)
+            raise ValueError(holes_are_nan)
 
     def od_cost_matrix(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         *,
         rowwise: bool = False,
@@ -176,21 +186,21 @@
 
         Returns:
             A DataFrame with the weight column and the columns 'origin' and
             'destination', containing the indices of the origins and destinations
             GeoDataFrames. If lines is True, also returns a geometry column with
             straight lines between origin and destination.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Create some origin and destination points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> origins = points.loc[:99, ["geometry"]]
@@ -419,16 +429,16 @@
 
     def get_route_frequencies(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         weight_df: DataFrame | None = None,
         default_weight: int | float | None = None,
-        strict: bool = False,
         rowwise: bool = False,
+        strict: bool = False,
         frequency_col: str = "frequency",
     ) -> GeoDataFrame:
         """Finds the number of times each line segment was visited in all trips.
 
         Finds the route with the lowest cost (minutes, meters, etc.) from a set of
         origins to a set of destinations and summarises the number of times each
         segment was used. The aggregation is done on the line indices, which is much
@@ -442,14 +452,19 @@
             destinations: GeoDataFrame of points from where the routes will terminate.
             weight_df: A long formated DataFrame where each row contains the indices of
                 an origin-destination pair and the number to multiply the frequency for
                 this route by. The DataFrame can either contain three columns (origin
                 index, destination index and weight. In that order) or only a weight
                 column and a MultiIndex where level 0 is origin index and level 1 is
                 destination index.
+            default_weight: If set, OD pairs not represented in 'weight_df'
+                will be given a default weight value.
+            rowwise: if False (default), it will calculate the cost from each
+                origins to each destination. If true, it will calculate the cost from
+                origin 1 to destination 1, origin 2 to destination 2 and so on.
             strict: If True, all OD pairs must be in weigth_df if specified. Defaults
                 to False.
             frequency_col: Name of column with the number of times each road was
                 visited. Defaults to 'frequency'.
 
         Returns:
             A GeoDataFrame with all line segments that were visited at least once,
@@ -459,22 +474,22 @@
         Note:
             The resulting lines will keep all columns of the 'gdf' of the Network.
 
         Raises:
             ValueError: If weight_df is not a DataFrame with one or three columns
                 that contain weights and all indices of 'origins' and 'destinations'.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> import pandas as pd
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Get some points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> origins = points.iloc[:25]
@@ -595,18 +610,21 @@
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
         if weight_df is not None:
             # map to temporary ids
             ori_idx_mapper = {v: k for k, v in self.origins.idx_dict.items()}
             des_idx_mapper = {v: k for k, v in self.destinations.idx_dict.items()}
-            multiindex_mapper = lambda x: (
-                ori_idx_mapper.get(x[0]),
-                des_idx_mapper.get(x[1]),
-            )
+
+            def multiindex_mapper(x: tuple[int, int]) -> tuple[int, int]:
+                return (
+                    ori_idx_mapper.get(x[0]),
+                    des_idx_mapper.get(x[1]),
+                )
+
             weight_df.index = weight_df.index.map(multiindex_mapper)
         else:
             od_pairs = self._create_od_pairs(
                 self.origins.gdf.set_index("temp_idx"),
                 self.destinations.gdf.set_index("temp_idx"),
                 rowwise=rowwise,
             )
@@ -669,21 +687,21 @@
                 is specified.
 
         Returns:
             A DataFrame with the geometry of the routes between origin and destination.
             Also returns a weight column and the columns 'origin' and 'destination',
             containing the indices of the origins and destinations GeoDataFrames.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Get routes from 1 to 1000 points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
@@ -797,21 +815,21 @@
             very hard to find more than one path for each OD pair.
             If 'drop_middle_percent' is 1, the resulting routes might be very similar,
             depending on the layout of the network.
 
         Raises:
             ValueError: if drop_middle_percent is not between 0 and 100.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url('https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet')
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Getting 10 fastest routes from one point to another point.
 
         >>> points = sg.read_parquet_url('https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet')
         >>> point1 = points.iloc[[0]]
@@ -939,25 +957,25 @@
                 be returned.
 
         Returns:
             A GeoDataFrame with one row per break per origin, with the origin index and
             a dissolved line geometry. If dissolve is False, it will return each line
             that is part of the service area.
 
-        See also:
+        See Also:
             precice_service_area: Equivelent method where lines are also cut to get
             precice results.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         10 minute service area for three origin points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> service_areas = nwa.service_area(
@@ -968,15 +986,14 @@
            origin  minutes                                           geometry
         0       0       10  MULTILINESTRING Z ((264348.673 6648271.134 17....
         1       1       10  MULTILINESTRING Z ((266909.769 6651075.250 114...
         2       2       10  MULTILINESTRING Z ((266909.769 6651075.250 114...
 
         Service areas of 5, 10 and 15 minutes from three origin points.
 
-        >>> nwa = NetworkAnalysis(network=nw, rules=rules)
         >>> service_areas = nwa.service_area(
         ...         points.iloc[:2],
         ...         breaks=[5, 10, 15],
         ... )
         >>> service_areas
            origin  minutes                                           geometry
         0       0        5  MULTILINESTRING Z ((265378.000 6650581.600 85....
@@ -1068,24 +1085,24 @@
                 be returned.
 
         Returns:
             A GeoDataFrame with one row per break per origin, with a dissolved line
             geometry. If dissolve is False, it will return all the columns of the
             network.gdf as well.
 
-        See also:
+        See Also:
             service_area: Faster method where lines are not cut to get precice results.
 
-        Examples
+        Examples:
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
         >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
         >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         10 minute service area for one origin point.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
@@ -1095,15 +1112,14 @@
         ...     )
         >>> sa
             idx  minutes                                           geometry
         0    1       10  MULTILINESTRING Z ((264348.673 6648271.134 17....
 
         Service areas of 5, 10 and 15 minutes from three origin points.
 
-        >>> nwa = NetworkAnalysis(network=nw, rules=rules)
         >>> sa = nwa.precice_service_area(
         ...         points.iloc[:2],
         ...         breaks=[5, 10, 15],
         ...     )
         >>> sa
             idx  minutes                                           geometry
         0    1        5  MULTILINESTRING Z ((265378.000 6650581.600 85....
@@ -1185,15 +1201,15 @@
             "'weight_df' should be a DataFrame with the columns "
             "'origin', 'destination' and 'weight', where the first "
             "two contain the indices of the origins and destinations "
             "and the weight column contains the number to multiply "
             "the trip frequency for this origin-destination pair."
         )
 
-        if not isinstance(weight_df, (DataFrame, pd.Series)):
+        if not isinstance(weight_df, (DataFrame | pd.Series)):
             raise ValueError(error_message)
 
         if isinstance(weight_df, pd.Series):
             weight_df = weight_df.to_frame()
 
         weight_df = weight_df.copy()
 
@@ -1217,15 +1233,15 @@
                 "indices when weight_df is specified."
             )
 
     @staticmethod
     def _make_sure_index_match(
         weight_df: DataFrame,
         od_pairs: MultiIndex,
-    ):
+    ) -> None:
         """Make sure this index matches the index of origins and destinations."""
         if not od_pairs.isin(weight_df.index).all():
             if not od_pairs.isin(weight_df.index).any():
                 raise ValueError(
                     "None of the origin-destination pair indices are in 'weight_df'."
                 )
             raise ValueError(
@@ -1317,31 +1333,33 @@
         else:
             df["destinations_count"] = len(self.destinations.gdf)
 
         if self.detailed_log:
             for key, value in kwargs.items():
                 if isinstance(value, np.ndarray):
                     value = list(value)
-                if isinstance(value, (list, tuple)):
+                if isinstance(value, (list | tuple)):
                     value = [str(x) for x in value]
                     value = ", ".join(value)
                 df[key] = value
 
         self.log = pd.concat([self.log, df], ignore_index=True)
 
     def _prepare_network_analysis(
-        self, origins, destinations=None, rowwise: bool = False
+        self,
+        origins: GeoDataFrame,
+        destinations: GeoDataFrame | None = None,
+        rowwise: bool = False,
     ) -> None:
         """Prepares the weight column, node ids, origins, destinations and graph.
 
         Updates the graph only if it is not yet created and no parts of the analysis
         has changed. this method is run inside od_cost_matrix, get_route and
         service_area.
         """
-
         if rowwise and len(origins) != len(destinations):
             raise ValueError(
                 "'origins' and 'destinations' must have the same length when "
                 "rowwise=True"
             )
 
         self.network.gdf = self.rules._validate_weight(self.network.gdf)
@@ -1581,22 +1599,22 @@
 
         if self.destinations is not None:
             self.wkts["destinations"] = [
                 geom.wkt for geom in self.destinations.gdf.geometry
             ]
 
     @staticmethod
-    def _sort_breaks(breaks) -> list[float | int]:
+    def _sort_breaks(breaks: str | list | tuple | int | float) -> list[float | int]:
         if isinstance(breaks, str):
             breaks = float(breaks)
 
         if hasattr(breaks, "__iter__"):
             return list(sorted(list(breaks)))
 
-        if isinstance(breaks, (int, float)):
+        if isinstance(breaks, (int | float)):
             return [breaks]
 
         raise ValueError(
             "'breaks' should be integer, float, string or an iterable of "
             f" one of these. Got {type(breaks)!r}"
         )
 
@@ -1624,19 +1642,19 @@
             f"{self.__class__.__name__}(\n"
             f"    network={self.network.__repr__()},\n"
             f"    rules={rules}{x}),\n"
             f"    log={self._log}, detailed_log={self.detailed_log},"
             "\n)"
         )
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str) -> Any:
         """To be able to write self['origins'] as well as self.origins."""
         return getattr(self, item)
 
-    def copy(self, deep=True):
+    def copy(self, deep: bool = True) -> "NetworkAnalysis":
         """Returns a (deep) copy of the class instance.
 
         Args:
             deep: Whether to return a deep or shallow copy. Defaults to True.
         """
         if deep:
             return deepcopy(self)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """The NetworkAnalysisRules class sets the rules for the network analysis.
 
 The class is to be used as the 'rules' parameter in the NetworkAnalysis
 class.
 """
-from copy import copy, deepcopy
+
+from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass
 
 from geopandas import GeoDataFrame
 
 from ..helpers import unit_is_meters
 
 
@@ -16,15 +18,15 @@
     """Sets the rules for the network analysis.
 
     To be used as the 'rules' parameter in the NetworkAnalysis class.
 
     Args:
         weight: Either a column in the GeoDataFrame of the Network or
             'meters'/'metres'. A 'minutes' column can be created with the
-            'make_directed_network' method of the DirectedNetwork class.
+            'make_directed_network' or 'make_directed_network_norway' functions.
         directed: Whether the lines will be considered traversable in both directions.
         search_tolerance: distance to search for nodes in the network. Origins and
             destinations further away from the network than the search_tolerance will
             not find any paths. Defaults to 250.
         search_factor: number of meters and percent to add to the closest distance to a
             node when connecting origins and destinations to the network. Defaults to
             0, meaning only the closest node is used. If search_factor is 10 and the
@@ -43,32 +45,32 @@
             that connect them. Defaults to None, meaning 0 weight is added for the
             edges.
         nodedist_multiplier: When using "meters" as weight, this sets the weight for
             the edges between origins/destinations and the network nodes that connect
             them. Defaults to None, meaning 0 weight is added for these edges. If set
             to 1, the weight will be equal to the straigt line distance.
 
-    Examples
+    Examples:
     --------
     Read testdata.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
     Let's start by setting the default rules. 'weight' and 'directed' have no default
     values.
 
     >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
-    >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
-    >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
+    >>> directed_roads = sg.get_connected_components(roads).loc[lambda x: x["connected"] == 1].pipe(sg.make_directed_network_norway, dropnegative=True)
+    >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=True)
     >>> nwa
     NetworkAnalysis(
-        network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
+        network=Network(6364 km, percent_bidirectional=87),
+        rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=True, ...),
         log=True, detailed_log=True,
     )
 
     Setting 'split_lines' to True, means the points will be connected to the closest
     part of the closest network line. If False, the lines are connected to the closest
     endpoint of the lines. split_lines defaults to False, since splitting lines takes
     some time and doesn't make a huge difference in most cases.
@@ -167,29 +169,29 @@
     weight: str
     search_tolerance: int = 250
     search_factor: int = 0
     split_lines: bool = True
     nodedist_multiplier: int | float | None = None
     nodedist_kmh: int | float | None = None
 
-    def _update_rules(self):
+    def _update_rules(self) -> None:
         """Stores the rules as separate attributes.
 
         Used for checking whether the rules have changed and the graph have to be
         remade.
         """
         self._directed = self.directed
         self._weight = self.weight
         self._search_tolerance = self.search_tolerance
         self._search_factor = self.search_factor
         self._split_lines = self.split_lines
         self._nodedist_multiplier = self.nodedist_multiplier
         self._nodedist_kmh = self.nodedist_kmh
 
-    def _rules_have_changed(self):
+    def _rules_have_changed(self) -> bool:
         """Checks if any of the rules have changed since the graph was last created.
 
         If no rules have changed, time can be saved by not remaking the graph
         (the network and the points have to be unchanged as well).
         """
         if self.directed != self._directed:
             return True
@@ -231,16 +233,16 @@
 
         elif self.weight in gdf.columns:
             self._check_for_nans(gdf, self.weight)
             gdf = self._try_to_float(gdf, self.weight)
             self._check_for_negative_values(gdf, self.weight)
             return gdf
 
-        # at this point, the weight is wrong. Now to determine the error
-        # message
+        # at this point, the weight is wrong.
+        # Now to determine the error message
 
         if "meter" in self.weight or "metre" in self.weight:
             raise ValueError(
                 "the crs of the roads have to have units in 'meters' when the "
                 "weight is 'meters'."
             )
 
@@ -253,46 +255,48 @@
 
         else:
             incorrect_weight_column = f"Cannot find 'weight' column {self.weight}"
 
         raise KeyError(incorrect_weight_column)
 
     @staticmethod
-    def _check_for_nans(df, col):
+    def _check_for_nans(df: GeoDataFrame, col: str) -> None:
         """Remove NaNs and give warning if there are any."""
         if all(df[col].isna()):
             raise ValueError(f"All values in the {col!r} column are NaN.")
 
         nans = sum(df[col].isna())
         if nans:
             raise ValueError(
                 f"{nans} rows have missing values in the {col!r} column. "
                 "Fill these rows with 0 or another number.",
             )
 
     @staticmethod
-    def _check_for_negative_values(df, col):
+    def _check_for_negative_values(df: GeoDataFrame, col: str) -> None:
         """Remove negative values and give warning if there are any."""
         negative = sum(df[col] < 0)
         if negative:
             raise ValueError(
                 f"{negative} negative values found in the {col!r} column. Fill these "
                 "with a number greater than or equal to zero.",
             )
 
     @staticmethod
-    def _try_to_float(df, col):
+    def _try_to_float(df: GeoDataFrame, col: str) -> GeoDataFrame:
         """Try to convert weight column to float, raise ValueError if it fails."""
         try:
             df[col] = df[col].astype(float)
         except ValueError as e:
             raise ValueError(
                 f"The {col!r} column must be numeric. Got characters that couldn't be "
                 "interpreted as numbers."
             ) from e
         return df
 
-    def copy(self):
+    def copy(self) -> "NetworkAnalysisRules":
+        """Return a shallow copy the instance."""
         return copy(self)
 
-    def deepcopy(self):
+    def deepcopy(self) -> "NetworkAnalysisRules":
+        """Return a deep copy the instance."""
         return deepcopy(self)
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 The functions are used inside inside other functions, and aren't needed
 to use explicitly.
 """
 
 import geopandas as gpd
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from shapely.geometry import Point
 
 from ..geopandas_tools.general import _push_geom_col
 
 
 def make_node_ids(
     gdf: GeoDataFrame,
@@ -30,15 +31,14 @@
 
     Returns:
         A tuple of two GeoDataFrames, one with the lines and one with the nodes.
 
     Note:
         The lines must be singlepart linestrings.
     """
-
     gdf = gdf.explode(index_parts=False).explode(index_parts=False)
 
     if wkt:
         gdf = make_edge_wkt_cols(gdf)
         geomcol1, geomcol2, geomcol_final = "source_wkt", "target_wkt", "wkt"
     else:
         gdf = make_edge_coords_cols(gdf)
@@ -188,15 +188,14 @@
     return lines, endpoints
 
 
 def _prepare_make_edge_cols_simple(
     lines: GeoDataFrame,
 ) -> tuple[GeoDataFrame, GeoDataFrame]:
     """Faster version of _prepare_make_edge_cols."""
-
     endpoints = lines[lines._geometry_column_name].boundary.explode(ignore_index=True)
 
     if len(lines) and len(endpoints) / len(lines) != 2:
         raise ValueError(
             "The lines should have only two endpoints each. "
             "Try splitting multilinestrings with explode."
         )
```

### Comparing `ssb_sgis-1.0.1/src/sgis/networkanalysis/traveling_salesman.py` & `ssb_sgis-1.0.2/src/sgis/networkanalysis/traveling_salesman.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import networkx as nx
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from networkx.utils import pairwise
 from shapely.geometry import Point
 
 from ..geopandas_tools.conversion import to_geoseries
 from ..geopandas_tools.neighbors import get_all_distances
 
 
@@ -26,16 +27,18 @@
             If not provided, the calculation is done within this function.
             The DataFrame should be identical to the DataFrame created
             from sgis.get_all_distances from and to the points.
 
     Returns:
         List of Points making up the traveling salesman's path.
 
-    Examples
+    Examples:
     --------
+    >>> import sgis as sg
+    >>> from shapely.geometry import LineString
     >>> points = sg.to_gdf(
     ...     [
     ...         (0, 0),
     ...         (10, -10),
     ...         (10, 10),
     ...         (0, 10),
     ...         (0, -10),
```

### Comparing `ssb_sgis-1.0.1/src/sgis/parallel/parallel.py` & `ssb_sgis-1.0.2/src/sgis/parallel/parallel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import functools
 import inspect
 import itertools
 import multiprocessing
 import warnings
-from collections.abc import Callable, Collection, Iterable
+from collections.abc import Callable
+from collections.abc import Collection
+from collections.abc import Iterable
 from pathlib import Path
 from typing import Any
 
-
 try:
     import dapla as dp
 except ImportError:
     pass
 
 import joblib
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
 from pandas import DataFrame
-from shapely.geometry import MultiPolygon, Polygon
+from pandas import Series
 
-from ..geopandas_tools.general import clean_clip, clean_geoms
 from ..geopandas_tools.neighbors import get_neighbor_indices
 from ..geopandas_tools.overlay import clean_overlay
-from ..helpers import LocalFunctionError, dict_zip, dict_zip_union, in_jupyter
-
+from ..helpers import LocalFunctionError
+from ..helpers import dict_zip_union
+from ..helpers import in_jupyter
 
 try:
-    from ..io.dapla_functions import exists, read_geopandas, write_geopandas
+    from ..io.dapla_functions import read_geopandas
+    from ..io.dapla_functions import write_geopandas
 
     # from ..io.write_municipality_data import write_municipality_data
 except ImportError:
     pass
 
 
 try:
-    from dapla import read_pandas, write_pandas
+    from dapla import read_pandas
+    from dapla import write_pandas
+    from dapla.gcs import GCSFileSystem
 except ImportError:
-    pass
 
-
-def turn_args_into_kwargs(func: Callable, args: tuple, index_start: int):
-    if not isinstance(args, tuple):
-        raise TypeError("args should be a tuple (it should not be unpacked with *)")
-    argnames = inspect.getfullargspec(func).args[index_start:]
-    return {name: value for value, name in zip(args, argnames, strict=False)}
+    class GCSFileSystem:
+        """Placeholder."""
 
 
 class Parallel:
     """Run functions in parallell.
 
     The main method is 'map', which runs a single function for
     each item of an iterable. If the items of the iterable also are iterables,
@@ -83,48 +82,60 @@
 
     def __init__(
         self,
         processes: int,
         backend: str = "multiprocessing",
         context: str = "spawn",
         maxtasksperchild: int = 10,
+        chunksize: int = 1,
         **kwargs,
-    ):
+    ) -> None:
+        """Initialize a Parallel instance with specified settings for parallel execution.
+
+        Args:
+            processes: Number of parallel processes. Set to 1 to run without parallelization.
+            backend: The backend to use for parallel execution. Defaults to 'multiprocessing'.
+            context: The context setting for multiprocessing. Defaults to 'spawn'.
+            maxtasksperchild: The maximum number of tasks a worker process can complete
+                before it is replaced. Defaults to 10.
+            chunksize: The size of the chunks of the iterable to distribute to workers.
+            **kwargs: Additional keyword arguments passed to the underlying parallel execution backend.
+        """
         self.processes = int(processes)
         self.maxtasksperchild = maxtasksperchild
+        self.chunksize = chunksize
         self.backend = backend
         self.context = context
         self.kwargs = kwargs
         self.funcs: list[functools.partial] = []
         self.results: list[Any] = []
 
     def map(
         self,
         func: Callable,
         iterable: Collection,
         args: tuple | None = None,
         kwargs: dict | None = None,
-        chunksize: int = 1,
     ) -> list[Any]:
         """Run functions in parallel with items of an iterable as 0th arguemnt.
 
         Args:
             func: Function to be run.
             iterable: An iterable where each item will be passed to func as
                 0th positional argument.
-            Args: Positional arguments passed to 'func' starting from the 1st argument.
+            args: Positional arguments passed to 'func' starting from the 1st argument.
                 The 0th argument will be reserved for the values of 'iterable'.
             kwargs: Keyword arguments passed to 'func'. Must be passed as a dict,
                 not unpacked into separate keyword arguments.
 
         Returns:
             A list of the return values of the function, one for each item in
             'iterable'.
 
-        Examples
+        Examples:
         --------
         Multiply each list element by 2.
 
         >>> iterable = [1, 2, 3]
         >>> def x2(x):
         ...     return x * 2
         >>> p = sg.Parallel(4, backend="loky")
@@ -155,22 +166,21 @@
         >>> from .file import x2
         >>> if __name__ == "__main__":
         ...     p = sg.Parallel(4, backend="loky")
         ...     results = p.map(x2, iterable)
         ...     print(results)
         [2, 4, 6]
         """
-
         if args:
             # start at index 1, meaning the 0th argument (the iterable) is still available
-            args_as_kwargs = turn_args_into_kwargs(func, args, index_start=1)
+            args_as_kwargs = _turn_args_into_kwargs(func, args, index_start=1)
         else:
             args_as_kwargs = {}
 
-        self.validate_execution(func)
+        self._validate_execution(func)
 
         kwargs = self._validate_kwargs(kwargs) | args_as_kwargs
 
         func_with_kwargs = functools.partial(func, **kwargs)
 
         if self.processes == 1:
             return list(map(func_with_kwargs, iterable))
@@ -184,15 +194,17 @@
             return []
 
         if self.backend == "multiprocessing":
             with multiprocessing.get_context(self.context).Pool(
                 processes, maxtasksperchild=self.maxtasksperchild, **self.kwargs
             ) as pool:
                 try:
-                    return pool.map(func_with_kwargs, iterable, chunksize=chunksize)
+                    return pool.map(
+                        func_with_kwargs, iterable, chunksize=self.chunksize
+                    )
                 except Exception as e:
                     pool.terminate()
                     raise e
 
         with joblib.Parallel(
             n_jobs=processes, backend=self.backend, **self.kwargs
         ) as parallel:
@@ -200,35 +212,34 @@
 
     def starmap(
         self,
         func: Callable,
         iterable: Collection[Iterable[Any]],
         args: tuple | None = None,
         kwargs: dict | None = None,
-        chunksize: int = 1,
     ) -> list[Any]:
         """Run functions in parallel where items of the iterable are unpacked.
 
         This requires the items of the iterable to be iterables as well. See
         https://docs.python.org/3/library/itertools.html#itertools.starmap
 
         Args:
             func: Function to be run.
             iterable: An iterable of iterables, where each item will be
                 unpacked as positional argument to the function.
-            Args: Positional arguments passed to 'func' starting at argument position
+            args: Positional arguments passed to 'func' starting at argument position
                 n + 1, where n is the length of the iterables inside the iterable.
             kwargs: Keyword arguments passed to 'func'. Must be passed as a dict,
                 not unpacked into separate keyword arguments.
 
         Returns:
             A list of the return values of the function, one for each item in
             'iterable'.
 
-        Examples
+        Examples:
         --------
         Multiply each list element by 2.
 
         >>> iterable = [(1, 2), (2, 3), (3, 4)]
         >>> def add(x, y):
         ...     return x + y
         >>> p = sg.Parallel(3, backend="loky")
@@ -258,21 +269,21 @@
         ...     print(results)
         [3, 5, 7]
 
         """
         if args:
             # starting the count at the length of the iterables inside the iterables
             iterable = list(iterable)
-            args_as_kwargs = turn_args_into_kwargs(
+            args_as_kwargs = _turn_args_into_kwargs(
                 func, args, index_start=len(iterable[0])
             )
         else:
             args_as_kwargs = {}
 
-        self.validate_execution(func)
+        self._validate_execution(func)
 
         kwargs = self._validate_kwargs(kwargs) | args_as_kwargs
 
         func_with_kwargs = functools.partial(func, **kwargs)
 
         if self.processes == 1:
             return list(itertools.starmap(func_with_kwargs, iterable))
@@ -286,15 +297,17 @@
             return []
 
         if self.backend == "multiprocessing":
             with multiprocessing.get_context(self.context).Pool(
                 processes, maxtasksperchild=self.maxtasksperchild, **self.kwargs
             ) as pool:
                 try:
-                    return pool.starmap(func_with_kwargs, iterable, chunksize=chunksize)
+                    return pool.starmap(
+                        func_with_kwargs, iterable, chunksize=self.chunksize
+                    )
                 except Exception as e:
                     pool.terminate()
                     raise e
 
         with joblib.Parallel(
             n_jobs=processes, backend=self.backend, **self.kwargs
         ) as parallel:
@@ -316,18 +329,18 @@
             ignore_index: Defaults to True.
             strict: If True (default), all files must exist.
             **kwargs: Keyword arguments passed to dapla.read_pandas.
 
         Returns:
             A DataFrame, or a list of DataFrames if concat is False.
         """
-        if not strict:
-            files = [file for file in files if exists(file)]
-
-        res = self.map(dp.read_pandas, files, kwargs=kwargs)
+        if strict:
+            res = self.map(read_pandas, files, kwargs=kwargs)
+        else:
+            res = self.map(_try_to_read_pandas, files, kwargs=kwargs)
 
         return pd.concat(res, ignore_index=ignore_index) if concat else res
 
     def read_geopandas(
         self,
         files: list[str],
         concat: bool = True,
@@ -338,22 +351,27 @@
         """Read geospatial files from a list in parallel.
 
         Args:
             files: List of file paths.
             concat: Whether to concat the results to a GeoDataFrame.
             ignore_index: Defaults to True.
             strict: If True (default), all files must exist.
+            chunksize: The size of the chunks of the iterable to distribute to workers.
             **kwargs: Keyword arguments passed to sgis.read_geopandas.
 
         Returns:
             A GeoDataFrame, or a list of GeoDataFrames if concat is False.
         """
-        if not strict:
-            files = [file for file in files if exists(file)]
-        res = self.map(read_geopandas, files, kwargs=kwargs)
+        if "file_system" not in kwargs:
+            kwargs["file_system"] = dp.FileClient.get_gcs_file_system()
+
+        if strict:
+            res = self.map(read_geopandas, files, kwargs=kwargs)
+        else:
+            res = self.map(_try_to_read_geopandas, files, kwargs=kwargs)
 
         return pd.concat(res, ignore_index=ignore_index) if concat else res
 
     def write_municipality_data(
         self,
         in_data: dict[str, str | GeoDataFrame],
         out_data: str | dict[str, str],
@@ -363,18 +381,22 @@
         file_type: str = "parquet",
         muni_number_col: str = "KOMMUNENR",
         strict: bool = False,
         write_empty: bool = False,
         clip: bool = True,
         max_rows_per_chunk: int = 150_000,
         processes_in_clip: int = 1,
-    ):
+        verbose: bool = True,
+    ) -> None:
         """Split multiple datasets into municipalities and write as separate files.
 
         The files will be named as the municipality number.
+        Each dataset in 'in_data' is intersected with 'municipalities'
+        in parallel. The intersections themselves can also be run in parallel
+        with the 'processes_in_clip' argument.
 
         Args:
             in_data: Dictionary with dataset names as keys and file paths or
                 (Geo)DataFrames as values. Note that the files will be read
                 in parallel if file paths are used.
             out_data: Either a single folder path or a dictionary with same keys as
                 'in_data' and folder paths as values. If a single folder is passed,
@@ -393,38 +415,46 @@
                 number/identifier. Defaults to KOMMUNENR. If the column is not present
                 in the data to be split, the data will be intersected with the
                 municipalities.
             strict: If False (default), the dictionaries 'out_data' and 'funcdict' does
                 not have to have the same length as 'in_data'.
             write_empty: If False (default), municipalities with no data will be skipped.
                 If True, an empty parquet file will be written.
-            clip: If True (default), the data will be clipped.
+            clip: If True (default), the data will be clipped. If False, the data will
+                be spatial joined.
+            max_rows_per_chunk: Number of rows per data chunk for processing.
+            processes_in_clip: Number of parallel processes for data clipping.
+            verbose: Whether to print during execution.
+
         """
         shared_kwds = {
             "municipalities": municipalities,
             "file_type": file_type,
             "muni_number_col": muni_number_col,
             "write_empty": write_empty,
             "with_neighbors": with_neighbors,
             "clip": clip,
             "max_rows_per_chunk": max_rows_per_chunk,
             "processes_in_clip": processes_in_clip,
             "strict": strict,
+            "verbose": verbose,
         }
 
         if isinstance(out_data, (str, Path)):
             out_data = {name: Path(out_data) / name for name in in_data}
 
         if funcdict is None:
             funcdict = {}
 
-        zip_func = dict_zip if strict else dict_zip_union
+        fs = dp.FileClient.get_gcs_file_system()
 
-        for _, data, folder, postfunc in zip_func(in_data, out_data, funcdict):
-            if data is None:
+        for _, data, folder, postfunc in dict_zip_union(in_data, out_data, funcdict):
+            if data is None or (
+                not strict and isinstance(data, (str | Path)) and not fs.exists(data)
+            ):
                 continue
 
             kwds = shared_kwds | {
                 "data": data,
                 "func": postfunc,
                 "out_folder": folder,
             }
@@ -435,23 +465,41 @@
 
     def chunkwise(
         self,
         func: Callable,
         df: GeoDataFrame,
         args: tuple | None = None,
         kwargs: dict | None = None,
-        max_rows_per_chunk: int = 150_000,
-        n_chunks: int = None,
-        concat: bool = False,
+        n_chunks: int | None = None,
+        max_rows_per_chunk: int | None = None,
+        concat: bool = True,
     ) -> GeoDataFrame:
-        if len(df) < max_rows_per_chunk:
-            return func(df, *args, **kwargs)
+        """Run a function in parallel on chunks of a (Geo)DataFrame.
 
-        if n_chunks is None:
-            n_chunks = len(df) // max_rows_per_chunk
+        Args:
+            func: Function to run chunkwise. It should take
+                a (Geo)DataFrame as first argument.
+            df: (Geo)DataFrame to split in n_chunks and passed
+                as first argument to 'func'.
+            args: Positional arguments in 'func' after the DataFrame.
+            kwargs: Additional keyword arguments in 'func'.
+            n_chunks: Optionally set number of chunks to split
+                'df' into. Defaults to the 'processes' attribute
+                of the Parallel instance.
+            max_rows_per_chunk: Alternatively decide number of chunks
+                by a maximum number of rows per chunk.
+            concat: Whether to use pd.concat on the results.
+                Defaults to True.
+        """
+        if max_rows_per_chunk is None and n_chunks is None:
+            n_chunks: int = self.processes
+        elif n_chunks is None:
+            n_chunks: int = len(df) // max_rows_per_chunk
+        elif max_rows_per_chunk is not None and len(df) < max_rows_per_chunk:
+            return func(df, *args, **kwargs)
 
         chunks = np.array_split(np.arange(len(df)), n_chunks)
 
         df_chunked: list[GeoDataFrame] = [df.iloc[chunk] for chunk in chunks]
 
         out = self.map(
             func,
@@ -460,38 +508,38 @@
             kwargs=kwargs,
         )
         if concat:
             return pd.concat(out, ignore_index=True)
         else:
             return out
 
-    def validate_execution(self, func):
+    def _validate_execution(self, func: Callable) -> None:
         """Multiprocessing doesn't work with local variables in interactive interpreter.
 
         Raising Exception to avoid confusion.
         """
         if (
             func.__module__ == "__main__"
             and self.context == "spawn"
             and self.backend == "multiprocessing"
             and in_jupyter()
         ):
             raise LocalFunctionError(func)
 
     @staticmethod
-    def _validate_kwargs(kwargs) -> dict:
-        """Make sure kwargs is a dict (not ** unpacked or None)"""
+    def _validate_kwargs(kwargs: dict) -> dict:
+        """Make sure kwargs is a dict (not ** unpacked or None)."""
         if kwargs is None:
             kwargs = {}
         elif not isinstance(kwargs, dict):
             raise TypeError("kwargs must be a dict")
         return kwargs
 
     def _execute(self) -> list[Any]:
-        [self.validate_execution(func) for func in self.funcs]
+        [self._validate_execution(func) for func in self.funcs]
 
         if self.processes == 1:
             return [func() for func in self.funcs]
 
         # don't use unnecessary processes
         if self.processes > len(self.funcs):
             processes = len(self.funcs)
@@ -509,202 +557,296 @@
 
         with multiprocessing.get_context(self.context).Pool(
             processes, **self.kwargs
         ) as pool:
             results = [pool.apply_async(func) for func in self.funcs]
             return [result.get() for result in results]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
+        """String representation."""
         return (
             f"{self.__class__.__name__}(processes={self.processes}, "
             f"backend='{self.backend}', context='{self.context}')"
         )
 
 
 def write_municipality_data(
     data: str | GeoDataFrame | DataFrame,
     out_folder: str,
-    municipalities: GeoDataFrame,
+    municipalities: GeoDataFrame | list[str] | None = None,
     with_neighbors: bool = False,
     muni_number_col: str = "KOMMUNENR",
     file_type: str = "parquet",
     func: Callable | None = None,
     write_empty: bool = False,
     clip: bool = True,
     max_rows_per_chunk: int = 150_000,
     processes_in_clip: int = 1,
     strict: bool = True,
+    verbose: bool = True,
 ) -> None:
+    """Splits and writes data into municipality-specific files.
+
+    Args:
+        data: Path to the data file or a GeoDataFrame.
+        out_folder: Path to the output directory where the municipality data
+            is written.
+        municipalities: Either a sequence of municipality numbers or a GeoDataFrame
+            of municipality polygons and municipality numbers in the column 'muni_number_col'.
+            Defaults to None.
+        with_neighbors: If True, include data from neighboring municipalities
+            for each municipality.
+        muni_number_col: Column name for municipality codes in 'municipalities'.
+        file_type: Format of the output file.
+        func: Function to process data before writing.
+        write_empty: If True, write empty files for municipalities without data.
+        clip: If True, clip the data to municipality boundaries. If False
+            the data is spatial joined.
+        max_rows_per_chunk: Maximum number of rows in each processed chunk.
+        processes_in_clip: Number of processes to use for clipping.
+        strict: If True (default) and the data has a municipality column,
+            all municipality numbers in 'data' must be present in 'municipalities'.
+        verbose: Whether to print during execution.
+
+    Returns:
+        None. The function writes files directly.
+    """
     write_func = (
         _write_neighbor_municipality_data
         if with_neighbors
         else _write_municipality_data
     )
-
     return write_func(
         data=data,
         out_folder=out_folder,
         municipalities=municipalities,
         muni_number_col=muni_number_col,
         file_type=file_type,
         func=func,
         write_empty=write_empty,
         clip=clip,
         max_rows_per_chunk=max_rows_per_chunk,
         processes_in_clip=processes_in_clip,
         strict=strict,
+        verbose=verbose,
     )
 
 
-def _validate_data(data: str | list[str]) -> str:
-    if isinstance(data, (str, Path)):
-        return data
+def _validate_data(
+    data: str | list[str] | DataFrame | GeoDataFrame,
+) -> DataFrame | GeoDataFrame:
     if hasattr(data, "__iter__") and len(data) == 1:
-        return data[0]
-    elif not isinstance(data, GeoDataFrame):
-        raise TypeError("'data' Must be a file path or a GeoDataFrame. Got", type(data))
+        data = data[0]
+    if isinstance(data, (str, Path)):
+        try:
+            return read_geopandas(str(data))
+        except ValueError as e:
+            try:
+                return read_pandas(str(data))
+            except ValueError as e2:
+                raise e.__class__(e, data) from e2
     return data
 
 
-def _get_out_path(out_folder, muni, file_type):
+def _get_out_path(out_folder: str | Path, muni: str, file_type: str) -> str:
     return str(Path(out_folder) / f"{muni}.{file_type.strip('.')}")
 
 
 def _write_municipality_data(
     data: str | GeoDataFrame | DataFrame,
     out_folder: str,
-    municipalities: GeoDataFrame,
+    municipalities: GeoDataFrame | list[str] | None = None,
     muni_number_col: str = "KOMMUNENR",
     file_type: str = "parquet",
     func: Callable | None = None,
     write_empty: bool = False,
     clip: bool = True,
     max_rows_per_chunk: int = 150_000,
     processes_in_clip: int = 1,
     strict: bool = True,
+    verbose: bool = True,
 ) -> None:
-    data = _validate_data(data)
-
-    if isinstance(data, (str, Path)):
-        try:
-            gdf = read_geopandas(str(data))
-        except ValueError as e:
-            try:
-                gdf = read_pandas(str(data))
-            except ValueError:
-                raise e.__class__(e, data)
-    elif isinstance(data, DataFrame):
-        gdf = data
+    if verbose:
+        to_print = out_folder
+        print(to_print)
     else:
-        raise TypeError(type(data))
+        to_print = None
+
+    gdf = _validate_data(data)
 
     if func is not None:
         gdf = func(gdf)
 
     gdf = _fix_missing_muni_numbers(
         gdf,
         municipalities,
         muni_number_col,
         clip,
         max_rows_per_chunk,
         processes_in_clip=processes_in_clip,
         strict=strict,
+        to_print=to_print,
     )
 
-    for muni in municipalities[muni_number_col]:
-        print(muni)
-        out = _get_out_path(out_folder, muni, file_type)
-
-        gdf_muni = gdf.loc[gdf[muni_number_col] == muni]
-
-        if not len(gdf_muni):
-            if write_empty:
-                gdf_muni = gdf_muni.drop(columns="geometry", errors="ignore")
-                gdf_muni["geometry"] = None
-                write_pandas(gdf_muni, out)
-            continue
+    if municipalities is None:
+        muni_numbers = gdf[muni_number_col]
+    elif not isinstance(municipalities, DataFrame):
+        muni_numbers = municipalities
+    else:
+        muni_numbers = municipalities[muni_number_col]
 
-        write_geopandas(gdf_muni, out)
+    # hardcode this to threading for efficiency in io bound task
+    Parallel(processes_in_clip, backend="threading").map(
+        _write_one_muni,
+        muni_numbers,
+        kwargs=dict(
+            gdf=gdf,
+            out_folder=out_folder,
+            muni_number_col=muni_number_col,
+            file_type=file_type,
+            write_empty=write_empty,
+            to_print=to_print,
+        ),
+    )
 
 
 def _write_neighbor_municipality_data(
     data: str | GeoDataFrame | DataFrame,
     out_folder: str,
     municipalities: GeoDataFrame,
     muni_number_col: str = "KOMMUNENR",
     file_type: str = "parquet",
     func: Callable | None = None,
     write_empty: bool = False,
     clip: bool = True,
     max_rows_per_chunk: int = 150_000,
     processes_in_clip: int = 1,
     strict: bool = True,
+    verbose: bool = True,
 ) -> None:
-    data = _validate_data(data)
+    if verbose:
+        to_print = out_folder
+        print("out_folder:", to_print)
+    else:
+        to_print = None
 
-    if isinstance(data, (str, Path)):
-        gdf = read_geopandas(str(data))
+    gdf = _validate_data(data)
 
     if func is not None:
         gdf = func(gdf)
 
     gdf = _fix_missing_muni_numbers(
         gdf,
         municipalities,
         muni_number_col,
         clip,
         max_rows_per_chunk,
         processes_in_clip,
         strict=strict,
+        to_print=to_print,
     )
 
     if municipalities.index.name != muni_number_col:
         municipalities = municipalities.set_index(muni_number_col)
 
     neighbor_munis = get_neighbor_indices(
         municipalities, municipalities, max_distance=1
     )
 
-    for muni in municipalities.index:
-        out = _get_out_path(out_folder, muni, file_type)
+    # hardcode this to threading for efficiency in io bound task
+    Parallel(processes_in_clip, backend="threading").map(
+        _write_one_muni_with_neighbors,
+        municipalities.index,
+        kwargs=dict(
+            gdf=gdf,
+            neighbor_munis=neighbor_munis,
+            out_folder=out_folder,
+            muni_number_col=muni_number_col,
+            file_type=file_type,
+            write_empty=write_empty,
+            to_print=to_print,
+        ),
+    )
+
+
+def _write_one_muni(
+    muni_number: Any,
+    gdf: GeoDataFrame | DataFrame,
+    out_folder: str | Path,
+    muni_number_col: str,
+    file_type: str,
+    write_empty: bool,
+    to_print: str | None = None,
+) -> None:
+    out = _get_out_path(out_folder, muni_number, file_type)
+
+    if to_print:
+        print("writing:", out)
+
+    gdf_muni = gdf.loc[gdf[muni_number_col] == muni_number]
 
-        muni_and_neighbors = neighbor_munis.loc[[muni]]
-        gdf_neighbor = gdf.loc[gdf[muni_number_col].isin(muni_and_neighbors)]
+    if not len(gdf_muni):
+        if write_empty:
+            gdf_muni = gdf_muni.drop(columns="geometry", errors="ignore")
+            gdf_muni["geometry"] = None
+            write_pandas(gdf_muni, out)
+        return
+
+    write_geopandas(gdf_muni, out)
+
+
+def _write_one_muni_with_neighbors(
+    muni_number: Any,
+    gdf: GeoDataFrame | DataFrame,
+    neighbor_munis: Series,
+    out_folder: str | Path,
+    muni_number_col: str,
+    file_type: str,
+    write_empty: bool,
+    to_print: str | None = None,
+) -> None:
+    out = _get_out_path(out_folder, muni_number, file_type)
+
+    if to_print:
+        print("writing:", out)
+
+    muni_and_neighbors: Series = neighbor_munis.loc[[muni_number]]
+    gdf_neighbor = gdf.loc[gdf[muni_number_col].isin(muni_and_neighbors)]
 
-        if not len(gdf_neighbor):
-            if write_empty:
-                gdf_neighbor["geometry"] = gdf_neighbor["geometry"].astype(str)
-                write_pandas(gdf_neighbor, out)
-            continue
+    if not len(gdf_neighbor):
+        if write_empty:
+            gdf_neighbor = gdf_neighbor.drop(columns="geometry", errors="ignore")
+            gdf_neighbor["geometry"] = None
+            write_pandas(gdf_neighbor, out)
+        return
 
-        write_geopandas(gdf_neighbor, out)
+    write_geopandas(gdf_neighbor, out)
 
 
 def _fix_missing_muni_numbers(
-    gdf,
-    municipalities,
-    muni_number_col,
-    clip,
-    max_rows_per_chunk,
-    processes_in_clip,
-    strict,
-):
+    gdf: GeoDataFrame,
+    municipalities: GeoDataFrame,
+    muni_number_col: str,
+    clip: bool,
+    max_rows_per_chunk: int,
+    processes_in_clip: int,
+    strict: bool,
+    to_print: str,
+) -> GeoDataFrame:
     if muni_number_col in gdf and gdf[muni_number_col].notna().all():
         if municipalities is None:
             return gdf
         if diffs := set(gdf[muni_number_col].values).difference(
             set(municipalities[muni_number_col].values)
         ):
-            message = (
-                f"Different municipality numbers: {diffs}. Set 'strict=False' to ignore"
-            )
+            message = f"Different municipality numbers: {diffs}. Set 'strict=False' to ignore."
             if strict:
                 raise ValueError(message)
             else:
-                warnings.warn(message)
+                warnings.warn(message, stacklevel=1)
         return gdf
 
     if municipalities is None:
         if muni_number_col not in gdf:
             raise ValueError(
                 f"Cannot find column {muni_number_col}. "
                 "Specify another column or a municipality GeoDataFrame to clip "
@@ -713,60 +855,81 @@
         assert gdf[muni_number_col].isna().any()
         raise ValueError(
             f"Column {muni_number_col} has missing values. Make sure gdf has "
             "correct municipality number info or specify a municipality "
             "GeoDataFrame to clip the geometries by."
         )
 
-    municipalities = municipalities[[muni_number_col, "geometry"]].to_crs(gdf.crs)
+    try:
+        municipalities = municipalities[[muni_number_col, "geometry"]].to_crs(gdf.crs)
+    except Exception as e:
+        raise e.__class__(e, to_print) from e
 
     if muni_number_col in gdf and gdf[muni_number_col].isna().any():
         notna = gdf[gdf[muni_number_col].notna()]
 
         isna = gdf[gdf[muni_number_col].isna()].drop(muni_number_col, axis=1)
 
         if not clip:
             notna_anymore = isna.sjoin(municipalities).drop(columns="index_right")
         else:
             notna_anymore = parallel_overlay(
                 isna,
                 municipalities[[muni_number_col, municipalities._geometry_column_name]],
                 processes=processes_in_clip,
                 max_rows_per_chunk=max_rows_per_chunk,
+                to_print=to_print,
             )
 
         return pd.concat([notna, notna_anymore], ignore_index=True)
 
     if not clip:
         return gdf.sjoin(municipalities).drop(columns="index_right")
     else:
         return parallel_overlay(
             gdf,
             municipalities[[muni_number_col, municipalities._geometry_column_name]],
             processes=processes_in_clip,
             max_rows_per_chunk=max_rows_per_chunk,
+            to_print=to_print,
         )
 
 
 def parallel_overlay(
     df1: GeoDataFrame,
     df2: GeoDataFrame,
-    # muni_number_col: str,
     processes: int,
     max_rows_per_chunk: int,
     backend: str = "loky",
+    to_print: str | None = None,
     **kwargs,
 ) -> GeoDataFrame:
-    # df2 = df2[[muni_number_col, df2._geometry_column_name]]
+    """Perform spatial overlay operations on two GeoDataFrames in parallel.
+
+    This function splits the first GeoDataFrame into chunks, processes each chunk in parallel using the specified
+    overlay operation with the second GeoDataFrame, and then concatenates the results.
+
+    Note that this function is most useful if df2 has few and simple geometries.
+
+    Args:
+        df1: The first GeoDataFrame for the overlay operation.
+        df2: The second GeoDataFrame for the overlay operation.
+        how: Type of overlay operation ('intersection', 'union', etc.).
+        processes: Number of parallel processes to use.
+        max_rows_per_chunk: Maximum number of rows per chunk for processing. This helps manage memory usage.
+        backend: The parallelization backend to use ('loky', 'multiprocessing', 'threading').
+        to_print: Optional text to print to see progression.
+        **kwargs: Additional keyword arguments to pass to the overlay function.
 
+    Returns:
+        A GeoDataFrame containing the result of the overlay operation.
+    """
     if len(df1) < max_rows_per_chunk:
         return clean_overlay(df1, df2, **kwargs)
 
-    # df2 = df2.dissolve(by=muni_number_col, as_index=False)
-
     n_chunks = len(df1) // max_rows_per_chunk
     chunks = np.array_split(np.arange(len(df1)), n_chunks)
 
     try:
         x_mapper = dict(enumerate(df1.centroid))
         sorted_xs = dict(reversed(sorted(x_mapper.items(), key=lambda item: item[1])))
         df1 = df1.iloc[list(sorted_xs)]
@@ -774,34 +937,58 @@
         pass
 
     df1_chunked: list[GeoDataFrame] = [df1.iloc[chunk] for chunk in chunks]
 
     out = Parallel(processes, backend=backend).map(
         _clean_intersection,
         df1_chunked,
-        args=(df2,),
+        args=(df2, to_print) if to_print else (df2,),
     )
     return pd.concat(out, ignore_index=True)
 
 
-def _clean_intersection(df1, df2):
-    print(len(df1))
+def _clean_intersection(
+    df1: GeoDataFrame, df2: GeoDataFrame, to_print: str | None = None
+) -> GeoDataFrame:
+    print(to_print, "- intersection chunk len:", len(df1))
     return clean_overlay(df1, df2, how="intersection")
 
 
 def chunkwise(
     func: Callable,
-    df: GeoDataFrame,
+    df: GeoDataFrame | pd.DataFrame,
     max_rows_per_chunk: int = 150_000,
-    n_chunks: int = None,
+    n_chunks: int | None = None,
     args: tuple | None = None,
     kwargs: dict | None = None,
     n_jobs: int = 1,
     backend: str = "loky",
-) -> GeoDataFrame:
+) -> GeoDataFrame | pd.DataFrame:
+    """Run a function in parallel on chunks of a DataFrame.
+
+    This method is used to process large (Geo)DataFrames in manageable pieces,
+    optionally in parallel.
+
+    Args:
+        func: The function to apply to each chunk. This function must accept a DataFrame as
+            its first argument and return a DataFrame.
+        df: The DataFrame to be chunked and processed.
+        max_rows_per_chunk: The maximum number of rows each chunk should contain.
+        n_chunks: The exact number of chunks to divide the dataframe into. If None, it will be
+            calculated based on 'max_rows_per_chunk'.
+        args: Additional positional arguments to pass to 'func'.
+        kwargs: Keyword arguments to pass to 'func'.
+        n_jobs: The number of parallel jobs to run. Defaults to 1 (no parallel execution).
+        backend: The backend to use for parallel execution (e.g., 'loky', 'multiprocessing').
+
+    Returns:
+        GeoDataFrame: A GeoDataFrame resulting from concatenating the results of applying 'func'
+            to each chunk of the original GeoDataFrame.
+
+    """
     if len(df) < max_rows_per_chunk:
         return func(df, *args, **kwargs)
 
     if n_chunks is None:
         n_chunks = len(df) // max_rows_per_chunk
 
     chunks = np.array_split(np.arange(len(df)), n_chunks)
@@ -811,7 +998,30 @@
     out = Parallel(n_jobs, backend=backend).map(
         func,
         df_chunked,
         args=args,
         kwargs=kwargs,
     )
     return pd.concat(out, ignore_index=True)
+
+
+def _turn_args_into_kwargs(func: Callable, args: tuple, index_start: int) -> dict:
+    if not isinstance(args, tuple):
+        raise TypeError("args should be a tuple (it should not be unpacked with *)")
+    argnames = inspect.getfullargspec(func).args[index_start:]
+    return {name: value for value, name in zip(args, argnames, strict=False)}
+
+
+def _try_to_read_geopandas(path: str, **kwargs) -> GeoDataFrame | DataFrame | None:
+    """Read with try/except because it's faster than checking exists first."""
+    try:
+        return read_geopandas(path, **kwargs)
+    except FileNotFoundError:
+        return None
+
+
+def _try_to_read_pandas(path: str, **kwargs) -> DataFrame | None:
+    """Read with try/except because it's faster than checking exists first."""
+    try:
+        return read_pandas(path, **kwargs)
+    except FileNotFoundError:
+        return None
```

### Comparing `ssb_sgis-1.0.1/src/sgis/raster/cube.py` & `ssb_sgis-1.0.2/src/sgis/raster/cube.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,149 @@
 import functools
 import itertools
 import multiprocessing
-import os
 import re
-from copy import copy, deepcopy
+from collections.abc import Callable
+from collections.abc import Iterable
+from collections.abc import Iterator
+from copy import copy
+from copy import deepcopy
 from pathlib import Path
-from typing import Any, Callable, Iterable, Optional, Sequence
+from typing import Any
+from typing import ClassVar
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio
 import shapely
-from geopandas import GeoDataFrame, GeoSeries
-from pandas import DataFrame, Series
-from pandas.api.types import is_dict_like, is_list_like
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
+from pandas import DataFrame
+from pandas import Series
+from pandas.api.types import is_dict_like
+from pandas.api.types import is_list_like
 from rasterio import merge as rasterio_merge
 
-
 try:
     import xarray as xr
-    from rioxarray.merge import merge_arrays
     from xarray import Dataset
 except ImportError:
 
     class Dataset:
-        pass
+        """Placeholder."""
 
 
-from rtree.index import Index, Property
+from rtree.index import Index
+from rtree.index import Property
 from shapely import Geometry
 from typing_extensions import Self  # TODO: imperter fra typing når python 3.11
 
-from ..geopandas_tools.bounds import get_total_bounds, make_grid
-from ..geopandas_tools.conversion import (
-    crs_to_string,
-    is_bbox_like,
-    to_bbox,
-    to_shapely,
-)
+from ..geopandas_tools.bounds import make_grid
+from ..geopandas_tools.conversion import is_bbox_like
+from ..geopandas_tools.conversion import to_bbox
+from ..geopandas_tools.conversion import to_shapely
 from ..geopandas_tools.general import get_common_crs
 from ..geopandas_tools.overlay import clean_overlay
-from ..helpers import dict_zip_intersection, get_all_files, get_numpy_func
+from ..helpers import get_all_files
+from ..helpers import get_numpy_func
 from ..io._is_dapla import is_dapla
 from ..io.opener import opener
 from ..parallel.parallel import Parallel
 from .raster import Raster
 
-
 try:
     from torchgeo.datasets.geo import RasterDataset
     from torchgeo.datasets.utils import BoundingBox
 except ImportError:
 
     class BoundingBox:
         """Placeholder."""
 
-        def __init__(self, *args, **kwargs):
+        def __init__(self, *args, **kwargs) -> None:
+            """Placeholder."""
             raise ImportError("missing optional dependency 'torchgeo'")
 
     class RasterDataset:
         """Placeholder."""
 
-        def __init__(self, *args, **kwargs):
+        def __init__(self, *args, **kwargs) -> None:
+            """Placeholder."""
             raise ImportError("missing optional dependency 'torchgeo'")
 
 
 try:
     import torch
     from torchgeo.datasets.utils import disambiguate_timestamp
 except ImportError:
 
     class torch:
         """Placeholder."""
 
         class Tensor:
-            pass
+            """Placeholder to reference torch.Tensor."""
 
 
 try:
     from ..io.dapla_functions import read_geopandas
 except ImportError:
     pass
 
 try:
-    from dapla import FileClient, write_pandas
+    from dapla import FileClient
+    from dapla import write_pandas
 except ImportError:
     pass
 
-from .bands import Sentinel2
-from .base import ALLOWED_KEYS, NESSECARY_META, get_index_mapper
-from .cubebase import _from_gdf_func, _method_as_func, _raster_from_path, _write_func
-from .indices import get_raster_pairs, index_calc_pair
-from .zonal import make_geometry_iterrows, prepare_zonal, zonal_func, zonal_post
+from .base import ALLOWED_KEYS
+from .base import NESSECARY_META
+from .base import get_index_mapper
+from .cubebase import _from_gdf_func
+from .cubebase import _method_as_func
+from .cubebase import _raster_from_path
+from .cubebase import _write_func
+from .indices import get_raster_pairs
+from .indices import index_calc_pair
+from .zonal import _make_geometry_iterrows
+from .zonal import _prepare_zonal
+from .zonal import _zonal_func
+from .zonal import _zonal_post
 
+TORCHGEO_RETURN_TYPE = dict[str, torch.Tensor | pyproj.CRS | BoundingBox]
 
-class DataCube:
-    """Experimental.
-
-    Examples
-    --------
 
-    >>> cube = sg.DataCube.from_root(...)
-    >>> clipped = cube.clip(mask).merge(by="date")
-    >>>
-    """
-
-    CUBE_DF_NAME = "cube_df.parquet"
+class DataCube:
+    """Experimental."""
 
-    CANON_RASTER_TYPES = {
-        "Raster": Raster,
-        "Sentinel2": Sentinel2,
-    }
+    CUBE_DF_NAME: ClassVar[str] = "cube_df.parquet"
 
-    separate_files = True
-    is_image = True
+    separate_files: ClassVar[bool] = True
+    is_image: ClassVar[bool] = True
+    date_format: ClassVar[str | None] = None
 
     def __init__(
         self,
         data: Iterable[Raster] | None = None,
         crs: Any | None = None,
         res: int | None = None,
         nodata: int | None = None,
         copy: bool = False,
-        parallelizer: Optional[Parallel] = None,
+        parallelizer: Parallel | None = None,
     ) -> None:
+        """Initialize a DataCube instance with optional Raster data.
+
+        Args:
+            data: Iterable of Raster objects or a single DataCube to copy data from.
+            crs: Coordinate reference system to be applied to the images.
+            res: Spatial resolution of the images, applied uniformly to all Rasters.
+            nodata: Nodata value to unify across all Rasters within the cube.
+            copy: If True, makes deep copies of Rasters provided.
+            parallelizer: sgis.Parallel instance to handle concurrent operations.
+        """
         self._arrays = None
         self._res = res
         self.parallelizer = parallelizer
 
         # hasattr check to allow class attribute
         if not hasattr(self, "_nodata"):
             self._nodata = nodata
@@ -186,70 +200,68 @@
 
     @classmethod
     def from_root(
         cls,
         root: str | Path,
         *,
         res: int | None = None,
-        raster_type: Raster = Raster,
         check_for_df: bool = True,
         contains: str | None = None,
         endswith: str = ".tif",
-        regex: str | None = None,
-        parallelizer: Optional[Parallel] = None,
+        filename_regex: str | None = None,
+        parallelizer: Parallel | None = None,
         file_system=None,
         **kwargs,
-    ):
-        kwargs = {
-            "raster_type": raster_type,
-            "res": res,
-        } | kwargs
+    ) -> "DataCube":
+        """Construct a DataCube by searching for files starting from a root directory.
+
+        Args:
+            root: Root directory path to search for raster image files.
+            res: Resolution to unify the data within the cube.
+            check_for_df: Check for a parquet file in the root directory
+                that holds metadata for the files in the directory.
+            contains: Filter files containing specific substrings.
+            endswith: Filter files that end with specific substrings.
+            filename_regex: Regular expression to match file names
+                and attributes (date, band, tile, resolution).
+            parallelizer: sgis.Parallel instance for concurrent file processing.
+            file_system: File system to use for file operations, used in GCS environment.
+            **kwargs: Additional keyword arguments to pass to 'from_path' method.
+
+        Returns:
+            An instance of DataCube containing the raster data from specified paths.
+        """
+        kwargs["res"] = res
+        kwargs["filename_regex"] = filename_regex
+        kwargs["contains"] = contains
+        kwargs["endswith"] = endswith
 
         if is_dapla():
             if file_system is None:
                 file_system = FileClient.get_gcs_file_system()
             glob_pattern = str(Path(root) / "**")
             paths: list[str] = file_system.glob(glob_pattern)
             if contains:
                 paths = [path for path in paths if contains in path]
 
         else:
             paths = get_all_files(root)
 
         dfs = [path for path in paths if path.endswith(cls.CUBE_DF_NAME)]
 
-        if contains:
-            paths = [path for path in paths if contains in path]
-        if endswith:
-            paths = [path for path in paths if path.endswith(endswith)]
-        if regex:
-            regex = re.compile(regex)
-            paths = [path for path in paths if re.search(regex, path)]
-        if raster_type.filename_regex is not None:
-            # regex = raster_type.filename_regex
-            # paths = [path for path in paths if re.search(regex, Path(path).name)]
-            regex = re.compile(raster_type.filename_regex, re.VERBOSE)
-            paths = [
-                path
-                for path in paths
-                if re.match(regex, os.path.basename(path))
-                or re.search(regex, os.path.basename(path))
-            ]
-
         if not check_for_df or not len(dfs):
             return cls.from_paths(
                 paths,
-                # indexes=indexes,
                 parallelizer=parallelizer,
                 **kwargs,
             )
 
         folders_with_df: set[Path] = {Path(path).parent for path in dfs if path}
 
-        cubes: list[DataCube] = [cls.from_cube_df(df, **kwargs) for df in dfs]
+        cubes: list[DataCube] = [cls.from_cube_df(df, res=res) for df in dfs]
 
         paths_in_folders_without_df = [
             path for path in paths if Path(path).parent not in folders_with_df
         ]
 
         if paths_in_folders_without_df:
             cubes += [
@@ -264,28 +276,54 @@
 
     @classmethod
     def from_paths(
         cls,
         paths: Iterable[str | Path],
         *,
         res: int | None = None,
-        raster_type: Raster = Raster,
-        parallelizer: Optional[Parallel] = None,
+        parallelizer: Parallel | None = None,
         file_system=None,
+        contains: str | None = None,
+        endswith: str = ".tif",
+        filename_regex: str | None = None,
         **kwargs,
-    ):
+    ) -> "DataCube":
+        """Create a DataCube from a list of file paths.
+
+        Args:
+            paths: Iterable of file paths to raster files.
+            res: Resolution to unify the data within the cube.
+            parallelizer: Joblib Parallel instance for concurrent file processing.
+            file_system: File system to use for file operations, used in Dapla environment.
+            contains: Filter files containing specific substrings.
+            endswith: Filter files that end with specific substrings.
+            filename_regex: Regular expression to match file names.
+            **kwargs: Additional keyword arguments to pass to the raster loading function.
+
+        Returns:
+            An instance of DataCube containing the raster data from specified paths.
+        """
         crs = kwargs.pop("crs", None)
 
+        if contains:
+            paths = [path for path in paths if contains in path]
+        if endswith:
+            paths = [path for path in paths if path.endswith(endswith)]
+        if filename_regex:
+            compiled = re.compile(filename_regex, re.VERBOSE)
+            paths = [path for path in paths if re.search(compiled, Path(path).name)]
+
         if not paths:
             return cls(crs=crs, parallelizer=parallelizer, res=res)
 
-        kwargs = dict(raster_type=raster_type, res=res) | kwargs
+        kwargs["res"] = res
+        kwargs["filename_regex"] = filename_regex
 
         if file_system is None and is_dapla():
-            kwargs |= {"file_system": FileClient.get_gcs_file_system()}
+            kwargs["file_system"] = FileClient.get_gcs_file_system()
 
         if parallelizer is None:
             rasters: list[Raster] = [
                 _raster_from_path(path, **kwargs) for path in paths
             ]
         else:
             rasters: list[Raster] = parallelizer.map(
@@ -298,25 +336,32 @@
 
     @classmethod
     def from_gdf(
         cls,
         gdf: GeoDataFrame | Iterable[GeoDataFrame],
         columns: str | Iterable[str],
         res: int,
-        parallelizer: Optional[Parallel] = None,
+        parallelizer: Parallel | None = None,
         tile_size: int | None = None,
         grid: GeoSeries | None = None,
-        raster_type: Raster = Raster,
         **kwargs,
-    ):
-        """
+    ) -> "DataCube":
+        """Create a DataCube from a GeoDataFrame or a set of them, tiling the spatial data as specified.
 
         Args:
-            grid: A grid.
-            **kwargs: Keyword arguments passed to Raster.from_gdf.
+            gdf: GeoDataFrame or an iterable of GeoDataFrames to rasterize.
+            columns: The column(s) in the GeoDataFrame that will be used as values for the rasterization.
+            res: Spatial resolution of the output rasters.
+            parallelizer: Joblib Parallel instance for concurrent processing.
+            tile_size: Size of each tile/grid cell in the output raster.
+            grid: Predefined grid to align the rasterization.
+            **kwargs: Additional keyword arguments passed to Raster.from_gdf.
+
+        Returns:
+            An instance of DataCube containing rasterized data from the GeoDataFrame(s).
         """
         if grid is None and tile_size is None:
             raise ValueError("Must specify either 'tile_size' or 'grid'.")
 
         if isinstance(gdf, GeoDataFrame):
             gdf = [gdf]
         elif not all(isinstance(frame, GeoDataFrame) for frame in gdf):
@@ -331,44 +376,54 @@
 
         grid["tile_idx"] = range(len(grid))
 
         partial_func = functools.partial(
             _from_gdf_func,
             columns=columns,
             res=res,
-            raster_type=raster_type,
             **kwargs,
         )
 
         def to_gdf_list(gdf: GeoDataFrame) -> list[GeoDataFrame]:
             return [gdf.loc[gdf["tile_idx"] == i] for i in gdf["tile_idx"].unique()]
 
         rasters = []
 
-        if processes > 1:
+        if parallelizer.processes > 1:
             rasters = parallelizer.map(
                 clean_overlay, gdf, args=(grid,), kwargs=dict(keep_geom_type=True)
             )
-            with multiprocessing.get_context("spawn").Pool(processes) as p:
+            with multiprocessing.get_context("spawn").Pool(parallelizer.processes) as p:
                 for frame in gdf:
                     frame = frame.overlay(grid, keep_geom_type=True)
                     gdfs = to_gdf_list(frame)
                     rasters += p.map(partial_func, gdfs)
-        elif processes < 1:
+        elif parallelizer.processes < 1:
             raise ValueError("processes must be an integer 1 or greater.")
         else:
             for frame in gdf:
                 frame = frame.overlay(grid, keep_geom_type=True)
                 gdfs = to_gdf_list(frame)
                 rasters += [partial_func(gdf) for gdf in gdfs]
 
         return cls(rasters, res=res)
 
     @classmethod
-    def from_cube_df(cls, df: DataFrame | str | Path, res: int | None = None):
+    def from_cube_df(
+        cls, df: DataFrame | str | Path, res: int | None = None
+    ) -> "DataCube":
+        """Construct a DataCube from a DataFrame or path containing metadata or paths of rasters.
+
+        Args:
+            df: DataFrame, path to a DataFrame, or string path pointing to cube data.
+            res: Optional resolution to standardize all rasters to this resolution.
+
+        Returns:
+            A DataCube instance containing the raster data described by the DataFrame.
+        """
         if isinstance(df, (str, Path)):
             df = read_geopandas(df) if is_dapla() else gpd.read_parquet(df)
 
         # recursive
         if not is_dict_like(df) and all(
             isinstance(x, (str, Path, DataFrame)) for x in df
         ):
@@ -377,94 +432,84 @@
             return cube
 
         if isinstance(df, dict):
             df = DataFrame(df)
         elif not isinstance(df, DataFrame):
             raise TypeError("df must be DataFrame or file path to a parquet file.")
 
-        try:
-            raster_types = [cls.CANON_RASTER_TYPES[x] for x in df["type"]]
-        except KeyError:
-            for x in df["type"]:
-                try:
-                    cls.CANON_RASTER_TYPES[x]
-                except KeyError:
-                    raise ValueError(
-                        f"Cannot convert raster type '{x}' to a Raster instance."
-                    )
-
         rasters: list[Raster] = [
-            raster_type.from_dict(meta)
-            for raster_type, (_, meta) in zip(
-                raster_types, df[NESSECARY_META].iterrows()
-            )
+            Raster.from_dict(meta) for _, meta in (df[NESSECARY_META].iterrows())
         ]
         return cls(rasters)
 
     def to_gdf(
         self, column: str | None = None, ignore_index: bool = False, concat: bool = True
     ) -> GeoDataFrame:
+        """Convert DataCube to GeoDataFrame."""
         gdfs = self.run_raster_method("to_gdf", column=column, return_self=False)
 
         if concat:
             return pd.concat(gdfs, ignore_index=ignore_index)
         return gdfs
 
     def to_xarray(self) -> Dataset:
+        """Convert DataCube to an xarray.Dataset."""
         return xr.Dataset({i: r.to_xarray() for i, r in enumerate(self.data)})
 
     def zonal(
         self,
         polygons: GeoDataFrame,
         aggfunc: str | Callable | list[Callable | str],
         array_func: Callable | None = None,
         by_date: bool | None = None,
         dropna: bool = True,
     ) -> GeoDataFrame:
+        """Calculate zonal statistics within polygons."""
         idx_mapper, idx_name = get_index_mapper(polygons)
-        polygons, aggfunc, func_names = prepare_zonal(polygons, aggfunc)
-        poly_iter = make_geometry_iterrows(polygons)
+        polygons, aggfunc, func_names = _prepare_zonal(polygons, aggfunc)
+        poly_iter = _make_geometry_iterrows(polygons)
 
         if by_date is None:
             by_date: bool = all(r.date is not None for r in self)
 
         if not self.parallelizer:
             aggregated: list[DataFrame] = [
-                zonal_func(
+                _zonal_func(
                     poly,
                     cube=self,
                     array_func=array_func,
                     aggfunc=aggfunc,
                     func_names=func_names,
                     by_date=by_date,
                 )
                 for poly in poly_iter
             ]
         else:
             aggregated: list[DataFrame] = self.parallelizer.map(
-                zonal_func,
+                _zonal_func,
                 poly_iter,
                 kwargs=dict(
                     cube=self,
                     array_func=array_func,
                     aggfunc=aggfunc,
                     func_names=func_names,
                     by_date=by_date,
                 ),
             )
 
-        return zonal_post(
+        return _zonal_post(
             aggregated,
             polygons=polygons,
             idx_mapper=idx_mapper,
             idx_name=idx_name,
             dropna=dropna,
         )
 
     def gradient(self, degrees: bool = False) -> Self:
+        """Get gradients in each image."""
         self.data = self.run_raster_method("gradient", degrees=degrees)
         return self
 
     def map(self, func: Callable, return_self: bool = True, **kwargs) -> Self:
         """Maps each raster array to a function.
 
         The function must take a numpy array as first positional argument,
@@ -496,38 +541,44 @@
             data = [func(r, **kwargs) for r in self]
         if not return_self:
             return data
         self.data = data
         return self
 
     def load(self, copy: bool = True, **kwargs) -> Self:
+        """Load all images as arrays into a DataCube copy."""
         if self.crs is None:
             self._crs = get_common_crs(self.data)
 
         cube = self.copy() if copy else self
 
         cube.data = cube.run_raster_method("load", **kwargs)
 
         return cube
 
-    def intersects(self, other, copy: bool = True) -> Self:
+    def intersection(self, other: Any, copy: bool = True) -> Self:
+        """Select the images that intersect 'other'."""
         other = to_shapely(other)
         cube = self.copy() if copy else self
         cube = cube[cube.boxes.intersects(other)]
         return cube
 
-    def sfilter(self, other, copy: bool = True) -> Self:
+    def sfilter(
+        self, other: GeoDataFrame | GeoSeries | Geometry | tuple, copy: bool = True
+    ) -> Self:
+        """Spatially filter images by bounding box or geometry object."""
         other = to_shapely(other)
         cube = self.copy() if copy else self
         cube.data = [raster for raster in self if raster.unary_union.intersects(other)]
         return cube
 
     def clip(
         self, mask: GeoDataFrame | GeoSeries | Geometry, copy: bool = True, **kwargs
     ) -> Self:
+        """Clip the images by bounding box or geometry object."""
         if self.crs is None:
             self._crs = get_common_crs(self.data)
 
         if (
             hasattr(mask, "crs")
             and mask.crs
             and not pyproj.CRS(self.crs).equals(pyproj.CRS(mask.crs))
@@ -537,24 +588,32 @@
         cube = self.copy() if copy else self
 
         cube = cube.sfilter(to_shapely(mask), copy=False)
 
         cube.data = cube.run_raster_method("clip", mask=mask, **kwargs)
         return cube
 
-    def clipmerge(self, mask, **kwargs) -> Self:
-        return clipmerge(self, mask, **kwargs)
+    def clipmerge(self, mask: GeoDataFrame | GeoSeries | Geometry, **kwargs) -> Self:
+        """Clip the images and merge to one image."""
+        return _clipmerge(self, mask, **kwargs)
 
     def merge_by_bounds(self, by: str | list[str] | None = None, **kwargs) -> Self:
-        return merge_by_bounds(self, by=by, **kwargs)
+        """Merge images with the same bounding box."""
+        return _merge_by_bounds(self, by=by, **kwargs)
 
     def merge(self, by: str | list[str] | None = None, **kwargs) -> Self:
-        return merge(self, by=by, **kwargs)
+        """Merge all images to one."""
+        return _merge(self, by=by, **kwargs)
 
     def explode(self) -> Self:
+        """Convert from 3D to 2D arrays.
+
+        Make multi-banded arrays (3d) into multiple single-banded arrays (2d).
+        """
+
         def explode_one_raster(raster: Raster) -> list[Raster]:
             property_values = {key: getattr(raster, key) for key in raster.properties}
 
             all_meta = {
                 key: value
                 for key, value in (
                     raster.__dict__ | raster.meta | property_values
@@ -577,15 +636,16 @@
         self.data = list(
             itertools.chain.from_iterable(
                 [explode_one_raster(raster) for raster in self]
             )
         )
         return self
 
-    def dissolve_bands(self, aggfunc, copy: bool = True) -> Self:
+    def dissolve_bands(self, aggfunc: Callable | str, copy: bool = True) -> Self:
+        """Aggregate values in 3D arrays to a single value in a 2D array."""
         self._check_for_array()
         if not callable(aggfunc) and not isinstance(aggfunc, str):
             raise TypeError("Can only supply a single aggfunc")
 
         cube = self.copy() if copy else self
 
         aggfunc = get_numpy_func(aggfunc)
@@ -601,31 +661,40 @@
     ) -> None:
         """Writes arrays as tif files and df with file info.
 
         This method should be run after the rasters have been clipped, merged or
         its array values have been recalculated.
 
         Args:
+            root: Directory path where the images will be written to.
+            file_format: File extension.
+            **kwargs: Keyword arguments passed to rasterio.open.
 
         """
         self._check_for_array()
 
         if any(raster.name is None for raster in self):
             raise ValueError("")
 
         paths = [
             (Path(root) / raster.name).with_suffix(f".{file_format}") for raster in self
         ]
 
         if self.parallelizer:
-            self.parallelizer.starmap(_write_func, zip(self, paths), kwargs=kwargs)
+            self.parallelizer.starmap(
+                _write_func, zip(self, paths, strict=False), kwargs=kwargs
+            )
         else:
-            [_write_func(raster, path, **kwargs) for raster, path in zip(self, paths)]
+            [
+                _write_func(raster, path, **kwargs)
+                for raster, path in zip(self, paths, strict=False)
+            ]
 
     def write_df(self, folder: str) -> None:
+        """Write metadata DataFrame."""
         df = pd.DataFrame(self.meta)
 
         folder = Path(folder)
         if not folder.is_dir():
             raise ValueError()
 
         if is_dapla():
@@ -634,17 +703,18 @@
             df.to_parquet(folder / self.CUBE_DF_NAME)
 
     def calculate_index(
         self,
         index_func: Callable,
         band_name1: str,
         band_name2: str,
-        copy=True,
+        copy: bool = True,
         **kwargs,
     ) -> Self:
+        """Calculate an index based on a function."""
         cube = self.copy() if copy else self
 
         raster_pairs: list[tuple[Raster, Raster]] = get_raster_pairs(
             cube, band_name1=band_name1, band_name2=band_name2
         )
 
         kwargs = dict(index_formula=index_func) | kwargs
@@ -654,79 +724,87 @@
                 index_calc_pair, raster_pairs, kwargs=kwargs
             )
         else:
             rasters = [index_calc_pair(items, **kwargs) for items in raster_pairs]
 
         return cube.__class__(rasters)
 
-    def reproject_match(self) -> Self:
-        pass
+    # def reproject_match(self) -> Self:
+    #     pass
 
-    def to_crs(self, crs, copy: bool = True) -> Self:
+    def to_crs(self, crs: Any, copy: bool = True) -> Self:
+        """Reproject the coordinates of each image."""
         cube = self.copy() if copy else self
         cube.data = [r.to_crs(crs) for r in cube]
         cube._warped_crs = crs
         return cube
 
-    def set_crs(self, crs, allow_override: bool = False, copy: bool = True) -> Self:
+    def set_crs(
+        self, crs: Any, allow_override: bool = False, copy: bool = True
+    ) -> Self:
+        """Set the CRS of each image."""
         cube = self.copy() if copy else self
         cube.data = [r.set_crs(crs, allow_override=allow_override) for r in cube]
         cube._warped_crs = crs
         return cube
 
     def min(self) -> Series:
+        """Get minimum array values for each image."""
         return Series(
             self.run_raster_method("min"),
             name="min",
         )
 
     def max(self) -> Series:
+        """Get maximum array values for each image."""
         return Series(
             self.run_raster_method("max"),
             name="max",
         )
 
     def raster_attribute(self, attribute: str) -> Series | GeoSeries:
         """Get a Raster attribute returned as values in a pandas.Series."""
         data = [getattr(r, attribute) for r in self]
         if any(isinstance(x, Geometry) for x in data):
             return GeoSeries(data, name=attribute)
         return Series(data, name=attribute)
 
     def run_raster_method(
-        self, method: str, *args, copy: bool = True, return_self=False, **kwargs
+        self, method: str, *args, copy: bool = True, return_self: bool = False, **kwargs
     ) -> Self:
         """Run a Raster method for each raster in the cube."""
         if not all(hasattr(r, method) for r in self):
             raise AttributeError(f"Raster has no method {method!r}.")
 
         method_as_func = functools.partial(
-            _method_as_func, method=method, *args, **kwargs
+            _method_as_func, *args, method=method, **kwargs
         )
 
         cube = self.copy() if copy else self
 
         return cube.raster_map(method_as_func, return_self=return_self)
 
     @property
     def meta(self) -> list[dict]:
+        """Get metadata property of each raster."""
         return [raster.meta for raster in self]
 
     # @property
     # def cube_df_meta(self) -> dict[list]:
     #     return {
     #         "path": [r.path for r in self],
     #         "indexes": [r.indexes for r in self],
     #         "type": [r.__class__.__name__ for r in self],
     #         "bounds": [r.bounds for r in self],
     #         "crs": [crs_to_string(r.crs) for r in self],
     #     }
 
     @property
     def data(self) -> list[Raster]:
+        """The Rasters as a list."""
         return self._data
 
     @data.setter
     def data(self, data: list[Raster]):
         self.index = Index(interleaved=False, properties=Property(dimension=3))
 
         if data is None or not len(data):
@@ -734,188 +812,207 @@
             return
         if not all(isinstance(x, Raster) for x in data):
             types = {type(x).__name__ for x in data}
             raise TypeError(f"data must be Raster. Got {', '.join(types)}")
         self._data = list(data)
 
         for i, raster in enumerate(self._data):
-            if raster.date and raster.date_format:
+            if raster.date:
                 try:
-                    mint, maxt = disambiguate_timestamp(raster.date, raster.date_format)
-                except NameError:
+                    mint, maxt = disambiguate_timestamp(raster.date, self.date_format)
+                except (NameError, TypeError):
                     mint, maxt = 0, 1
             else:
                 mint, maxt = 0, 1
             # important: torchgeo has a different order of the bbox than shapely and geopandas
             minx, miny, maxx, maxy = raster.bounds
             self.index.insert(i, (minx, maxx, miny, maxy, mint, maxt))
 
     @property
     def arrays(self) -> list[np.ndarray]:
+        """The arrays of the images as a list."""
         return [raster.array for raster in self]
 
     @arrays.setter
     def arrays(self, new_arrays: list[np.ndarray]):
         if len(new_arrays) != len(self):
             raise ValueError(
                 f"Number of arrays ({len(new_arrays)}) must be same as length as cube ({len(self)})."
             )
         if not all(isinstance(arr, np.ndarray) for arr in new_arrays):
             raise ValueError("Must be list of numpy ndarrays")
 
-        self.data = [raster.update(array=arr) for raster, arr in zip(self, new_arrays)]
-
-    @property
-    def raster_type(self) -> Series:
-        return Series(
-            [r.__class__ for r in self],
-            name="raster_type",
-        )
+        self.data = [
+            raster.update(array=arr)
+            for raster, arr in zip(self, new_arrays, strict=False)
+        ]
 
     @property
     def band(self) -> Series:
+        """Get the 'band' attribute of the rasters."""
         return Series(
             [r.band for r in self],
             name="band",
         )
 
     @property
     def dtype(self) -> Series:
+        """Get the 'dtype' attribute of the rasters."""
         return Series(
             [r.dtype for r in self],
             name="dtype",
         )
 
     @property
     def nodata(self) -> int | None:
+        """No data value."""
         return self._nodata
 
     @property
     def path(self) -> Series:
+        """Get the 'path' attribute of the rasters."""
         return self.raster_attribute("path")
 
     @property
     def name(self) -> Series:
+        """Get the 'name' attribute of the rasters."""
         return self.raster_attribute("name")
 
     @property
     def date(self) -> Series:
+        """Get the 'date' attribute of the rasters."""
         return self.raster_attribute("date")
 
     @property
     def indexes(self) -> Series:
+        """Get the 'indexes' attribute of the rasters."""
         return self.raster_attribute("indexes")
 
     # @property
     # def raster_id(self) -> Series:
     #     return self.raster_attribute("raster_id")
 
     @property
     def area(self) -> Series:
+        """Get the 'area' attribute of the rasters."""
         return self.raster_attribute("area")
 
     @property
     def length(self) -> Series:
+        """Get the 'length' attribute of the rasters."""
         return self.raster_attribute("length")
 
     @property
     def height(self) -> Series:
+        """Get the 'height' attribute of the rasters."""
         return self.raster_attribute("height")
 
     @property
     def width(self) -> Series:
+        """Get the 'width' attribute of the rasters."""
         return self.raster_attribute("width")
 
     @property
     def shape(self) -> Series:
+        """Get the 'shape' attribute of the rasters."""
         return self.raster_attribute("shape")
 
     @property
     def count(self) -> Series:
+        """Get the 'count' attribute of the rasters."""
         return self.raster_attribute("count")
 
     @property
     def res(self) -> int:
+        """Spatial resolution of the images."""
         return self._res
 
     @res.setter
-    def res(self, value):
+    def res(self, value) -> None:
         self._res = value
 
     @property
     def crs(self) -> pyproj.CRS:
+        """Coordinate reference system of the images."""
         crs = self._warped_crs if hasattr(self, "_warped_crs") else self._crs
         if crs is not None:
             return crs
         try:
             get_common_crs(self.data)
         except ValueError:
             return None
 
     @property
     def unary_union(self) -> Geometry:
+        """Box polygon of the combined bounds of each image."""
         return shapely.unary_union([shapely.box(*r.bounds) for r in self])
 
     @property
     def centroid(self) -> GeoSeries:
+        """Get the 'centroid' attribute of the rasters."""
         return GeoSeries(
             [r.centroid for r in self],
             name="centroid",
             crs=self.crs,
         )
 
     @property
     def tile(self) -> Series:
+        """Get the 'tile' attribute of the rasters."""
         return self.raster_attribute("tile")
 
     @property
     def boxes(self) -> GeoSeries:
-        """GeoSeries of each raster's bounds as polygon."""
+        """Get the 'bounds' attribute of the rasters."""
         return GeoSeries(
             [shapely.box(*r.bounds) if r.bounds is not None else None for r in self],
             name="boxes",
             crs=self.crs,
         )
 
     @property
     def total_bounds(self) -> tuple[float, float, float, float]:
+        """Combined minimum and maximum longitude and latitude."""
         return tuple(x for x in self.boxes.total_bounds)
 
     @property
     def bounds(self) -> BoundingBox:
         """Pytorch bounds of the index.
 
         Returns:
             (minx, maxx, miny, maxy, mint, maxt) of the dataset
         """
         return BoundingBox(*self.index.bounds)
 
-    def copy(self, deep=True) -> Self:
+    def copy(self, deep: bool = True) -> Self:
         """Returns a (deep) copy of the class instance and its rasters.
 
         Args:
             deep: Whether to return a deep or shallow copy. Defaults to True.
         """
         copied = deepcopy(self) if deep else copy(self)
         copied.data = [raster.copy() for raster in copied]
         return copied
 
-    def _check_for_array(self, text="") -> None:
+    def _check_for_array(self, text: str = "") -> None:
         mess = "Arrays are not loaded. " + text
         if all(raster.array is None for raster in self):
             raise ValueError(mess)
 
     def __getitem__(
-        self, item: slice | int | Series | Sequence | Callable | Geometry | BoundingBox
-    ) -> Self | Raster:
-        """
-
-        Examples
-        --------
-        >>> cube = sg.DataCube.from_root(testdata, endswith=".tif", crs=25833).load()
+        self,
+        item: slice | int | Series | list | tuple | Callable | Geometry | BoundingBox,
+    ) -> Self | Raster | TORCHGEO_RETURN_TYPE:
+        """Select one or more of the Rasters based on indexing or spatial or boolean predicates.
+
+        Examples:
+        ------------
+        >>> import sgis as sg
+        >>> root = 'https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/raster'
+        >>> cube = sg.DataCube.from_root(root, filename_regex=sg.raster.SENTINEL2_FILENAME_REGEX, crs=25833).load()
 
         List slicing:
 
         >>> cube[1:3]
         >>> cube[3:]
 
         Single integer returns a Raster, not a cube.
@@ -933,15 +1030,15 @@
             copy.data = copy.data[item]
             return copy
         elif isinstance(item, int):
             return copy.data[item]
         elif callable(item):
             item = item(copy)
         elif isinstance(item, BoundingBox):
-            return cube_to_torch(self, item)
+            return cube_to_torchgeo(self, item)
 
         elif isinstance(item, (GeoDataFrame, GeoSeries, Geometry)) or is_bbox_like(
             item
         ):
             item = to_shapely(item)
             copy.data = [
                 raster for raster in copy.data if raster.bounds.intersects(item)
@@ -952,35 +1049,39 @@
             raster
             for raster, condition in zip(copy.data, item, strict=True)
             if condition
         ]
 
         return copy
 
-    def __setattr__(self, attr, value):
+    def __setattr__(self, attr: str, value: Any) -> None:
+        """Set an attribute of the cube."""
         if (
             attr in ["data", "_data"]
             or not is_list_like(value)
             or not hasattr(self, "data")
         ):
             return super().__setattr__(attr, value)
         if len(value) != len(self.data):
             raise ValueError(
                 "custom cube attributes must be scalar or same length as number of rasters. "
                 f"Got self.data {len(self)} and new attribute {len(value)}"
             )
         return super().__setattr__(attr, value)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Raster]:
+        """Iterate over the Rasters."""
         return iter(self.data)
 
     def __len__(self) -> int:
+        """Number of Rasters."""
         return len(self.data)
 
     def __repr__(self) -> str:
+        """String representation."""
         return f"{self.__class__.__name__}({len(self)})"
 
     # def __mul__(self, scalar) -> Self:
     #     return self.map(_mul, scalar=scalar)
 
     # def __add__(self, scalar) -> Self:
     #     return self.map(_add, scalar=scalar)
@@ -994,31 +1095,40 @@
     # def __floordiv__(self, scalar) -> Self:
     #     return self.map(_floordiv, scalar=scalar)
 
     # def __pow__(self, scalar) -> Self:
     #     return self.map(_pow, scalar=scalar)
 
 
-def concat_cubes(cube_list: list[DataCube], res: int | None = None) -> DataCube:
-    if not all(isinstance(cube, DataCube) for cube in cube_list):
-        raise TypeError
+def concat_cubes(cubes: list[DataCube], res: int | None = None) -> DataCube:
+    """Concatenate cubes to one.
+
+    Args:
+        cubes: A sequence of DataCubes.
+        res: Spatial resolution.
+
+    Returns:
+        The cubes combined to one.
+    """
+    if not all(isinstance(cube, DataCube) for cube in cubes):
+        raise TypeError("cubes must be of type DataCube.")
 
     return DataCube(
-        list(itertools.chain.from_iterable([cube.data for cube in cube_list])), res=res
+        list(itertools.chain.from_iterable([cube.data for cube in cubes])), res=res
     )
 
 
-def clipmerge(cube: DataCube, mask, **kwargs) -> DataCube:
-    return merge(cube, bounds=mask, **kwargs)
+def _clipmerge(cube: DataCube, mask: Any, **kwargs) -> DataCube:
+    return _merge(cube, bounds=mask, **kwargs)
 
 
-def merge(
+def _merge(
     cube: DataCube,
-    by=None,
-    bounds=None,
+    by: str | list[str] | None = None,
+    bounds: Any | None = None,
     **kwargs,
 ) -> DataCube:
     if not all(r.array is None for r in cube):
         raise ValueError("Arrays can't be loaded when calling merge.")
 
     bounds = to_bbox(bounds) if bounds is not None else bounds
 
@@ -1049,104 +1159,66 @@
             )
             for idxs in grouped_indices
         ],
         res=cube.res,
     )
 
 
-def merge_by_bounds(
+def _merge_by_bounds(
     cube: DataCube,
-    by=None,
-    bounds=None,
+    by: str | list[str] | None = None,
+    bounds: Any | None = None,
     **kwargs,
 ) -> DataCube:
     if isinstance(by, str):
         by = [by, "tile"]
     elif by is None:
         by = ["tile"]
     else:
-        by = by + ["tile"]
+        by = list(by) + ["tile"]
 
-    return merge(
+    return _merge(
         cube,
         by=by,
         bounds=bounds,
         **kwargs,
     )
 
 
-def _merge(cube, **kwargs) -> DataCube:
+def _merge(cube: DataCube, **kwargs) -> DataCube:
     if cube.crs is None:
         cube._crs = get_common_crs(cube.data)
 
     indexes = cube[0].indexes_as_tuple()
 
-    datasets = [load_raster(raster.path) for raster in cube]
+    datasets = [_load_raster(raster.path) for raster in cube]
     array, transform = rasterio_merge.merge(datasets, indexes=indexes, **kwargs)
     cube.data = [Raster.from_array(array, crs=cube.crs, transform=transform)]
 
     return cube
 
-    if all(arr is None for arr in cube.arrays):
-        datasets = [load_raster(raster.path) for raster in cube]
-        array, transform = rasterio_merge.merge(datasets, indexes=indexes, **kwargs)
-        cube.data = [Raster.from_array(array, crs=cube.crs, transform=transform)]
-        return cube
-
-    bounds = kwargs.pop("bounds", None)
-
-    if bounds:
-        xarrays = [
-            r.to_xarray().transpose("y", "x")
-            for r in cube.explode()
-            if r.intersects(bounds)
-        ]
-    else:
-        xarrays = [r.to_xarray().transpose("y", "x") for r in cube.explode()]
-
-    if len(xarrays) > 1:
-        merged = merge_arrays(
-            xarrays,
-            bounds=bounds,
-            res=cube.res,
-            nodata=cube.nodata,
-            **kwargs,
-        )
-    else:
-        try:
-            merged = xarrays[0]
-        except IndexError:
-            cube.data = []
-            return cube
-
-    array = merged.to_numpy()
-
-    raster = cube[0].__class__
-    out_bounds = bounds or cube.total_bounds
-    cube.data = [raster.from_array(array, bounds=out_bounds, crs=cube.crs)]
-
-    return cube
-
 
-def load_raster(path):
+def _load_raster(path: str | Path) -> rasterio.io.DatasetReader:
     with opener(path) as file:
         return rasterio.open(file)
 
 
 def numpy_to_torch(array: np.ndarray) -> torch.Tensor:
+    """Convert numpy array to a pytorch tensor."""
     # fix numpy dtypes which are not supported by pytorch tensors
     if array.dtype == np.uint16:
         array = array.astype(np.int32)
     elif array.dtype == np.uint32:
         array = array.astype(np.int64)
 
     return torch.tensor(array)
 
 
-def cube_to_torch(cube: DataCube, query: BoundingBox):
+def cube_to_torchgeo(cube: DataCube, query: BoundingBox) -> TORCHGEO_RETURN_TYPE:
+    """Convert a DayaCube to the type of dict returned from torchgeo datasets __getitem__."""
     bbox = shapely.box(*to_bbox(query))
     if cube.separate_files:
         cube = cube.sfilter(bbox).explode().load()
     else:
         cube = cube.clipmerge(bbox).explode()
 
     data: torch.Tensor = torch.cat([numpy_to_torch(array) for array in cube.arrays])
```

### Comparing `ssb_sgis-1.0.1/src/sgis/raster/indices.py` & `ssb_sgis-1.0.2/src/sgis/raster/indices.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from collections.abc import Callable
 
 import numpy as np
 import pandas as pd
 
 from .raster import Raster
 
 
@@ -14,37 +14,33 @@
     return np.where((green + nir) == 0, 0, (nir - green) / (nir + green))
 
 
 def water(green: np.ndarray, nir: np.ndarray) -> np.ndarray:
     return np.where((green + nir) == 0, 0, (green - nir) / (green + nir))
 
 
-def water(swir: np.ndarray, nir: np.ndarray) -> np.ndarray:
-    return np.where((swir + nir) == 0, 0, (nir - swir) / (nir + swir))
-
-
 def builtup(swir: np.ndarray, nir: np.ndarray) -> np.ndarray:
     return np.where((swir + nir) == 0, 0, (swir - nir) / (swir + nir))
 
 
 def moisture(swir: np.ndarray, nir: np.ndarray) -> np.ndarray:
     return np.where((swir + nir) == 0, 0, (nir - swir) / (nir + swir))
 
 
 def get_raster_pairs(
     cube,
     band_name1: str,
     band_name2: str,
-):
+) -> list[tuple[Raster, Raster]]:
     unique = pd.DataFrame({"tile": cube.tile, "date": cube.date}).drop_duplicates(
         ["tile", "date"]
     )
 
     raster_pairs = []
-    for tile, date in zip(unique["tile"], unique["date"]):
+    for tile, date in zip(unique["tile"], unique["date"], strict=False):
         query = (cube.tile == tile) & (cube.date == date)
         band1 = cube.copy()[query & (cube.band == band_name1)]
         band2 = cube.copy()[query & (cube.band == band_name2)]
         if not len(band1) and not len(band2):
             continue
         if len(band1) > 1:
             raise ValueError("Cannot have more than one B4 band per tile.")
```

### Comparing `ssb_sgis-1.0.1/src/sgis/raster/raster.py` & `ssb_sgis-1.0.2/src/sgis/raster/raster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,101 @@
 import functools
 import numbers
+import os
 import re
 import warnings
-from collections.abc import Callable, Iterable
-from copy import copy, deepcopy
+from collections.abc import Callable
+from collections.abc import Iterable
+from collections.abc import Iterator
+from copy import copy
+from copy import deepcopy
 from json import loads
 from pathlib import Path
+from typing import Any
+from typing import ClassVar
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio
+import rasterio.windows
 import shapely
 from typing_extensions import Self  # TODO: imperter fra typing når python 3.11
 
-
 try:
     import xarray as xr
     from xarray import DataArray
 except ImportError:
 
     class DataArray:
-        pass
+        """Placeholder."""
+
+
+try:
+    from dapla.gcs import GCSFileSystem
+except ImportError:
+
+    class GCSFileSystem:
+        """Placeholder."""
 
 
 try:
     from rioxarray.rioxarray import _generate_spatial_coords
 except ImportError:
     pass
 from affine import Affine
-from geopandas import GeoDataFrame, GeoSeries
+from geopandas import GeoDataFrame
+from geopandas import GeoSeries
 from pandas.api.types import is_list_like
 from rasterio import features
 from rasterio.enums import MergeAlg
 from rasterio.io import DatasetReader
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import reproject
 from shapely import Geometry
-from shapely.geometry import Point, Polygon, shape
-
-from ..geopandas_tools.conversion import to_bbox, to_gdf, to_shapely
-from ..geopandas_tools.general import is_bbox_like, is_wkt
+from shapely.geometry import Point
+from shapely.geometry import Polygon
+from shapely.geometry import shape
+
+from ..geopandas_tools.conversion import to_bbox
+from ..geopandas_tools.conversion import to_gdf
+from ..geopandas_tools.conversion import to_shapely
+from ..geopandas_tools.general import is_bbox_like
+from ..geopandas_tools.general import is_wkt
 from ..helpers import is_property
 from ..io.opener import opener
-from .base import ALLOWED_KEYS, NESSECARY_META, get_index_mapper, memfile_from_array
-from .gradient import get_gradient
-from .zonal import (
-    _aggregate,
-    _no_overlap_df,
-    make_geometry_iterrows,
-    prepare_zonal,
-    zonal_post,
-)
-
+from .base import ALLOWED_KEYS
+from .base import NESSECARY_META
+from .base import get_index_mapper
+from .base import memfile_from_array
+from .zonal import _aggregate
+from .zonal import _make_geometry_iterrows
+from .zonal import _no_overlap_df
+from .zonal import _prepare_zonal
+from .zonal import _zonal_post
 
 numpy_func_message = (
     "aggfunc must be functions or strings of numpy functions or methods."
 )
 
 
 class Raster:
     """For reading, writing and working with rasters.
 
     Raster instances should be created with the methods 'from_path', 'from_array' or
     'from_gdf'.
 
 
-    Examples
+    Examples:
     --------
-
     Read tif file.
 
+    >>> import sgis as sg
     >>> path = 'https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/raster/dtm_10.tif'
     >>> raster = sg.Raster.from_path(path)
     >>> raster
     Raster(shape=(1, 201, 201), res=10, crs=ETRS89 / UTM zone 33N (N-E), path=https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/raster/dtm_10.tif)
 
     Load the entire image as an numpy ndarray.
     Operations are done in place to save memory.
@@ -143,68 +162,72 @@
     25097   9.4   9.4  POLYGON ((-24925.000 6674005.000, -24925.000 6...
     25098   5.3   5.3  POLYGON ((-24915.000 6674005.000, -24915.000 6...
     25099   2.3   2.3  POLYGON ((-24905.000 6674005.000, -24905.000 6...
     25100   0.1   0.1  POLYGON ((-24895.000 6674005.000, -24895.000 6...
 
     """
 
-    # attributes conserning file path
-    filename_regex: str | None = None
-    date_format: str | None = None
-    contains: str | None = None
-    endswith: str = ".tif"
-
-    # attributes conserning rasterio metadata
-    _profile = {
+    # attributes concerning rasterio metadata
+    _profile: ClassVar[dict[str, str | None]] = {
         "driver": "GTiff",
         "compress": "LZW",
         "nodata": None,
         "dtype": None,
         "crs": None,
         "tiled": None,
         "indexes": None,
     }
 
-    # driver: str = "GTiff"
-    # compress: str = "LZW"
-    # _nodata: int | float | None = None
-    # _dtype: type | None = None
-
     def __init__(
         self,
-        raster=None,
+        data: Self | str | np.ndarray | None = None,
         *,
-        path: str | None = None,
-        # indexes: int | list[int] | None = None,
-        array: np.ndarray | None = None,
-        file_system=None,
+        file_system: GCSFileSystem | None = None,
+        filename_regex: str | None = None,
         **kwargs,
-    ):
-        if raster is not None:
-            if not isinstance(raster, Raster):
-                raise TypeError(
-                    "Raster should be constructed with the classmethods (from_...)."
-                )
-            for key, value in raster.__dict__.items():
-                setattr(raster, key, value)
+    ) -> None:
+        """Note: use the classmethods from_path, from_array, from_gdf etc. instead of the initialiser.
+
+        Args:
+            data: A file path, an array or a Raster object.
+            file_system: Optional GCSFileSystem.
+            filename_regex: Regular expression to match file name attributes (date, band, tile, resolution).
+            **kwargs: Arguments concerning file metadata or
+                spatial properties of the image.
+        """
+        self.filename_regex = filename_regex
+
+        if isinstance(data, Raster):
+            for key, value in data.__dict__.items():
+                setattr(data, key, value)
             return
 
-        if path is None and not any([kwargs.get("transform"), kwargs.get("bounds")]):
+        if isinstance(data, (str | Path | os.PathLike)):
+            self.path = data
+
+        else:
+            self.path = None
+
+        if isinstance(data, (np.ndarray)):
+            self.array = data
+        else:
+            self.array = None
+
+        if self.path is None and not any(
+            [kwargs.get("transform"), kwargs.get("bounds")]
+        ):
             raise TypeError(
                 "Must specify either bounds or transform when constructing raster from array."
             )
 
-        # add class profile first to override with args and kwargs
+        # add class profile first, then override with args and kwargs
         self.update(**self._profile)
 
         self._crs = kwargs.pop("crs", self._crs if hasattr(self, "_crs") else None)
         self._bounds = None
-
-        self.path = path
-        self.array = array
         self.file_system = file_system
         self._indexes = self._get_indexes(kwargs.pop("indexes", self.indexes))
 
         # override the above with kwargs
         self.update(**kwargs)
 
         attributes = set(self.__dict__.keys()).difference(set(self.properties))
@@ -216,58 +239,66 @@
         self._prev_crs = self._crs
 
     @classmethod
     def from_path(
         cls,
         path: str,
         res: int | None = None,
-        file_system=None,
+        file_system: GCSFileSystem | None = None,
+        filename_regex: str | None = None,
         **kwargs,
-    ):
+    ) -> Self:
         """Construct Raster from file path.
 
         Args:
             path: Path to a raster image file.
+            res: Spatial resolution when reading the image.
+            file_system: Optional file system.
+            filename_regex: Regular expression with optional match groups.
+            **kwargs: Arguments concerning file metadata or
+                spatial properties of the image.
 
         Returns:
             A Raster instance.
         """
         return cls(
-            path=str(path),
+            str(path),
             file_system=file_system,
             res=res,
+            filename_regex=filename_regex,
             **kwargs,
         )
 
     @classmethod
     def from_array(
         cls,
         array: np.ndarray,
-        crs,
+        crs: Any,
         *,
         transform: Affine | None = None,
         bounds: tuple | Geometry | None = None,
         copy: bool = True,
         **kwargs,
-    ):
+    ) -> Self:
         """Construct Raster from numpy array.
 
-        Metadata must be specified, either individually or in a dictionary
-        (hint: use the 'meta' attribute of an existing Raster object if applicable).
-        The necessary metadata is 'crs' and either 'transform' (Affine object) or 'bounds',
-        which transform will then be created from.
+        Must also specify nessecary spatial properties
+        The necessary metadata is 'crs' and either 'transform' (Affine object)
+        or 'bounds', which transform will then be created from.
 
         Args:
             array: 2d or 3d numpy ndarray.
             crs: Coordinate reference system.
             transform: Affine transform object. Can be specified instead
                 of bounds.
             bounds: Minimum and maximum x and y coordinates. Can be specified instead
                 of transform.
-            name: Optional name to give the raster.
+            copy: Whether to copy the array.
+            **kwargs: Arguments concerning file metadata or
+                spatial properties of the image.
 
         Returns:
             A Raster instance.
         """
         if array is None:
             raise TypeError("Must specify array.")
 
@@ -291,37 +322,54 @@
             bounds = to_bbox(bounds)
 
         if transform and not bounds:
             bounds = rasterio.transform.array_bounds(height, width, transform)
 
         crs = pyproj.CRS(crs) if crs else None
 
-        return cls(array=array, crs=crs, transform=transform, bounds=bounds, **kwargs)
+        return cls(array, crs=crs, transform=transform, bounds=bounds, **kwargs)
 
     @classmethod
     def from_gdf(
         cls,
         gdf: GeoDataFrame,
         columns: str | Iterable[str],
         res: int,
-        fill=0,
-        all_touched=False,
-        merge_alg=MergeAlg.replace,
-        default_value=1,
-        dtype=None,
+        fill: int = 0,
+        all_touched: bool = False,
+        merge_alg: Callable = MergeAlg.replace,
+        default_value: int = 1,
+        dtype: Any | None = None,
         **kwargs,
-    ):
+    ) -> Self:
         """Construct Raster from a GeoDataFrame.
 
         Args:
-            gdf: The GeoDataFrame.
-            column: The column to be used as values for the array.
-            res: Resolution of the raster in units of gdf's coordinate
-                reference system.
+            gdf: The GeoDataFrame to rasterize.
+            columns: Column(s) in the GeoDataFrame whose values are used to populate the raster.
+                This can be a single column name or a list of column names.
+            res: Resolution of the raster in units of the GeoDataFrame's coordinate reference system.
+            fill: Fill value for areas outside of input geometries (default is 0).
+            all_touched: Whether to consider all pixels touched by geometries,
+                not just those whose center is within the polygon (default is False).
+            merge_alg: Merge algorithm to use when combining geometries
+                (default is 'MergeAlg.replace').
+            default_value: Default value to use for the rasterized pixels
+                (default is 1).
+            dtype: Data type of the output array. If None, it will be
+                determined automatically.
+            **kwargs: Additional keyword arguments passed to the raster
+                creation process, e.g., custom CRS or transform settings.
 
+        Returns:
+            A Raster instance based on the specified GeoDataFrame and parameters.
+
+        Raises:
+            TypeError: If 'transform' is provided in kwargs, as this is
+            computed based on the GeoDataFrame bounds and resolution.
         """
         if not isinstance(gdf, GeoDataFrame):
             gdf = to_gdf(gdf)
 
         if "transform" in kwargs:
             raise TypeError("Unexpected argument 'transform'")
 
@@ -358,18 +406,18 @@
             for col in columns:
                 arr = _rasterize(gdf, col)
                 array.append(arr)
             array = np.array(array)
             assert len(array.shape) == 3
             name = kwargs.get("name", None)
 
-        return cls.from_array(array=array, name=name, **kwargs)
+        return cls.from_array(array, name=name, **kwargs)
 
     @classmethod
-    def from_dict(cls, dictionary: dict):
+    def from_dict(cls, dictionary: dict) -> Self:
         """Construct Raster from metadata dict to fastpass the initializer.
 
         This is the fastest way to create a Raster since a metadata lookup is not
         needed.
 
         The dictionary must have all the keys ...
         and at least one of the keys 'transform' and 'bounds'.
@@ -383,31 +431,36 @@
             A Raster instance.
         """
         cls._validate_dict(dictionary)
 
         return cls(**dictionary)
 
     def update(self, **kwargs) -> Self:
+        """Update attributes of the Raster."""
         for key, value in kwargs.items():
             self._validate_key(key)
             if is_property(self, key):
                 key = "_" + key
             setattr(self, key, value)
         return self
 
-    def write(self, path: str, window=None, **kwargs) -> None:
+    def write(
+        self, path: str, window: rasterio.windows.Window | None = None, **kwargs
+    ) -> None:
         """Write the raster as a single file.
 
         Multiband arrays will result in a multiband image file.
 
         Args:
             path: File path to write to.
             window: Optional window to clip the image to.
+            **kwargs: Keyword arguments passed to rasterio.open.
+                Thise will override the items in the Raster's profile,
+                if overlapping.
         """
-
         if self.array is None:
             raise AttributeError("The image hasn't been loaded.")
 
         profile = self.profile | kwargs
 
         with opener(path, file_system=self.file_system) as file:
             with rasterio.open(file, "w", **profile) as dst:
@@ -432,51 +485,59 @@
 
         self._read_tif(**kwargs)
 
         return self
 
     def clip(
         self,
-        mask,
+        mask: Any,
         masked: bool = False,
         boundless: bool = True,
         **kwargs,
     ) -> Self:
         """Load the part of the image inside the mask.
 
         The returned array is stored in the 'array' attribute
         of the Raster.
 
         Args:
             mask: Geometry-like object or bounding box.
+            masked: If 'masked' is True the return value will be a masked
+                array. Otherwise (default) the return value will be a
+                regular array. Masks will be exactly the inverse of the
+                GDAL RFC 15 conforming arrays returned by read_masks().
+            boundless: If True, windows that extend beyond the dataset's extent
+                are permitted and partially or completely filled arrays will
+                be returned as appropriate.
             **kwargs: Keyword arguments passed to the mask function
                 from the rasterio.mask module.
 
         Returns:
             Self, but with the array loaded.
         """
         if not isinstance(mask, GeoDataFrame):
             mask = self._return_gdf(mask)
 
         try:
             mask = mask.to_crs(self.crs)
         except ValueError:
             mask = mask.set_crs(self.crs)
 
-        # if not self.crs.equals(pyproj.CRS(mask.crs)):
-        #     raise ValueError("crs mismatch.")
-
         self._read_with_mask(mask=mask, masked=masked, boundless=boundless, **kwargs)
 
         return self
 
-    def intersects(self, other) -> bool:
+    def intersects(self, other: Any) -> bool:
+        """Returns True if the image bounds intersect with 'other'."""
         return self.unary_union.intersects(to_shapely(other))
 
-    def sample(self, n=1, size=20, mask=None, copy=True, **kwargs) -> Self:
+    def sample(
+        self, n: int = 1, size: int = 20, mask: Any = None, copy: bool = True, **kwargs
+    ) -> Self:
+        """Take a random spatial sample of the image."""
         if mask is not None:
             points = GeoSeries(self.unary_union).clip(mask).sample_points(n)
         else:
             points = GeoSeries(self.unary_union).sample_points(n)
         buffered = points.buffer(size / self.res)
         boxes = to_gdf(
             [shapely.box(*arr) for arr in buffered.bounds.values], crs=self.crs
@@ -504,27 +565,27 @@
             dropna: If True (default), polygons with all missing
                 values will be removed.
 
         Returns:
             A GeoDataFrame with aggregated values per polygon.
         """
         idx_mapper, idx_name = get_index_mapper(polygons)
-        polygons, aggfunc, func_names = prepare_zonal(polygons, aggfunc)
-        poly_iter = make_geometry_iterrows(polygons)
+        polygons, aggfunc, func_names = _prepare_zonal(polygons, aggfunc)
+        poly_iter = _make_geometry_iterrows(polygons)
 
         aggregated = []
         for i, poly in poly_iter:
             clipped = self.clip(poly)
             if not np.size(clipped.array):
                 aggregated.append(_no_overlap_df(func_names, i, date=self.date))
             aggregated.append(
                 _aggregate(clipped.array, array_func, aggfunc, func_names, self.date, i)
             )
 
-        return zonal_post(
+        return _zonal_post(
             aggregated,
             polygons=polygons,
             idx_mapper=idx_mapper,
             idx_name=idx_name,
             dropna=dropna,
         )
 
@@ -542,15 +603,15 @@
                 the values will be in degrees from 0 to 90.
             copy: Whether to copy or overwrite the original Raster.
                 Defaults to False to save memory.
 
         Returns:
             The class instance with new array values, or a copy if copy is True.
 
-        Examples
+        Examples:
         --------
         Making an array where the gradient to the center is always 10.
 
         >>> import sgis as sg
         >>> import numpy as np
         >>> arr = np.array(
         ...         [
@@ -576,14 +637,15 @@
             [1., 1., 0., 1., 1.],
             [1., 1., 1., 1., 1.],
             [0., 1., 1., 1., 0.]])
         """
         return get_gradient(self, degrees=degrees, copy=copy)
 
     def to_xarray(self) -> DataArray:
+        """Convert the raster to  an xarray.DataArray."""
         self._check_for_array()
         self.name = self.name or self.__class__.__name__.lower()
         coords = _generate_spatial_coords(self.transform, self.width, self.height)
         if len(self.array.shape) == 2:
             dims = ["y", "x"]
             # dims = ["band", "y", "x"]
             # array = np.array([self.array])
@@ -598,14 +660,15 @@
             coords=coords,
             dims=dims,
             name=self.name,
             attrs={"crs": self.crs},
         )  # .transpose("y", "x")
 
     def to_dict(self) -> dict:
+        """Get a dictionary of Raster attributes."""
         out = {}
         for col in self.ALL_ATTRS:
             try:
                 out[col] = self[col]
             except AttributeError:
                 pass
         return out
@@ -638,44 +701,44 @@
         if column is None:
             column = ["value"] * len(array_list)
 
         if isinstance(column, str):
             column = [column] * len(array_list)
 
         gdfs = []
-        for i, (column, array) in enumerate(zip(column, array_list, strict=True)):
+        for i, (col, array) in enumerate(zip(column, array_list, strict=True)):
             gdf = gpd.GeoDataFrame(
                 pd.DataFrame(
                     self._array_to_geojson(array, self.transform),
-                    columns=[column, "geometry"],
+                    columns=[col, "geometry"],
                 ),
                 geometry="geometry",
                 crs=self.crs,
             )
             gdf["indexes"] = i + 1
             gdfs.append(gdf)
 
         return pd.concat(gdfs, ignore_index=True)
 
     def set_crs(
         self,
-        crs,
+        crs: pyproj.CRS | Any,
         allow_override: bool = False,
     ) -> Self:
         """Set coordinate reference system."""
         if not allow_override and self.crs is not None:
             raise ValueError("Cannot overwrite crs when allow_override is False.")
 
         if self.array is None:
             raise ValueError("array must be loaded/clipped before set_crs")
 
         self._crs = pyproj.CRS(crs)
         return self
 
-    def to_crs(self, crs, **kwargs) -> Self:
+    def to_crs(self, crs: pyproj.CRS | Any, **kwargs) -> Self:
         """Reproject the raster.
 
         Args:
             crs: The new coordinate reference system.
             **kwargs: Keyword arguments passed to the reproject function
                 from the rasterio.warp module.
         """
@@ -735,17 +798,17 @@
             )
 
         self._warped_crs = pyproj.CRS(crs)
         self._prev_crs = pyproj.CRS(crs)
 
         return self
 
-    def plot(self, mask=None) -> None:
-        self._check_for_array()
+    def plot(self, mask: Any | None = None) -> None:
         """Plot the images. One image per band."""
+        self._check_for_array()
         if mask is not None:
             raster = self.copy().clip(mask)
         else:
             raster = self
 
         if len(raster.shape) == 2:
             array = np.array([raster.array])
@@ -756,34 +819,38 @@
             ax = plt.axes()
             ax.imshow(arr)
             ax.axis("off")
             plt.show()
             plt.close()
 
     def astype(self, dtype: type) -> Self:
+        """Convert the datatype of the array."""
         if self.array is None:
             raise ValueError("Array is not loaded.")
         if not rasterio.dtypes.can_cast_dtype(self.array, dtype):
             min_dtype = rasterio.dtypes.get_minimum_dtype(self.array)
             raise ValueError(f"Cannot cast to dtype. Minimum dtype is {min_dtype}")
         self.array = self.array.astype(dtype)
         self._dtype = dtype
         return self
 
     def as_minimum_dtype(self) -> Self:
+        """Convert the array to the minimum dtype without overflow."""
         min_dtype = rasterio.dtypes.get_minimum_dtype(self.array)
         self.array = self.array.astype(min_dtype)
         return self
 
     def min(self) -> int | None:
+        """Minimum value in the array."""
         if np.size(self.array):
             return np.min(self.array)
         return None
 
     def max(self) -> int | None:
+        """Maximum value in the array."""
         if np.size(self.array):
             return np.max(self.array)
         return None
 
     def _add_meta(self) -> Self:
         mess = "Cannot add metadata after image has been "
         if hasattr(self, "_clipped"):
@@ -794,102 +861,105 @@
         with opener(self.path, file_system=self.file_system) as file:
             with rasterio.open(file) as src:
                 self._add_meta_from_src(src)
 
         return self
 
     def array_list(self) -> list[np.ndarray]:
+        """Get a list of 2D arrays."""
         self._check_for_array()
         if len(self.array.shape) == 2:
             return [self.array]
         elif len(self.array.shape) == 3:
             return list(self.array)
         else:
             raise ValueError
 
     @property
     def indexes(self) -> int | tuple[int] | None:
+        """Band indexes of the image."""
         return self._indexes
 
     @property
     def name(self) -> str | None:
+        """Name of the file in the file path, if any."""
         try:
             return self._name
         except AttributeError:
             try:
                 return Path(self.path).name
             except TypeError:
                 return None
 
     @name.setter
-    def name(self, value):
+    def name(self, value) -> None:
         self._name = value
-        return self._name
 
     @property
-    def date(self):
+    def date(self) -> str | None:
+        """Date in the image file name, if filename_regex is present."""
         try:
             pattern = re.compile(self.filename_regex, re.VERBOSE)
             return re.match(pattern, Path(self.path).name).group("date")
         except (AttributeError, TypeError):
             return None
 
     @property
     def band(self) -> str | None:
+        """Band name of the image file name, if filename_regex is present."""
         try:
             pattern = re.compile(self.filename_regex, re.VERBOSE)
             return re.match(pattern, Path(self.path).name).group("band")
         except (AttributeError, TypeError):
             return None
 
-    # @property
-    # def band_color(self):
-    #     """To be implemented in subclasses."""
-    #     pass
-
     @property
-    def dtype(self):
+    def dtype(self) -> Any:
+        """Data type of the array."""
         try:
             return self.array.dtype
         except AttributeError:
             try:
                 return self._dtype
             except AttributeError:
                 return None
 
     @dtype.setter
-    def dtype(self, new_dtype):
+    def dtype(self, new_dtype: Any) -> None:
         self.array = self.array.astype(new_dtype)
-        return self.array.dtype
 
     @property
     def nodata(self) -> int | None:
+        """No data value."""
         try:
             return self._nodata
         except AttributeError:
             return None
 
     @property
     def tile(self) -> str | None:
+        """The lower left corner (minx, miny) of the image as a string."""
         if self.bounds is None:
             return None
         return f"{int(self.bounds[0])}_{int(self.bounds[1])}"
 
     @property
     def meta(self) -> dict:
+        """Metadata dict."""
         return {
             "path": self.path,
             "type": self.__class__.__name__,
             "bounds": self.bounds,
             "indexes": self.indexes,
             "crs": self.crs,
         }
 
     @property
     def profile(self) -> dict:
+        """Profile of the image file."""
         # TODO: .crs blir feil hvis warpa. Eller?
         return {
             "driver": self.driver,
             "compress": self.compress,
             "dtype": self.dtype,
             "crs": self.crs,
             "transform": self.transform,
@@ -898,41 +968,45 @@
             "height": self.height,
             "width": self.width,
             "indexes": self.indexes,
         }
 
     @property
     def read_kwargs(self) -> dict:
+        """Keywords passed to the read method of rasterio.io.DatasetReader."""
         return {
             "indexes": self.indexes,
             "fill_value": self.nodata,
             "masked": True,
         }
 
     @property
     def res(self) -> float | None:
+        """Get the spatial resolution of the image."""
         if hasattr(self, "_res") and self._res is not None:
             return self._res
         if self.width is None:
             return None
         diffx = self.bounds[2] - self.bounds[0]
         return diffx / self.width
 
     @property
     def height(self) -> int | None:
+        """Get the height of the image as number of pixels."""
         if self.array is None:
             try:
                 return self._height
             except AttributeError:
                 return None
         i = 1 if len(self.array.shape) == 3 else 0
         return self.array.shape[i]
 
     @property
     def width(self) -> int | None:
+        """Get the width of the image as number of pixels."""
         if self.array is None:
             try:
                 return self._width
             except AttributeError:
                 try:
                     heigth, width = get_shape_from_bounds(self, self.res)  # .res[0])
                     self._width = width
@@ -941,14 +1015,15 @@
                 except Exception:
                     return None
         i = 2 if len(self.array.shape) == 3 else 1
         return self.array.shape[i]
 
     @property
     def count(self) -> int:
+        """Get the number of bands in the image."""
         if self.array is not None:
             if len(self.array.shape) == 3:
                 return self.array.shape[0]
             if len(self.array.shape) == 2:
                 return 1
         if not hasattr(self._indexes, "__iter__"):
             return 1
@@ -961,83 +1036,93 @@
             return self.array.shape
         if hasattr(self._indexes, "__iter__"):
             return self.count, self.width, self.height
         return self.width, self.height
 
     @property
     def transform(self) -> Affine | None:
+        """Get the Affine transform of the image."""
         try:
             return rasterio.transform.from_bounds(*self.bounds, self.width, self.height)
         except (ZeroDivisionError, TypeError):
             if not self.width or not self.height:
                 return None
 
     @property
     def bounds(self) -> tuple[float, float, float, float] | None:
+        """Get the bounds of the image."""
         try:
             return to_bbox(self._bounds)
         except (AttributeError, TypeError):
             return None
 
     @property
-    def crs(self):
+    def crs(self) -> pyproj.CRS | None:
+        """Get the coordinate reference system of the image."""
         try:
             return self._warped_crs
         except AttributeError:
             try:
                 return self._crs
             except AttributeError:
                 return None
 
     @property
     def area(self) -> float:
+        """Get the area of the image."""
         return shapely.area(self.unary_union)
 
     @property
     def length(self) -> float:
+        """Get the circumfence of the image."""
         return shapely.length(self.unary_union)
 
     @property
     def unary_union(self) -> Polygon:
+        """Get the image bounds as a Polygon."""
         return shapely.box(*self.bounds)
 
     @property
     def centroid(self) -> Point:
+        """Get the centerpoint of the image."""
         x = (self.bounds[0] + self.bounds[2]) / 2
         y = (self.bounds[1] + self.bounds[3]) / 2
         return Point(x, y)
 
     @property
     def properties(self) -> list[str]:
+        """List of all properties of the class."""
         out = []
         for attr in dir(self):
             try:
                 if is_property(self, attr):
                     out.append(attr)
             except AttributeError:
                 pass
         return out
 
     def indexes_as_tuple(self) -> tuple[int, ...]:
+        """Get the band index(es) as a tuple of integers."""
         if len(self.shape) == 2:
             return (1,)
         return tuple(i + 1 for i in range(self.shape[0]))
 
-    def copy(self, deep=True):
+    def copy(self, deep: bool = True) -> "Raster":
         """Returns a (deep) copy of the class instance.
 
         Args:
             deep: Whether to return a deep or shallow copy. Defaults to True.
         """
         if deep:
             return deepcopy(self)
         else:
             return copy(self)
 
-    def equals(self, other) -> bool:
+    def equals(self, other: Any) -> bool:
+        """Check if the Raster is equal to another Raster."""
         if not isinstance(other, Raster):
             raise NotImplementedError("other must be of type Raster")
         if type(other) != type(self):
             return False
         if self.array is None and other.array is not None:
             return False
         if self.array is not None and other.array is None:
@@ -1057,65 +1142,81 @@
         shp = ", ".join([str(x) for x in shape])
         try:
             res = int(self.res)
         except TypeError:
             res = None
         return f"{self.__class__.__name__}(shape=({shp}), res={res}, name={self.name}, path={self.path})"
 
-    def __mul__(self, scalar):
+    def __iter__(self) -> Iterator[np.ndarray]:
+        """Iterate over the arrays."""
+        if len(self.array.shape) == 2:
+            return iter([self.array])
+        if len(self.array.shape) == 3:
+            return iter(self.array)
+        raise ValueError(
+            f"Array should have shape length 2 or 3. Got {len(self.array.shape)}"
+        )
+
+    def __mul__(self, scalar: int | float) -> "Raster":
+        """Multiply the array values with *."""
         self._check_for_array()
         self.array = self.array * scalar
         return self
 
-    def __add__(self, scalar):
+    def __add__(self, scalar: int | float) -> "Raster":
+        """Add to the array values with +."""
         self._check_for_array()
         self.array = self.array + scalar
         return self
 
-    def __sub__(self, scalar):
+    def __sub__(self, scalar: int | float) -> "Raster":
+        """Subtract the array values with -."""
         self._check_for_array()
         self.array = self.array - scalar
         return self
 
-    def __truediv__(self, scalar):
+    def __truediv__(self, scalar: int | float) -> "Raster":
+        """Divide the array values with /."""
         self._check_for_array()
         self.array = self.array / scalar
         return self
 
-    def __floordiv__(self, scalar):
+    def __floordiv__(self, scalar: int | float) -> "Raster":
+        """Floor divide the array values with //."""
         self._check_for_array()
         self.array = self.array // scalar
         return self
 
-    def __pow__(self, exponent):
+    def __pow__(self, exponent: int | float) -> "Raster":
+        """Exponentiate the array values with **."""
         self._check_for_array()
         self.array = self.array**exponent
         return self
 
-    def _has_nessecary_attrs(self, dict_like) -> bool:
+    def _has_nessecary_attrs(self, dict_like: dict) -> bool:
         """Check if Raster init got enough kwargs to not need to read src."""
         try:
             self._validate_dict(dict_like)
             return all(
                 x is not None for x in [self.indexes, self.res, self.crs, self.bounds]
             )
         except AttributeError:
             return False
 
-    def _return_self_or_copy(self, array, copy: bool):
+    def _return_self_or_copy(self, array: np.ndarray, copy: bool) -> "Raster":
         if not copy:
             self.array = array
             return self
         else:
             copy = self.copy()
             copy.array = array
             return copy
 
     @classmethod
-    def _validate_dict(cls, dict_like) -> None:
+    def _validate_dict(cls, dict_like: dict) -> None:
         missing = []
         for attr in NESSECARY_META:
             if any(
                 [
                     attr in dict_like,
                     f"_{attr}" in dict_like,
                     attr.lstrip("_") in dict_like,
@@ -1123,35 +1224,37 @@
             ):
                 continue
             missing.append(attr)
         if missing:
             raise AttributeError(f"Missing nessecary key(s) {', '.join(missing)}")
 
     @classmethod
-    def _validate_key(cls, key) -> None:
+    def _validate_key(cls, key: str) -> None:
         if key not in ALLOWED_KEYS:
             raise ValueError(
                 f"Got an unexpected key {key!r}. Allowed keys are ",
                 ", ".join(ALLOWED_KEYS),
             )
 
-    def _get_shape_from_res(self, res) -> tuple[int] | None:
+    def _get_shape_from_res(self, res: int) -> tuple[int] | None:
         if res is None:
             return None
         if hasattr(res, "__iter__") and len(res) == 2:
             res = res[0]
         diffx = self.bounds[2] - self.bounds[0]
         diffy = self.bounds[3] - self.bounds[1]
         width = int(diffx / res)
         height = int(diffy / res)
         if hasattr(self.indexes, "__iter__"):
             return len(self.indexes), width, height
         return width, height
 
-    def _write(self, dst, window):
+    def _write(
+        self, dst: rasterio.io.DatasetReader, window: rasterio.windows.Window
+    ) -> None:
         if np.ma.is_masked(self.array):
             if len(self.array.shape) == 2:
                 return dst.write(
                     self.array.filled(self.nodata), indexes=1, window=window
                 )
 
             for i in range(len(self.indexes_as_tuple())):
@@ -1164,15 +1267,15 @@
         else:
             if len(self.array.shape) == 2:
                 return dst.write(self.array, indexes=1, window=window)
 
             for i, idx in enumerate(self.indexes_as_tuple()):
                 dst.write(self.array[i], indexes=idx, window=window)
 
-    def _get_indexes(self, indexes):
+    def _get_indexes(self, indexes: int | tuple[int] | None) -> int | tuple[int] | None:
         if isinstance(indexes, numbers.Number):
             return int(indexes)
         if indexes is None:
             if self.array is not None and len(self.array.shape) == 3:
                 return tuple(i + 1 for i in range(self.array.shape[0]))
             elif self.array is not None and len(self.array.shape) == 2:
                 return 1
@@ -1184,15 +1287,15 @@
             return tuple(int(x) for x in indexes)
         except Exception as e:
             raise TypeError(
                 "indexes should be an integer or an iterable of integers."
                 f"Got {type(indexes)}: {indexes}"
             ) from e
 
-    def _return_gdf(self, obj) -> GeoDataFrame:
+    def _return_gdf(self, obj: Any) -> GeoDataFrame:
         if isinstance(obj, str) and not is_wkt(obj):
             return self._read_tif(obj)
         elif isinstance(obj, Raster):
             return obj.to_gdf()
         elif is_bbox_like(obj):
             return to_gdf(shapely.box(*to_bbox(obj)), crs=self.crs)
         else:
@@ -1206,42 +1309,44 @@
 
     @staticmethod
     def _gdf_to_geojson_with_col(gdf: GeoDataFrame, column: str) -> list[dict]:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             return [
                 (feature["geometry"], val)
-                for val, feature in zip(gdf[column], loads(gdf.to_json())["features"])
+                for val, feature in zip(
+                    gdf[column], loads(gdf.to_json())["features"], strict=False
+                )
             ]
 
     @staticmethod
-    def _array_to_geojson(array: np.ndarray, transform: Affine):
+    def _array_to_geojson(array: np.ndarray, transform: Affine) -> list[tuple]:
         try:
             return [
                 (value, shape(geom))
                 for geom, value in features.shapes(array, transform=transform)
             ]
         except ValueError:
             array = array.astype(np.float32)
             return [
                 (value, shape(geom))
                 for geom, value in features.shapes(array, transform=transform)
             ]
 
-    def _add_indexes_from_array(self, indexes):
+    def _add_indexes_from_array(self, indexes: int | tuple[int]) -> int | tuple[int]:
         if indexes is not None:
             return indexes
         elif len(self.array.shape) == 3:
             return tuple(x + 1 for x in range(len(self.array)))
         elif len(self.array.shape) == 2:
             return 1
         else:
             raise ValueError
 
-    def _add_meta_from_src(self, src):
+    def _add_meta_from_src(self, src: rasterio.io.DatasetReader) -> None:
         if not hasattr(self, "_bounds") or self._bounds is None:
             self._bounds = tuple(src.bounds)
 
         try:
             self._crs = pyproj.CRS(src.crs)
         except pyproj.exceptions.CRSError:
             self._crs = None
@@ -1289,15 +1394,15 @@
             return vrt
         return src
 
     def _read_tif(self, **kwargs) -> None:
         return self._read(self.path, **kwargs)
 
     @functools.lru_cache(maxsize=128)
-    def _read(self, path, **kwargs):
+    def _read(self, path: str | Path, **kwargs) -> None:
         with opener(path, file_system=self.file_system) as file:
             with rasterio.open(file) as src:
                 self._add_meta_from_src(src)
                 out_shape = self._get_shape_from_res(self.res)
 
                 if hasattr(self, "_warped_crs"):
                     src = WarpedVRT(src, crs=self.crs)
@@ -1307,15 +1412,17 @@
                     **(self.read_kwargs | kwargs),
                 )
                 if self._dtype:
                     self = self.astype(self.dtype)
                 else:
                     self = self.as_minimum_dtype()
 
-    def _read_with_mask(self, mask, masked, boundless, **kwargs):
+    def _read_with_mask(
+        self, mask: Any, masked: bool, boundless: bool, **kwargs
+    ) -> None:
         kwargs["mask"] = mask
 
         def _read(self, src, mask, **kwargs):
             self._add_meta_from_src(src)
             if self.bounds is None:
                 self._bounds = to_bbox(mask)
 
@@ -1388,7 +1495,86 @@
 
     minx, miny, maxx, maxy = to_bbox(obj)
     diffx = maxx - minx
     diffy = maxy - miny
     width = int(diffx / resx)
     heigth = int(diffy / resy)
     return heigth, width
+
+
+def get_gradient(raster: Raster, degrees: bool = False, copy: bool = False) -> Raster:
+    """Get the slope of an elevation raster.
+
+    Calculates the absolute slope between the grid cells
+    based on the image resolution.
+
+    For multiband images, the calculation is done for each band.
+
+    Args:
+        raster: Raster instance.
+        degrees: If False (default), the returned values will be in ratios,
+            where a value of 1 means 1 meter up per 1 meter forward. If True,
+            the values will be in degrees from 0 to 90.
+        copy: Whether to copy or overwrite the original Raster.
+            Defaults to False to save memory.
+
+    Returns:
+        The class instance with new array values, or a copy if copy is True.
+
+    Examples:
+    --------
+    Making an array where the gradient to the center is always 10.
+
+    >>> import sgis as sg
+    >>> import numpy as np
+    >>> arr = np.array(
+    ...         [
+    ...             [100, 100, 100, 100, 100],
+    ...             [100, 110, 110, 110, 100],
+    ...             [100, 110, 120, 110, 100],
+    ...             [100, 110, 110, 110, 100],
+    ...             [100, 100, 100, 100, 100],
+    ...         ]
+    ...     )
+
+    Now let's create a Raster from this array with a resolution of 10.
+
+    >>> r = sg.Raster.from_array(arr, crs=None, bounds=(0, 0, 50, 50), res=10)
+
+    The gradient will be 1 (1 meter up for every meter forward).
+    The calculation is by default done in place to save memory.
+
+    >>> r.gradient()
+    >>> r.array
+    array([[0., 1., 1., 1., 0.],
+        [1., 1., 1., 1., 1.],
+        [1., 1., 0., 1., 1.],
+        [1., 1., 1., 1., 1.],
+        [0., 1., 1., 1., 0.]])
+    """
+    out_array = []
+    for array in raster:
+        results = _slope_2d(array, raster.res, degrees=degrees)
+        out_array.append(results)
+
+    if len(raster.shape) == 2:
+        out_array = out_array[0]
+    else:
+        out_array = np.array(out_array)
+
+    return raster._return_self_or_copy(out_array, copy)
+
+
+def _slope_2d(array: np.ndarray, res: int, degrees: int) -> np.ndarray:
+    gradient_x, gradient_y = np.gradient(array, res, res)
+
+    gradient = abs(gradient_x) + abs(gradient_y)
+
+    if not degrees:
+        return gradient
+
+    radians = np.arctan(gradient)
+    degrees = np.degrees(radians)
+
+    assert np.max(degrees) <= 90
+
+    return degrees
```

### Comparing `ssb_sgis-1.0.1/src/sgis/raster/torchgeo.py` & `ssb_sgis-1.0.2/src/sgis/raster/torchgeo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,87 @@
 import glob
 import os
 import warnings
-from typing import Iterable
+from collections.abc import Callable
+from collections.abc import Iterable
+from typing import ClassVar
 
 import rasterio
 import rasterio.merge
 from rasterio.io import DatasetReader
 from rasterio.vrt import WarpedVRT
 from torchgeo.datasets.geo import RasterDataset
 from torchgeo.datasets.sentinel import Sentinel2 as TorchgeoSentinel2
 
-
 try:
     import dapla as dp
 except ImportError:
     pass
 
 try:
+    from dapla.gcs import GCSFileSystem
+except ImportError:
+
+    class GCSFileSystem:
+        """Placeholder."""
+
+
+try:
     from gcsfs.core import GCSFile
 except ImportError:
 
     class GCSFile:
-        pass
+        """Placeholder."""
 
 
 from ..io._is_dapla import is_dapla
 from ..io.opener import opener
-from .bands import SENTINEL2_FILENAME_REGEX
+
+SENTINEL2_FILENAME_REGEX = r"""
+    ^SENTINEL2X_
+    (?P<date>\d{8})
+    .*T(?P<tile>\d{2}[A-Z]{3})
+    .*(?:_(?P<resolution>{}m))?
+    .*(?P<band>B\d{1,2}A|B\d{1,2})
+    .*\..*$
+"""
+
+SENTINEL_2_BANDS = [
+    # "B1",
+    "B2",
+    "B3",
+    "B4",
+    "B5",
+    "B6",
+    "B7",
+    "B8",
+    "B8A",
+    # "B9",
+    # "B10",
+    "B11",
+    "B12",
+]
+SENTINEL_2_RBG_BANDS = ["B4", "B3", "B2"]
 
 
 class GCSRasterDataset(RasterDataset):
     """Wrapper around torchgeo's RasterDataset that works in and outside of Dapla (stat norway)."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
+        """Initialiser. Args and kwargs passed to torchgeo.datasets.geo.RasterDataset."""
         super().__init__(*args, **kwargs)
         if is_dapla():
             [file.close() for file in self.files]
 
     @property
     def files(self) -> set[GCSFile] | set[str]:
         """A list of all files in the dataset.
 
         Returns:
             All files in the dataset.
-
-        .. versionadded:: 0.5
         """
         if isinstance(self.paths, str):
             paths: list[str] = [self.paths]
         else:
             paths = self.paths
 
         if is_dapla():
@@ -72,41 +105,44 @@
             elif os.path.isfile(path):
                 files.add(path)
             else:
                 warnings.warn(
                     f"Could not find any relevant files for provided path '{path}'. "
                     f"Path was ignored.",
                     UserWarning,
+                    stacklevel=1,
                 )
 
         return files
 
     def _load_warp_file(self, filepath: str) -> DatasetReader:
         """Load and warp a file to the correct CRS and resolution.
 
         Args:
-            filepath: file to load and warp
+            filepath: file to load and warp.
 
         Returns:
-            file handle of warped VRT
+            file handle of warped VRT.
         """
         with opener(filepath) as f:
             src = rasterio.open(f)
 
             # Only warp if necessary
             if src.crs != self.crs:
                 vrt = WarpedVRT(src, crs=self.crs)
                 src.close()
                 return vrt
             else:
                 return src
 
 
 def _get_gcs_paths(
-    paths: str | Iterable[str], filename_glob: str, file_system=None
+    paths: str | Iterable[str],
+    filename_glob: str,
+    file_system: GCSFileSystem | None = None,
 ) -> set[str]:
     if file_system is None:
         file_system = dp.FileClient.get_gcs_file_system()
 
     # Using set to remove any duplicates if directories are overlapping
     out_paths: set[str] = set()
     for path in paths:
@@ -117,34 +153,19 @@
             }
     return out_paths
 
 
 class Sentinel2(GCSRasterDataset):
     """Works like torchgeo's Sentinel2, with custom regexes."""
 
-    date_format: str = "%Y%m%d"
-    filename_glob = "SENTINEL2X_*_*.*"
-
-    filename_regex = SENTINEL2_FILENAME_REGEX
+    date_format: ClassVar[str] = "%Y%m%d"
+    filename_glob: ClassVar[str] = "SENTINEL2X_*_*.*"
 
-    all_bands = [
-        # "B1",
-        "B2",
-        "B3",
-        "B4",
-        "B5",
-        "B6",
-        "B7",
-        "B8",
-        "B8A",
-        # "B9",
-        # "B10",
-        "B11",
-        "B12",
-    ]
-    rgb_bands = ["B4", "B3", "B2"]
+    filename_regex: ClassVar[str] = SENTINEL2_FILENAME_REGEX
+    all_bands: ClassVar[list[str]] = SENTINEL_2_BANDS
+    rgb_bands: ClassVar[list[str]] = SENTINEL_2_RBG_BANDS
 
-    separate_files = True
+    separate_files: ClassVar[bool] = True
 
-    cmap: dict[int, tuple[int, int, int, int]] = {}
+    cmap: ClassVar[dict[int, tuple[int, int, int, int]]] = {}
 
-    plot = TorchgeoSentinel2.plot
+    plot: Callable = TorchgeoSentinel2.plot
```

### Comparing `ssb_sgis-1.0.1/src/sgis/raster/zonal.py` & `ssb_sgis-1.0.2/src/sgis/raster/zonal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from collections.abc import Callable
+from collections.abc import Sequence
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
+from shapely import Geometry
 from shapely.geometry import Polygon
 
-from ..helpers import get_non_numpy_func_name, get_numpy_func
+from ..helpers import get_non_numpy_func_name
+from ..helpers import get_numpy_func
 
 
-def prepare_zonal(polygons: gpd.GeoDataFrame, aggfunc):
+def _prepare_zonal(
+    polygons: gpd.GeoDataFrame,
+    aggfunc: str | Callable | Sequence[Callable | str],
+) -> tuple[gpd.GeoDataFrame, list[Callable], list[str]]:
     polygons = polygons.reset_index(drop=True)[["geometry"]]
 
     if isinstance(aggfunc, str) or callable(aggfunc):
         aggfunc = [aggfunc]
 
     aggfunc = [f if callable(f) else get_numpy_func(f) for f in aggfunc]
 
     func_names = [get_non_numpy_func_name(f) for f in aggfunc]
 
     return polygons, aggfunc, func_names
 
 
-def make_geometry_iterrows(gdf):
-    """Because pandas iterrows returns non-geo Series"""
+def _make_geometry_iterrows(gdf: gpd.GeoDataFrame) -> list[tuple[int, Geometry]]:
+    """Because pandas iterrows returns non-geo Series."""
     return list(gdf.geometry.items())
 
 
-def zonal_func(
+def _zonal_func(
     poly_iter: tuple[int, Polygon],
     cube,
     array_func: Callable,
-    aggfunc,
-    func_names,
-    by_date,
+    aggfunc: str | Callable | Sequence[Callable | str],
+    func_names: list[str],
+    by_date: bool,
 ) -> pd.DataFrame:
     cube = cube.copy()
     i, polygon = poly_iter
     if not by_date or cube.date.isna().all():
         df = _clip_and_aggregate(
             cube, polygon, array_func, aggfunc, func_names, date=None, i=i
         )
@@ -58,35 +64,50 @@
             cube_date, polygon, array_func, aggfunc, func_names, dt, i
         )
         out.append(df)
 
     return pd.concat(out)
 
 
-def _no_overlap_df(func_names, i, date):
+def _no_overlap_df(func_names: list[str], i: int, date: str) -> pd.DataFrame:
     df = pd.DataFrame(columns=func_names, index=[i])
     df["date"] = date
     df["_no_overlap"] = 1
     return df
 
 
-def _clip_and_aggregate(cube, polygon, array_func, aggfunc, func_names, date, i):
+def _clip_and_aggregate(
+    cube,
+    polygon: Geometry,
+    array_func: Callable,
+    aggfunc: Callable,
+    func_names: list[str],
+    date: str,
+    i: int,
+) -> pd.DataFrame:
     if not len(cube):
         return _no_overlap_df(func_names, i, date)
     clipped = cube.clipmerge(polygon)
     print(list(clipped))
     if not len(clipped) or [arr is None for arr in clipped.arrays]:
         return _no_overlap_df(func_names, i, date)
     assert len(clipped) == 1
     array = clipped[0].array
     df = _aggregate(array, array_func, aggfunc, func_names, date, i)
     return df
 
 
-def _aggregate(array, array_func, aggfunc, func_names, date, i):
+def _aggregate(
+    array: np.ndarray,
+    array_func: Callable,
+    aggfunc: Callable,
+    func_names: list[str],
+    date: str,
+    i: int,
+) -> pd.DataFrame:
     if array_func:
         array = array_func(array)
     # flat_array = array.astype(np.float64).flatten()
     flat_array = array.flatten()
     no_nans = flat_array[~np.isnan(flat_array)]
     data = {}
     for f, name in zip(aggfunc, func_names, strict=True):
@@ -94,16 +115,20 @@
         data[name] = num
     df = pd.DataFrame(data, index=[i])
     df["date"] = date
     df["_no_overlap"] = 0
     return df
 
 
-def zonal_post(
-    aggregated: list[pd.DataFrame], polygons, idx_mapper, idx_name, dropna
+def _zonal_post(
+    aggregated: list[pd.DataFrame],
+    polygons: gpd.GeoDataFrame,
+    idx_mapper: dict | pd.Series,
+    idx_name: str,
+    dropna: bool,
 ) -> pd.DataFrame:
     out = gpd.GeoDataFrame(
         pd.concat(aggregated), geometry=polygons.geometry.values, crs=polygons.crs
     ).sort_index()
 
     out.index = out.index.map(idx_mapper)
     out.index.name = idx_name
```

### Comparing `ssb_sgis-1.0.1/PKG-INFO` & `ssb_sgis-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,123 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 1.0.1
+Version: 1.0.2
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
-Author: Statistics Norway
-Author-email: ort@ssb.no
+Author: Morten Letnes
+Author-email: morten.letnes@ssb.no
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
+Provides-Extra: all
+Provides-Extra: bucket
+Provides-Extra: test
+Provides-Extra: torch
+Provides-Extra: xarray
+Requires-Dist: affine (>=2.4.0)
 Requires-Dist: branca (>=0.6.0)
+Requires-Dist: dapla-toolbelt (>=2.0.12) ; extra == "all" or extra == "bucket"
 Requires-Dist: dask (>=2024.1.1)
+Requires-Dist: dask-geopandas (>=0.3.0)
 Requires-Dist: folium (>=0.14.0)
+Requires-Dist: gcsfs (>=2024.3.1) ; extra == "all" or extra == "bucket"
 Requires-Dist: geocoder (>=1.38.1)
 Requires-Dist: geopandas (>=0.14.0)
 Requires-Dist: igraph (>=0.11.2)
 Requires-Dist: ipython (>=8.13.2)
 Requires-Dist: jenkspy (>=0.3.2)
+Requires-Dist: jinja2 (>=3.1.3)
+Requires-Dist: joblib (>=1.4.0)
 Requires-Dist: mapclassify (>=2.5.0)
 Requires-Dist: matplotlib (>=3.7.0)
 Requires-Dist: networkx (>=3.0)
 Requires-Dist: numpy (>=1.24.2)
-Requires-Dist: pandas (>=2.0.3)
-Requires-Dist: pip (>=23.2.1)
+Requires-Dist: pandas (>=2.2.1)
 Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: pyproj (>=3.6.1)
 Requires-Dist: rasterio (>=1.3.8)
 Requires-Dist: requests (>=2.28.2)
+Requires-Dist: rioxarray (>=0.15.5) ; extra == "all" or extra == "xarray" or extra == "test"
 Requires-Dist: rtree (>=1.0.1)
 Requires-Dist: scikit-learn (>=1.2.1)
 Requires-Dist: shapely (>=2.0.1)
+Requires-Dist: torch (==2.2.2) ; extra == "all" or extra == "torch" or extra == "test"
+Requires-Dist: torchgeo (>=0.5.2) ; extra == "all" or extra == "torch" or extra == "test"
+Requires-Dist: typing-extensions (>=4.11.0)
+Requires-Dist: xarray (>=2024.3.0) ; extra == "all" or extra == "xarray" or extra == "test"
 Requires-Dist: xyzservices (>=2023.2.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-sgis/releases
+Project-URL: Documentation, https://statisticsnorway.github.io/ssb-sgis
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-sgis
 Description-Content-Type: text/markdown
 
 # ssb-sgis
 
 GIS Python tools used in [Statistics Norway](https://www.ssb.no/en).
 
 See documentation [here](https://statisticsnorway.github.io/ssb-sgis/reference/index.html).
 
-[![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
+[![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][pypi status]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
-[![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
-[![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
+[![Documentation](https://github.com/statisticsnorway/ssb-sgis/actions/workflows/docs.yml/badge.svg)][documentation]
+[![Tests](https://github.com/statisticsnorway/ssb-sgis/actions/workflows/tests.yml/badge.svg)][tests]
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=coverage)][sonarcov]
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=alert_status)][sonarquality]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
-[pypi_]: https://pypi.org/project/ssb-sgis/
-[status]: https://pypi.org/project/ssb-sgis/
-[python version]: https://pypi.org/project/ssb-sgis
-[read the docs]: https://ssb-sgis.readthedocs.io/
+[pypi status]: https://pypi.org/project/ssb-sgis/
+[documentation]: https://statisticsnorway.github.io/ssb-sgis
 [tests]: https://github.com/statisticsnorway/ssb-sgis/actions?workflow=Tests
-[coverage]: https://sonarcloud.io/component_measures?metric=coverage&id=statisticsnorway_ssb-sgis
+[sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-sgis
+[sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-sgis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
+[poetry]: https://python-poetry.org/
 
 sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
 To install, use one of:
 
 ```shell
 poetry add ssb-sgis
 pip install ssb-sgis
 ```
 
+The sgis package has the following optional dependencies:
+
+- bucket: For working with files stored in GCP buckets
+- torch: Use functionality from PyTorch and torchgeo
+- xarray: Use functionality from xarray and rioxarray
+- test: Packages needed for running pytest
+- all: All optional dependencies
+
+The optional dependencies can be installed by adding them in
+brackets when installing, like this:
+
+```shell
+poetry add ssb-sgis[all]
+pip install ssb-sgis[all]
+```
+
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
 
@@ -201,15 +238,15 @@
 
 ### Dependencies
 
 [Poetry](https://python-poetry.org/) is used for dependency management. Install
 poetry and run the command below from the root directory to install the dependencies.
 
 ```shell
-poetry install --no-root
+poetry install -E test --no-root
 ```
 
 ### Tests
 
 Use the following command from the root directory to run the tests:
 
 ```shell
@@ -228,14 +265,22 @@
 poetry run jupter lab
 ```
 
 For VS Code there are extensions for opening a python script as Jupyter Notebook,
 for example:
 [Jupytext for Notebooks](https://marketplace.visualstudio.com/items?itemName=donjayamanne.vscode-jupytext).
 
+### Code quality
+
+Run 'ruff' on all files with safe fixes:
+
+```shell
+poetry run ruff check --fix .
+```
+
 ### Formatting
 
 Format the code with `black` and `isort` by running the following command from the
 root directory:
 
 ```shell
 poetry run black .
@@ -272,12 +317,38 @@
 
 To check and run the docstrings examples, run this command:
 
 ```shell
 poetry run xdoctest --command=all ./src/sgis
 ```
 
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_SSB sgis_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [Statistics Norway]'s [SSB PyPI Template].
+
+[statistics norway]: https://www.ssb.no/en
+[pypi]: https://pypi.org/
+[ssb pypi template]: https://github.com/statisticsnorway/ssb-pypitemplate
+[file an issue]: https://github.com/statisticsnorway/ssb-sgis/issues
+[pip]: https://pip.pypa.io/
+
 <!-- github-only -->
 
 [license]: https://github.com/statisticsnorway/ssb-sgis/blob/main/LICENSE
 [contributor guide]: https://github.com/statisticsnorway/ssb-sgis/blob/main/CONTRIBUTING.md
+[reference guide]: https://statisticsnorway.github.io/ssb-sgis/reference.html
```


# Comparing `tmp/lonboard-0.9.1.tar.gz` & `tmp/lonboard-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lonboard-0.9.1.tar", max compression
+gzip compressed data, was "lonboard-0.9.2.tar", max compression
```

## Comparing `lonboard-0.9.1.tar` & `lonboard-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1073 2024-05-07 19:06:06.930557 lonboard-0.9.1/LICENSE
--rw-r--r--   0        0        0       36 2024-05-07 19:06:06.930557 lonboard-0.9.1/MANIFEST.in
--rw-r--r--   0        0        0     3074 2024-05-07 19:06:06.930557 lonboard-0.9.1/README.md
--rw-r--r--   0        0        0      445 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/__init__.py
--rw-r--r--   0        0        0       39 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/__main__.py
--rw-r--r--   0        0        0     1418 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_base.py
--rw-r--r--   0        0        0     4645 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_cli.py
--rw-r--r--   0        0        0      862 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_constants.py
--rw-r--r--   0        0        0     1421 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_environment.py
--rw-r--r--   0        0        0       95 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/__init__.py
--rw-r--r--   0        0        0     8042 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/_duckdb.py
--rw-r--r--   0        0        0      509 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/crs.py
--rw-r--r--   0        0        0    13399 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/extension_types.py
--rw-r--r--   0        0        0      716 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/geopandas_interop.py
--rw-r--r--   0        0        0      174 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/__init__.py
--rw-r--r--   0        0        0     2619 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/bbox.py
--rw-r--r--   0        0        0     4584 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/centroid.py
--rw-r--r--   0        0        0     3170 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/coord_layout.py
--rw-r--r--   0        0        0     8208 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/reproject.py
--rw-r--r--   0        0        0     4725 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/parse_wkb.py
--rw-r--r--   0        0        0     1801 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_geoarrow/sanitize.py
--rw-r--r--   0        0        0    60118 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_layer.py
--rw-r--r--   0        0        0    13878 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_map.py
--rw-r--r--   0        0        0     3578 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_serialization.py
--rw-r--r--   0        0        0      285 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_testing.py
--rw-r--r--   0        0        0     5293 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_utils.py
--rw-r--r--   0        0        0      166 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_version.py
--rw-r--r--   0        0        0     2380 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_viewport.py
--rw-r--r--   0        0        0    20582 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_viz.py
--rw-r--r--   0        0        0     1367 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/basemap.py
--rw-r--r--   0        0        0     6914 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/colormap.py
--rw-r--r--   0        0        0     2758 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/controls.py
--rw-r--r--   0        0        0      207 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/experimental/__init__.py
--rw-r--r--   0        0        0     9728 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/experimental/_layer.py
--rw-r--r--   0        0        0    14555 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/layer_extension.py
--rw-r--r--   0        0        0      357 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/models.py
--rw-r--r--   0        0        0        0 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/py.typed
--rw-r--r--   0        0        0      385 2024-05-07 19:06:16.526643 lonboard-0.9.1/lonboard/static/index.css
--rw-r--r--   0        0        0  2155294 2024-05-07 19:06:16.526643 lonboard-0.9.1/lonboard/static/index.js
--rw-r--r--   0        0        0    37110 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/traits.py
--rw-r--r--   0        0        0        0 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/__init__.py
--rw-r--r--   0        0        0     4535 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/layer.py
--rw-r--r--   0        0        0      466 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/map.py
--rw-r--r--   0        0        0     2211 2024-05-07 19:06:07.138558 lonboard-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 lonboard-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-14 15:44:43.382092 lonboard-0.9.2/LICENSE
+-rw-r--r--   0        0        0       36 2024-05-14 15:44:43.382092 lonboard-0.9.2/MANIFEST.in
+-rw-r--r--   0        0        0     3074 2024-05-14 15:44:43.382092 lonboard-0.9.2/README.md
+-rw-r--r--   0        0        0      445 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/__main__.py
+-rw-r--r--   0        0        0     1418 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_base.py
+-rw-r--r--   0        0        0     4645 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_cli.py
+-rw-r--r--   0        0        0      862 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_constants.py
+-rw-r--r--   0        0        0     1421 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_environment.py
+-rw-r--r--   0        0        0       95 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_geoarrow/__init__.py
+-rw-r--r--   0        0        0     8040 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_geoarrow/_duckdb.py
+-rw-r--r--   0        0        0      509 2024-05-14 15:44:43.586094 lonboard-0.9.2/lonboard/_geoarrow/crs.py
+-rw-r--r--   0        0        0    13405 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/extension_types.py
+-rw-r--r--   0        0        0      716 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/geopandas_interop.py
+-rw-r--r--   0        0        0      174 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/ops/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/ops/bbox.py
+-rw-r--r--   0        0        0     4584 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/ops/centroid.py
+-rw-r--r--   0        0        0     3166 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/ops/coord_layout.py
+-rw-r--r--   0        0        0     8192 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/ops/reproject.py
+-rw-r--r--   0        0        0     4666 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/parse_wkb.py
+-rw-r--r--   0        0        0     1801 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_geoarrow/sanitize.py
+-rw-r--r--   0        0        0    60118 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_layer.py
+-rw-r--r--   0        0        0    14360 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_map.py
+-rw-r--r--   0        0        0     3578 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_serialization.py
+-rw-r--r--   0        0        0      285 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_testing.py
+-rw-r--r--   0        0        0     5581 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_utils.py
+-rw-r--r--   0        0        0      166 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_version.py
+-rw-r--r--   0        0        0     2380 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_viewport.py
+-rw-r--r--   0        0        0    20582 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/_viz.py
+-rw-r--r--   0        0        0     1367 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/basemap.py
+-rw-r--r--   0        0        0     6914 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/colormap.py
+-rw-r--r--   0        0        0     2758 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/controls.py
+-rw-r--r--   0        0        0      207 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/experimental/__init__.py
+-rw-r--r--   0        0        0     9728 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/experimental/_layer.py
+-rw-r--r--   0        0        0    14555 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/layer_extension.py
+-rw-r--r--   0        0        0      357 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/models.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/py.typed
+-rw-r--r--   0        0        0      385 2024-05-14 15:44:53.274151 lonboard-0.9.2/lonboard/static/index.css
+-rw-r--r--   0        0        0  2155294 2024-05-14 15:44:53.274151 lonboard-0.9.2/lonboard/static/index.js
+-rw-r--r--   0        0        0    37100 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/traits.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/types/__init__.py
+-rw-r--r--   0        0        0     4535 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/types/layer.py
+-rw-r--r--   0        0        0      466 2024-05-14 15:44:43.590094 lonboard-0.9.2/lonboard/types/map.py
+-rw-r--r--   0        0        0     2818 2024-05-14 15:44:43.590094 lonboard-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 lonboard-0.9.2/PKG-INFO
```

### Comparing `lonboard-0.9.1/LICENSE` & `lonboard-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/README.md` & `lonboard-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_base.py` & `lonboard-0.9.2/lonboard/_base.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_cli.py` & `lonboard-0.9.2/lonboard/_cli.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_constants.py` & `lonboard-0.9.2/lonboard/_constants.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_environment.py` & `lonboard-0.9.2/lonboard/_environment.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/_duckdb.py` & `lonboard-0.9.2/lonboard/_geoarrow/_duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     # Create the geoarrow Polygon offset arrays
     # Each ring has 5 coordinates
     ring_offsets = np.arange(0, (len(geom_col) + 1) * 5, 5, dtype=np.int32)
     # Each geometry has a single ring
     geom_offsets = np.arange(0, len(ring_offsets), dtype=np.int32)
 
     # Construct the final PolygonArray
-    coords = pa.FixedSizeListArray.from_arrays(coords.flatten("C"), 2)
+    coords = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), 2)
     ring_array = pa.ListArray.from_arrays(ring_offsets, coords)
     polygon_array = pa.ListArray.from_arrays(geom_offsets, ring_array)
     return polygon_array
 
 
 # TODO: refactor, put helper in lonboard._geoarrow.crs?
 def _make_geoarrow_field_metadata(
```

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/extension_types.py` & `lonboard-0.9.2/lonboard/_geoarrow/extension_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -301,86 +301,86 @@
         raise ValueError(f"Unexpected coords dimensions: {coords.shape}")
 
     extension_metadata: Dict[str, str] = {}
     if crs_str is not None:
         extension_metadata["ARROW:extension:metadata"] = json.dumps({"crs": crs_str})
 
     if geom_type == GeometryType.POINT:
-        parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         extension_metadata["ARROW:extension:name"] = "geoarrow.point"
         field = pa.field(
             field_name,
             parr.type,
             nullable=True,
             metadata=extension_metadata,
         )
         return field, parr
 
     elif geom_type == GeometryType.LINESTRING:
         assert len(offsets) == 1, "Expected one offsets array"
         (geom_offsets,) = offsets
-        _parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        _parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         parr = pa.ListArray.from_arrays(pa.array(geom_offsets), _parr)
         extension_metadata["ARROW:extension:name"] = "geoarrow.linestring"
         field = pa.field(
             field_name,
             parr.type,
             nullable=True,
             metadata=extension_metadata,
         )
         return field, parr
 
     elif geom_type == GeometryType.POLYGON:
         assert len(offsets) == 2, "Expected two offsets arrays"
         ring_offsets, geom_offsets = offsets
-        _parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        _parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         _parr1 = pa.ListArray.from_arrays(pa.array(ring_offsets), _parr)
         parr = pa.ListArray.from_arrays(pa.array(geom_offsets), _parr1)
         extension_metadata["ARROW:extension:name"] = "geoarrow.polygon"
         field = pa.field(
             field_name,
             parr.type,
             nullable=True,
             metadata=extension_metadata,
         )
         return field, parr
 
     elif geom_type == GeometryType.MULTIPOINT:
         assert len(offsets) == 1, "Expected one offsets array"
         (geom_offsets,) = offsets
-        _parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        _parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         parr = pa.ListArray.from_arrays(pa.array(geom_offsets), _parr)
         extension_metadata["ARROW:extension:name"] = "geoarrow.multipoint"
         field = pa.field(
             field_name,
             parr.type,
             nullable=True,
             metadata=extension_metadata,
         )
         return field, parr
 
     elif geom_type == GeometryType.MULTILINESTRING:
         assert len(offsets) == 2, "Expected two offsets arrays"
         ring_offsets, geom_offsets = offsets
-        _parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        _parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         _parr1 = pa.ListArray.from_arrays(pa.array(ring_offsets), _parr)
         parr = pa.ListArray.from_arrays(pa.array(geom_offsets), _parr1)
         extension_metadata["ARROW:extension:name"] = "geoarrow.multilinestring"
         field = pa.field(
             field_name,
             parr.type,
             nullable=True,
             metadata=extension_metadata,
         )
         return field, parr
 
     elif geom_type == GeometryType.MULTIPOLYGON:
         assert len(offsets) == 3, "Expected three offsets arrays"
         ring_offsets, polygon_offsets, geom_offsets = offsets
-        _parr = pa.FixedSizeListArray.from_arrays(coords.flatten(), len(dims))
+        _parr = pa.FixedSizeListArray.from_arrays(coords.ravel("C"), len(dims))
         _parr1 = pa.ListArray.from_arrays(pa.array(ring_offsets), _parr)
         _parr2 = pa.ListArray.from_arrays(pa.array(polygon_offsets), _parr1)
         parr = pa.ListArray.from_arrays(pa.array(geom_offsets), _parr2)
         extension_metadata["ARROW:extension:name"] = "geoarrow.multipolygon"
         field = pa.field(
             field_name,
             parr.type,
```

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/geopandas_interop.py` & `lonboard-0.9.2/lonboard/_geoarrow/geopandas_interop.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/ops/bbox.py` & `lonboard-0.9.2/lonboard/_geoarrow/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/ops/centroid.py` & `lonboard-0.9.2/lonboard/_geoarrow/ops/centroid.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/ops/coord_layout.py` & `lonboard-0.9.2/lonboard/_geoarrow/ops/coord_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,22 +71,22 @@
 def _transpose_coords(arr: Union[pa.FixedSizeListArray, pa.StructArray]):
     if isinstance(arr, pa.FixedSizeListArray):
         return arr
 
     if arr.type.num_fields == 2:
         x = arr.field("x").to_numpy()
         y = arr.field("y").to_numpy()
-        coords = np.column_stack([x, y]).flatten("C")
+        coords = np.column_stack([x, y]).ravel("C")
         return pa.FixedSizeListArray.from_arrays(coords, 2)
 
     if arr.type.num_fields == 3:
         x = arr.field("x").to_numpy()
         y = arr.field("y").to_numpy()
         z = arr.field("z").to_numpy()
-        coords = np.column_stack([x, y, z]).flatten("C")
+        coords = np.column_stack([x, y, z]).ravel("C")
         return pa.FixedSizeListArray.from_arrays(coords, 3)
 
     raise ValueError(f"Expected struct with 2 or 3 fields, got {arr.type.num_fields}")
 
 
 def _transpose_chunk_nest_0(arr: pa.ListArray):
     return _map_coords_nest_0(arr, _transpose_coords)
```

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/ops/reproject.py` & `lonboard-0.9.2/lonboard/_geoarrow/ops/reproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,15 @@
             transformer.transform(np_arr[:, 0], np_arr[:, 1], np_arr[:, 2])
         )
         dims = CoordinateDimension.XYZ
     else:
         raise ValueError(f"Unexpected list size {list_size}")
 
     coord_field = pa.list_(pa.field(dims, pa.float64()), len(dims))
-    return pa.FixedSizeListArray.from_arrays(
-        output_np_arr.flatten("C"), type=coord_field
-    )
+    return pa.FixedSizeListArray.from_arrays(output_np_arr.ravel("C"), type=coord_field)
 
 
 def _reproject_chunk_nest_0(arr: pa.ListArray, transformer: Transformer):
     callback = partial(_reproject_coords, transformer=transformer)
     return _map_coords_nest_0(arr, callback)
```

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/parse_wkb.py` & `lonboard-0.9.2/lonboard/_geoarrow/parse_wkb.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     extension_type_name = field.metadata.get(b"ARROW:extension:name")
 
     # For native GeoArrow input, return table as-is
     if extension_type_name not in {EXTENSION_NAME.WKB, EXTENSION_NAME.OGC_WKB}:
         return [table]
 
     # Handle WKB input
-    parsed_tables = []
     crs_str = get_field_crs(field)
     shapely_arr = shapely.from_wkb(column)
 
     type_ids = np.array(shapely.get_type_id(shapely_arr))
     unique_type_ids = set(np.unique(type_ids))
 
     if GeometryType.GEOMETRYCOLLECTION in unique_type_ids:
@@ -63,43 +62,37 @@
         | (type_ids == GeometryType.MULTILINESTRING)
     )[0]
 
     polygon_indices = np.where(
         (type_ids == GeometryType.POLYGON) | (type_ids == GeometryType.MULTIPOLYGON)
     )[0]
 
-    if len(point_indices) > 0:
-        point_field, point_arr = construct_geometry_array(
-            shapely_arr[point_indices],
-            crs_str=crs_str,
-        )
-        point_table = table.take(point_indices).set_column(
-            field_idx, point_field, point_arr
-        )
-        parsed_tables.append(point_table)
-
-    if len(linestring_indices) > 0:
-        linestring_field, linestring_arr = construct_geometry_array(
-            shapely_arr[linestring_indices],
-            crs_str=crs_str,
-        )
-        linestring_table = table.take(linestring_indices).set_column(
-            field_idx, linestring_field, linestring_arr
-        )
-        parsed_tables.append(linestring_table)
-
-    if len(polygon_indices) > 0:
-        polygon_field, polygon_arr = construct_geometry_array(
-            shapely_arr[polygon_indices],
-            crs_str=crs_str,
-        )
-        polygon_table = table.take(polygon_indices).set_column(
-            field_idx, polygon_field, polygon_arr
-        )
-        parsed_tables.append(polygon_table)
+    # Here we intentionally check geometries in a specific order.
+    # Starting from polygons, then linestrings, then points,
+    # so that the order of generated layers is polygon, then path then scatterplot.
+    # This ensures that points are rendered on top and polygons on the bottom.
+    parsed_tables = []
+    for single_type_geometry_indices in (
+        polygon_indices,
+        linestring_indices,
+        point_indices,
+    ):
+        if len(single_type_geometry_indices) > 0:
+            single_type_geometry_field, single_type_geometry_arr = (
+                construct_geometry_array(
+                    shapely_arr[single_type_geometry_indices],
+                    crs_str=crs_str,
+                )
+            )
+            single_type_geometry_table = table.take(
+                single_type_geometry_indices
+            ).set_column(
+                field_idx, single_type_geometry_field, single_type_geometry_arr
+            )
+            parsed_tables.append(single_type_geometry_table)
 
     return parsed_tables
 
 
 def parse_geoparquet_table(table: pa.Table) -> pa.Table:
     """Parse GeoParquet table metadata, assigning it to GeoArrow metadata"""
     # If a column already has geoarrow metadata, don't parse from GeoParquet metadata
```

### Comparing `lonboard-0.9.1/lonboard/_geoarrow/sanitize.py` & `lonboard-0.9.2/lonboard/_geoarrow/sanitize.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_layer.py` & `lonboard-0.9.2/lonboard/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_map.py` & `lonboard-0.9.2/lonboard/_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         self.view_state = view_state
 
     def fly_to(
         self,
         *,
         longitude: Union[int, float],
         latitude: Union[int, float],
-        zoom: float,
+        zoom: Union[int, float],
         duration: int = 4000,
         pitch: Union[int, float] = 0,
         bearing: Union[int, float] = 0,
         curve: Optional[Union[int, float]] = None,
         speed: Optional[Union[int, float]] = None,
         screen_speed: Optional[Union[int, float]] = None,
     ):
@@ -335,14 +335,27 @@
             speed: The average speed of the animation defined in relation to
                 `curve`, it linearly affects the duration, higher speed returns smaller
                 durations and vice versa. Default `1.2`.
             screen_speed: The average speed of the animation measured in screenfuls per
                 second. Similar to speed it linearly affects the duration, when
                 specified speed is ignored.
         """
+        if not isinstance(longitude, (int, float)):
+            raise TypeError(
+                f"Expected longitude to be an int or float, got {type(longitude)}"
+            )
+
+        if not isinstance(latitude, (int, float)):
+            raise TypeError(
+                f"Expected latitude to be an int or float, got {type(latitude)}"
+            )
+
+        if not isinstance(zoom, (int, float)):
+            raise TypeError(f"Expected zoom to be an int or float, got {type(zoom)}")
+
         data = {
             "type": "fly-to",
             "longitude": longitude,
             "latitude": latitude,
             "zoom": zoom,
             "pitch": pitch,
             "bearing": bearing,
@@ -402,15 +415,15 @@
             inner(filename)
 
     def as_html(self) -> HTML:
         """Render the current map as a static HTML file in IPython.
 
         !!! warning
 
-            The primary, recommended way to display a map is by "displaying" it by
+            The primary, recommended way to display a map is by
             leaving it as the last line in a cell.
 
             ```py
             from lonboard import Map
 
             m = Map(layers=[])
             m
```

### Comparing `lonboard-0.9.1/lonboard/_serialization.py` & `lonboard-0.9.2/lonboard/_serialization.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_utils.py` & `lonboard-0.9.2/lonboard/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,28 +136,34 @@
 
         if unique_type_ids == {GeometryType.LINESTRING, GeometryType.MULTILINESTRING}:
             return [gdf]
 
         if unique_type_ids == {GeometryType.POLYGON, GeometryType.MULTIPOLYGON}:
             return [gdf]
 
-    gdfs = []
     point_indices = np.where(
         (type_ids == GeometryType.POINT) | (type_ids == GeometryType.MULTIPOINT)
     )[0]
-    if len(point_indices) > 0:
-        gdfs.append(gdf.iloc[point_indices])
 
     linestring_indices = np.where(
         (type_ids == GeometryType.LINESTRING)
         | (type_ids == GeometryType.MULTILINESTRING)
     )[0]
-    if len(linestring_indices) > 0:
-        gdfs.append(gdf.iloc[linestring_indices])
 
     polygon_indices = np.where(
         (type_ids == GeometryType.POLYGON) | (type_ids == GeometryType.MULTIPOLYGON)
     )[0]
-    if len(polygon_indices) > 0:
-        gdfs.append(gdf.iloc[polygon_indices])
+
+    # Here we intentionally check geometries in a specific order.
+    # Starting from polygons, then linestrings, then points,
+    # so that the order of generated layers is polygon, then path then scatterplot.
+    # This ensures that points are rendered on top and polygons on the bottom.
+    gdfs = []
+    for single_type_geometry_indices in (
+        polygon_indices,
+        linestring_indices,
+        point_indices,
+    ):
+        if len(single_type_geometry_indices) > 0:
+            gdfs.append(gdf.iloc[single_type_geometry_indices])
 
     return gdfs
```

### Comparing `lonboard-0.9.1/lonboard/_viewport.py` & `lonboard-0.9.2/lonboard/_viewport.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/_viz.py` & `lonboard-0.9.2/lonboard/_viz.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/basemap.py` & `lonboard-0.9.2/lonboard/basemap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/colormap.py` & `lonboard-0.9.2/lonboard/colormap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/controls.py` & `lonboard-0.9.2/lonboard/controls.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/experimental/_layer.py` & `lonboard-0.9.2/lonboard/experimental/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/layer_extension.py` & `lonboard-0.9.2/lonboard/layer_extension.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/static/index.js` & `lonboard-0.9.2/lonboard/static/index.js`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/lonboard/traits.py` & `lonboard-0.9.2/lonboard/traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
             if list_size not in (3, 4):
                 self.error(
                     obj,
                     value,
                     info="Color array must have 3 or 4 as its second dimension.",
                 )
 
-            return pa.FixedSizeListArray.from_arrays(value.flatten("C"), list_size)
+            return pa.FixedSizeListArray.from_arrays(value.ravel("C"), list_size)
 
         # Check for Arrow PyCapsule Interface
         # https://arrow.apache.org/docs/format/CDataInterface/PyCapsuleInterface.html
         # TODO: with pyarrow v16 also import chunked array from stream
         if not isinstance(value, (pa.ChunkedArray, pa.Array)):
             if hasattr(value, "__arrow_c_array__"):
                 value = pa.array(value)
@@ -498,15 +498,15 @@
             if list_size not in (2, 3):
                 self.error(
                     obj,
                     value,
                     info="Point array to have 2 or 3 as its second dimension",
                 )
 
-            return pa.FixedSizeListArray.from_arrays(value.flatten("C"), list_size)
+            return pa.FixedSizeListArray.from_arrays(value.ravel("C"), list_size)
 
         if isinstance(value, (pa.ChunkedArray, pa.Array)):
             if not pa.types.is_fixed_size_list(value.type):
                 self.error(obj, value, info="Point pyarrow array to be a FixedSizeList")
 
             if value.type.list_size not in (2, 3):
                 self.error(
@@ -677,15 +677,15 @@
                     value,
                     info=(
                         f"filter_size ({filter_size}) to match 2nd dimension of "
                         "numpy array"
                     ),
                 )
 
-            return pa.FixedSizeListArray.from_arrays(value.flatten("C"), filter_size)
+            return pa.FixedSizeListArray.from_arrays(value.ravel("C"), filter_size)
 
         # Check for Arrow PyCapsule Interface
         # https://arrow.apache.org/docs/format/CDataInterface/PyCapsuleInterface.html
         # TODO: with pyarrow v16 also import chunked array from stream
         if not isinstance(value, (pa.ChunkedArray, pa.Array)):
             if hasattr(value, "__arrow_c_array__"):
                 value = pa.array(value)
@@ -796,15 +796,15 @@
             if not np.issubdtype(value.dtype, np.float32):
                 warnings.warn(
                     """Warning: Numpy array should be float32 type.
                     Converting to float32 point pyarrow array"""
                 )
                 value = value.astype(np.float32)
 
-            return pa.FixedSizeListArray.from_arrays(value.flatten("C"), 3)
+            return pa.FixedSizeListArray.from_arrays(value.ravel("C"), 3)
 
         # Check for Arrow PyCapsule Interface
         # https://arrow.apache.org/docs/format/CDataInterface/PyCapsuleInterface.html
         # TODO: with pyarrow v16 also import chunked array from stream
         if not isinstance(value, (pa.ChunkedArray, pa.Array)):
             if hasattr(value, "__arrow_c_array__"):
                 value = pa.array(value)
@@ -928,15 +928,15 @@
                     info="NumPy array must have 2 as its second dimension.",
                 )
 
             # Cast float64 to float32; leave other data types the same
             if np.issubdtype(value.dtype, np.float64):
                 value = value.astype(np.float32)
 
-            return pa.FixedSizeListArray.from_arrays(value.flatten("C"), list_size)
+            return pa.FixedSizeListArray.from_arrays(value.ravel("C"), list_size)
 
         # Check for Arrow PyCapsule Interface
         # https://arrow.apache.org/docs/format/CDataInterface/PyCapsuleInterface.html
         # TODO: with pyarrow v16 also import chunked array from stream
         if not isinstance(value, (pa.ChunkedArray, pa.Array)):
             if hasattr(value, "__arrow_c_array__"):
                 value = pa.array(value)
```

### Comparing `lonboard-0.9.1/lonboard/types/layer.py` & `lonboard-0.9.2/lonboard/types/layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.1/pyproject.toml` & `lonboard-0.9.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 [tool.poetry]
 name = "lonboard"
-version = "0.9.1"
-description = "Python library for fast, interactive geospatial vector data visualization in Jupyter."
+version = "0.9.2"
+description = "Fast, interactive geospatial data visualization in Jupyter."
 authors = ["Kyle Barron <kyle@developmentseed.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lonboard" }]
 include = ["lonboard/static/*.js", "lonboard/static/*.css", "MANIFEST.in"]
+repository = "https://github.com/developmentseed/lonboard"
+documentation = "https://developmentseed.org/lonboard/latest/"
+keywords = [
+    "GIS",
+    "cartography",
+    "visualization",
+    "geopandas",
+    "pandas",
+    "shapely",
+]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Framework :: Jupyter",
+    "Framework :: Jupyter :: JupyterLab",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: GIS",
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 anywidget = "^0.9.0"
 pyarrow = ">=14.0.1"
 geopandas = ">=0.13"
 pandas = "^2"
```

### Comparing `lonboard-0.9.1/PKG-INFO` & `lonboard-0.9.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: lonboard
-Version: 0.9.1
-Summary: Python library for fast, interactive geospatial vector data visualization in Jupyter.
+Version: 0.9.2
+Summary: Fast, interactive geospatial data visualization in Jupyter.
+Home-page: https://github.com/developmentseed/lonboard
 License: MIT
+Keywords: GIS,cartography,visualization,geopandas,pandas,shapely
 Author: Kyle Barron
 Author-email: kyle@developmentseed.org
 Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: GIS
 Provides-Extra: cli
 Requires-Dist: anywidget (>=0.9.0,<0.10.0)
 Requires-Dist: click (>=8.1.7,<9.0.0) ; extra == "cli"
 Requires-Dist: geopandas (>=0.13)
 Requires-Dist: matplotlib (>=3.7,<4.0)
 Requires-Dist: palettable (>=3.3.3,<4.0.0)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: pyarrow (>=14.0.1)
 Requires-Dist: pyogrio (>=0.7.2,<0.8.0) ; extra == "cli"
 Requires-Dist: shapely (>=2,<3)
 Requires-Dist: typing-extensions (>=4.6.0,<5.0.0) ; python_version < "3.12"
+Project-URL: Documentation, https://developmentseed.org/lonboard/latest/
+Project-URL: Repository, https://github.com/developmentseed/lonboard
 Description-Content-Type: text/markdown
 
 # Lonboard
 
 [![PyPI][pypi_badge]][pypi_link]
 [![Conda Version][conda_version_badge]][conda_version]
 [![Binder][binder_badge]][binder_jupyterlab_url]
```

#### html2text {}

```diff
@@ -1,21 +1,29 @@
-Metadata-Version: 2.1 Name: lonboard Version: 0.9.1 Summary: Python library for
-fast, interactive geospatial vector data visualization in Jupyter. License: MIT
-Author: Kyle Barron Author-email: kyle@developmentseed.org Requires-Python:
->=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
-Extra: cli Requires-Dist: anywidget (>=0.9.0,<0.10.0) Requires-Dist: click
+Metadata-Version: 2.1 Name: lonboard Version: 0.9.2 Summary: Fast, interactive
+geospatial data visualization in Jupyter. Home-page: https://github.com/
+developmentseed/lonboard License: MIT Keywords:
+GIS,cartography,visualization,geopandas,pandas,shapely Author: Kyle Barron
+Author-email: kyle@developmentseed.org Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 4 - Beta Classifier: Framework :: Jupyter Classifier:
+Framework :: Jupyter :: JupyterLab Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Scientific/Engineering :: GIS Provides-Extra: cli
+Requires-Dist: anywidget (>=0.9.0,<0.10.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) ; extra == "cli" Requires-Dist: geopandas (>=0.13) Requires-
 Dist: matplotlib (>=3.7,<4.0) Requires-Dist: palettable (>=3.3.3,<4.0.0)
 Requires-Dist: pandas (>=2,<3) Requires-Dist: pyarrow (>=14.0.1) Requires-Dist:
 pyogrio (>=0.7.2,<0.8.0) ; extra == "cli" Requires-Dist: shapely (>=2,<3)
 Requires-Dist: typing-extensions (>=4.6.0,<5.0.0) ; python_version < "3.12"
+Project-URL: Documentation, https://developmentseed.org/lonboard/latest/
+Project-URL: Repository, https://github.com/developmentseed/lonboard
 Description-Content-Type: text/markdown # Lonboard [![PyPI][pypi_badge]]
 [pypi_link] [![Conda Version][conda_version_badge]][conda_version] [![Binder]
 [binder_badge]][binder_jupyterlab_url] [![open_in_colab][colab_badge]]
 [colab_notebook_link] [pypi_badge]: https://badge.fury.io/py/lonboard.svg
 [pypi_link]: https://pypi.org/project/lonboard/ [binder_badge]: https://
 mybinder.org/badge_logo.svg [binder_jupyterlab_url]: https://mybinder.org/v2/
 gh/developmentseed/lonboard/HEAD?urlpath=lab/tree/examples/ [colab_badge]:
```


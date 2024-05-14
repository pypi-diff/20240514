# Comparing `tmp/searvey-0.3.8-py3-none-any.whl.zip` & `tmp/searvey-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 44097 bytes, number of entries: 18
--rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 searvey/__init__.py
--rw-r--r--  2.0 unx    35931 b- defN 80-Jan-01 00:00 searvey/coops.py
--rw-r--r--  2.0 unx     2497 b- defN 80-Jan-01 00:00 searvey/critech.py
+Zip file size: 44159 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      440 b- defN 80-Jan-01 00:00 searvey/__init__.py
+-rw-r--r--  2.0 unx    35985 b- defN 80-Jan-01 00:00 searvey/coops.py
+-rw-r--r--  2.0 unx     2474 b- defN 80-Jan-01 00:00 searvey/critech.py
 -rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 searvey/custom_types.py
 -rw-r--r--  2.0 unx     2544 b- defN 80-Jan-01 00:00 searvey/erddap.py
--rw-r--r--  2.0 unx    13072 b- defN 80-Jan-01 00:00 searvey/ioc.py
--rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 searvey/models.py
--rw-r--r--  2.0 unx     4405 b- defN 80-Jan-01 00:00 searvey/multi.py
+-rw-r--r--  2.0 unx    13095 b- defN 80-Jan-01 00:00 searvey/ioc.py
+-rw-r--r--  2.0 unx     1401 b- defN 80-Jan-01 00:00 searvey/models.py
+-rw-r--r--  2.0 unx     4411 b- defN 80-Jan-01 00:00 searvey/multi.py
 -rw-r--r--  2.0 unx      975 b- defN 80-Jan-01 00:00 searvey/rate_limit.py
 -rw-r--r--  2.0 unx     5244 b- defN 80-Jan-01 00:00 searvey/stations.py
--rw-r--r--  2.0 unx     2896 b- defN 80-Jan-01 00:00 searvey/uhslc.py
+-rw-r--r--  2.0 unx     2873 b- defN 80-Jan-01 00:00 searvey/uhslc.py
 -rw-r--r--  2.0 unx     1358 b- defN 80-Jan-01 00:00 searvey/us_states.json
 -rw-r--r--  2.0 unx    13174 b- defN 80-Jan-01 00:00 searvey/usgs.py
 -rw-r--r--  2.0 unx     6688 b- defN 80-Jan-01 00:00 searvey/utils.py
--rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.8.dist-info/RECORD
-18 files, 131637 bytes uncompressed, 41965 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4107 b- defN 80-Jan-01 00:00 searvey-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.9.dist-info/RECORD
+18 files, 131810 bytes uncompressed, 42027 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: searvey/usgs.py
 Comment: 
 
 Filename: searvey/utils.py
 Comment: 
 
-Filename: searvey-0.3.8.dist-info/LICENSE
+Filename: searvey-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: searvey-0.3.8.dist-info/METADATA
+Filename: searvey-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: searvey-0.3.8.dist-info/WHEEL
+Filename: searvey-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: searvey-0.3.8.dist-info/RECORD
+Filename: searvey-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## searvey/__init__.py

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from searvey.coops import get_coops_stations
 from searvey.ioc import get_ioc_data
 from searvey.ioc import get_ioc_stations
 from searvey.stations import get_stations
 from searvey.stations import Provider
+from searvey.usgs import get_usgs_stations
 
 
 __all__: list[str] = [
     "get_coops_stations",
     "get_ioc_data",
     "get_ioc_stations",
     "get_stations",
+    "get_usgs_stations",
     "Provider",
 ]
```

## searvey/coops.py

```diff
@@ -771,29 +771,29 @@
     discontinued_stations = dataframes[StationStatus.DISCONTINUED]
     discontinued_stations.loc[
         discontinued_stations.index.isin(active_stations.index), "status"
     ] = StationStatus.ACTIVE.value
 
     stations = pandas.concat(
         (
-            active_stations[~active_stations.index.isin(discontinued_stations.index)],
+            active_stations[~active_stations.index.isin(discontinued_stations.index)].drop(columns="removed"),  # fmt: skip
             discontinued_stations,
         )
     )
     stations.loc[pandas.isna(stations["status"]), "status"] = StationStatus.ACTIVE.value
     stations.sort_values(["status", "removed"], na_position="first", inplace=True)
 
     if station_status is not None:
         if isinstance(station_status, StationStatus):
             station_status = station_status.value
         stations = stations[stations["status"] == station_status]
 
     return GeoDataFrame(
         stations[["nws_id", "name", "state", "status", "removed"]],
-        geometry=geopandas.points_from_xy(stations["x"], stations["y"]),
+        geometry=geopandas.points_from_xy(stations["x"], stations["y"], crs="EPSG:4326"),
     )
 
 
 def coops_stations_within_region(
     region: Polygon | None = None,
     station_status: StationStatus | None = None,
 ) -> GeoDataFrame:
```

## searvey/critech.py

```diff
@@ -23,15 +23,15 @@
     "longitude (degrees_east)": "lon",
     "SLEV (m)": "sea_level",
     "timestamp (UTC)": "timestamp",
 }
 
 
 EMODNET_CRITECH = ERDDAPDataset(
-    server_url=pydantic.parse_obj_as(pydantic.HttpUrl, "https://erddap.emodnet-physics.eu/erddap"),
+    server_url=pydantic.HttpUrl("https://erddap.emodnet-physics.eu/erddap"),
     dataset_id="TAD_Tsunami_Alert_Device",
     is_longitude_symmetric=True,
 )
 
 
 def normalize_names(df: pd.DataFrame) -> pd.DataFrame:
     df = df.rename(columns=_CRITECH_NORMALIZED_NAMES)
```

## searvey/ioc.py

```diff
@@ -10,14 +10,15 @@
 - ``performance``
 
 We parse all 3 of them and we merge them.
 """
 from __future__ import annotations
 
 import functools
+import io
 import logging
 import warnings
 from typing import Optional
 from typing import Union
 
 import bs4
 import geopandas as gpd
@@ -140,15 +141,15 @@
     soup = bs4.BeautifulSoup(response.content, "html5lib")
     logger.debug("Created soup: %s", url)
     table = soup.find("table", {"class": "nice"})
     trs = table.find_all("tr")
     table_contents = "\n".join(str(tr) for tr in trs[skip_table_rows:])
     html = f"<table>{table_contents}</table>"
     logger.debug("Created table: %s", url)
-    df = pd.read_html(html)[0]
+    df = pd.read_html(io.StringIO(html))[0]
     logger.debug("Parsed table: %s", url)
     df.columns = IOC_STATIONS_COLUMN_NAMES[output]
     df = df.drop(columns="view")
     return df
 
 
 def normalize_ioc_stations(df: pd.DataFrame) -> gpd.GeoDataFrame:
```

## searvey/models.py

```diff
@@ -10,22 +10,21 @@
 
 class ERDDAPProtocol(str, enum.Enum):
     TABLEDAP: Final = "tabledap"
     GRIDDAP: Final = "griddap"
 
 
 class BBox(pydantic.BaseModel):
+    model_config = pydantic.ConfigDict(extra="forbid")
+
     lon_min: float
     lon_max: float
     lat_min: float = pydantic.Field(default=-90, ge=-90, le=90)
     lat_max: float = pydantic.Field(default=90, ge=-90, le=90)
 
-    class Config:
-        extra = "forbid"
-
 
 class SymmetricBBox(BBox):
     lon_min: float = pydantic.Field(default=-180, ge=-180, le=180)
     lon_max: float = pydantic.Field(default=180, ge=-180, le=180)
 
 
 class AsymmetricBBox(BBox):
```

## searvey/multi.py

```diff
@@ -33,21 +33,20 @@
 except AttributeError:
     MAX_AVAILABLE_PROCESSES = os.cpu_count()
     if MAX_AVAILABLE_PROCESSES is None:
         MAX_AVAILABLE_PROCESSES = 1
 
 
 class FutureResult(pydantic.BaseModel):
+    model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
+
     exception: Optional[Exception] = None
     kwargs: Optional[Dict[str, Any]] = None
     result: Any = None
 
-    class Config:
-        arbitrary_types_allowed: bool = True
-
     def __hash__(self) -> int:
         return hash((type(self),) + tuple(self.__dict__.values()))
 
 
 def multi(
     executor: Union[Type[ProcessPoolExecutor], Type[ThreadPoolExecutor]],
     func: Callable[..., Any],
```

## searvey/uhslc.py

```diff
@@ -20,15 +20,15 @@
     "time (UTC)": "time",
     "latitude (degrees_north)": "lat",
     "longitude (degrees_east)": "lon",
     "last_rq_date (UTC)": "last_rq_date",
 }
 
 SOEST_UHSLC = ERDDAPDataset(
-    server_url=pydantic.parse_obj_as(pydantic.HttpUrl, "https://uhslc.soest.hawaii.edu/erddap"),
+    server_url=pydantic.HttpUrl("https://uhslc.soest.hawaii.edu/erddap"),
     dataset_id="global_hourly_fast",
     is_longitude_symmetric=False,
 )
 
 
 def normalize_names(df: pd.DataFrame) -> pd.DataFrame:
     df = df.rename(columns=_UHSLC_NORMALIZED_NAMES)
```

## Comparing `searvey-0.3.8.dist-info/LICENSE` & `searvey-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `searvey-0.3.8.dist-info/METADATA` & `searvey-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: searvey
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Home-page: https://github.com/oceanmodeling/searvey.git
 License: GPL-3.0-or-later
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Dist: Shapely
 Requires-Dist: beautifulsoup4
 Requires-Dist: dataretrieval (>=1)
 Requires-Dist: erddapy
 Requires-Dist: geopandas
 Requires-Dist: html5lib
 Requires-Dist: limits
 Requires-Dist: lxml
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pydantic
+Requires-Dist: pydantic (>2)
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Requires-Dist: xarray
 Project-URL: Repository, https://github.com/oceanmodeling/searvey.git
 Description-Content-Type: text/markdown
```

## Comparing `searvey-0.3.8.dist-info/RECORD` & `searvey-0.3.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-searvey/__init__.py,sha256=tGsvJhmuYSykgwKFvDGTXiKFsQg3F1Fj8wWQPsiNzgw,372
-searvey/coops.py,sha256=a-dXKDvgjCchu7TKwaERnmGnPAwps1bZChBxkJQmU_w,35931
-searvey/critech.py,sha256=rlHWrtAKdFza9N7GMoKltvslqmkmdRdutsbxKIcD7Jg,2497
+searvey/__init__.py,sha256=G_2MC_AEQUgqGzrA17siIqkAf6biQ08Xg4Eh3-yN8KE,440
+searvey/coops.py,sha256=AM9vszj4Cq2B_KLbdx6pEpaS_xiH0u-lx9OzRkLS_Lk,35985
+searvey/critech.py,sha256=r5ZuEaXjr5V0lyunme1RsNBusfpffOSGtSyGt89dLMw,2474
 searvey/custom_types.py,sha256=PSuBMk5LVuPeWY8CotZyi_8-ZblmP-mocAl4o2oEpOU,466
 searvey/erddap.py,sha256=zBSZ554zU_l2mapfsZNAD_s70Hgw_A-9_BKm5gwA8DM,2544
-searvey/ioc.py,sha256=8qitNnOgAkdjsprfseUNIdaCdUaWWNlPGbwwShoGu1E,13072
-searvey/models.py,sha256=fmRVoh9pnYE9nUzp1n53fkJVWPvJU3E38qmCZn0u5qk,1389
-searvey/multi.py,sha256=0ueJdcyqVpj3PSEhGQkO1UEVl5jBjrdPaOz7NM-lneg,4405
+searvey/ioc.py,sha256=k9KUw-J3KFycnIZmGSnPfQL0gnHjGs5WNzeLRbKkWzU,13095
+searvey/models.py,sha256=u0zopYDUz8MjCMgHSuiAJSoMWNhC9JJn9F0CgaHMhdQ,1401
+searvey/multi.py,sha256=tDRq_By8hR0Hz6SjuXqgmDLL7Lp-O_7szzzxFPTMFEI,4411
 searvey/rate_limit.py,sha256=DgvKX8Ww1qej2gZrJquoetHi9vSk4ErI6iTYQ3oGTdA,975
 searvey/stations.py,sha256=7s97dZLNwZ2DQd6Luo7YD1TnmmLj6dvUmqH6rJIZdZ8,5244
-searvey/uhslc.py,sha256=i4g2O-ie3gj6IPzpsS9ySSbMl9YtU_cGBXs_qoyt1VA,2896
+searvey/uhslc.py,sha256=6iLIaGDrJkVRflZkru7EskDv_sRMXhZMFFyvB7w6LzY,2873
 searvey/us_states.json,sha256=EBZm8uzX4PWgD1kgg2hBR-TEl2QbduSq2tG9sekOywE,1358
 searvey/usgs.py,sha256=wHrBQv9bB5jINimVkmsQlAN_Ok0w2bZx5FygBMrXBo8,13174
 searvey/utils.py,sha256=oTD9mRK6-rm_0yykhaSyjqHPz7DjPyBqnbl3sdl6MEs,6688
-searvey-0.3.8.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
-searvey-0.3.8.dist-info/METADATA,sha256=ldna23EZwqWcOGoPAPAcqudB1OUN7XGZLm_iJrTwYFk,4051
-searvey-0.3.8.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-searvey-0.3.8.dist-info/RECORD,,
+searvey-0.3.9.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
+searvey-0.3.9.dist-info/METADATA,sha256=UXNnBtbAyPZqkgVKQF0hQQb0EoQhr-NWiPVGqWyn61g,4107
+searvey-0.3.9.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+searvey-0.3.9.dist-info/RECORD,,
```


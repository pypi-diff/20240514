# Comparing `tmp/pyefergy-22.1.0.tar.gz` & `tmp/pyefergy-22.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyefergy-22.1.0.tar", last modified: Fri Jan 28 19:54:37 2022, max compression
+gzip compressed data, was "pyefergy-22.1.1.tar", last modified: Sat Jan 29 02:45:05 2022, max compression
```

## Comparing `pyefergy-22.1.0.tar` & `pyefergy-22.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:54:37.123196 pyefergy-22.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-28 19:54:26.000000 pyefergy-22.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-28 19:54:26.000000 pyefergy-22.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-01-28 19:54:37.123196 pyefergy-22.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-01-28 19:54:26.000000 pyefergy-22.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:54:37.123196 pyefergy-22.1.0/pyefergy/
--rw-r--r--   0 runner    (1001) docker     (121)    21516 2022-01-28 19:54:26.000000 pyefergy-22.1.0/pyefergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-01-28 19:54:26.000000 pyefergy-22.1.0/pyefergy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 19:54:26.000000 pyefergy-22.1.0/pyefergy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:54:37.123196 pyefergy-22.1.0/pyefergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-01-28 19:54:36.000000 pyefergy-22.1.0/pyefergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-28 19:54:37.000000 pyefergy-22.1.0/pyefergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 19:54:36.000000 pyefergy-22.1.0/pyefergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-28 19:54:36.000000 pyefergy-22.1.0/pyefergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-28 19:54:36.000000 pyefergy-22.1.0/pyefergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-28 19:54:37.123196 pyefergy-22.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-01-28 19:54:36.000000 pyefergy-22.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 02:45:05.706458 pyefergy-22.1.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-29 02:44:54.000000 pyefergy-22.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-29 02:44:54.000000 pyefergy-22.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-01-29 02:45:05.706458 pyefergy-22.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-01-29 02:44:54.000000 pyefergy-22.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 02:45:05.706458 pyefergy-22.1.1/pyefergy/
+-rw-r--r--   0 runner    (1001) docker     (121)    21562 2022-01-29 02:44:54.000000 pyefergy-22.1.1/pyefergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-01-29 02:44:54.000000 pyefergy-22.1.1/pyefergy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-29 02:44:54.000000 pyefergy-22.1.1/pyefergy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 02:45:05.706458 pyefergy-22.1.1/pyefergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-01-29 02:45:05.000000 pyefergy-22.1.1/pyefergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-29 02:45:05.000000 pyefergy-22.1.1/pyefergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-29 02:45:05.000000 pyefergy-22.1.1/pyefergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-29 02:45:05.000000 pyefergy-22.1.1/pyefergy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-29 02:45:05.000000 pyefergy-22.1.1/pyefergy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-29 02:45:05.706458 pyefergy-22.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-01-29 02:45:04.000000 pyefergy-22.1.1/setup.py
```

### Comparing `pyefergy-22.1.0/LICENSE` & `pyefergy-22.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyefergy-22.1.0/PKG-INFO` & `pyefergy-22.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyefergy
-Version: 22.1.0
+Version: 22.1.1
 Summary: An API library for Efergy energy meters.
 Home-page: https://github.com/tkdrob/pyefergy
 Author: Robert Hillis
 Author-email: tkdrob4390@yahoo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyefergy-22.1.0/README.md` & `pyefergy-22.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyefergy-22.1.0/pyefergy/__init__.py` & `pyefergy-22.1.1/pyefergy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
         Set alt to true to use the alternate API endpoint.
         """
         if session is None:
             session = ClientSession()
             self._close_session = True
         self._session = session
-        self.info: dict[str, str | list[str]] = {}
+        self.info: dict[str, str] = {}
+        self.sids: list[int] = []
         self._utc_offset = 0
         self._cachettl = 60
         self.update_params(api_key=api_key, **kwargs)
 
     async def __aenter__(self) -> Efergy:
         """Async enter."""
         self._from_aenter = True
@@ -155,23 +156,23 @@
             )
         return _data
 
     async def async_get_sids(self) -> None:
         """Get current values sids."""
         sids = []
         for sid in await self._async_req("getCurrentValuesSummary"):
-            sids.append(sid[SID])
-        self.info["sids"] = sids
+            sids.append(int(sid[SID]))
+        self.sids = sids
 
     async def async_get_reading(
         self,
         reading_type: str,
-        period: str = DEFAULT_PERIOD,
-        sid: str = None,
-    ) -> str | int | dict[str, int]:
+        period: str | None = DEFAULT_PERIOD,
+        sid: int | None = None,
+    ) -> str | int | float | dict[str, int]:
         """Get reading for instant, budget, or summary.
 
         'reading_type' can be any of the following:
         instant: Current Watt usage.
         energy: kWh of energy used during specified period.
         cost: Cost of energy used during specified period.
         budget: Currently set budget and status of that budget.
@@ -209,15 +210,15 @@
                 "Currency provided does not match device settings. "
                 "This can affect energy cost statistics"
             )
         if type_str:
             return _data[type_str]
         _readings = {}
         for sensor in _data:
-            if sid == sensor[SID]:
+            if sid == int(sensor[SID]):
                 return list(sensor[DATA][0].values())[0]
             _readings[sensor[SID]] = list(sensor[DATA][0].values())[0]
         return _readings
 
     async def async_hid_simple_tarrif(self, cost: str | int) -> dict:
         """Create and Apply tariff. Only requires a pence per kWh value."""
         return await self._async_req(
```

### Comparing `pyefergy-22.1.0/pyefergy/exceptions.py` & `pyefergy-22.1.1/pyefergy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyefergy-22.1.0/pyefergy.egg-info/PKG-INFO` & `pyefergy-22.1.1/pyefergy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyefergy
-Version: 22.1.0
+Version: 22.1.1
 Summary: An API library for Efergy energy meters.
 Home-page: https://github.com/tkdrob/pyefergy
 Author: Robert Hillis
 Author-email: tkdrob4390@yahoo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyefergy-22.1.0/setup.py` & `pyefergy-22.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyefergy",
-    version="22.1.0",
+    version="22.1.1",
     author="Robert Hillis",
     author_email="tkdrob4390@yahoo.com",
     description="An API library for Efergy energy meters.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tkdrob/pyefergy",
     package_data={"pyefergy": ["py.typed"]},
```


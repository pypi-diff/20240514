# Comparing `tmp/dfipy-9.0.1.tar.gz` & `tmp/dfipy-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-9.0.1.tar", max compression
+gzip compressed data, was "dfipy-9.1.0.tar", max compression
```

## Comparing `dfipy-9.0.1.tar` & `dfipy-9.1.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      568 2024-03-25 11:15:34.499269 dfipy-9.0.1/LICENCE
--rw-r--r--   0        0        0     1573 2024-03-25 11:15:34.499269 dfipy-9.0.1/README.md
--rw-r--r--   0        0        0      223 2024-03-25 11:15:34.499269 dfipy-9.0.1/dfi/__init__.py
--rw-r--r--   0        0        0     1845 2024-03-25 11:15:34.499269 dfipy-9.0.1/dfi/client.py
--rw-r--r--   0        0        0     8537 2024-03-25 11:15:34.499269 dfipy-9.0.1/dfi/connect.py
--rw-r--r--   0        0        0     3304 2024-03-25 11:15:34.499269 dfipy-9.0.1/dfi/errors.py
--rw-r--r--   0        0        0      236 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/__init__.py
--rw-r--r--   0        0        0      219 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/__init__.py
--rw-r--r--   0        0        0    14043 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/filter_fields.py
--rw-r--r--   0        0        0      347 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/geometry/__init__.py
--rw-r--r--   0        0        0     4521 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/geometry/bbox.py
--rw-r--r--   0        0        0     3135 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/geometry/point.py
--rw-r--r--   0        0        0     6687 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/geometry/polygon.py
--rw-r--r--   0        0        0      445 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/only.py
--rw-r--r--   0        0        0     7516 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/filters/time_range.py
--rw-r--r--   0        0        0    10660 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/query_document.py
--rw-r--r--   0        0        0      155 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/returns/__init__.py
--rw-r--r--   0        0        0     2005 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/returns/count.py
--rw-r--r--   0        0        0     2425 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/models/returns/records.py
--rw-r--r--   0        0        0       23 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/__init__.py
--rw-r--r--   0        0        0    18061 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/datasets.py
--rw-r--r--   0        0        0     7973 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/identities.py
--rw-r--r--   0        0        0     1336 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/info.py
--rw-r--r--   0        0        0    35222 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/ingest.py
--rw-r--r--   0        0        0    23325 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/query.py
--rw-r--r--   0        0        0     4393 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/services/users.py
--rw-r--r--   0        0        0     1468 2024-03-25 11:15:34.503269 dfipy-9.0.1/dfi/validate.py
--rw-r--r--   0        0        0     4012 2024-03-25 11:15:40.027397 dfipy-9.0.1/pyproject.toml
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 dfipy-9.0.1/PKG-INFO
+-rw-r--r--   0        0        0      568 2024-05-14 14:41:24.951838 dfipy-9.1.0/LICENCE
+-rw-r--r--   0        0        0     1573 2024-05-14 14:41:24.951838 dfipy-9.1.0/README.md
+-rw-r--r--   0        0        0      223 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/__init__.py
+-rw-r--r--   0        0        0     1924 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/client.py
+-rw-r--r--   0        0        0    11584 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/connect.py
+-rw-r--r--   0        0        0     3304 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/errors.py
+-rw-r--r--   0        0        0      236 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/__init__.py
+-rw-r--r--   0        0        0      219 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/__init__.py
+-rw-r--r--   0        0        0    15044 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/filter_fields.py
+-rw-r--r--   0        0        0      347 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/geometry/__init__.py
+-rw-r--r--   0        0        0     4521 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/geometry/bbox.py
+-rw-r--r--   0        0        0     3135 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/geometry/point.py
+-rw-r--r--   0        0        0     6955 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/geometry/polygon.py
+-rw-r--r--   0        0        0      553 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/only.py
+-rw-r--r--   0        0        0     7516 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/filters/time_range.py
+-rw-r--r--   0        0        0    10660 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/query_document.py
+-rw-r--r--   0        0        0      155 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/returns/__init__.py
+-rw-r--r--   0        0        0     2076 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/returns/count.py
+-rw-r--r--   0        0        0     2533 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/models/returns/records.py
+-rw-r--r--   0        0        0       23 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/__init__.py
+-rw-r--r--   0        0        0    17404 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/datasets.py
+-rw-r--r--   0        0        0     7624 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/identities.py
+-rw-r--r--   0        0        0     1256 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/info.py
+-rw-r--r--   0        0        0    36161 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/ingest.py
+-rw-r--r--   0        0        0    23065 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/query.py
+-rw-r--r--   0        0        0     4221 2024-05-14 14:41:24.951838 dfipy-9.1.0/dfi/services/users.py
+-rw-r--r--   0        0        0     4005 2024-05-14 14:41:29.779940 dfipy-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 dfipy-9.1.0/PKG-INFO
```

### Comparing `dfipy-9.0.1/LICENCE` & `dfipy-9.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/README.md` & `dfipy-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/client.py` & `dfipy-9.1.0/dfi/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         --------
         ```python
         from dfi import Client
 
         dfi = Client(token, url)
         ```
         """
+        # TODO: remove Connect class and just pass arguments into each service
         self.conn = Connect(
             api_token=api_token,
             base_url=base_url,
             query_timeout=query_timeout,
             progress_bar=progress_bar,
         )
         self.datasets = Datasets(self.conn)
```

### Comparing `dfipy-9.0.1/dfi/connect.py` & `dfipy-9.1.0/dfi/connect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 """Class to connect to the DFI server."""
 
 import logging
+from enum import Enum
+from http import HTTPStatus
+from json import dumps
+from typing import Any
 
 import requests
+from requests.exceptions import HTTPError
+from requests.models import Response
 
-from dfi import validate
+from dfi.errors import DFIResponseError
 
 _logger = logging.getLogger(__name__)
 
 
+# this class exists in python >=3.11 so we reimplement for 3.10 support
+class HTTPMethod(str, Enum):
+    """Defines a set of HTTP methods and descriptions."""
+
+    GET = "GET"
+    HEAD = "HEAD"
+    POST = "POST"
+    PUT = "PUT"
+    DELETE = "DELETE"
+    CONNECT = "CONNECT"
+    OPTIONS = "OPTIONS"
+    TRACE = "TRACE"
+    PATCH = "PATCH"
+
+
 class Connect:
     """Class instantiating the connectors to the DFI API.
 
     Parameters
     ----------
     api_token: token provided by generalsystem.com to access the running DFI environments.
     base_url: Base url where the service is located
@@ -32,14 +53,16 @@
         base_url: str | None = None,
         query_timeout: int | None = 60,
         progress_bar: bool | None = False,
     ) -> None:
         self.api_token = api_token
         self.base_url = base_url
         self.query_timeout = query_timeout
+
+        # TODO: remove headers here and pass them into this class from Client
         self.streaming_headers = {
             "Authorization": f"Bearer {api_token}",
             "Accept": "text/event-stream",
         }
         self.synchronous_headers = {
             "Authorization": f"Bearer {api_token}",
             "Accept": "application/json",
@@ -70,32 +93,31 @@
         stream:
             Whether to use streaming headers or synchronous headers.
         params:
             Dictionary, list of tuples or bytes to send in the query string for the request.
         """
         headers = self.streaming_headers if stream else self.synchronous_headers
         url = f"{self.base_url}/{endpoint}"
-        _logger.debug(
-            dict(
-                url=url,
-                headers=headers,
-                stream=stream,
-                params=params,
-                timeout=self.query_timeout,
-            )
-        )
+
         response = requests.get(
             url,
             headers=headers,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
 
-        validate.response(response, url, headers, params)
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            msg = format_response_log(response, HTTPMethod.GET, url, headers, params)
+
+            _logger.error(f"DFIResponseError: {dumps(msg, indent=4)}")
+            raise DFIResponseError(msg) from exc
+
         return response
 
     def api_post(
         self,
         endpoint: str,
         stream: bool = True,
         params: dict | None = None,  # type: ignore
@@ -126,15 +148,23 @@
             headers=headers,
             json=json,
             data=data,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
-        validate.response(response, url, headers, params, json)
+
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            msg = format_response_log(response, HTTPMethod.POST, url, headers, params, json)
+
+            _logger.error(f"DFIResponseError: {dumps(msg, indent=4)}")
+            raise DFIResponseError(msg) from exc
+
         return response
 
     def api_put(
         self,
         endpoint: str,
         stream: bool = True,
         params: dict | None = None,  # type: ignore
@@ -165,15 +195,23 @@
             headers=headers,
             json=json,
             data=data,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
-        validate.response(response, url, headers, params, json)
+
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            msg = format_response_log(response, HTTPMethod.PUT, url, headers, params, json)
+
+            _logger.error(f"DFIResponseError: {dumps(msg, indent=4)}")
+            raise DFIResponseError(msg) from exc
+
         return response
 
     def api_delete(
         self,
         endpoint: str,
         stream: bool = True,
         params: dict | None = None,  # type: ignore
@@ -204,15 +242,23 @@
             headers=headers,
             json=json,
             data=data,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
-        validate.response(response, url, headers, params, json)
+
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            msg = format_response_log(response, HTTPMethod.DELETE, url, headers, params, json)
+
+            _logger.error(f"DFIResponseError: {dumps(msg, indent=4)}")
+            raise DFIResponseError(msg) from exc
+
         return response
 
     def api_patch(
         self,
         endpoint: str,
         stream: bool = True,
         params: dict | None = None,  # type: ignore
@@ -243,9 +289,74 @@
             headers=headers,
             json=json,
             data=data,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
-        validate.response(response, url, headers, params, json)
+
+        try:
+            response.raise_for_status()
+        except HTTPError as exc:
+            msg = format_response_log(response, HTTPMethod.PATCH, url, headers, params, json)
+
+            _logger.error(f"DFIResponseError: {dumps(msg, indent=4)}")
+            raise DFIResponseError(msg) from exc
+
         return response
+
+
+def format_response_log(
+    response: Response,
+    method: HTTPMethod,
+    url: str,
+    headers: dict,
+    params: dict | None = None,
+    payload: dict | list | None = None,
+) -> dict[str, Any]:
+    """Human-friendly formatting for a response.
+
+    Parameters
+    ----------
+    resp:
+        a response object
+    method:
+        the HTTP method used (e.g. GET / POST / PUT / PATCH  / DELETE)
+    url:
+        the queried url
+    headers:
+        request headers
+    params:
+        request params
+    payload:
+        request payload
+
+    Raises
+    ------
+    DFIResponseError
+        If there was an error querying the DFI API.
+    """
+    msg = f"STATUS CODE: {response.status_code} - {HTTPStatus(response.status_code).name}"
+    msg += f"ERROR: {response.text}"
+    msg += f"METHOD: {method.name}"
+    msg += f"URL: {url}"
+    msg += f"PARAMS: {dumps(params, sort_keys=True, indent=4)}"
+
+    # prevent from showing the user token to terminal and logs
+    headers = headers.copy()
+    headers["Authorization"] = "Bearer XXX"
+    msg += f"HEADERS: {dumps(headers, sort_keys=True, indent=4)}"
+
+    log = {
+        "STATUS CODE": response.status_code,
+        "STATUS NAME": HTTPStatus(response.status_code).name,
+        "ERROR": response.text,
+        "METHOD": method.name,
+        "URL": url,
+        "PARAMS": params,
+        "HEADERS": headers,
+        "PAYLOAD": payload,
+    }
+
+    msg += f"PAYLOAD: {dumps(payload, sort_keys=True, indent=4)}"
+
+    return log
```

### Comparing `dfipy-9.0.1/dfi/errors.py` & `dfipy-9.1.0/dfi/errors.py`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/models/filters/filter_fields.py` & `dfipy-9.1.0/dfi/models/filters/filter_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,38 +28,63 @@
 _logger = logging.getLogger(__name__)
 
 
 class FilterOperator(str, Enum):
     """Enumerates the valid operations on FilterFields."""
 
     LT = "lt"
+    """"""  # needed for enum value to render in docs
     LG = "gt"
+    """"""  # needed for enum value to render in docs
     GTE = "gte"
+    """"""  # needed for enum value to render in docs
     LTE = "lte"
+    """"""  # needed for enum value to render in docs
     EQ = "eq"
+    """"""  # needed for enum value to render in docs
     NEQ = "neq"
+    """"""  # needed for enum value to render in docs
     BETWEEN = "between"
+    """
+    !!! info "Bounds are inclusive"
+       
+        The comparison is *inclusive* of bounds i.e.
+
+        `lower_bound <= field_value <= upper_bound`
+    """  # needed for enum value to render in docs
+
     OUTSIDE = "outside"
+    """
+    !!! info "Bounds are exclusive"
+
+        The comparison is *exclusive* of bounds (this is the inverse of `BETWEEN`) i.e.
+        
+        `not (lower_bound <= field_value <= upper_bound)`
+    """  # needed for enum value to render in docs
 
     def __str__(self) -> str:
         """Return the value as a string rather than a string of the full enum."""
         return self.value
 
     def build(self) -> str:
         """Return a FilterOperator definition for QueryDocument."""
         return str(self)
 
 
 class FieldType(str, Enum):
     """Enumerates the valid types for a FilterField."""
 
     SIGNED_NUMBER = "signed number"
+    """"""  # needed for enum value to render in docs
     UNSIGNED_NUMBER = "unsigned number"
+    """"""  # needed for enum value to render in docs
     IP = "ip"
+    """"""  # needed for enum value to render in docs
     ENUM = "enum"
+    """"""  # needed for enum value to render in docs
 
 
 class FilterField:
     """Provides type deifnition and validation for defining how to filter on FilterFields in a dataset."""
 
     _name: str
     _field_type: FieldType
```

### Comparing `dfipy-9.0.1/dfi/models/filters/geometry/bbox.py` & `dfipy-9.1.0/dfi/models/filters/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/models/filters/geometry/point.py` & `dfipy-9.1.0/dfi/models/filters/geometry/point.py`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/models/filters/geometry/polygon.py` & `dfipy-9.1.0/dfi/models/filters/geometry/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-"""Polygon model definition."""
+"""Polygon model definition.
+
+!!! info "Polygon validations"
+
+    Only some validations are performed on a Polygon (PolygonNotClosedError, LinearRingError, LongitudeOutOfBoundsError, LatitudeOutOfBoundsError).
+    More complex validations are left to the API (no 'holes', winding order, etc.)
+"""
 
 from typing import Any, TypeAlias
 
 from typing_extensions import Self
 
 from dfi.errors import LinearRingError, PolygonNotClosedError, PolygonUndefinedError
 from dfi.models.filters.geometry import Point
@@ -10,15 +16,15 @@
 RawCoords: TypeAlias = tuple[float, float]
 """Alias for `tuple[float, float]`"""
 
 MIN_VERTICES = 4
 
 
 class Polygon:
-    """A 2D Polygon as defined in GeoJSON https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6.
+    """A 2D Polygon as defined in [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6).
 
     ??? attention
         Polygons should be composed of a singular linear ring.  MultiPolygons are not supported.
 
     """
 
     _coordinates: tuple[Point, ...]
```

### Comparing `dfipy-9.0.1/dfi/models/filters/time_range.py` & `dfipy-9.1.0/dfi/models/filters/time_range.py`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/models/query_document.py` & `dfipy-9.1.0/dfi/models/query_document.py`

 * *Files identical despite different names*

### Comparing `dfipy-9.0.1/dfi/models/returns/count.py` & `dfipy-9.1.0/dfi/models/returns/count.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 _logger = logging.getLogger(__name__)
 
 
 class GroupBy(str, Enum):
     """Enumerates the valid groupby fields."""
 
     UNIQUE_IDS = "uniqueId"
+    """"""  # empty docstring needed for Enum option to appear in docs
 
     def __str__(self) -> str:
         """Return the value as a string rather than a string of the full enum."""
         return self.value
 
     def build(self) -> dict[str, dict[str, str]]:
         """Return a GroupBy return model definition for QueryDocument."""
```

### Comparing `dfipy-9.0.1/dfi/models/returns/records.py` & `dfipy-9.1.0/dfi/models/returns/records.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 _logger = logging.getLogger(__name__)
 
 
 class IncludeField(str, Enum):
     """Enumerates the valid types for a extra fields that can be returned with records."""
 
     FIELDS = "fields"
+    """"""  # needed for enum value to render in docs
     METADATA_ID = "metadataId"
+    """"""  # needed for enum value to render in docs
 
     def __str__(self) -> str:
         """Return the value as a string rather than a string of the full enum."""
         return self.value
 
     def build(self) -> str:
         """Return an IncludeField return model definition for QueryDocument."""
```

### Comparing `dfipy-9.0.1/dfi/services/datasets.py` & `dfipy-9.1.0/dfi/services/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,40 +76,39 @@
                             "brussel sprouts",
                             "cabbage",
                             "cauliflower",
                             "collards",
                         ],
                     },
                 },
-                "boundingBox": [-180.0, -90.0, 180.0, 90.0],
+                "boundingBox": [[-180.0, -90.0], [180.0, 90.0]],
                 "minDatetime": "2021-01-01T00:00:00.000Z",
                 "maxDatetime": "2022-01-01T00:00:00.000Z",
             },
             "source": {"s3SourceUrl": "s3://test-bucket/dataset-0"},
             "pipeline": {"curationConfiguration": {}},
             "pii": {"keepPii": False, "piiFields": []},
             "storage": {
                 "dataStoreType": "dfi",
                 "dataStoreConnectionDetails": {
                     "host": "0.0.0.0",
-                    "port": "1234",
-                    "queryTimeout": "3600000",
+                    "port": 1234,
+                    "queryTimeout": 3600000,
                 },
             },
             "destination": {"dataStoreRetentionLength": 0},
             "permissions": [{"type": "reader", "scope": "all"}],
         }
 
         dfi = Client(token, url)
         dfi.datasets.create(dataset)
         ```
 
         """
         with self.conn.api_post("v1/datasets", stream=False, json=dataset) as response:
-            response.raise_for_status()
             dataset_info: dict[str, Any] = response.json()
             return dataset_info
 
     def find(
         self,
         name: str | None = None,
         before: datetime | None = None,
@@ -150,15 +149,14 @@
         params = {
             "name": name,
             "before": before.isoformat() if before else None,
             "limit": limit,
         }
 
         with self.conn.api_get("v1/datasets", stream=False, params=params) as response:
-            response.raise_for_status()
             datasets: list[dict[str, Any]] = response.json()
             return datasets
 
     def find_by_id(self, dataset_id: str) -> dict[str, Any]:
         """Find a dataset by id.
 
         ??? info "Endpoint"
@@ -185,15 +183,14 @@
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.datasets.find_by_id(dataset_id="1234")
         ```
         """
         with self.conn.api_get(f"v1/datasets/{dataset_id}", stream=False) as response:
-            response.raise_for_status()
             dataset: dict[str, Any] = response.json()
             return dataset
 
     def update(self, dataset_id: str, dataset: dict[str, Any]) -> dict[str, Any]:
         """Update a dataset by id.
 
         ??? info "Endpoint"
@@ -231,18 +228,15 @@
             },
         }
 
         dfi.datasets.update(dataset_id, dataset_update)
         ```
 
         """
-        with self.conn.api_patch(
-            f"v1/datasets/{dataset_id}", stream=False, json=dataset
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_patch(f"v1/datasets/{dataset_id}", stream=False, json=dataset) as response:
             dataset_info: dict[str, Any] = response.json()
             return dataset_info
 
     def delete(self, dataset_id: str) -> None:
         """Delete a dataset by id.
 
         ??? info "Endpoint"
@@ -264,18 +258,15 @@
         dfi = Client(token, url)
 
         dataset_id = "1234"
         dfi.datasets.delete(dataset_id)
         ```
 
         """
-        with self.conn.api_delete(
-            f"v1/datasets/{dataset_id}", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_delete(f"v1/datasets/{dataset_id}", stream=False):
             return None
 
     def get_permissions(self, dataset_id: str) -> list[dict[str, Any]]:
         """Get list of permissions for this dataset.
 
         ??? info "Endpoint"
             [GET /v1/datasets/{id}/permissions](https://api.prod.generalsystem.com/docs/api#/Dataset%20Management%20(v1)/get_v1_datasets__id__permissions)
@@ -296,24 +287,19 @@
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.datasets.get_permissions(dataset_id="1234")
         ```
 
         """
-        with self.conn.api_get(
-            f"v1/datasets/{dataset_id}/permissions", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get(f"v1/datasets/{dataset_id}/permissions", stream=False) as response:
             permissions: list[dict[str, Any]] = response.json()
             return permissions
 
-    def add_permissions(
-        self, dataset_id: str, permissions: list[dict[str, Any]]
-    ) -> list[dict[str, Any]]:
+    def add_permissions(self, dataset_id: str, permissions: list[dict[str, Any]]) -> list[dict[str, Any]]:
         """Add new permissions to a dataset.
 
         ??? info "Endpoint"
             [POST /v1/datasets/{id}/permissions](https://api.prod.generalsystem.com/docs/api#/Dataset%20Management%20(v1)/post_v1_datasets__id__permissions)
 
         ??? tip "Admin Request"
             You need to be an admin for this request.
@@ -359,24 +345,19 @@
         dfi = Client(token, url)
         updated_permissions = dfi.datasets.add_permissions(
             dataset_id=dataset_id, permissions=permissions
         )
         ```
 
         """
-        with self.conn.api_post(
-            f"v1/datasets/{dataset_id}/permissions", stream=False, json=permissions
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_post(f"v1/datasets/{dataset_id}/permissions", stream=False, json=permissions) as response:
             updated_permissions: list[dict[str, Any]] = response.json()
             return updated_permissions
 
-    def delete_permissions(
-        self, dataset_id: str, permissions: list[dict[str, Any]]
-    ) -> list[dict[str, Any]]:
+    def delete_permissions(self, dataset_id: str, permissions: list[dict[str, Any]]) -> list[dict[str, Any]]:
         """Remove permissions from a dataset.  Given permission must match exactly to be removed.
 
         ??? info "Endpoint"
             [DELETE /v1/datasets/{id}/permissions](https://api.prod.generalsystem.com/docs/api#/Dataset%20Management%20(v1)/delete_v1_datasets__id__permissions)
 
         ??? tip "Admin Request"
             You need to be an admin for this request.
@@ -410,18 +391,15 @@
         dfi = Client(token, url)
         dfi.datasets.delete_permissions(
             dataset_id=dataset_id, permissions=permissions
         )
         ```
 
         """
-        with self.conn.api_delete(
-            f"v1/datasets/{dataset_id}/permissions", stream=False, json=permissions
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_delete(f"v1/datasets/{dataset_id}/permissions", stream=False, json=permissions) as response:
             removed_permissions: list[dict[str, Any]] = response.json()
             return removed_permissions
 
     def get_my_permissions(self, dataset_id: str) -> dict:
         """Get list of the current identity's permissions on a dataset.
 
         ??? info "Endpoint"
@@ -443,18 +421,15 @@
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.datasets.get_my_permissions(dataset_id="1234")
         ```
 
         """
-        with self.conn.api_get(
-            f"v1/datasets/{dataset_id}/permissions/me", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get(f"v1/datasets/{dataset_id}/permissions/me", stream=False) as response:
             permissions: dict[str, Any] = response.json()
             return permissions
 
     def get_schema(
         self, dataset_id: str, schema_type: str = "full", media_type: str = "json"
     ) -> dict[str, Any] | pa.Schema:
         """Retrieve a copy of the schema for this dataset.
@@ -514,39 +489,33 @@
             "with_metadata_id": "withMetadataId",
             "with_filter_fields": "withFilterFields",
         }
         params = {"type": schema_types[schema_type]}
 
         headers = {
             "Authorization": f"Bearer {self.conn.api_token}",
-            "Accept": (
-                "application/feather" if media_type == "feather" else "application/json"
-            ),
+            "Accept": ("application/feather" if media_type == "feather" else "application/json"),
         }
         url = f"{self.conn.base_url}/v1/datasets/{dataset_id}/schema"
 
         with requests.get(
             url,
             headers=headers,
             stream=False,
             params=params,
             timeout=self.conn.query_timeout,
         ) as response:
-            response.raise_for_status()
-
             if media_type == "feather":
                 buffer = memoryview(response.content)
                 with pa.input_stream(buffer) as stream:
                     schema = stream.read_buffer()
                     return feather.read_table(schema).schema
             return response.json()
 
-    def add_enums(
-        self, dataset_id: str, metadata_enums: dict[str, Any]
-    ) -> dict[str, Any]:
+    def add_enums(self, dataset_id: str, metadata_enums: dict[str, Any]) -> dict[str, Any]:
         """Add new values to an enum field. Any new values added to fields here are merged into the existing values.
 
         ??? info "Endpoint"
             [POST /v1/datasets/{id}/schema/values](https://api.prod.generalsystem.com/docs/api#/Dataset%20Management%20(v1)/post_v1_datasets__id__schema_values)
 
         Parameters
         ----------
@@ -580,10 +549,9 @@
         ```
         """
         with self.conn.api_post(
             f"v1/datasets/{dataset_id}/schema/values",
             stream=False,
             json=metadata_enums,
         ) as response:
-            response.raise_for_status()
             schema: dict[str, Any] = response.json()
             return schema
```

### Comparing `dfipy-9.0.1/dfi/services/identities.py` & `dfipy-9.1.0/dfi/services/identities.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
         dfi = Client(token, url)
         tokens = dfi.identities.get_tokens(include_expired=False)
         ```
         """
         params = {"includeExpired": str(include_expired).lower()}
         with self.conn.api_get("v1/tokens", params=params, stream=False) as response:
-            response.raise_for_status()
             tokens: list[dict] = response.json()
             return tokens
 
     def create_token(self, name: str, validity: str) -> dict:
         r"""Generate a new API token for the current user.
 
         ??? info "Endpoint"
@@ -82,15 +81,14 @@
         validity = "P1Y"
         token_info = dfi.identities.create_token(name, validity)
         token = token_info["token]
         ```
         """
         payload = {"name": name, "validity": validity}
         with self.conn.api_post("v1/tokens", json=payload, stream=False) as response:
-            response.raise_for_status()
             token_info: dict = response.json()
             return token_info
 
     def expire_token(self, token_id: str) -> None:
         """Expires the given api token.
 
         ??? info "Endpoint"
@@ -110,16 +108,15 @@
         from dfi import Client
 
         dfi = Client(token, url)
 
         dfi.identities.expire_token("<token id>")
         ```
         """
-        with self.conn.api_delete(f"v1/tokens/{token_id}", stream=False) as response:
-            response.raise_for_status()
+        with self.conn.api_delete(f"v1/tokens/{token_id}", stream=False):
             return None
 
     def get_identities(self) -> list[dict[str, Any]]:
         """Retrieve a list of identities.
 
         ??? info "Endpoint"
             [GET /v1/identities](https://api.prod.generalsystem.com/docs/api#/Identity%20Management%20(v1)/get_v1_identities)
@@ -139,15 +136,14 @@
 
         dfi = Client(token, url)
 
         identities = dfi.identities.get_identities()
         ```
         """
         with self.conn.api_get("v1/identities", stream=False) as response:
-            response.raise_for_status()
             identities: list[dict[str, Any]] = response.json()
             return identities
 
     def get_my_identity(self) -> dict[str, Any]:
         """Retrieve data about the identity who made this request.
 
         ??? info "Endpoint"
@@ -165,15 +161,14 @@
 
         dfi = Client(token, url)
 
         identity = dfi.identities.get_my_identity()
         ```
         """
         with self.conn.api_get("v1/identities/me", stream=False) as response:
-            response.raise_for_status()
             identity: dict[str, Any] = response.json()
             return identity
 
     def get_identity(self, identity_id: str) -> dict[str, Any]:
         """Retrieve data about a specific identity.
 
         ??? info "Endpoint"
@@ -198,22 +193,19 @@
         from dfi import Client
 
         dfi = Client(token, url)
 
         identity = dfi.identities.get_identity("<identity id>")
         ```
         """
-        with self.conn.api_get(
-            f"v1/identities/{identity_id}", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get(f"v1/identities/{identity_id}", stream=False) as response:
             identity: dict[str, Any] = response.json()
             return identity
 
-    def _delete_identity(self, identity_id: str) -> None:
+    def delete_identity(self, identity_id: str) -> None:
         """Remove an identity and all opaque tokens.
 
         ??? info "Endpoint"
             [DELETE /v1/identities/{id}](https://api.prod.generalsystem.com/docs/api#/Identity%20Management%20(v1)/delete_v1_identities__id_)
 
         ??? attention
             This should be done in conjunction with removing the user.
@@ -236,18 +228,15 @@
         from dfi import Client
 
         dfi = Client(token, url)
 
         identity = dfi.identities.delete_identity("<identity id>")
         ```
         """
-        with self.conn.api_delete(
-            f"v1/identities/{identity_id}", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_delete(f"v1/identities/{identity_id}", stream=False):
             return None
 
     def get_user_id(self, identity_id: str) -> str:
         """Extract the User ID from an Identity ID.
 
         Parameters
         ----------
```

### Comparing `dfipy-9.0.1/dfi/services/info.py` & `dfipy-9.1.0/dfi/services/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,19 +26,17 @@
     def api_version(self) -> str:
         """Return the version of the Data Flow Index (DFI) API.
 
         ??? info "Endpoint"
             `GET version`
         """
         with self.conn.api_get("version", stream=False, params=None) as response:
-            response.raise_for_status()
             return response.text
 
     def product_version(self) -> str:
         """Return the Data Flow Index (DFI) product version.
 
         ??? info "Endpoint"
             `GET product/version`
         """
         with self.conn.api_get("product/version", stream=False, params=None) as response:
-            response.raise_for_status()
             return response.text
```

### Comparing `dfipy-9.0.1/dfi/services/ingest.py` & `dfipy-9.1.0/dfi/services/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     These parameters are a subset of the aws AssumeRoleCommand
     [https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/clients/client-account/classes/assumerolecommand.html](https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/clients/client-account/classes/assumerolecommand.html)
     """
 
     def __init__(
         self,
         role_arn: str,
-        policy: dict | None = None,
-        policy_arns: list[str] | None = None,
+        policy: dict | None = None,  # TODO: make types for these?
+        policy_arns: list[dict[str, str]] | None = None,  # TODO: make types for these?
     ) -> None:
         """Initilaize class and stores values.
 
         Parameters
         ----------
         role_arn:
             The Amazon Resource Name (ARN) of the AWS role for us to assume.
@@ -64,15 +64,21 @@
         if self.policy_arns:
             aws_credentials.update({"PolicyArns": self.policy_arns})
 
         return aws_credentials
 
 
 class BatchURLFiles:
-    """A constructor class for building an BatchURLFiles document.  Indicates that this import batch should source files from a provided list of URLs."""
+    """A constructor class for building an BatchURLFiles document.  Indicates that this import batch should source files from a provided list of URLs.
+
+    !!! warning "Importing many URLs"
+
+        Importing too many URLs in a single request may result in a 413 response.  Either make multiple imports with separate requests
+        or use the BatchS3Files import method.
+    """
 
     def __init__(self, urls: list[str]) -> None:
         """Initialize and store values.
 
         Examples
         --------
         In this example, we've generated presigned URLs for 4 files on S3.  These files can now be ingested without
@@ -105,17 +111,15 @@
         """Build a BatchURLFiles document from given inputs."""
         return {"urls": self.urls}
 
 
 class BatchS3Files:
     """A constructor class for building an BatchS3Files document. Indicates that this import batch should source files from S3."""
 
-    def __init__(
-        self, bucket: str, credentials: AWSCredentials, glob: str, prefix: str | None
-    ) -> None:
+    def __init__(self, bucket: str, credentials: AWSCredentials, glob: str, prefix: str | None) -> None:
         """Initilaize class and stores values.
 
         Examples
         --------
         ```python
         from dfi.services.ingest import AWSCredentials, BatchS3Files
 
@@ -299,17 +303,15 @@
 
         boto3.setup_default_session(profile_name=self.profile)
         config = Config(region_name=self.region, signature_version="s3v4")
 
         self.s3_client = boto3.client("s3", config=config)
         self.s3_resource = boto3.resource("s3", config=config)
 
-    def find_files(
-        self, prefix: str, suffix: str, sort: bool = True, verbose: bool = False
-    ) -> list[str]:
+    def find_files(self, prefix: str, suffix: str, sort: bool = True, verbose: bool = False) -> list[str]:
         """Globs for files in S3 Bucket/Prefix ending with suffix.  Will sort files by name using natural sort.
 
         Parameters
         ----------
         prefix:
             S3 prefix to search in.
         suffix:
@@ -362,15 +364,15 @@
         """Create a presigned URL for the key.
 
         Parameters
         ----------
         object_key:
             S3 object key.
         expiration:
-            Time in minutes for the presigned URL to remain valid.  min=1, max=720
+            Time in seconds for the presigned URL to remain valid.  min=1, max=43200  (12 hours)
 
         Returns
         -------
         presigned URL
             URL will be valid for the set `expiration` time.
 
         Examples
@@ -410,15 +412,15 @@
         Parameters
         ----------
         prefix:
             S3 object prefix
         suffix:
             Suffix patten to search during glob
         expiration:
-            Time in minutes for the presigned URL to remain valid.  min=1, max=720
+            Time in seconds for the presigned URL to remain valid.  min=1, max=43200  (12 hours)
         sort:
             Whether to sort the files.  Sort is done via natural sort.
         verbose:
             If true, will show a progress bar.
 
         Returns
         -------
@@ -492,15 +494,14 @@
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.ingest.get_aws_trust_policy()
         ```
         """
         with self.conn.api_get("v1/import/awsTrustPolicy", stream=False) as response:
-            response.raise_for_status()
             aws_trust_policy: dict[Any, Any] = response.json()
             return aws_trust_policy
 
     def put_batch(
         self,
         dataset_id: str,
         source: BatchURLFiles | BatchS3Files,
@@ -536,32 +537,24 @@
             No data will be imported into the Data Flow Index.
 
         Returns
         -------
         ingest info
             information about the ingest.  If `dry_run=True` a report of the run will be returned.
         """
-        if isinstance(source, BatchS3Files):
-            raise NotImplementedError(
-                "'BatchS3Files` stubs are present but not yet implemented.  Instead use `BatchURLFiles`."
-            )
-
         payload = {
             "datasetId": dataset_id,
             "source": source.build(),
             "format": file_format.build(),
         }
 
         # requests will serialize True / False into "True" / "False", which is not a JSON boolean
         params = {"dryRun": json.dumps(dry_run)}
 
-        with self.conn.api_put(
-            "v1/import/batch", params=params, json=payload, stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_put("v1/import/batch", params=params, json=payload, stream=False) as response:
             ingest_info: dict[str, Any] = response.json()
             return ingest_info
 
     def get_batch_info(
         self,
         import_batch_id: str,
     ) -> dict[str, Any]:
@@ -585,18 +578,15 @@
         ```python
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.ingest.get_batch_info(<import_batch_id>)
         ```
         """
-        with self.conn.api_get(
-            f"v1/import/batch/{import_batch_id}", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get(f"v1/import/batch/{import_batch_id}", stream=False) as response:
             batch_info: dict[str, Any] = response.json()
             return batch_info
 
     def update_batch_status(self, import_batch_id: str, status: str) -> dict[str, str]:
         """Update information about a previously created import batch.
 
         ??? info "Endpoint"
@@ -625,18 +615,15 @@
         dfi = Client(token, url)
 
         status = "aborted"
         dfi.ingest.update_batch_status(<import_batch_id>, status)
         ```
         """
         body = {"status": status}
-        with self.conn.api_patch(
-            f"v1/import/batch/{import_batch_id}", json=body, stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_patch(f"v1/import/batch/{import_batch_id}", json=body, stream=False) as response:
             batch_status: dict[str, str] = response.json()
             return batch_status
 
     def get_batch_status(self, import_batch_id: str) -> list[dict[str, Any]]:
         """Retrieve a chronological series of status updates about an import batch.
 
         ??? info "Endpoint"
@@ -657,13 +644,42 @@
         ```python
         from dfi import Client
 
         dfi = Client(token, url)
         dfi.ingest.get_batch_status(<import_batch_id>)
         ```
         """
-        with self.conn.api_get(
-            f"v1/import/batch/{import_batch_id}/status", stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get(f"v1/import/batch/{import_batch_id}/status", stream=False) as response:
+            batch_status: list[dict[str, Any]] = response.json()
+            return batch_status
+
+    def get_import_status(self, dataset_id: str) -> list[dict[str, Any]]:
+        """Retrieve information about a running import batches on the dataset. Requires write or administrate permission on ther dataset.
+
+        ??? info "Endpoint"
+            [GET /v1/import/batch/{id}/status](https://api.prod.generalsystem.com/docs/api#/Data%20Import%20(v1)/get_v1_import_batch__importBatchId__status)
+
+        ??? tip "Admin or write permissions"
+            You need to be an admin or have write permissions for this request.
+
+        Parameters
+        ----------
+        dataset_id:
+            the dataset id to retrive the live imports for.
+
+        Returns
+        -------
+        statuses
+            a list of status updates for the batch.
+
+        Examples
+        --------
+        ```python
+        from dfi import Client
+
+        dfi = Client(token, url)
+        dfi.ingest.get_batch_status(<import_batch_id>)
+        ```
+        """
+        with self.conn.api_get(f"v1/import/status/{dataset_id}", stream=False) as response:
             batch_status: list[dict[str, Any]] = response.json()
             return batch_status
```

### Comparing `dfipy-9.0.1/dfi/services/query.py` & `dfipy-9.1.0/dfi/services/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,18 +178,15 @@
         """
         params = {
             "identityId": identity_id,
             "datasetId": dataset_id,
             "before": before,
             "pageSize": page_size,
         }
-        with self.conn.api_get(
-            "v1/query/instrumentation", params=params, stream=False
-        ) as response:
-            response.raise_for_status()
+        with self.conn.api_get("v1/query/instrumentation", params=params, stream=False) as response:
             return response.json()
 
     def manage(self, dataset_id: str, operation: str) -> dict[str, str]:  # type: ignore[type-arg]
         """Run a data management query.
 
         This allows you to perform data management operations on a dataset.
         **All operations are irrevokable and cannot be undone.**
@@ -217,25 +214,22 @@
         dfi = Client("<token>", "<url>")
 
         dataset_id = "<dataset id>"
         operation = "truncate"
         dfi.query.manage(dataset_id, operation)
         ```
         ```python
-        {
-            "status": "success"
-        }
+        {"status": "success"}
         ```
         """
         body = {
             "datasetId": dataset_id,
             "operation": operation,
         }
         with self.conn.api_post("v1/query/manage", json=body, stream=False) as response:
-            response.raise_for_status()
             return response.json()
 
     def count(
         self,
         dataset_id: str,
         uids: list[str | int] | None = None,
         geometry: Polygon | BBox | None = None,
@@ -593,17 +587,15 @@
 
         if not finish_message:
             raise NoFinishMessageReceivedError(
                 "Stream ended before finish message received.  Results may not be complete."
             )
 
         if messages_received != messages_sent:
-            raise EventsMissedError(
-                f"Received {messages_received}/{messages_sent} events from DFI API."
-            )
+            raise EventsMissedError(f"Received {messages_received}/{messages_sent} events from DFI API.")
 
         return counts
 
     def _receive_unique_id_counts(self, client: SSEClient) -> dict[str | int, int]:
         """Collect 'uniqueIds groupBy' results.
 
         Parameters
@@ -636,17 +628,15 @@
 
             match event.event:
                 case "keepAlive":
                     continue
                 case "message":
                     messages_received += 1
                     unique_id_counts.update(json.loads(event.data))
-                    pbar.set_description(
-                        f"Collecting {len(unique_id_counts):,} id counts."
-                    )
+                    pbar.set_description(f"Collecting {len(unique_id_counts):,} id counts.")
                     continue
                 case "finish":
                     finish_message = True
                     messages_sent = json.loads(event.data).get("messageCount")
                     break
                 case "queryError":
                     raise DFIResponseError(event.data)
@@ -658,17 +648,15 @@
 
         if not finish_message:
             raise NoFinishMessageReceivedError(
                 "Stream ended before finish message received.  Results may not be complete."
             )
 
         if messages_received != messages_sent:
-            raise EventsMissedError(
-                f"Received {messages_received}/{messages_sent} events from DFI API."
-            )
+            raise EventsMissedError(f"Received {messages_received}/{messages_sent} events from DFI API.")
 
         return unique_id_counts
 
     def _receive_records(self, client: SSEClient) -> pd.DataFrame:
         """Collect 'records' results into Pandas DataFrame.
 
         Parameters
@@ -721,15 +709,13 @@
 
         if not finish_message:
             raise NoFinishMessageReceivedError(
                 "Stream ended before finish message received.  Results may not be complete."
             )
 
         if messages_received != messages_sent:
-            raise EventsMissedError(
-                f"Received {messages_received}/{messages_sent} events from DFI API."
-            )
+            raise EventsMissedError(f"Received {messages_received}/{messages_sent} events from DFI API.")
 
         if len(records) > 0:
             return pd.DataFrame(records).assign(time=lambda df: pd.to_datetime(df.time))
         else:
             return pd.DataFrame(columns=["id", "coordinate", "time"])
```

### Comparing `dfipy-9.0.1/dfi/services/users.py` & `dfipy-9.1.0/dfi/services/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             ],
             "active": True,
         }
         created_user = dfi.users.create_user(user)
         ```
         """
         with self.conn.api_post("v1/users", json=user, stream=False) as response:
-            response.raise_for_status()
             created_user: dict = response.json()
             return created_user
 
     def get_users(self) -> list[dict]:
         """Retrieve the list of users in the realm.
 
         ??? info "Endpoint"
@@ -86,15 +85,14 @@
 
         dfi = Client(token, url)
 
         users = dfi.users.get_users()
         ```
         """
         with self.conn.api_get("v1/users", stream=False) as response:
-            response.raise_for_status()
             users: list[dict] = response.json()
             return users
 
     def get_user(self, user_id: str) -> dict:
         """Retrieve details about a user by id.
 
         ??? info "Endpoint"
@@ -120,15 +118,14 @@
 
         dfi = Client(token, url)
 
         identity = dfi.users.get_user("<user id>")
         ```
         """
         with self.conn.api_get(f"v1/users/{user_id}", stream=False) as response:
-            response.raise_for_status()
             user: dict = response.json()
             return user
 
     def delete_user(self, user_id: str) -> None:
         """Remove a user from the system. This removes all identities and access tokens that exist for the user as well.
 
         ??? info "Endpoint"
@@ -153,10 +150,9 @@
         from dfi import Client
 
         dfi = Client(token, url)
 
         identity = dfi.users.delete_user("<user id>")
         ```
         """
-        with self.conn.api_delete(f"v1/users/{user_id}", stream=False) as response:
-            response.raise_for_status()
+        with self.conn.api_delete(f"v1/users/{user_id}", stream=False):
             return None
```

### Comparing `dfipy-9.0.1/pyproject.toml` & `dfipy-9.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
-version = "9.0.1"
+version = "9.1.0"
 description = "Python SDK targeting the DFI API"
 authors = [
   "Robert Edwards <robert.edwards@generalsystem.com>",
   "Maurizio Morriello <maurizio.morriello@generalsystem.com>",
   "Sebastiano Ferraris <sebastiano.ferraris@generalsystem.com>",
   "Tom Pierce <tom.pierce@generalsystem.com>",
   "Tom Reeve <tom.reeve@generalsystem.com>",
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 pandas = "^2.0.1"
 python = "^3.10"
 requests = "^2.30.0"
 sseclient-py = "^1.7.2"
 tqdm = "^4.65.0"
-pyarrow = "14.0.1"
+pyarrow = "^15.0.2"
 boto3 = "^1.34.19"
 natsort = "^8.4.0"
 typing-extensions = "^4.10.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.5"
 pytest = "^7.2.2"
@@ -43,18 +43,18 @@
 jupyterlab = "^4.1.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5.12"
-mkdocstrings = {extras = ["python"], version = "^0.24.1"}
+mkdocstrings = { extras = ["python"], version = "^0.24.1" }
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.1"
-black = "^24.2.0" # mkdocs uses black for formatting
+black = "^24.2.0"                                           # mkdocs uses black for formatting
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
@@ -78,86 +78,89 @@
 no_warn_return_any = true
 warn_unreachable = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests", "integration_tests"]
 log_cli = true
 log_cli_level = "WARNING"
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
 
 ######################
 # ruff
 ######################
 [tool.ruff]
 line-length = 120
 indent-width = 4
 target-version = "py310"
-include = ["pyproject.toml", "dfi/**/*.py", "tests/**/*.py", "integration_tests/**/*.py"]
+include = [
+  "pyproject.toml",
+  "dfi/**/*.py",
+  "tests/**/*.py",
+  "integration_tests/**/*.py",
+]
 extend-include = ["*.ipynb"]
 # Exclude a variety of commonly ignored directories.
 exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".git-rewrite",
-    ".hg",
-    ".ipynb_checkpoints",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pyenv",
-    ".pytest_cache",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    ".vscode",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "site-packages",
-    "venv",
+  ".bzr",
+  ".direnv",
+  ".eggs",
+  ".git",
+  ".git-rewrite",
+  ".hg",
+  ".ipynb_checkpoints",
+  ".mypy_cache",
+  ".nox",
+  ".pants.d",
+  ".pyenv",
+  ".pytest_cache",
+  ".pytype",
+  ".ruff_cache",
+  ".svn",
+  ".tox",
+  ".venv",
+  ".vscode",
+  "__pypackages__",
+  "_build",
+  "buck-out",
+  "build",
+  "dist",
+  "node_modules",
+  "site-packages",
+  "venv",
 ]
 
 [tool.ruff.format]
 # Black compatible settings
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
 
 docstring-code-format = true
 docstring-code-line-length = 60
 
 [tool.ruff.lint]
 select = [
-    "E", # pycodestyle
-    "F", # Pyflakes
-    "UP", # pyupgrade
-    "B", # flake8-bugbear
-    "SIM", # flake8-simplify
-    "I", # isort
-    "RUF", # ruff-specific-rules
-    "PL", # Pylint rules
+  "E",   # pycodestyle
+  "F",   # Pyflakes
+  "UP",  # pyupgrade
+  "B",   # flake8-bugbear
+  "SIM", # flake8-simplify
+  "I",   # isort
+  "RUF", # ruff-specific-rules
+  "PL",  # Pylint rules
 ]
 ignore = [
   "D203", # one-blank-line-before-class
   "D213", # multi-line-summary-second-line
   "E501", # line-too-long
 ]
 extend-select = [
-  "UP",  # pyupgrade
-  "D",   # pydocstyle
+  "UP", # pyupgrade
+  "D",  # pydocstyle
 ]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
@@ -167,8 +170,9 @@
 "integration_tests/**/*.py" = ["D103", "PLR0913"]
 "tests/**/*.py" = ["D103", "PLR0913"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.lint.pylint]
-max-args=8
+max-args = 8
+
```

### Comparing `dfipy-9.0.1/PKG-INFO` & `dfipy-9.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 9.0.1
+Version: 9.1.0
 Summary: Python SDK targeting the DFI API
 Home-page: https://www.generalsystem.com/
 Author: Robert Edwards
 Author-email: robert.edwards@generalsystem.com
 Maintainer: General System
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.19,<2.0.0)
 Requires-Dist: natsort (>=8.4.0,<9.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pyarrow (==14.0.1)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Project-URL: Documentation, https://dfipy.docs.generalsystem.com/
 Project-URL: Repository, https://github.com/thegeneralsystem/dfipy
 Description-Content-Type: text/markdown
```


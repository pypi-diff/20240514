# Comparing `tmp/ecoindex_compute-5.7.0.tar.gz` & `tmp/ecoindex_compute-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_compute-5.7.0.tar", max compression
+gzip compressed data, was "ecoindex_compute-5.8.0.tar", max compression
```

## Comparing `ecoindex_compute-5.7.0.tar` & `ecoindex_compute-5.8.0.tar`

### file list

```diff
@@ -1,27 +1,21 @@
--rw-r--r--   0        0        0      984 2023-11-22 12:38:21.862213 ecoindex_compute-5.7.0/README.md
--rw-r--r--   0        0        0        6 2023-11-25 17:53:37.123717 ecoindex_compute-5.7.0/ecoindex/compute/VERSION
--rw-r--r--   0        0        0      373 2023-11-22 17:34:10.771415 ecoindex_compute-5.7.0/ecoindex/compute/__init__.py
--rw-r--r--   0        0        0     1843 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/compute/ecoindex.py
--rw-r--r--   0        0        0     1275 2023-11-25 17:28:46.564494 ecoindex_compute-5.7.0/ecoindex/data/__init__.py
--rw-r--r--   0        0        0       98 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/data/colors.py
--rw-r--r--   0        0        0       48 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/data/grades.py
--rw-r--r--   0        0        0       52 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/data/medians.py
--rw-r--r--   0        0        0      688 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/data/quantiles.py
--rw-r--r--   0        0        0       52 2023-11-11 17:30:14.625606 ecoindex_compute-5.7.0/ecoindex/data/targets.py
--rw-r--r--   0        0        0      871 2023-11-22 12:38:21.856213 ecoindex_compute-5.7.0/ecoindex/models/__init__.py
--rw-r--r--   0        0        0     1018 2023-11-22 12:38:21.856213 ecoindex_compute-5.7.0/ecoindex/models/api.py
--rw-r--r--   0        0        0     4130 2023-11-22 17:35:56.566128 ecoindex_compute-5.7.0/ecoindex/models/compute.py
--rw-r--r--   0        0        0      441 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/models/enums.py
--rw-r--r--   0        0        0      475 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/models/parameters.py
--rw-r--r--   0        0        0     3828 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/models/response_examples.py
--rw-r--r--   0        0        0      241 2023-11-11 17:30:14.626606 ecoindex_compute-5.7.0/ecoindex/models/scraper.py
--rw-r--r--   0        0        0      133 2023-11-11 17:30:14.626606 ecoindex_compute-5.7.0/ecoindex/models/sort.py
--rw-r--r--   0        0        0     1868 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/models/tasks.py
--rw-r--r--   0        0        0      167 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/utils/__init__.py
--rw-r--r--   0        0        0     3088 2023-11-11 17:30:14.626606 ecoindex_compute-5.7.0/ecoindex/utils/cli_translations/en.yml
--rw-r--r--   0        0        0     3321 2023-11-11 17:30:14.626606 ecoindex_compute-5.7.0/ecoindex/utils/cli_translations/fr.yml
--rw-r--r--   0        0        0     2237 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/utils/files.py
--rw-r--r--   0        0        0      679 2023-11-22 12:38:21.857213 ecoindex_compute-5.7.0/ecoindex/utils/screenshots.py
--rw-r--r--   0        0        0      174 2023-11-22 17:28:50.433848 ecoindex_compute-5.7.0/ecoindex/utils/sync_version.py
--rw-r--r--   0        0        0      736 2023-11-25 17:53:39.388856 ecoindex_compute-5.7.0/pyproject.toml
--rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 ecoindex_compute-5.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1407 2024-05-14 12:27:45.715888 ecoindex_compute-5.8.0/README.md
+-rw-r--r--   0        0        0        6 2024-05-14 12:27:59.503902 ecoindex_compute-5.8.0/ecoindex/compute/VERSION
+-rw-r--r--   0        0        0      373 2024-05-14 12:27:45.703888 ecoindex_compute-5.8.0/ecoindex/compute/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-14 12:27:45.703888 ecoindex_compute-5.8.0/ecoindex/compute/ecoindex.py
+-rw-r--r--   0        0        0     1004 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/colors.py
+-rw-r--r--   0        0        0       48 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/grades.py
+-rw-r--r--   0        0        0       52 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/medians.py
+-rw-r--r--   0        0        0      688 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/quantiles.py
+-rw-r--r--   0        0        0       52 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/data/targets.py
+-rw-r--r--   0        0        0      935 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/__init__.py
+-rw-r--r--   0        0        0     1018 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/api.py
+-rw-r--r--   0        0        0       91 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/cli.py
+-rw-r--r--   0        0        0     4524 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/compute.py
+-rw-r--r--   0        0        0      551 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/enums.py
+-rw-r--r--   0        0        0     3828 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/response_examples.py
+-rw-r--r--   0        0        0     1089 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/scraper.py
+-rw-r--r--   0        0        0      133 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/sort.py
+-rw-r--r--   0        0        0     1868 2024-05-14 12:27:45.707888 ecoindex_compute-5.8.0/ecoindex/models/tasks.py
+-rw-r--r--   0        0        0      736 2024-05-14 12:28:02.127905 ecoindex_compute-5.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 ecoindex_compute-5.8.0/PKG-INFO
```

### Comparing `ecoindex_compute-5.7.0/ecoindex/compute/ecoindex.py` & `ecoindex_compute-5.8.0/ecoindex/compute/ecoindex.py`

 * *Files identical despite different names*

### Comparing `ecoindex_compute-5.7.0/ecoindex/data/__init__.py` & `ecoindex_compute-5.8.0/ecoindex/data/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from ecoindex.data.colors import A as A_color
 from ecoindex.data.colors import B as B_color
 from ecoindex.data.colors import C as C_color
 from ecoindex.data.colors import D as D_color
 from ecoindex.data.colors import E as E_color
 from ecoindex.data.colors import F as F_color
 from ecoindex.data.colors import G as G_color
@@ -19,15 +17,14 @@
     quantiles_size,
 )
 from ecoindex.data.targets import (
     target_dom,
     target_req,
     target_size,
 )
-from ecoindex.utils.sync_version import read_version_from_file
 
 __all__ = [
     "A",
     "B",
     "C",
     "D",
     "E",
@@ -46,12 +43,7 @@
     "quantiles_dom",
     "quantiles_req",
     "quantiles_size",
     "target_dom",
     "target_req",
     "target_size",
 ]
-
-current_directory = os.path.dirname(os.path.realpath(__file__))
-filename = os.path.join(current_directory, "..", "compute", "VERSION")
-
-ecoindex_compute_version = read_version_from_file(filename)
```

### Comparing `ecoindex_compute-5.7.0/ecoindex/data/quantiles.py` & `ecoindex_compute-5.8.0/ecoindex/data/quantiles.py`

 * *Files identical despite different names*

### Comparing `ecoindex_compute-5.7.0/ecoindex/models/__init__.py` & `ecoindex_compute-5.8.0/ecoindex/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from ecoindex.models.cli import (
+    CliHost,
+)
 from ecoindex.models.compute import (
     Ecoindex,
     PageMetrics,
     PageType,
     Request,
     Result,
     ScreenShot,
@@ -15,14 +18,15 @@
     example_file_not_found,
     example_page_listing_empty,
 )
 from ecoindex.models.scraper import RequestItem, Requests
 from ecoindex.models.sort import Sort
 
 __all__ = [
+    "CliHost",
     "Ecoindex",
     "example_daily_limit_response",
     "example_ecoindex_not_found",
     "example_file_not_found",
     "example_page_listing_empty",
     "ExportFormat",
     "Language",
```

### Comparing `ecoindex_compute-5.7.0/ecoindex/models/api.py` & `ecoindex_compute-5.8.0/ecoindex/models/api.py`

 * *Files identical despite different names*

### Comparing `ecoindex_compute-5.7.0/ecoindex/models/compute.py` & `ecoindex_compute-5.8.0/ecoindex/models/compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+import os
 from datetime import datetime
+from functools import lru_cache
 from pathlib import Path
 from typing import Any
 
-from ecoindex.data import ecoindex_compute_version
+from ecoindex.models.enums import Grade
 from pydantic import AnyHttpUrl, BaseModel, Field, field_validator
 
 PageType = str
 
 
+@lru_cache
+def get_compute_version() -> str:
+    current_directory = os.path.dirname(os.path.realpath(__file__))
+    version_filename = os.path.join(current_directory, "..", "compute", "VERSION")
+
+    with open(version_filename, "r") as f:
+        return (f.read()).strip()
+
+
 class Ecoindex(BaseModel):
-    grade: str | None = Field(
+    grade: Grade | None = Field(
         default=None,
         title="Ecoindex grade",
         description="Is the corresponding ecoindex grade of the page (from A to G)",
     )
     score: float | None = Field(
         default=None,
         title="Ecoindex score",
@@ -32,15 +43,15 @@
     water: float | None = Field(
         default=None,
         title="Ecoindex Water equivalent",
         description="Is the equivalent water consumption (in `cl`) of the page",
         ge=0,
     )
     ecoindex_version: str | None = Field(
-        default=ecoindex_compute_version,
+        default=get_compute_version(),
         title="Ecoindex version",
         description="Is the version of the ecoindex used to compute the score",
     )
 
 
 class PageMetrics(BaseModel):
     size: float = Field(
@@ -88,21 +99,22 @@
         examples=["https://www.ecoindex.fr"],
     )
 
     @field_validator("url")
     @classmethod
     def url_as_http_url(cls, v: str) -> str:
         url_object = AnyHttpUrl(url=v)
+        assert url_object.scheme in {"http", "https"}, "scheme must be http or https"
 
         return url_object.unicode_string()
 
     def get_url_host(self) -> str:
-        url_obect = AnyHttpUrl(url=self.url)
+        url_object = AnyHttpUrl(url=self.url)
 
-        return str(url_obect.host)
+        return str(url_object.host)
 
     def get_url_path(self) -> str:
         url_obect = AnyHttpUrl(url=self.url)
 
         return str(url_obect.path)
```

### Comparing `ecoindex_compute-5.7.0/ecoindex/models/response_examples.py` & `ecoindex_compute-5.8.0/ecoindex/models/response_examples.py`

 * *Files identical despite different names*

### Comparing `ecoindex_compute-5.7.0/ecoindex/models/tasks.py` & `ecoindex_compute-5.8.0/ecoindex/models/tasks.py`

 * *Files identical despite different names*

### Comparing `ecoindex_compute-5.7.0/pyproject.toml` & `ecoindex_compute-5.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecoindex_compute"
-version = "5.7.0"
+version = "5.8.0"
 readme = "README.md"
 description = "Ecoindex module provides a simple way to measure the Ecoindex score based on the 3 parameters: The DOM elements of the page, the size of the page and the number of external requests of the page"
 authors = ['Vincent Vatelot <vincent.vatelot@ik.me>']
 license = "Creative Commons BY-NC-ND"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_python"
 include = ["LICENSE"]
```

### Comparing `ecoindex_compute-5.7.0/PKG-INFO` & `ecoindex_compute-5.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
-Name: ecoindex-compute
-Version: 5.7.0
+Name: ecoindex_compute
+Version: 5.8.0
 Summary: Ecoindex module provides a simple way to measure the Ecoindex score based on the 3 parameters: The DOM elements of the page, the size of the page and the number of external requests of the page
 Home-page: http://www.ecoindex.fr
 License: Creative Commons BY-NC-ND
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofile (>=3.8.8,<4.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/cnumr/ecoindex_python
 Description-Content-Type: text/markdown
 
 # Ecoindex python
 
+[![Validate project quality](https://github.com/cnumr/ecoindex_python_fullstack/actions/workflows/quality_check.yml/badge.svg?branch=main)](https://github.com/cnumr/ecoindex_python_fullstack/actions/workflows/quality_check.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/ecoindex-compute?logo=pypi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/ecoindex-compute?style=social&logo=pypi)
+
 This basic module provides a simple interface to get the [Ecoindex](http://www.ecoindex.fr) based on 3 parameters:
 
 - The number of DOM elements in the page
 - The size of the page
 - The number of external requests of the page
 
 ## Requirements
@@ -33,32 +38,32 @@
 
 ```shell
 pip install ecoindex_compute
 ```
 
 ## Use
 
-### Get ecoindex
+### Compute ecoindex
 
-You can easily get the ecoindex by calling the function `get_ecoindex()`:
+You can easily compute the ecoindex by calling the function `compute_ecoindex()`:
 
 ```python
-(function) get_ecoindex: (dom: int, size: float, requests: int) -> Coroutine[Any, Any, Ecoindex]
+(function) compute_ecoindex: (dom: int, size: float, requests: int) -> Coroutine[Any, Any, Ecoindex]
 ```
 
 Example:
 
 ```python
 import asyncio
 from pprint import pprint
 
-from ecoindex.compute import get_ecoindex
+from ecoindex.compute import compute_ecoindex
 
 # Get ecoindex from DOM elements, size of page and requests of the page
-ecoindex = asyncio.run(get_ecoindex(dom=100, size=100, requests=100))
+ecoindex = asyncio.run(compute_ecoindex(nodes=100, size=100, requests=100))
 pprint(ecoindex)
 ```
 
 Result example:
 
 ```python
 Ecoindex(grade='B', score=72.0, ges=1.56, water=2.34, ecoindex_version='3.0.0')
```


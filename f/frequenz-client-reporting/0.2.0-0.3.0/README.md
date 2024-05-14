# Comparing `tmp/frequenz-client-reporting-0.2.0.tar.gz` & `tmp/frequenz-client-reporting-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-reporting-0.2.0.tar", last modified: Mon Apr 29 14:30:54 2024, max compression
+gzip compressed data, was "frequenz-client-reporting-0.3.0.tar", last modified: Tue May 14 14:01:27 2024, max compression
```

## Comparing `frequenz-client-reporting-0.2.0.tar` & `frequenz-client-reporting-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/examples/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.808779 frequenz-client-reporting-0.2.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.808779 frequenz-client-reporting-0.2.0/src/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/examples/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.411909 frequenz-client-reporting-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.411909 frequenz-client-reporting-0.3.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.411909 frequenz-client-reporting-0.3.0/src/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:14.000000 frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:01:27.415909 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-14 14:01:27.000000 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 14:01:27.000000 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:01:27.000000 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-14 14:01:27.000000 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 14:01:27.000000 frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/top_level.txt
```

### Comparing `frequenz-client-reporting-0.2.0/LICENSE` & `frequenz-client-reporting-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-reporting-0.2.0/examples/client.py` & `frequenz-client-reporting-0.3.0/examples/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,52 +45,56 @@
     )
     parser.add_argument(
         "--end",
         type=datetime.fromisoformat,
         help="End datetime in YYYY-MM-DDTHH:MM:SS format",
         required=True,
     )
+    parser.add_argument("--resolution", type=int, help="Resolution", default=None)
     parser.add_argument("--psize", type=int, help="Page size", default=100)
     parser.add_argument(
         "--display", choices=["iter", "df", "dict"], help="Display format", default="df"
     )
     args = parser.parse_args()
     asyncio.run(
         run(
             args.mid,
             args.cid,
             args.metrics,
             args.start,
             args.end,
+            args.resolution,
             page_size=args.psize,
             service_address=args.url,
             display=args.display,
         )
     )
 
 
-# pylint: disable=too-many-arguments
+# pylint: disable=too-many-arguments, too-many-locals
 async def run(
     microgrid_id: int,
     component_id: int,
     metric_names: list[str],
     start_dt: datetime,
     end_dt: datetime,
+    resolution: int,
     page_size: int,
     service_address: str,
     display: str,
 ) -> None:
     """Test the ReportingApiClient.
 
     Args:
         microgrid_id: microgrid ID
         component_id: component ID
         metric_names: list of metric names
         start_dt: start datetime
         end_dt: end datetime
+        resolution: resampling resolution in sec
         page_size: page size
         service_address: service address
         display: display format
 
     Raises:
         ValueError: if display format is invalid
     """
@@ -108,14 +112,15 @@
         """
         return client.list_single_component_data(
             microgrid_id=microgrid_id,
             component_id=component_id,
             metrics=metrics,
             start_dt=start_dt,
             end_dt=end_dt,
+            resolution=resolution,
             page_size=page_size,
         )
 
     if display == "iter":
         print("########################################################")
         print("Iterate over single metric generator")
         async for sample in data_iter():
```

### Comparing `frequenz-client-reporting-0.2.0/pyproject.toml` & `frequenz-client-reporting-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 dev-flake8 = [
   "flake8 == 6.1.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.3.2",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 23.9.1", "isort == 5.12.0"]
+dev-formatting = ["black == 24.4.2", "isort == 5.12.0"]
 dev-mkdocs = [
-  "black == 23.9.1",
+  "black == 24.4.2",
   "Markdown==3.4.4",
   "mike == 2.0.0",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.4",
   "mkdocs-material == 9.3.1",
   "mkdocstrings[python] == 0.23.0",
@@ -60,15 +60,15 @@
   "mypy == 1.5.1",
   "types-Markdown == 3.4.2.10",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-reporting[dev-mkdocs,dev-noxfile,dev-pytest]",
   "pandas-stubs >= 2, < 3",  # Only required for example
 ]
 dev-noxfile = [
-  "nox == 2023.4.22",
+  "nox == 2024.4.15",
   "frequenz-repo-config[lib] == 0.9.1",
 ]
 dev-pylint = [
   "pylint == 3.0.2",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-reporting[dev-mkdocs,dev-noxfile,dev-pytest]",
   "pandas >= 2, < 3",  # Only required for example
```

### Comparing `frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/_client.py` & `frequenz-client-reporting-0.3.0/src/frequenz/client/reporting/_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 )
 from frequenz.api.reporting.v1.reporting_pb2 import (
     ListMicrogridComponentsDataRequest as PBListMicrogridComponentsDataRequest,
 )
 from frequenz.api.reporting.v1.reporting_pb2 import (
     ListMicrogridComponentsDataResponse as PBListMicrogridComponentsDataResponse,
 )
+from frequenz.api.reporting.v1.reporting_pb2 import (
+    ResamplingOptions as PBResamplingOptions,
+)
 from frequenz.api.reporting.v1.reporting_pb2 import TimeFilter as PBTimeFilter
 from frequenz.api.reporting.v1.reporting_pb2_grpc import ReportingStub
 from frequenz.client.common.metric import Metric
 from google.protobuf.timestamp_pb2 import Timestamp as PBTimestamp
 
 # pylint: enable=no-name-in-module
 
@@ -126,59 +129,64 @@
         self,
         *,
         microgrid_id: int,
         component_id: int,
         metrics: Metric | list[Metric],
         start_dt: datetime,
         end_dt: datetime,
+        resolution: int | None,
         page_size: int = 1000,
     ) -> AsyncIterator[MetricSample]:
         """Iterate over the data for a single metric.
 
         Args:
             microgrid_id: The microgrid ID.
             component_id: The component ID.
             metrics: The metric name or list of metric names.
             start_dt: The start date and time.
             end_dt: The end date and time.
+            resolution: The resampling resolution for the data, represented in seconds.
             page_size: The page size.
 
         Yields:
             A named tuple with the following fields:
             * timestamp: The timestamp of the metric sample.
             * value: The metric value.
         """
         async for page in self._list_microgrid_components_data_pages(
             microgrid_components=[(microgrid_id, [component_id])],
             metrics=[metrics] if isinstance(metrics, Metric) else metrics,
             start_dt=start_dt,
             end_dt=end_dt,
+            resolution=resolution,
             page_size=page_size,
         ):
             for entry in page:
                 yield entry
 
     # pylint: disable=too-many-arguments
     async def list_microgrid_components_data(
         self,
         *,
         microgrid_components: list[tuple[int, list[int]]],
         metrics: Metric | list[Metric],
         start_dt: datetime,
         end_dt: datetime,
+        resolution: int | None,
         page_size: int = 1000,
     ) -> AsyncIterator[MetricSample]:
         """Iterate over the data for multiple microgrids and components.
 
         Args:
             microgrid_components: List of tuples where each tuple contains
                                   microgrid ID and corresponding component IDs.
             metrics: The metric name or list of metric names.
             start_dt: The start date and time.
             end_dt: The end date and time.
+            resolution: The resampling resolution for the data, represented in seconds.
             page_size: The page size.
 
         Yields:
             A named tuple with the following fields:
             * microgrid_id: The microgrid ID.
             * component_id: The component ID.
             * metric: The metric name.
@@ -186,39 +194,42 @@
             * value: The metric value.
         """
         async for page in self._list_microgrid_components_data_pages(
             microgrid_components=microgrid_components,
             metrics=[metrics] if isinstance(metrics, Metric) else metrics,
             start_dt=start_dt,
             end_dt=end_dt,
+            resolution=resolution,
             page_size=page_size,
         ):
             for entry in page:
                 yield entry
 
     # pylint: disable=too-many-arguments
     async def _list_microgrid_components_data_pages(
         self,
         *,
         microgrid_components: list[tuple[int, list[int]]],
         metrics: list[Metric],
         start_dt: datetime,
         end_dt: datetime,
-        page_size: int = 1000,
+        resolution: int | None,
+        page_size: int,
     ) -> AsyncIterator[ComponentsDataPage]:
         """Iterate over the pages of microgrid components data.
 
         Note: This does not yet support resampling or aggregating the data. It
         also does not yet support fetching bound and state data.
 
         Args:
             microgrid_components: A list of tuples of microgrid IDs and component IDs.
             metrics: A list of metrics.
             start_dt: The start date and time.
             end_dt: The end date and time.
+            resolution: The resampling resolution for the data, represented in seconds.
             page_size: The page size.
 
         Yields:
             A ComponentsDataPage object of microgrid components data.
         """
         microgrid_components_pb = [
             PBMicrogridComponentIDs(microgrid_id=mid, component_ids=cids)
@@ -233,14 +244,15 @@
         time_filter = PBTimeFilter(
             start=dt2ts(start_dt),
             end=dt2ts(end_dt),
         )
 
         list_filter = PBListMicrogridComponentsDataRequest.ListFilter(
             time_filter=time_filter,
+            resampling_options=PBResamplingOptions(resolution=resolution),
         )
 
         metrics_pb = [metric.to_proto() for metric in metrics]
 
         page_token = None
 
         while True:
```

### Comparing `frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/requires.txt` & `frequenz-client-reporting-0.3.0/src/frequenz_client_reporting.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 flake8==6.1.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.3.2
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==23.9.1
+black==24.4.2
 isort==5.12.0
 
 [dev-mkdocs]
-black==23.9.1
+black==24.4.2
 Markdown==3.4.4
 mike==2.0.0
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mkdocs-macros-plugin==1.0.4
 mkdocs-material==9.3.1
 mkdocstrings[python]==0.23.0
@@ -30,15 +30,15 @@
 [dev-mypy]
 mypy==1.5.1
 types-Markdown==3.4.2.10
 frequenz-client-reporting[dev-mkdocs,dev-noxfile,dev-pytest]
 pandas-stubs<3,>=2
 
 [dev-noxfile]
-nox==2023.4.22
+nox==2024.4.15
 frequenz-repo-config[lib]==0.9.1
 
 [dev-pylint]
 pylint==3.0.2
 frequenz-client-reporting[dev-mkdocs,dev-noxfile,dev-pytest]
 pandas<3,>=2
```


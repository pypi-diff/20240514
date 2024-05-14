# Comparing `tmp/csbschema-1.1.1.tar.gz` & `tmp/csbschema-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csbschema-1.1.1.tar", last modified: Fri Aug  4 20:16:47 2023, max compression
+gzip compressed data, was "csbschema-1.1.2.tar", last modified: Tue May 14 13:27:00 2024, max compression
```

## Comparing `csbschema-1.1.1.tar` & `csbschema-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.234769 csbschema-1.1.1/
--rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.1.1/LICENSE.txt
--rw-r--r--   0 miles      (505) staff       (20)      433 2023-08-04 20:13:07.000000 csbschema-1.1.1/MANIFEST.in
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-04 20:16:47.234655 csbschema-1.1.1/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.1.1/README.md
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.231333 csbschema-1.1.1/csbschema/
--rw-r--r--   0 miles      (505) staff       (20)     2041 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/__init__.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.232574 csbschema-1.1.1/csbschema/command/
--rw-r--r--   0 miles      (505) staff       (20)      285 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)     1368 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/__main__.py
--rw-r--r--   0 miles      (505) staff       (20)     1234 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/validate.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.234534 csbschema-1.1.1/csbschema/data/
--rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    27028 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    24735 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)    24283 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_2_0-BETA.json
--rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    24608 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)    21489 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.1.1/csbschema/data/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)    32476 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/validators.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.232003 csbschema-1.1.1/csbschema.egg-info/
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)      780 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/SOURCES.txt
--rw-r--r--   0 miles      (505) staff       (20)        1 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/dependency_links.txt
--rw-r--r--   0 miles      (505) staff       (20)       62 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/entry_points.txt
--rw-r--r--   0 miles      (505) staff       (20)      135 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/requires.txt
--rw-r--r--   0 miles      (505) staff       (20)       10 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/top_level.txt
--rw-r--r--   0 miles      (505) staff       (20)     1059 2023-08-01 19:35:57.000000 csbschema-1.1.1/pyproject.toml
--rw-r--r--   0 miles      (505) staff       (20)       38 2023-08-04 20:16:47.234806 csbschema-1.1.1/setup.cfg
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2024-05-14 13:27:00.588613 csbschema-1.1.2/
+-rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.1.2/LICENSE.txt
+-rw-r--r--   0 miles      (505) staff       (20)      543 2024-05-14 13:24:37.000000 csbschema-1.1.2/MANIFEST.in
+-rw-r--r--   0 miles      (505) staff       (20)     5421 2024-05-14 13:27:00.588444 csbschema-1.1.2/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)     4477 2024-05-14 13:24:37.000000 csbschema-1.1.2/README.md
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2024-05-14 13:27:00.584460 csbschema-1.1.2/csbschema/
+-rw-r--r--   0 miles      (505) staff       (20)     2285 2024-05-14 13:24:37.000000 csbschema-1.1.2/csbschema/__init__.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2024-05-14 13:27:00.585776 csbschema-1.1.2/csbschema/command/
+-rw-r--r--   0 miles      (505) staff       (20)      285 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/command/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1368 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/command/__main__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1234 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/command/validate.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2024-05-14 13:27:00.587869 csbschema-1.1.2/csbschema/data/
+-rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    27028 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_1_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24735 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_1_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    24856 2024-05-14 13:24:37.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_1_0-2024-04.json
+-rw-r--r--   0 miles      (505) staff       (20)    24295 2024-05-14 13:24:37.000000 csbschema-1.1.2/csbschema/data/CSB-schema-3_2_0-BETA.json
+-rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24608 2023-08-01 19:35:57.000000 csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    21489 2023-08-04 20:13:07.000000 csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    21610 2024-05-14 13:24:37.000000 csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_1_0-2024-04.json
+-rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.1.2/csbschema/data/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)    34506 2024-05-14 13:24:37.000000 csbschema-1.1.2/csbschema/validators.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2024-05-14 13:27:00.588003 csbschema-1.1.2/csbschema.egg-info/
+-rw-r--r--   0 miles      (505) staff       (20)     5421 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)      874 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/SOURCES.txt
+-rw-r--r--   0 miles      (505) staff       (20)        1 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/dependency_links.txt
+-rw-r--r--   0 miles      (505) staff       (20)       62 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/entry_points.txt
+-rw-r--r--   0 miles      (505) staff       (20)      136 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/requires.txt
+-rw-r--r--   0 miles      (505) staff       (20)       10 2024-05-14 13:27:00.000000 csbschema-1.1.2/csbschema.egg-info/top_level.txt
+-rw-r--r--   0 miles      (505) staff       (20)     1060 2024-05-14 13:24:37.000000 csbschema-1.1.2/pyproject.toml
+-rw-r--r--   0 miles      (505) staff       (20)       38 2024-05-14 13:27:00.588656 csbschema-1.1.2/setup.cfg
```

### Comparing `csbschema-1.1.1/LICENSE.txt` & `csbschema-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/PKG-INFO` & `csbschema-1.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-Metadata-Version: 2.1
-Name: csbschema
-Version: 1.1.1
-Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
-Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
-Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
-Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 ![example workflow](https://github.com/CCOMJHC/csbschema/actions/workflows/flake8-and-unit-tests.yml/badge.svg)
 
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
-[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
+[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/bathy/B_12_CSB-Guidance_Document-Edition_3.0.0_Final.pdf) 
 metadata and data.
 
 # Installation
 To install from PyPi, first create a virtual environment for your project, then:
 ```shell
 pip install csbschema
 ```
@@ -31,46 +16,49 @@
 ```shell
 $ pip install .
 ```
 
 # Usage
 
 ## Convention GeoJSON CSB 3.1
-JSON files conforming to [GeoJSON CSB 3.0.0 metadata](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
-can be validated using the 3.1.0-2023-03 [schema](csbschema/data/CSB-schema-3_1_0-2023-03.json)
+JSON files conforming to [IHO B-12 Edition 3.0.0](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
+can be validated using the 3.1.0-2024-04 [schema](csbschema/data/CSB-schema-3_1_0-2024-04.json)
 (e.g., convention 'GeoJSON CSB 3.1'):
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example.json
-CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2023-03'.
+CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2024-04'.
 ```
 
 Validating an invalid document will show where in the document errors were be found:
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example-invalid.json 
-Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2023-03 failed due to the following errors: 
+Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2024-04 failed due to the following errors: 
 Path: /properties/trustedNode/convention, error: 'GeoJSON CSB 3.0' is not one of ['GeoJSON CSB 3.1']
+Path: /properties/processing/5, error: {'type': 'VerticalOffsetAnalysis', 'timestamp': '2021-11-22T16:10:09.346821Z', 'name': 'CIDCO Vertical Offset Analysis', 'version': '1.0.0', 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE', 'analysis': [{'name': 'Chi2', 'pass': True, 'parameters': {'a': 123.456, 'b': 789.012, 'target': 'Normal', 'df': 15, 'alpha': 0.05, 'pmf': {'centers': [-1.0, -0.5, 0, 0.5, 1.0], 'counts': [0, 24, 50, 120, 23, 0]}}, 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE'}]} is not valid under any of the given schemas
 Path: /features/1/properties, error: 'depth' is a required property
 Path: /features/3/properties, error: 'time' is a required property
 Path: /features/4/properties/time, error: '2016-03-03 18:41:49Z' does not match '^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$'
 Path: /properties/platform/IDNumber, error: IDNumber IMO3699580 is not valid for IDType MMSI.
 Path: /properties/platform/dataProcessed, error: dataProcessed flag is 'false', but 'processing' properties were found.
 Path: /properties/platform/uniqueID, error: uniqueID: SEAID-45f5c322-10f2-4946-802e-d5992ad36727 does not match /properties/trustedNode/uniqueVesselID: SEAID-e8c469f8-df38-11e5-b86d-9a79f06e9478
+Path: /features/1/properties, error: Observation uncertainty found, but Uncertainty metadata was not found.
 ```
 
 ## Conventions GeoJSON CSB 3.0 and XYZ CSB 3.0
 A schema for the provisional JSON encoding of B12 3.0.0 data and metadata (e.g., convention 'GeoJSON CSB 3.0') is 
 available under the schema name '3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/example_csb_geojson_file.geojson --version 3.0.0-2023-03
 ```
 
 Similarly, a metadata-only schema (e.g., convention 'XYZ CSB 3.0') is available under the schema name 
 'XYZ-3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/noaa_b12_v3_0_0_xyz_required.json --version XYZ-3.0.0-2023-03
+CSB data file 'docs/NOAA/noaa_b12_v3_0_0_xyz_required.json' successfully validated against schema 'XYZ-3.0.0-2023-03'.
 ```
 
 The metadata-only 'XYZ schema' is meant to be used for JSON metadata supplied alongside CSB data in CSV or another 
 format.
 
 ## Convention GeoJSON CSB 3.2
 A schema for a beta JSON encoding of B12 3.0.0 (e.g., convention 'GeoJSON CSB 3.2') is available under the schema
```

### Comparing `csbschema-1.1.1/README.md` & `csbschema-1.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,35 @@
+Metadata-Version: 2.1
+Name: csbschema
+Version: 1.1.2
+Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
+Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
+Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
+Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: jsonschema[format]~=4.21.0
+Provides-Extra: test
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: unittest-xml-reporting>=3.2.0; extra == "test"
+Requires-Dist: lxml>=4.6.5; extra == "test"
+Requires-Dist: pytest>=7.2.0; extra == "test"
+Requires-Dist: pytest-cov>=4.0.0; extra == "test"
+Requires-Dist: pytest-xdist>=3.0.2; extra == "test"
+
 ![example workflow](https://github.com/CCOMJHC/csbschema/actions/workflows/flake8-and-unit-tests.yml/badge.svg)
 
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
-[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
+[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/bathy/B_12_CSB-Guidance_Document-Edition_3.0.0_Final.pdf) 
 metadata and data.
 
 # Installation
 To install from PyPi, first create a virtual environment for your project, then:
 ```shell
 pip install csbschema
 ```
@@ -16,46 +38,49 @@
 ```shell
 $ pip install .
 ```
 
 # Usage
 
 ## Convention GeoJSON CSB 3.1
-JSON files conforming to [GeoJSON CSB 3.0.0 metadata](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
-can be validated using the 3.1.0-2023-03 [schema](csbschema/data/CSB-schema-3_1_0-2023-03.json)
+JSON files conforming to [IHO B-12 Edition 3.0.0](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
+can be validated using the 3.1.0-2024-04 [schema](csbschema/data/CSB-schema-3_1_0-2024-04.json)
 (e.g., convention 'GeoJSON CSB 3.1'):
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example.json
-CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2023-03'.
+CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2024-04'.
 ```
 
 Validating an invalid document will show where in the document errors were be found:
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example-invalid.json 
-Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2023-03 failed due to the following errors: 
+Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2024-04 failed due to the following errors: 
 Path: /properties/trustedNode/convention, error: 'GeoJSON CSB 3.0' is not one of ['GeoJSON CSB 3.1']
+Path: /properties/processing/5, error: {'type': 'VerticalOffsetAnalysis', 'timestamp': '2021-11-22T16:10:09.346821Z', 'name': 'CIDCO Vertical Offset Analysis', 'version': '1.0.0', 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE', 'analysis': [{'name': 'Chi2', 'pass': True, 'parameters': {'a': 123.456, 'b': 789.012, 'target': 'Normal', 'df': 15, 'alpha': 0.05, 'pmf': {'centers': [-1.0, -0.5, 0, 0.5, 1.0], 'counts': [0, 24, 50, 120, 23, 0]}}, 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE'}]} is not valid under any of the given schemas
 Path: /features/1/properties, error: 'depth' is a required property
 Path: /features/3/properties, error: 'time' is a required property
 Path: /features/4/properties/time, error: '2016-03-03 18:41:49Z' does not match '^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$'
 Path: /properties/platform/IDNumber, error: IDNumber IMO3699580 is not valid for IDType MMSI.
 Path: /properties/platform/dataProcessed, error: dataProcessed flag is 'false', but 'processing' properties were found.
 Path: /properties/platform/uniqueID, error: uniqueID: SEAID-45f5c322-10f2-4946-802e-d5992ad36727 does not match /properties/trustedNode/uniqueVesselID: SEAID-e8c469f8-df38-11e5-b86d-9a79f06e9478
+Path: /features/1/properties, error: Observation uncertainty found, but Uncertainty metadata was not found.
 ```
 
 ## Conventions GeoJSON CSB 3.0 and XYZ CSB 3.0
 A schema for the provisional JSON encoding of B12 3.0.0 data and metadata (e.g., convention 'GeoJSON CSB 3.0') is 
 available under the schema name '3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/example_csb_geojson_file.geojson --version 3.0.0-2023-03
 ```
 
 Similarly, a metadata-only schema (e.g., convention 'XYZ CSB 3.0') is available under the schema name 
 'XYZ-3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/noaa_b12_v3_0_0_xyz_required.json --version XYZ-3.0.0-2023-03
+CSB data file 'docs/NOAA/noaa_b12_v3_0_0_xyz_required.json' successfully validated against schema 'XYZ-3.0.0-2023-03'.
 ```
 
 The metadata-only 'XYZ schema' is meant to be used for JSON metadata supplied alongside CSB data in CSV or another 
 format.
 
 ## Convention GeoJSON CSB 3.2
 A schema for a beta JSON encoding of B12 3.0.0 (e.g., convention 'GeoJSON CSB 3.2') is available under the schema
```

### Comparing `csbschema-1.1.1/csbschema/__init__.py` & `csbschema-1.1.2/csbschema/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from pathlib import Path
 from typing import Tuple, Union
 
 from csbschema import validators
 
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 # Current versions
-B12_VERSION_3_1_0_2023_08 = '3.1.0-2023-08'
+B12_VERSION_3_1_0_2024_04 = '3.1.0-2024-04'
 B12_VERSION_3_0_0_2023_08 = '3.0.0-2023-08'
-XYZ_B12_VERSION_3_1_0_2023_08 = 'XYZ-3.1.0-2023-08'
+XYZ_B12_VERSION_3_1_0_2024_04 = 'XYZ-3.1.0-2024-04'
 XYZ_B12_VERSION_3_0_0_2023_08 = 'XYZ-3.0.0-2023-08'
 # Previous versions
 B12_VERSION_3_0_0_2023_03 = '3.0.0-2023-03'
 XYZ_B12_VERSION_3_0_0_2023_03 = 'XYZ-3.0.0-2023-03'
+XYZ_B12_VERSION_3_1_0_2023_08 = 'XYZ-3.1.0-2023-08'
 B12_VERSION_3_1_0_2023_03 = '3.1.0-2023-03'
+B12_VERSION_3_1_0_2023_08 = '3.1.0-2023-08'
 # Development versions
 B12_VERSION_3_2_0_BETA = '3.2.0-BETA'
 
-DEFAULT_VALIDATOR_VERSION = B12_VERSION_3_1_0_2023_08
+DEFAULT_VALIDATOR_VERSION = B12_VERSION_3_1_0_2024_04
 VALIDATORS = {
     # Current versions
-    B12_VERSION_3_1_0_2023_08: validators.validate_b12_3_1_0_2023_08,
-    XYZ_B12_VERSION_3_1_0_2023_08: validators.validate_b12_xyz_3_1_0_2023_08,
+    B12_VERSION_3_1_0_2024_04: validators.validate_b12_3_1_0_2024_04,
+    XYZ_B12_VERSION_3_1_0_2024_04: validators.validate_b12_xyz_3_1_0_2024_04,
     B12_VERSION_3_0_0_2023_08: validators.validate_b12_3_0_0_2023_08,
     XYZ_B12_VERSION_3_0_0_2023_08: validators.validate_b12_xyz_3_0_0_2023_08,
     # Previous versions
     B12_VERSION_3_0_0_2023_03: validators.validate_b12_3_0_0_2023_03,
     XYZ_B12_VERSION_3_0_0_2023_03: validators.validate_b12_xyz_3_0_0_2023_03,
+    XYZ_B12_VERSION_3_1_0_2023_08: validators.validate_b12_xyz_3_1_0_2023_08,
     B12_VERSION_3_1_0_2023_03: validators.validate_b12_3_1_0_2023_03,
+    B12_VERSION_3_1_0_2023_08: validators.validate_b12_3_1_0_2023_08,
     # Development versions
     B12_VERSION_3_2_0_BETA: validators.validate_b12_3_2_0_BETA
 }
 
 
 def validate_data(document_path: Union[Path, str], *,
                   version=DEFAULT_VALIDATOR_VERSION) -> Tuple[bool, dict]:
```

### Comparing `csbschema-1.1.1/csbschema/command/__main__.py` & `csbschema-1.1.2/csbschema/command/__main__.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/command/validate.py` & `csbschema-1.1.2/csbschema/command/validate.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.2/csbschema/data/CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-08.json` & `csbschema-1.1.2/csbschema/data/CSB-schema-3_0_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-03.json` & `csbschema-1.1.2/csbschema/data/CSB-schema-3_1_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-08.json` & `csbschema-1.1.2/csbschema/data/CSB-schema-3_1_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/CSB-schema-3_2_0-BETA.json` & `csbschema-1.1.2/csbschema/data/CSB-schema-3_2_0-BETA.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999961514778325%*

 * *Differences: {"'definitions'": "{'ProcessingTimeStampInterpolation': {'properties': {'type': {'enum': "*

 * *                  "['TimeStampInterpolation']}}}}"}*

```diff
@@ -421,15 +421,15 @@
                     "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "soundSpeed"
+                        "TimeStampInterpolation"
                     ],
                     "type": "string"
                 },
                 "version": {
                     "description": "Version of timestamp interpolation method used.",
                     "type": "string"
                 }
```

### Comparing `csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json` & `csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json` & `csbschema-1.1.2/csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.1/csbschema/validators.py` & `csbschema-1.1.2/csbschema/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -349,29 +349,34 @@
                                 context_path: str = '/properties') -> None:
     """
     Do custom semantic validation on metadata properties
     """
     # There is 'platform' metadata, in which case we'll want to do some custom validation
     platform = properties['platform']
     # Custom validator for Platform.IDNumber, which depends on Platform.IDType
-    if 'IDType' not in platform:
+    if 'IDNumber' in platform:
+        if 'IDType' not in platform:
+            errors.append(_error_factory(f"{context_path}/platform",
+                                         ("'IDType' attribute is not present, "
+                                          "but must be as attribute 'IDNumber' is present.")
+                                         ))
+        else:
+            # IDNumber and IDType are specified, validate that IDNumber is of type IDType
+            id_type = platform['IDType']
+            id_number = platform['IDNumber']
+            try:
+                if not ID_NUMBER_RE[id_type].match(id_number):
+                    errors.append(_error_factory(f"{context_path}/platform/IDNumber",
+                                                 f"IDNumber {id_number} is not valid for IDType {id_type}."))
+            except KeyError:
+                errors.append(_error_factory(f"{context_path}/platform/IDType",
+                                             f"Unknown IDType {id_type}."))
+    elif 'IDType' in platform:
         errors.append(_error_factory(f"{context_path}/platform",
-                                     "'IDType' attribute not present, but must be."))
-    id_type = platform['IDType']
-    if 'IDNumber' not in platform:
-        errors.append(_error_factory(f"{context_path}/platform",
-                                     "'IDNumber' attribute not present, but must be."))
-    id_number = platform['IDNumber']
-    try:
-        if not ID_NUMBER_RE[id_type].match(id_number):
-            errors.append(_error_factory(f"{context_path}/platform/IDNumber",
-                                         f"IDNumber {id_number} is not valid for IDType {id_type}."))
-    except KeyError:
-        errors.append(_error_factory(f"{context_path}/platform/IDType",
-                                     f"Unknown IDType {id_type}."))
+                                     "'IDType' was specified but 'IDNumber' was not."))
 
     # Add custom validator for Platform.dataProcessed, which if False, Processing entries should not be present.
     data_processed = platform.get('dataProcessed', False)
     if data_processed:
         # dataProcessed is True, so "processing" entry ought to be present
         if 'processing' not in properties:
             errors.append(_error_factory(f"{context_path}/platform/dataProcessed",
@@ -524,30 +529,56 @@
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     return validate_b12_3_1_0('CSB-schema-3_1_0-2023-03.json', document_path,
                               validate_uncertainty=False)
 
 
+def validate_b12_3_1_0_2024_04(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.1.0 CSB data and metadata against 2024-04 JSON schema
+    :param document_path: The document to validate
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_3_1_0('CSB-schema-3_1_0-2024-04.json', document_path)
+
+
 def validate_b12_3_1_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.1.0 CSB data and metadata against 2023-08 JSON schema
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     return validate_b12_3_1_0('CSB-schema-3_1_0-2023-08.json', document_path)
 
 
+def validate_b12_xyz_3_1_0_2024_04(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.1.0 CSB XYZ metadata against 2024-04 JSON schema
+    :param document_path: The document to validate
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_xyz_3_1_0('XYZ-CSB-schema-3_1_0-2024-04.json', document_path)
+
+
 def validate_b12_xyz_3_1_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
-    Validate B12 version 3.1.0 CSB data and metadata against 2023-08 JSON schema
+    Validate B12 version 3.1.0 CSB XYZ metadata against 2023-08 JSON schema
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
```

### Comparing `csbschema-1.1.1/csbschema.egg-info/PKG-INFO` & `csbschema-1.1.2/csbschema.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.1.1
+Version: 1.1.2
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: jsonschema[format]~=4.21.0
+Provides-Extra: test
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: unittest-xml-reporting>=3.2.0; extra == "test"
+Requires-Dist: lxml>=4.6.5; extra == "test"
+Requires-Dist: pytest>=7.2.0; extra == "test"
+Requires-Dist: pytest-cov>=4.0.0; extra == "test"
+Requires-Dist: pytest-xdist>=3.0.2; extra == "test"
 
 ![example workflow](https://github.com/CCOMJHC/csbschema/actions/workflows/flake8-and-unit-tests.yml/badge.svg)
 
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
-[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
+[IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/bathy/B_12_CSB-Guidance_Document-Edition_3.0.0_Final.pdf) 
 metadata and data.
 
 # Installation
 To install from PyPi, first create a virtual environment for your project, then:
 ```shell
 pip install csbschema
 ```
@@ -31,46 +38,49 @@
 ```shell
 $ pip install .
 ```
 
 # Usage
 
 ## Convention GeoJSON CSB 3.1
-JSON files conforming to [GeoJSON CSB 3.0.0 metadata](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
-can be validated using the 3.1.0-2023-03 [schema](csbschema/data/CSB-schema-3_1_0-2023-03.json)
+JSON files conforming to [IHO B-12 Edition 3.0.0](docs/IHO/CSB-Guidance_Document-Edition_3.0.pdf)
+can be validated using the 3.1.0-2024-04 [schema](csbschema/data/CSB-schema-3_1_0-2024-04.json)
 (e.g., convention 'GeoJSON CSB 3.1'):
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example.json
-CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2023-03'.
+CSB data file 'docs/IHO/b12_v3_1_0_example.json' successfully validated against schema '3.1.0-2024-04'.
 ```
 
 Validating an invalid document will show where in the document errors were be found:
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_1_0_example-invalid.json 
-Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2023-03 failed due to the following errors: 
+Validation of docs/IHO/b12_v3_1_0_example-invalid.json against schema 3.1.0-2024-04 failed due to the following errors: 
 Path: /properties/trustedNode/convention, error: 'GeoJSON CSB 3.0' is not one of ['GeoJSON CSB 3.1']
+Path: /properties/processing/5, error: {'type': 'VerticalOffsetAnalysis', 'timestamp': '2021-11-22T16:10:09.346821Z', 'name': 'CIDCO Vertical Offset Analysis', 'version': '1.0.0', 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE', 'analysis': [{'name': 'Chi2', 'pass': True, 'parameters': {'a': 123.456, 'b': 789.012, 'target': 'Normal', 'df': 15, 'alpha': 0.05, 'pmf': {'centers': [-1.0, -0.5, 0, 0.5, 1.0], 'counts': [0, 24, 50, 120, 23, 0]}}, 'reference': 'DOI:10.47366/sabia.v5n1a3', 'comment': 'FREE TEXT HERE'}]} is not valid under any of the given schemas
 Path: /features/1/properties, error: 'depth' is a required property
 Path: /features/3/properties, error: 'time' is a required property
 Path: /features/4/properties/time, error: '2016-03-03 18:41:49Z' does not match '^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$'
 Path: /properties/platform/IDNumber, error: IDNumber IMO3699580 is not valid for IDType MMSI.
 Path: /properties/platform/dataProcessed, error: dataProcessed flag is 'false', but 'processing' properties were found.
 Path: /properties/platform/uniqueID, error: uniqueID: SEAID-45f5c322-10f2-4946-802e-d5992ad36727 does not match /properties/trustedNode/uniqueVesselID: SEAID-e8c469f8-df38-11e5-b86d-9a79f06e9478
+Path: /features/1/properties, error: Observation uncertainty found, but Uncertainty metadata was not found.
 ```
 
 ## Conventions GeoJSON CSB 3.0 and XYZ CSB 3.0
 A schema for the provisional JSON encoding of B12 3.0.0 data and metadata (e.g., convention 'GeoJSON CSB 3.0') is 
 available under the schema name '3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/example_csb_geojson_file.geojson --version 3.0.0-2023-03
 ```
 
 Similarly, a metadata-only schema (e.g., convention 'XYZ CSB 3.0') is available under the schema name 
 'XYZ-3.0.0-2023-03':
 ```shell
 $ csbschema validate -f docs/NOAA/noaa_b12_v3_0_0_xyz_required.json --version XYZ-3.0.0-2023-03
+CSB data file 'docs/NOAA/noaa_b12_v3_0_0_xyz_required.json' successfully validated against schema 'XYZ-3.0.0-2023-03'.
 ```
 
 The metadata-only 'XYZ schema' is meant to be used for JSON metadata supplied alongside CSB data in CSV or another 
 format.
 
 ## Convention GeoJSON CSB 3.2
 A schema for a beta JSON encoding of B12 3.0.0 (e.g., convention 'GeoJSON CSB 3.2') is available under the schema
```

### Comparing `csbschema-1.1.1/csbschema.egg-info/SOURCES.txt` & `csbschema-1.1.2/csbschema.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 csbschema/command/__init__.py
 csbschema/command/__main__.py
 csbschema/command/validate.py
 csbschema/data/CSB-schema-3_0_0-2023-03.json
 csbschema/data/CSB-schema-3_0_0-2023-08.json
 csbschema/data/CSB-schema-3_1_0-2023-03.json
 csbschema/data/CSB-schema-3_1_0-2023-08.json
+csbschema/data/CSB-schema-3_1_0-2024-04.json
 csbschema/data/CSB-schema-3_2_0-BETA.json
 csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
 csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
 csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json
+csbschema/data/XYZ-CSB-schema-3_1_0-2024-04.json
 csbschema/data/__init__.py
```

### Comparing `csbschema-1.1.1/pyproject.toml` & `csbschema-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'jsonschema[format]>=4.6.0',
+    'jsonschema[format]~=4.21.0',
 ]
 
 [project.optional-dependencies]
 test = [
     "flake8",
     "unittest-xml-reporting>=3.2.0",
     "lxml>=4.6.5",
```


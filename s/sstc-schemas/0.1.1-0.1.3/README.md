# Comparing `tmp/sstc_schemas-0.1.1.tar.gz` & `tmp/sstc_schemas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sstc_schemas-0.1.1.tar", max compression
+gzip compressed data, was "sstc_schemas-0.1.3.tar", max compression
```

## Comparing `sstc_schemas-0.1.1.tar` & `sstc_schemas-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      846 2023-11-28 15:44:37.459585 sstc_schemas-0.1.1/README.md
--rw-r--r--   0        0        0      528 2024-05-14 13:42:44.137480 sstc_schemas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 15:44:37.349585 sstc_schemas-0.1.1/src/sstc_schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 13:45:15.267425 sstc_schemas-0.1.1/src/sstc_schemas/schemas/__init__.py
--rw-r--r--   0        0        0     1871 2024-05-14 13:41:36.807504 sstc_schemas-0.1.1/src/sstc_schemas/schemas/sites_acronyms.yaml
--rw-r--r--   0        0        0       21 2024-05-14 13:42:07.467492 sstc_schemas-0.1.1/src/sstc_schemas/version.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 sstc_schemas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      846 2023-11-28 15:44:37.459585 sstc_schemas-0.1.3/README.md
+-rw-r--r--   0        0        0      564 2024-05-14 14:53:37.544925 sstc_schemas-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 15:44:37.349585 sstc_schemas-0.1.3/src/sstc_schemas/__init__.py
+-rw-r--r--   0        0        0       74 2024-05-14 14:53:03.654874 sstc_schemas-0.1.3/src/sstc_schemas/schemas/__init__.py
+-rw-r--r--   0        0        0     1871 2024-05-14 13:41:36.807504 sstc_schemas-0.1.3/src/sstc_schemas/schemas/sites_acronyms.yaml
+-rw-r--r--   0        0        0       21 2024-05-14 14:53:31.864934 sstc_schemas-0.1.3/src/sstc_schemas/version.py
+-rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 sstc_schemas-0.1.3/PKG-INFO
```

### Comparing `sstc_schemas-0.1.1/README.md` & `sstc_schemas-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sstc_schemas-0.1.1/pyproject.toml` & `sstc_schemas-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # poetry update
 # poetry export --without-hashes --format=requirements.txt > requirements.txt 
 # twine upload -r pypi dist/*
 
 [tool.poetry]
 name = "sstc-schemas"
-version = "0.1.1"
+version = "0.1.3"
 description = ""
 authors = ["Jobelund <124563223+jobelund@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "sstc_schemas", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11.8"
 mkdocs = "^1.5.3"
 pytest = "^7.4.3"
 pyyaml = "^6.0.1"
+sstc-io = "^0.1.0"
+bgsio = "^0.1.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sstc_schemas-0.1.1/src/sstc_schemas/schemas/sites_acronyms.yaml` & `sstc_schemas-0.1.3/src/sstc_schemas/schemas/sites_acronyms.yaml`

 * *Files identical despite different names*

### Comparing `sstc_schemas-0.1.1/PKG-INFO` & `sstc_schemas-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: sstc-schemas
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: Jobelund
 Author-email: 124563223+jobelund@users.noreply.github.com
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bgsio (>=0.1.4,<0.2.0)
 Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: sstc-io (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 ![alt text](https://h24-original.s3.amazonaws.com/231546/28893673-EQhe9.png "SITES Spectral Thematic Center")
 # Swedish Infrastructure for Ecosystem Science (SITES) - Spectral | Thematic Center (SSTC)
 ["SITES spectral"](https://www.fieldsites.se/en-GB/sites-thematic-programs/sites-spectral-32634403)
```


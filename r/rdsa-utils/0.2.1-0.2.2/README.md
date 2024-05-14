# Comparing `tmp/rdsa_utils-0.2.1.tar.gz` & `tmp/rdsa_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdsa_utils-0.2.1.tar", last modified: Fri May 10 11:52:22 2024, max compression
+gzip compressed data, was "rdsa_utils-0.2.2.tar", last modified: Tue May 14 11:56:40 2024, max compression
```

## Comparing `rdsa_utils-0.2.1.tar` & `rdsa_utils-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.402714 rdsa_utils-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-10 11:52:22.402714 rdsa_utils-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.394714 rdsa_utils-0.2.1/rdsa_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.394714 rdsa_utils-0.2.1/rdsa_utils/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.394714 rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/hdfs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/impala.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/cdp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/cdp/io/pipeline_runlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/gcp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/helpers/gcp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/gcp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/io/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/gcp/io/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/helpers/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/helpers/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/methods/averaging_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/rdsa_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/rdsa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-10 11:52:22.000000 rdsa_utils-0.2.1/rdsa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 11:52:22.000000 rdsa_utils-0.2.1/rdsa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:52:22.000000 rdsa_utils-0.2.1/rdsa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 11:52:22.000000 rdsa_utils-0.2.1/rdsa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 11:52:22.000000 rdsa_utils-0.2.1/rdsa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-10 11:52:22.402714 rdsa_utils-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:52:22.398714 rdsa_utils-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-10 11:52:17.000000 rdsa_utils-0.2.1/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/hdfs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/impala.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/pipeline_runlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/gcp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/methods/averaging_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 11:56:40.276249 rdsa_utils-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/tests/test_validation.py
```

### Comparing `rdsa_utils-0.2.1/LICENSE` & `rdsa_utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/PKG-INFO` & `rdsa_utils-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,38 +20,43 @@
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pydantic>=2.6.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: google-cloud-bigquery>=3.17.2
 Requires-Dist: google-cloud-storage>=2.14.0
+Requires-Dist: boto3>=1.34.103
 Provides-Extra: dev
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.6.0; extra == "dev"
 Requires-Dist: ruff>=0.0.270; extra == "dev"
 Requires-Dist: chispa>=0.9.2; extra == "dev"
 Requires-Dist: coverage[toml]>=7.1.0; extra == "dev"
 Requires-Dist: pytest<8.0.0,>=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-lazy-fixture>=0.6.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.8.0; extra == "dev"
 Requires-Dist: pyspark==3.5.1; extra == "dev"
+Requires-Dist: moto>=5.0.7; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs>=1.4.2; extra == "doc"
 Requires-Dist: mkdocs-tech-docs-template>=0.1.2; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == "doc"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "doc"
 Requires-Dist: mkdocs-mermaid2-plugin>=1.1.1; extra == "doc"
 
 # 🧰 rdsa-utils 
 
 [![Deploy to PyPI](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml)
 [![Deploy MkDocs](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml)
 [![PyPI version](https://badge.fury.io/py/rdsa-utils.svg)](https://pypi.org/project/rdsa-utils/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdsa-utils.svg)](#)
+[![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 
 A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
 The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
 `rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
```

### Comparing `rdsa_utils-0.2.1/README.md` & `rdsa_utils-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # 🧰 rdsa-utils 
 
 [![Deploy to PyPI](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml)
 [![Deploy MkDocs](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml)
 [![PyPI version](https://badge.fury.io/py/rdsa-utils.svg)](https://pypi.org/project/rdsa-utils/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdsa-utils.svg)](#)
+[![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 
 A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
 The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
 `rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
```

### Comparing `rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/hdfs_utils.py` & `rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/hdfs_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/cdp/helpers/impala.py` & `rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/impala.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/cdp/io/input.py` & `rdsa_utils-0.2.2/rdsa_utils/cdp/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/cdp/io/output.py` & `rdsa_utils-0.2.2/rdsa_utils/cdp/io/output.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/cdp/io/pipeline_runlog.py` & `rdsa_utils-0.2.2/rdsa_utils/cdp/io/pipeline_runlog.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/exceptions.py` & `rdsa_utils-0.2.2/rdsa_utils/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,7 +28,12 @@
     pass
 
 
 class TableNotFoundError(Exception):
     """Custom exception to raise when a table to be read is not found."""
 
     pass
+
+class InvalidBucketNameError(Exception):
+    """Custom exception to raise when an AWS S3 bucket name is invalid."""
+
+    pass
```

### Comparing `rdsa_utils-0.2.1/rdsa_utils/gcp/helpers/gcp_utils.py` & `rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/gcp/io/inputs.py` & `rdsa_utils-0.2.2/rdsa_utils/gcp/io/inputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/gcp/io/outputs.py` & `rdsa_utils-0.2.2/rdsa_utils/gcp/io/outputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/helpers/pyspark.py` & `rdsa_utils-0.2.2/rdsa_utils/helpers/pyspark.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/helpers/python.py` & `rdsa_utils-0.2.2/rdsa_utils/helpers/python.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/io/config.py` & `rdsa_utils-0.2.2/rdsa_utils/io/config.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/io/input.py` & `rdsa_utils-0.2.2/rdsa_utils/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/logging.py` & `rdsa_utils-0.2.2/rdsa_utils/logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/methods/averaging_methods.py` & `rdsa_utils-0.2.2/rdsa_utils/methods/averaging_methods.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/test_utils.py` & `rdsa_utils-0.2.2/rdsa_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/typing.py` & `rdsa_utils-0.2.2/rdsa_utils/typing.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils/validation.py` & `rdsa_utils-0.2.2/rdsa_utils/validation.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/rdsa_utils.egg-info/PKG-INFO` & `rdsa_utils-0.2.2/rdsa_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,38 +20,43 @@
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pydantic>=2.6.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: google-cloud-bigquery>=3.17.2
 Requires-Dist: google-cloud-storage>=2.14.0
+Requires-Dist: boto3>=1.34.103
 Provides-Extra: dev
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.6.0; extra == "dev"
 Requires-Dist: ruff>=0.0.270; extra == "dev"
 Requires-Dist: chispa>=0.9.2; extra == "dev"
 Requires-Dist: coverage[toml]>=7.1.0; extra == "dev"
 Requires-Dist: pytest<8.0.0,>=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-lazy-fixture>=0.6.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.8.0; extra == "dev"
 Requires-Dist: pyspark==3.5.1; extra == "dev"
+Requires-Dist: moto>=5.0.7; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: mkdocs>=1.4.2; extra == "doc"
 Requires-Dist: mkdocs-tech-docs-template>=0.1.2; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == "doc"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "doc"
 Requires-Dist: mkdocs-mermaid2-plugin>=1.1.1; extra == "doc"
 
 # 🧰 rdsa-utils 
 
 [![Deploy to PyPI](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_pypi.yaml)
 [![Deploy MkDocs](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml/badge.svg?branch=main)](https://github.com/ONSdigital/rdsa-utils/actions/workflows/deploy_mkdocs.yaml)
 [![PyPI version](https://badge.fury.io/py/rdsa-utils.svg)](https://pypi.org/project/rdsa-utils/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdsa-utils.svg)](#)
+[![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 
 A suite of PySpark, Pandas, and general pipeline utils for **Reproducible Data Science and Analysis (RDSA)** projects.
 
 The RDSA team sits within the Economic Statistics Change Directorate, and uses cutting-edge data science and engineering skills to produce the next generation of economic statistics. Current priorities include overhauling legacy systems and developing new systems for key statistics. More information about work at RDSA can be found here: [Using Data Science for Next-Gen Statistics](https://dataingovernment.blog.gov.uk/2023/02/14/using-data-science-for-next-gen-statistics/).
 
 `rdsa-utils` is a Python codebase built with Python 3.8 and higher, and uses `setup.py`, `setup.cfg`, and `pyproject.toml` for dependency management and packaging.
```

### Comparing `rdsa_utils-0.2.1/rdsa_utils.egg-info/SOURCES.txt` & `rdsa_utils-0.2.2/rdsa_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 rdsa_utils.egg-info/dependency_links.txt
 rdsa_utils.egg-info/requires.txt
 rdsa_utils.egg-info/top_level.txt
 rdsa_utils/cdp/__init__.py
 rdsa_utils/cdp/helpers/__init__.py
 rdsa_utils/cdp/helpers/hdfs_utils.py
 rdsa_utils/cdp/helpers/impala.py
+rdsa_utils/cdp/helpers/s3_utils.py
 rdsa_utils/cdp/io/__init__.py
 rdsa_utils/cdp/io/input.py
 rdsa_utils/cdp/io/output.py
 rdsa_utils/cdp/io/pipeline_runlog.py
 rdsa_utils/gcp/__init__.py
 rdsa_utils/gcp/helpers/__init__.py
 rdsa_utils/gcp/helpers/gcp_utils.py
```

### Comparing `rdsa_utils-0.2.1/rdsa_utils.egg-info/requires.txt` & `rdsa_utils-0.2.2/rdsa_utils.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 more-itertools>=9.0.0
 pandas==1.5.3
 pydantic>=2.6.2
 pyyaml>=6.0.1
 tomli>=2.0.1
 google-cloud-bigquery>=3.17.2
 google-cloud-storage>=2.14.0
+boto3>=1.34.103
 
 [dev]
 bump2version>=1.0.0
 pre-commit>=2.6.0
 ruff>=0.0.270
 chispa>=0.9.2
 coverage[toml]>=7.1.0
 pytest<8.0.0,>=7.1.0
 pytest-cov>=4.0.0
 pytest-lazy-fixture>=0.6.0
 pytest-mock>=3.8.0
 pyspark==3.5.1
+moto>=5.0.7
 
 [doc]
 mkdocs>=1.4.2
 mkdocs-tech-docs-template>=0.1.2
 mkdocstrings[python]>=0.22.0
 mkdocs-git-revision-date-localized-plugin>=1.2.1
 mkdocs-jupyter>=0.24.3
```

### Comparing `rdsa_utils-0.2.1/setup.cfg` & `rdsa_utils-0.2.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	more-itertools>=9.0.0
 	pandas==1.5.3
 	pydantic>=2.6.2
 	pyyaml>=6.0.1
 	tomli>=2.0.1
 	google-cloud-bigquery>=3.17.2
 	google-cloud-storage>=2.14.0
+	boto3>=1.34.103
 
 [options.packages.find]
 where = .
 include = rdsa_utils*
 
 [options.extras_require]
 dev = 
@@ -42,14 +43,15 @@
 	chispa>=0.9.2
 	coverage[toml]>=7.1.0
 	pytest>=7.1.0, <8.0.0  # Temporarily pin pytest due to https://github.com/TvoroG/pytest-lazy-fixture/issues/65
 	pytest-cov>=4.0.0
 	pytest-lazy-fixture>=0.6.0
 	pytest-mock>=3.8.0
 	pyspark==3.5.1
+	moto>=5.0.7
 doc = 
 	mkdocs>=1.4.2
 	mkdocs-tech-docs-template>=0.1.2
 	mkdocstrings[python]>=0.22.0
 	mkdocs-git-revision-date-localized-plugin>=1.2.1
 	mkdocs-jupyter>=0.24.3
 	mkdocs-mermaid2-plugin>=1.1.1
```

### Comparing `rdsa_utils-0.2.1/tests/test_logging.py` & `rdsa_utils-0.2.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.1/tests/test_validation.py` & `rdsa_utils-0.2.2/tests/test_validation.py`

 * *Files identical despite different names*


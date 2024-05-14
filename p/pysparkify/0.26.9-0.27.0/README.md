# Comparing `tmp/pysparkify-0.26.9.tar.gz` & `tmp/pysparkify-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.26.9.tar", last modified: Sun May  5 18:40:09 2024, max compression
+gzip compressed data, was "pysparkify-0.27.0.tar", last modified: Tue May 14 14:22:33 2024, max compression
```

## Comparing `pysparkify-0.26.9.tar` & `pysparkify-0.27.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.474460 pysparkify-0.26.9/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-05 18:40:09.474460 pysparkify-0.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-05 18:40:02.000000 pysparkify-0.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.466460 pysparkify-0.26.9/pysparkify/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.470460 pysparkify-0.26.9/pysparkify/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.470460 pysparkify-0.26.9/pysparkify/lib/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/postgres_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/redshift_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/s3_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.470460 pysparkify-0.26.9/pysparkify/lib/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/postgres_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/redshift_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/s3_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.474460 pysparkify-0.26.9/pysparkify/lib/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/lib/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.474460 pysparkify-0.26.9/pysparkify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-05 18:40:02.000000 pysparkify-0.26.9/pysparkify/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:09.474460 pysparkify-0.26.9/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 18:40:09.000000 pysparkify-0.26.9/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:40:09.474460 pysparkify-0.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 18:40:02.000000 pysparkify-0.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.203404 pysparkify-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-14 14:22:33.203404 pysparkify-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-14 14:22:27.000000 pysparkify-0.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.199404 pysparkify-0.27.0/pysparkify/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.199404 pysparkify-0.27.0/pysparkify/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.199404 pysparkify-0.27.0/pysparkify/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/postgres_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/redshift_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/s3_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.203404 pysparkify-0.27.0/pysparkify/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/postgres_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/redshift_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/s3_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.203404 pysparkify-0.27.0/pysparkify/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.203404 pysparkify-0.27.0/pysparkify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 14:22:27.000000 pysparkify-0.27.0/pysparkify/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:33.203404 pysparkify-0.27.0/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 14:22:33.000000 pysparkify-0.27.0/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:22:33.203404 pysparkify-0.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 14:22:27.000000 pysparkify-0.27.0/setup.py
```

### Comparing `pysparkify-0.26.9/PKG-INFO` & `pysparkify-0.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pysparkify
-Version: 0.26.9
-Summary: Spark based ETL
-Home-page: https://github.com/raohammad/pysparkify
-Author: Hammad Aslam KHAN
-Author-email: raohammad@gmail.com
-License: MIT
-Keywords: python,pysparkify,etl,bigdata
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Requires-Dist: pyspark>=3.0.0
-Requires-Dist: pyyaml>=5.3
-
 # Introduction
 The pysparkify library facilitates data processing from diverse sources, applying transformations, and writing outcomes to various destinations. It employs the pipeline design pattern, offering a flexible and modular approach to big data data processing.
 
 Supported sources and sinks include:
 
 - Amazon S3
 - Amazon Redshift
@@ -139,7 +122,13 @@
 
 
 ## How to Contribute
 
 1. There are plenty of ways, in which implementation of new Sources and Sinks top the list
 2. Open a PR
 3. PR is reviewed and approved, included `github actions` will deploy the version directly to pypi repository
+
+
+## Sponsors
+
+The project is being sponsord by [Dataflick](https://www.dataflick.dev).
+If you are considering using this library in your projects, [please consider becoming a sponsor for continued support](mailto:raohammad@gmail.com?subject=Become%20A%20Sponsor).
```

### Comparing `pysparkify-0.26.9/pysparkify/lib/app.py` & `pysparkify-0.27.0/pysparkify/lib/app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/sink/postgres_sink.py` & `pysparkify-0.27.0/pysparkify/lib/sink/postgres_sink.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/sink/redshift_sink.py` & `pysparkify-0.27.0/pysparkify/lib/sink/redshift_sink.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/sink/sink_factory.py` & `pysparkify-0.27.0/pysparkify/lib/sink/sink_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/source/postgres_source.py` & `pysparkify-0.27.0/pysparkify/lib/source/postgres_source.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/source/redshift_source.py` & `pysparkify-0.27.0/pysparkify/lib/source/redshift_source.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/source/s3_source.py` & `pysparkify-0.27.0/pysparkify/lib/source/s3_source.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/source/source_factory.py` & `pysparkify-0.27.0/pysparkify/lib/source/source_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/lib/transformer/sql_transformer.py` & `pysparkify-0.27.0/pysparkify/lib/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify/tests/test_app.py` & `pysparkify-0.27.0/pysparkify/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.27.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.9
+Version: 0.27.0
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -139,7 +139,13 @@
 
 
 ## How to Contribute
 
 1. There are plenty of ways, in which implementation of new Sources and Sinks top the list
 2. Open a PR
 3. PR is reviewed and approved, included `github actions` will deploy the version directly to pypi repository
+
+
+## Sponsors
+
+The project is being sponsord by [Dataflick](https://www.dataflick.dev).
+If you are considering using this library in your projects, [please consider becoming a sponsor for continued support](mailto:raohammad@gmail.com?subject=Become%20A%20Sponsor).
```

### Comparing `pysparkify-0.26.9/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.27.0/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.9/setup.py` & `pysparkify-0.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.26.9',
+    version='0.27.0',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
```


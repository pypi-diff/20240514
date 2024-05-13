# Comparing `tmp/wrapica-1.0.6.tar.gz` & `tmp/wrapica-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapica-1.0.6.tar", last modified: Sun May 12 02:39:36 2024, max compression
+gzip compressed data, was "wrapica-1.0.7.tar", last modified: Mon May 13 23:22:29 2024, max compression
```

## Comparing `wrapica-1.0.6.tar` & `wrapica-1.0.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.829247 wrapica-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-12 02:39:18.000000 wrapica-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 02:39:36.829247 wrapica-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-12 02:39:18.000000 wrapica-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 02:39:18.000000 wrapica-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 02:39:36.829247 wrapica-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/wrapica/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/wrapica/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/wrapica/job/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/wrapica/job/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/job/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/job/functions/job_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.821247 wrapica-1.0.6/src/wrapica/libica_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/libica_exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/libica_models/
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/libica_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project/functions/project_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_analysis/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_analysis/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_analysis/functions/project_analyses_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_data/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_data/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_data/functions/project_data_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_pipelines/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/classes/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/classes/cwl_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/classes/nextflow_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.825247 wrapica-1.0.6/src/wrapica/project_pipelines/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40164 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.829247 wrapica-1.0.6/src/wrapica/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/miscell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/user_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/websocket_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-12 02:39:18.000000 wrapica-1.0.6/src/wrapica/utils/websocket_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:39:36.829247 wrapica-1.0.6/src/wrapica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 02:39:36.000000 wrapica-1.0.6/src/wrapica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-12 02:39:36.000000 wrapica-1.0.6/src/wrapica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:39:36.000000 wrapica-1.0.6/src/wrapica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-12 02:39:36.000000 wrapica-1.0.6/src/wrapica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 02:39:36.000000 wrapica-1.0.6/src/wrapica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.457916 wrapica-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 23:22:12.000000 wrapica-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-13 23:22:29.457916 wrapica-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-13 23:22:12.000000 wrapica-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 23:22:12.000000 wrapica-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 23:22:29.457916 wrapica-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.449916 wrapica-1.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.449916 wrapica-1.0.7/src/wrapica/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/job/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/job/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/job/functions/job_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/libica_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/libica_exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/libica_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/libica_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project/functions/project_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_analysis/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_analysis/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17543 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_analysis/functions/project_analyses_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_data/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_data/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63488 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_data/functions/project_data_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.453916 wrapica-1.0.7/src/wrapica/project_pipelines/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/classes/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/classes/cwl_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/classes/nextflow_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.457916 wrapica-1.0.7/src/wrapica/project_pipelines/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40164 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.457916 wrapica-1.0.7/src/wrapica/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/miscell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/user_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/websocket_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 23:22:12.000000 wrapica-1.0.7/src/wrapica/utils/websocket_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:29.457916 wrapica-1.0.7/src/wrapica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-13 23:22:29.000000 wrapica-1.0.7/src/wrapica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-13 23:22:29.000000 wrapica-1.0.7/src/wrapica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:22:29.000000 wrapica-1.0.7/src/wrapica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-13 23:22:29.000000 wrapica-1.0.7/src/wrapica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 23:22:29.000000 wrapica-1.0.7/src/wrapica.egg-info/top_level.txt
```

### Comparing `wrapica-1.0.6/LICENSE` & `wrapica-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/PKG-INFO` & `wrapica-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.6
+Version: 1.0.7
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.6/README.md` & `wrapica-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/pyproject.toml` & `wrapica-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wrapica"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name = "Alexis Lucattini", email = "alexis.lucattini@umccr.org" },
 ]
 description = "Secondary level functions for ICAv2 based off libica"
 readme = "Readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `wrapica-1.0.6/src/wrapica/enums/__init__.py` & `wrapica-1.0.7/src/wrapica/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/job/functions/job_functions.py` & `wrapica-1.0.7/src/wrapica/job/functions/job_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/libica_models/__init__.py` & `wrapica-1.0.7/src/wrapica/libica_models/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project/functions/project_functions.py` & `wrapica-1.0.7/src/wrapica/project/functions/project_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project_analysis/__init__.py` & `wrapica-1.0.7/src/wrapica/project_analysis/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 # Import everything
 from .functions.project_analyses_functions import (
     # Project Analysis functions
     get_project_analysis_inputs,
     get_analysis_input_object_from_analysis_code,
     get_outputs_object_from_analysis_id,
     get_analysis_output_object_from_analysis_code,
+    get_cwl_outputs_json_from_analysis_id,
     get_analysis_obj,
     get_analysis_steps,
     get_analysis_log_from_analysis_step,
-    write_analysis_step_logs
+    write_analysis_step_logs,
+    abort_analysis
 )
 
 __all__ = [
     # Functions
     'get_project_analysis_inputs',
     'get_analysis_input_object_from_analysis_code',
     'get_outputs_object_from_analysis_id',
     'get_analysis_output_object_from_analysis_code',
+    'get_cwl_outputs_json_from_analysis_id',
     'get_analysis_obj',
     'get_analysis_steps',
     'get_analysis_log_from_analysis_step',
-    'write_analysis_step_logs'
+    'write_analysis_step_logs',
+    'abort_analysis'
 ]
```

### Comparing `wrapica-1.0.6/src/wrapica/project_analysis/functions/project_analyses_functions.py` & `wrapica-1.0.7/src/wrapica/project_analysis/functions/project_analyses_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -506,7 +506,53 @@
         else:
             write_websocket_to_file(
                 log_stream,
                 output_file=output_path
             )
     else:
         read_icav2_file_contents(project_id, log_data_id, output_path)
+
+
+def abort_analysis(
+    project_id: str,
+    analysis_id: str,
+) -> None:
+    """
+    Abort an analysis
+
+    :param project_id: The project id the analysis was run in
+    :param analysis_id: The analysis id to abort
+
+    :raises: ApiException
+
+    :return: None
+    :rtype: None
+
+    :Examples:
+
+    .. code-block:: python
+
+        :linenos:
+        from pathlib import Path
+        from wrapica.project_analysis import abort_analysis
+
+        # Set params
+        # Use wrapica.project.get_project_id_from_project_name
+        # If you need to convert a project_name to a project_id
+        project_id = "project_id"
+        analysis_id = "analysis_id"
+    """
+    # Get the configuration
+    configuration = get_icav2_configuration()
+
+    # Enter a context with an instance of the API client
+    with ApiClient(configuration) as api_client:
+        # Create an instance of the API class
+        api_instance = project_analysis_api.ProjectAnalysisApi(api_client)
+
+    # example passing only required values which don't have defaults set
+    try:
+        # Abort an analysis.
+        api_instance.abort_analysis(project_id, analysis_id)
+    except ApiException as e:
+        logger.error("Exception when calling ProjectAnalysisApi->abort_analysis: %s\n" % e)
+        raise ApiException
```

### Comparing `wrapica-1.0.6/src/wrapica/project_data/__init__.py` & `wrapica-1.0.7/src/wrapica/project_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     presign_cwl_directory,
     presign_cwl_directory_with_external_data_mounts,
     read_icav2_file_contents,
     read_icav2_file_contents_to_string,
     get_project_data_upload_url,
     write_icav2_file_contents,
     get_file_by_file_name_from_project_data_list,
-    project_data_copy_batch_handler
+    project_data_copy_batch_handler,
+    delete_project_data
 )
 
 __all__ = [
     # Functions
     'get_project_data_file_id_from_project_id_and_path',
     'create_data_in_project',
     'create_file_in_project',
@@ -60,9 +61,10 @@
     'presign_cwl_directory',
     'presign_cwl_directory_with_external_data_mounts',
     'read_icav2_file_contents',
     'read_icav2_file_contents_to_string',
     'get_project_data_upload_url',
     'write_icav2_file_contents',
     'get_file_by_file_name_from_project_data_list',
-    'project_data_copy_batch_handler'
+    'project_data_copy_batch_handler',
+    'delete_project_data'
 ]
```

### Comparing `wrapica-1.0.6/src/wrapica/project_data/functions/project_data_functions.py` & `wrapica-1.0.7/src/wrapica/project_data/functions/project_data_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -881,15 +881,15 @@
         data_type=data_type
     )
 
     # Check if we can pull out any items in the top directory
     if min_depth is None or min_depth <= 1:
         for data_item in data_items:
             data_item_match = name_regex_obj.match(data_item.data.details.name)
-            if data_type is not None and not data_item.data.details.data_type == data_type:
+            if data_type is not None and not DataType[data_item.data.details.data_type] == data_type:
                 continue
             if data_item_match is not None:
                 matched_data_items.append(data_item)
 
     # Otherwise look recursively
     if max_depth is None or not max_depth <= 1:
         # Listing sub folders
@@ -1877,7 +1877,50 @@
         )
     except ApiException as e:
         logger.error("Exception when calling ProjectDataApi->copy_project_data_batch: %s\n" % e)
         raise ApiException
 
     # Return the job ID for the project data copy batch
     return api_response.job
+
+
+def delete_project_data(project_id: str, data_id: str):
+    """
+    Delete a project data item using the projectData:delete endpoint
+
+    :param project_id: The project id the data belongs to
+    :param data_id: The data id we want to delete
+
+    :return: None
+    :rtype: None
+
+    :raises: ValueError, ApiException
+
+    :Examples:
+
+    .. code-block:: python
+
+        from wrapica.project_data import delete_project_data
+
+        # Use wrapica.project.get_project_id_from_project_name
+        # If you need to convert a project_name to a project_id
+
+        delete_project_data(
+            project_id="abcd-1234-efab-5678",
+            data_id="fol.abcdef1234567890"
+        )
+    """
+    # Get the configuration
+    configuration = get_icav2_configuration()
+
+    # Enter a context with an instance of the API client
+    with ApiClient(configuration) as api_client:
+        # Create an instance of the API class
+        api_instance = ProjectDataApi(api_client)
+
+    # example passing only required values which don't have defaults set
+    try:
+        # Schedule this data for deletion.
+        api_instance.delete_data(project_id, data_id)
+    except ApiException as e:
+        logger.error("Exception when calling ProjectDataApi->delete_data: %s\n" % e)
+        raise ApiException
```

### Comparing `wrapica-1.0.6/src/wrapica/project_pipelines/__init__.py` & `wrapica-1.0.7/src/wrapica/project_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project_pipelines/classes/analysis.py` & `wrapica-1.0.7/src/wrapica/project_pipelines/classes/analysis.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project_pipelines/classes/cwl_analysis.py` & `wrapica-1.0.7/src/wrapica/project_pipelines/classes/cwl_analysis.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project_pipelines/classes/nextflow_analysis.py` & `wrapica-1.0.7/src/wrapica/project_pipelines/classes/nextflow_analysis.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/project_pipelines/functions/project_pipelines_functions.py` & `wrapica-1.0.7/src/wrapica/project_pipelines/functions/project_pipelines_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/__init__.py` & `wrapica-1.0.7/src/wrapica/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/configuration.py` & `wrapica-1.0.7/src/wrapica/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/globals.py` & `wrapica-1.0.7/src/wrapica/utils/globals.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/logger.py` & `wrapica-1.0.7/src/wrapica/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/miscell.py` & `wrapica-1.0.7/src/wrapica/utils/miscell.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/subprocess_handler.py` & `wrapica-1.0.7/src/wrapica/utils/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica/utils/websocket_helpers.py` & `wrapica-1.0.7/src/wrapica/utils/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.6/src/wrapica.egg-info/PKG-INFO` & `wrapica-1.0.7/src/wrapica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.6
+Version: 1.0.7
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.6/src/wrapica.egg-info/SOURCES.txt` & `wrapica-1.0.7/src/wrapica.egg-info/SOURCES.txt`

 * *Files identical despite different names*


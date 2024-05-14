# Comparing `tmp/orch_api-0.0.1.tar.gz` & `tmp/orch_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orch_api-0.0.1.tar", last modified: Mon May 13 20:05:50 2024, max compression
+gzip compressed data, was "orch_api-0.0.2.tar", last modified: Tue May 14 08:29:12 2024, max compression
```

## Comparing `orch_api-0.0.1.tar` & `orch_api-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:50.521159 orch_api-0.0.1/
--rw-rw-rw-   0        0        0      870 2024-05-13 20:05:50.521159 orch_api-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 20:05:50.515312 orch_api-0.0.1/orch_api.egg-info/
--rw-rw-rw-   0        0        0      870 2024-05-13 20:05:49.000000 orch_api-0.0.1/orch_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-13 20:05:49.000000 orch_api-0.0.1/orch_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:05:49.000000 orch_api-0.0.1/orch_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:05:49.000000 orch_api-0.0.1/orch_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 20:05:50.529406 orch_api-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-13 18:32:59.000000 orch_api-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:29:12.056055 orch_api-0.0.2/
+-rw-rw-rw-   0        0        0      903 2024-05-14 08:29:12.047180 orch_api-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 08:29:12.047180 orch_api-0.0.2/orch_api.egg-info/
+-rw-rw-rw-   0        0        0      903 2024-05-14 08:29:11.000000 orch_api-0.0.2/orch_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-14 08:29:11.000000 orch_api-0.0.2/orch_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:29:11.000000 orch_api-0.0.2/orch_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-14 08:29:11.000000 orch_api-0.0.2/orch_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:29:11.000000 orch_api-0.0.2/orch_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:29:12.056055 orch_api-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      638 2024-05-14 08:26:57.000000 orch_api-0.0.2/setup.py
```

### Comparing `orch_api-0.0.1/PKG-INFO` & `orch_api-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: orch_api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connect to Uipath orchestrator api
 Home-page: https://github.com/foxpc-ai/orch_api
 Author: Muktadir
 Description-Content-Type: text/markdown
+Requires-Dist: requests==2.31.0
 
 # Orchestrator API Python Client
 
 This Python module provides a client for interacting with the UiPath Orchestrator API.
 
 ## Features
```

### Comparing `orch_api-0.0.1/orch_api.egg-info/PKG-INFO` & `orch_api-0.0.2/orch_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: orch_api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connect to Uipath orchestrator api
 Home-page: https://github.com/foxpc-ai/orch_api
 Author: Muktadir
 Description-Content-Type: text/markdown
+Requires-Dist: requests==2.31.0
 
 # Orchestrator API Python Client
 
 This Python module provides a client for interacting with the UiPath Orchestrator API.
 
 ## Features
```


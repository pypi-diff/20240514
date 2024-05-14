# Comparing `tmp/dock_cli-1.1.0.tar.gz` & `tmp/dock_cli-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock_cli-1.1.0.tar", last modified: Mon Apr 22 09:48:01 2024, max compression
+gzip compressed data, was "dock_cli-1.1.0rc0.tar", last modified: Thu Apr 18 01:41:43 2024, max compression
```

## Comparing `dock_cli-1.1.0.tar` & `dock_cli-1.1.0rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:48:01.200578 dock_cli-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 09:47:44.000000 dock_cli-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-22 09:48:01.200578 dock_cli-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-22 09:47:44.000000 dock_cli-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:48:01.196578 dock_cli-1.1.0/dock_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:48:01.196578 dock_cli-1.1.0/dock_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/cli/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:48:01.200578 dock_cli-1.1.0/dock_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-22 09:47:44.000000 dock_cli-1.1.0/dock_cli/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:48:01.200578 dock_cli-1.1.0/dock_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 09:48:01.000000 dock_cli-1.1.0/dock_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-22 09:47:44.000000 dock_cli-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:48:01.200578 dock_cli-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/dock_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/dock_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/cli/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/dock_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/dock_cli/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/dock_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 01:41:43.000000 dock_cli-1.1.0rc0/dock_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 01:41:26.000000 dock_cli-1.1.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:41:43.165163 dock_cli-1.1.0rc0/setup.cfg
```

### Comparing `dock_cli-1.1.0/LICENSE` & `dock_cli-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/PKG-INFO` & `dock_cli-1.1.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 1.1.0
+Version: 1.1.0rc0
 Summary: CLI for manage container applications
 Author-email: Posen <posen2101024@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Posen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dock_cli-1.1.0/README.md` & `dock_cli-1.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/cli/chart.py` & `dock_cli-1.1.0rc0/dock_cli/cli/chart.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/cli/image.py` & `dock_cli-1.1.0rc0/dock_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/main.py` & `dock_cli-1.1.0rc0/dock_cli/main.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/utils/callback.py` & `dock_cli-1.1.0rc0/dock_cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/utils/commands.py` & `dock_cli-1.1.0rc0/dock_cli/utils/commands.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/utils/helpers.py` & `dock_cli-1.1.0rc0/dock_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/utils/schema.py` & `dock_cli-1.1.0rc0/dock_cli/utils/schema.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli/utils/utils.py` & `dock_cli-1.1.0rc0/dock_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.1.0/dock_cli.egg-info/PKG-INFO` & `dock_cli-1.1.0rc0/dock_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 1.1.0
+Version: 1.1.0rc0
 Summary: CLI for manage container applications
 Author-email: Posen <posen2101024@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Posen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dock_cli-1.1.0/pyproject.toml` & `dock_cli-1.1.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dock-cli"
-version = "1.1.0"
+version = "1.1.0rc0"
 dependencies = [
   "click~=8.1.7",
 ]
 requires-python = ">=3.7"
 authors = [
   { name = "Posen", email = "posen2101024@gmail.com" },
 ]
```


# Comparing `tmp/aka-data-prep-0.0.5.tar.gz` & `tmp/aka-data-prep-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.0.5.tar", last modified: Tue May 14 07:54:50 2024, max compression
+gzip compressed data, was "aka-data-prep-0.0.6.tar", last modified: Tue May 14 08:14:53 2024, max compression
```

## Comparing `aka-data-prep-0.0.5.tar` & `aka-data-prep-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/
--rw-rw-rw-   0        0        0      190 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep/
--rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka-data-prep-0.0.5/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    18724 2024-05-14 07:53:34.000000 aka-data-prep-0.0.5/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      425 2024-05-14 07:46:36.000000 aka-data-prep-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/
+-rw-rw-rw-   0        0        0      190 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep/
+-rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka-data-prep-0.0.6/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    18735 2024-05-14 08:13:22.000000 aka-data-prep-0.0.6/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:14:54.000000 aka-data-prep-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      442 2024-05-14 08:14:20.000000 aka-data-prep-0.0.6/setup.py
```

### Comparing `aka-data-prep-0.0.5/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.0.6/aka_data_prep/aka_data_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
  
 import plotly.express as px
 import plotly.graph_objects as go
 
 import math
 from plotly.subplots import make_subplots
-
+import shap
 
 
 class aka_encoding:
     def __init__(self,df) -> None:
 
         str_col = []
         for val in df.columns:
```


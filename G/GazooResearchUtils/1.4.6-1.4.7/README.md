# Comparing `tmp/GazooResearchUtils-1.4.6.tar.gz` & `tmp/GazooResearchUtils-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.6.tar", last modified: Sat May 11 03:39:58 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.7.tar", last modified: Tue May 14 03:04:45 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.6.tar` & `GazooResearchUtils-1.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:39:58.635055 GazooResearchUtils-1.4.6/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 03:39:58.634790 GazooResearchUtils-1.4.6/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:39:58.632824 GazooResearchUtils-1.4.6/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:39:58.633292 GazooResearchUtils-1.4.6/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      119 2024-05-11 03:33:46.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:39:58.634418 GazooResearchUtils-1.4.6/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     6575 2024-05-11 03:33:39.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:39:58.634052 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 03:39:58.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 03:39:58.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 03:39:58.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 03:39:58.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 03:39:58.000000 GazooResearchUtils-1.4.6/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 03:39:58.635118 GazooResearchUtils-1.4.6/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 03:39:57.000000 GazooResearchUtils-1.4.6/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:04:45.648725 GazooResearchUtils-1.4.7/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-14 03:04:45.648446 GazooResearchUtils-1.4.7/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:04:45.646373 GazooResearchUtils-1.4.7/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:04:45.646802 GazooResearchUtils-1.4.7/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      149 2024-05-14 03:04:05.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:04:45.648084 GazooResearchUtils-1.4.7/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     7611 2024-05-14 03:03:58.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-14 03:04:45.647615 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-14 03:04:45.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-14 03:04:45.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-14 03:04:45.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-14 03:04:45.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-14 03:04:45.000000 GazooResearchUtils-1.4.7/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-14 03:04:45.648784 GazooResearchUtils-1.4.7/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-14 03:04:42.000000 GazooResearchUtils-1.4.7/setup.py
```

### Comparing `GazooResearchUtils-1.4.6/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.7/app/GazooResearchUtils/src/Analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,52 @@
 import pandas as pd
 from datetime import datetime
 from lifelines import KaplanMeierFitter
 import matplotlib.pyplot as plt
 
+def one_to_many_transformation(data):
+  """
+  Transforms from patient level analysis to target level analysis
+
+  Parameters:
+  data (DataFrame): dataframe from csv data
+
+  Returns:
+  df (DataFrame): dataframe from csv data
+  """
+  # Transformed Dataframe
+  df = pd.DataFrame()
+
+
+  # Unique Targets
+  targets = data.loc[data['field'] == 'target-id']
+  targets = targets[['mrn', 'value']]
+  targets.columns = ['mrn', 'target-id']
+  targets = targets.drop_duplicates().reset_index()
+
+  # Loop Through Targets
+  for index, row in targets.iterrows():
+    mrn = row['mrn']
+    target_id = row['target-id']
+
+    # Select Patients Tags
+    pt = data.loc[data['mrn'] == mrn]
+
+    # Remove Tags for other targets
+    other_target_ids_tag_ids = pt.loc[(pt['field'] == 'target-id') & (pt['value'] != target_id)]['tag_id'].unique().tolist()
+    # Filter out Non Target-ids
+    pt = pt[~pt['tag_id'].isin(other_target_ids_tag_ids)]
+    # Rename mrn
+    pt['mrn'] = pt['mrn'] + '-' + target_id
+
+    # Concat
+    df = pd.concat([df, pt])
+
+  return df
+
 def get_data_dictionary(data):
   """
   Returns data dictionary.
 
   Parameters:
     data (DataFrame): dataframe with csv data
```


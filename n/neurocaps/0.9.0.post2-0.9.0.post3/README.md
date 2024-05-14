# Comparing `tmp/neurocaps-0.9.0.post2.tar.gz` & `tmp/neurocaps-0.9.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.0.post2.tar", last modified: Tue May 14 17:55:37 2024, max compression
+gzip compressed data, was "neurocaps-0.9.0.post3.tar", last modified: Tue May 14 20:16:39 2024, max compression
```

## Comparing `neurocaps-0.9.0.post2.tar` & `neurocaps-0.9.0.post3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15100 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14142 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    57082 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/analysis/merge.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/analysis/standardize.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29643 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15100 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 17:55:37.000000 neurocaps-0.9.0.post2/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/tests/test_merge_dicts.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 17:55:18.000000 neurocaps-0.9.0.post2/tests/test_standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15137 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14179 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    57051 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/merge.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29643 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15137 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_merge_dicts.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.0.post2/LICENSE.md` & `neurocaps-0.9.0.post3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/PKG-INFO` & `neurocaps-0.9.0.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0.post2
+Version: 0.9.0.post3
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -166,15 +166,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics
+# Get CAP metrics; zero indicates the absence of a CAP
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
```

### Comparing `neurocaps-0.9.0.post2/README.md` & `neurocaps-0.9.0.post3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics
+# Get CAP metrics; zero indicates the absence of a CAP
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
```

### Comparing `neurocaps-0.9.0.post2/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.9.0.post3/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/analysis/cap.py` & `neurocaps-0.9.0.post3/neurocaps/analysis/cap.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,15 +616,15 @@
         Raises
         ------
         ValueError
             No valid metrics are detected in `metrics` parameter.
 
         Notes
         -----
-        The presence of NaN values for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
+        The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
         a specific CAP.
 
         References
         -----
         Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
         Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
@@ -694,15 +694,15 @@
                 distributed_list.append([subj_id,group,curr_run])
 
         for subj_id, group, curr_run in distributed_list:
             if "temporal fraction" in metrics or "counts" in metrics:
                 frequency_dict = dict(collections.Counter(predicted_subject_timeseries[subj_id][curr_run]))
                 sorted_frequency_dict = {key: frequency_dict[key] for key in sorted(list(frequency_dict.keys()))}
                 if len(sorted_frequency_dict) != len(cap_numbers):
-                    sorted_frequency_dict = {cap_number: sorted_frequency_dict[cap_number] if cap_number in sorted_frequency_dict.keys() else float("nan") for cap_number in cap_numbers}
+                    sorted_frequency_dict = {cap_number: sorted_frequency_dict[cap_number] if cap_number in sorted_frequency_dict.keys() else 0 for cap_number in cap_numbers}
                 if "temporal fraction" in metrics: 
                     proportion_dict = {key: item/(len(predicted_subject_timeseries[subj_id][curr_run])) for key, item in sorted_frequency_dict.items()}
                     # Populate Dataframe
                     df_dict["temporal fraction"].loc[len(df_dict["temporal fraction"])] = [subj_id, group, curr_run] + [items for _ , items in proportion_dict.items()]
                 if "counts" in metrics:
                     # Populate Dataframe
                     df_dict["counts"].loc[len(df_dict["counts"])] = [subj_id, group, curr_run] + [items for _ , items in sorted_frequency_dict.items()]
@@ -730,15 +730,15 @@
                     # If uninterrupted_volumes not zero, multiply elements in the list by repetition time, sum and divide
                     if len(uninterrupted_volumes) > 0:
                         if tr:
                             persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes)*tr)/(len(uninterrupted_volumes))})
                         else:
                             persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes))/(len(uninterrupted_volumes))})
                     else:
-                        persistence_dict.update({target: float("nan")})
+                        persistence_dict.update({target: 0})
                     # Reset variables
                     count = 0
                     uninterrupted_volumes = []
                 # Populate Dataframe
                 df_dict["persistence"].loc[len(df_dict["persistence"])] = [subj_id, group, curr_run] + [items for _ , items in persistence_dict.items()]
             if "transition frequency" in metrics:
                 count = 0
```

### Comparing `neurocaps-0.9.0.post2/neurocaps/analysis/merge.py` & `neurocaps-0.9.0.post3/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/analysis/standardize.py` & `neurocaps-0.9.0.post3/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.0.post3/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.0.post3/neurocaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0.post2
+Version: 0.9.0.post3
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -166,15 +166,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics
+# Get CAP metrics; zero indicates the absence of a CAP
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
```

### Comparing `neurocaps-0.9.0.post2/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.0.post3/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/pyproject.toml` & `neurocaps-0.9.0.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.9.0post2"
+version = "0.9.0post3"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.9.0.post2/tests/test_CAP.py` & `neurocaps-0.9.0.post3/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/tests/test_merge_dicts.py` & `neurocaps-0.9.0.post3/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post2/tests/test_standardize.py` & `neurocaps-0.9.0.post3/tests/test_standardize.py`

 * *Files identical despite different names*


# Comparing `tmp/neurocaps-0.8.9.tar.gz` & `tmp/neurocaps-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.8.9.tar", last modified: Fri May 10 00:26:26 2024, max compression
+gzip compressed data, was "neurocaps-0.9.0.tar", last modified: Tue May 14 03:01:07 2024, max compression
```

## Comparing `neurocaps-0.8.9.tar` & `neurocaps-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-10 00:25:35.000000 neurocaps-0.8.9/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14738 2024-05-10 00:26:26.000000 neurocaps-0.8.9/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    13847 2024-05-10 00:25:35.000000 neurocaps-0.8.9/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5249 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    50365 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/merge.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29236 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14738 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1001 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1235 2024-05-10 00:25:35.000000 neurocaps-0.8.9/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-10 00:26:26.000000 neurocaps-0.8.9/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_merge_dicts.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 02:59:55.000000 neurocaps-0.9.0/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15007 2024-05-14 03:01:07.000000 neurocaps-0.9.0/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14053 2024-05-14 02:59:55.000000 neurocaps-0.9.0/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    55573 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/merge.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29237 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15007 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1319 2024-05-14 02:59:55.000000 neurocaps-0.9.0/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 03:01:07.000000 neurocaps-0.9.0/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_merge_dicts.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_standardize.py
```

### Comparing `neurocaps-0.8.9/LICENSE.md` & `neurocaps-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/PKG-INFO` & `neurocaps-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.9
+Version: 0.9.0
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,15 +18,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
+Requires-Dist: nibabel
 Requires-Dist: nilearn==0.10.2
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
 **Still in beta but stable.**
 
@@ -104,14 +107,15 @@
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
+# Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
 from neurocaps.analysis import CAP
 
 """If an asterisk '*' is after a name, all confounds starting with the 
 term preceding the parameter will be used. in this case, all parameters 
 starting with cosine will be used."""
@@ -155,41 +159,47 @@
                             subplots=True)
 
 cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+```python
+
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
-
 ```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
 **DataFrame Output:**
 | Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
 | 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
 | 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
 | 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
 | 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
+```python
+cap_analysis.caps2surf(fwhm=1)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.8.9/README.md` & `neurocaps-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
+# Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
 from neurocaps.analysis import CAP
 
 """If an asterisk '*' is after a name, all confounds starting with the 
 term preceding the parameter will be used. in this case, all parameters 
 starting with cosine will be used."""
@@ -128,41 +129,47 @@
                             subplots=True)
 
 cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+```python
+
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
-
 ```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
 **DataFrame Output:**
 | Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
 | 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
 | 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
 | 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
 | 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
+```python
+cap_analysis.caps2surf(fwhm=1)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
@@ -172,8 +179,8 @@
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
 
 [^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
 
 [^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
 
-[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.9.0/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     if "Custom" in parcel_approach.keys():
         if call  == "TimeseriesExtractor" and "maps" not in parcel_approach["Custom"].keys():
             raise ValueError(f"For `Custom` parcel_approach, a nested key-value pair containing the key 'maps' with the value being a string specifying the location of the parcellation is needed. Example: {{'Custom' : valid_parcel_dict['Custom']}}")
         check_subkeys = ["nodes" in parcel_approach["Custom"].keys(), "regions" in parcel_approach["Custom"].keys()]
         if not all(check_subkeys):
             missing_subkeys = [["nodes", "regions"][x] for x,y in enumerate(check_subkeys) if y == False]
             error_message = f"The following subkeys haven't been detected {missing_subkeys}."
-            if call == "TimeseriesExtractor":warnings.warn(error_message + " These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
+            if call == "TimeseriesExtractor": warnings.warn(error_message + " These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
             else: 
                 custom_example = {"Custom": {"nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                                              "regions": {"Vis" : {"lh": [0,1],
                                                                    "rh": [3,4]}},
                                                                    "Hippocampus": {"lh": [2],"rh": [5]}}}
                 raise ValueError(error_message + f" These subkeys are needed for plotting. Please reassign `parcel_approach` using `self.parcel_approach` amd refer to the example structure: {custom_example}")
         if call  == "TimeseriesExtractor" and not os.path.isfile(parcel_approach["Custom"]["maps"]):
```

### Comparing `neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info, verbose, flush_print):
 
     from nilearn.maskers import NiftiLabelsMasker
     from nilearn.image import index_img, load_img
-    import pandas as pd, json, math, numpy as np, copy, warnings
+    import copy, json, math, numpy as np, pandas as pd, warnings
 
     # Intitialize subject dictionary
     subject_timeseries = {subj_id: {}}
     
     for run in run_list:
 
         run_id = "run-1" if run == None else run
```

### Comparing `neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/neurocaps/analysis/cap.py` & `neurocaps-0.9.0/neurocaps/analysis/cap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Union
-from sklearn.cluster import KMeans
+import numpy as np, re, warnings
 from kneed import KneeLocator
+from sklearn.cluster import KMeans
+from typing import Union
 from .._utils import _CAPGetter, _convert_pickle_to_dict, _check_parcel_approach
-import numpy as np, re, warnings
+
 
 class CAP(_CAPGetter):
     def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
         """
         Initialize the CAP (Co-activation Patterns) analysis class.
 
         Parameters
@@ -271,15 +272,15 @@
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
         """
-        import os, itertools
+        import itertools, os
 
         # Check parcel approach
 
         # Check if parcellation_approach is custom
         if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
             _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_caps")
 
@@ -343,20 +344,20 @@
         distributed_list = list(itertools.product(plot_options,visual_scope,self._groups.keys()))
 
         for plot_option, scope, group in distributed_list:
                 # Get correct labels depending on scope
                 if scope == "regions": 
                     if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
                         cap_dict, columns = self._region_caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]
-                    elif list(self._parcel_approach.keys())[0] == "Custom":
+                    else:
                         cap_dict, columns = self._region_caps, list(self._parcel_approach["Custom"]["regions"].keys())
                 elif scope == "nodes": 
                     if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
                         cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]
-                    elif list(self._parcel_approach.keys())[0] == "Custom":
+                    else:
                         cap_dict, columns = self._caps , [x[0] + " " + x[1] for x in list(itertools.product(["LH", "RH"],self._parcel_approach["Custom"]["regions"].keys()))]
 
                 #  Generate plot for each group
                 if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
                                                                                     output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
                 elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
                                                                             output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
@@ -382,16 +383,16 @@
                             region_caps= np.array([np.average(self._caps[group][cap][roi_indxs])])
                         else:
                             region_caps= np.hstack([region_caps, np.average(self._caps[group][cap][roi_indxs])])
 
                 self._region_caps[group].update({cap: region_caps})
     
     def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, task_title, show_figs, scope):
-        from seaborn import heatmap
         import matplotlib.pyplot as plt, os
+        from seaborn import heatmap
 
         # Nested dictionary for group
         self._outer_product[group] = {}
 
         # Create base grid for subplots
         if subplots:
             # Max five subplots per row for default
@@ -421,15 +422,15 @@
                 import collections
                 
                 # Get frequency of each major hemisphere and region in Schaefer, AAL, or Custom atlas
                 if list(self._parcel_approach.keys())[0] == "Schaefer":
                     frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
                 elif list(self._parcel_approach.keys())[0] == "AAL":
                     frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
-                elif list(self._parcel_approach.keys())[0] == "Custom":
+                else:
                     frequency_dict = {}
                     for id in columns:
                         hemisphere_id = "LH" if id.startswith("LH ") else "RH"
                         region_id = re.split("LH |RH ", id)[-1]
                         frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
                 # Get the names, which indicate the hemisphere and region
                 names_list = list(frequency_dict.keys())
@@ -517,30 +518,30 @@
             full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
         
         # Display figures
         if not show_figs: plt.close()
 
     def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
+        import matplotlib.pyplot as plt, os, pandas as pd
         from seaborn import heatmap
-        import matplotlib.pyplot as plt, pandas as pd, os
         
         # Initialize new grid
         plt.figure(figsize=plot_dict["figsize"])
 
         if scope == "regions": 
             display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]}) 
         else: 
             # Create Labels
             import collections
             if list(self._parcel_approach.keys())[0] == "Schaefer":
                 frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
             elif list(self._parcel_approach.keys())[0] == "AAL":
                 frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
-            elif list(self._parcel_approach.keys())[0] == "Custom":
+            else:
                     frequency_dict = {}
                     for id in columns:
                         hemisphere_id = "LH" if id.startswith("LH ") else "RH"
                         region_id = re.split("LH |RH ", id)[-1]
                         frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
             names_list = list(frequency_dict.keys())
             labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
@@ -625,15 +626,15 @@
         -----
         Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
         Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
         NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
         """
-        import collections, pandas as pd, os
+        import collections, os, pandas as pd
 
         metrics = [metrics] if isinstance(metrics, str) else metrics
 
         valid_metrics = ["temporal fraction", "persistence", "counts", "transition frequency"]
 
         boolean_list = [element in valid_metrics for element in metrics]
 
@@ -751,15 +752,113 @@
         if output_dir:
             for metric in df_dict.keys():
                 filename = file_name + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
                 df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
 
         if return_df:
             return df_dict
+        
+    def caps2surf(self, output_dir: str=None, show_figs: bool = True, 
+                      fwhm: float=None, return_stat_map: bool = False, **kwargs):
+        """Project CAPs back onto atlas used for spatial dimensionality reduction for visualization
+        
+        Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
+
+        Parameters
+        ----------
+        output_dir: str, default=None
+            Directory to save plots in. If None, plots will not be saved.
+        show_figs: bool, default=True
+            Display figures or not to display figures.
+        fwhm: float, defualt=None
+            Strength of spatial smoothing to apply in millimeters.
+        return_stat_map: bool, default=FAlse
+            Returns the atlas as a stat map.
+        **kwargs: dict
+            Additional parameters to pass to modify certain plot parameters. Options include "dpi", defaults to 300, "title_pad", defaults to -3,
+            "cmap", defaults to "cold_hot", "cbar_location", defaults to "bottom", "cbar_draw_border", defaults to False, "cbar_aspect", defaults to 10, "cbar_shrink", defaults 
+            to 0.2, "cbar_decimals", defaults to 0, and "cbar_pad", defaults to 0.
+            
+        Returns
+        -------
+        Nifti Stat map
+
+        Notes
+        -----
+        Assumes that atlas background label is zero.
+
+        """
+
+        import nibabel as nib, numpy as np, os
+        from nilearn import image
+        from nilearn.plotting.cm import _cmap_d 
+        from neuromaps.transforms import mni152_to_fslr
+        from neuromaps.datasets import fetch_fslr
+        from surfplot import Plot
+
+        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                         title_pad = kwargs["title_pad"] if kwargs and "title_pad" in kwargs.keys() else -3,
+                         cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "cold_hot",
+                         cbar_location = kwargs["cbar_location"] if kwargs and "cbar_location" in kwargs.keys() else "bottom",
+                         cbar_draw_border = kwargs["cbar_draw_border"] if kwargs and "cbar_draw_border" in kwargs.keys() else False,
+                         cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 10,
+                         cbar_shrink = kwargs["cbar_shrink"] if kwargs and "cbar_shrink" in kwargs.keys() else 0.2,
+                         cbar_decimals = kwargs["cbar_decimals"] if kwargs and "cbar_decimals" in kwargs.keys() else 0,
+                         cbar_pad = kwargs["cbar_pad"] if kwargs and "cbar_pad" in kwargs.keys() else 0)
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
+
+        for group in self._caps.keys():
+            for cap in self._caps[group].keys():
+                atlas = nib.load(self._parcel_approach[list(self._parcel_approach.keys())[0]]["maps"])
+                atlas_fdata = atlas.get_fdata()
+                for indx, value in enumerate(self._caps[group][cap]):
+                    actual_indx = indx + 1
+                    atlas_fdata[np.where(atlas_fdata == actual_indx)] = value
+                stat_map = nib.Nifti1Image(atlas_fdata, atlas.affine, atlas.header)
+                if fwhm != None:
+                    stat_map = image.smooth_img(stat_map, fwhm=fwhm)
+
+                # Code slightly adapted from surfplot example 2
+                gii_lh, gii_rh = mni152_to_fslr(stat_map, method="linear")
+                surfaces = fetch_fslr()
+                lh, rh = surfaces['inflated']
+                lh = str(lh) if not isinstance(lh, str) else lh
+                rh = str(rh) if not isinstance(rh, str) else rh
+                sulc_lh, sulc_rh = surfaces['sulc']
+                sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
+                sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
+                p = Plot(lh, rh)
+
+                # Add base layer
+                p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
+
+                # Add stat map layer
+                p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
+                            color_range=(round(atlas_fdata.min()), round(atlas_fdata.max())))
+
+                # Color bar
+                kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
+                        decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"])
+                fig = p.build(cbar_kws=kws)
+                fig_name = f"{group} - {cap}"
+                fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])      
+                
+                if show_figs:
+                    fig.show()
+                
+                if output_dir:
+                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}"
+                    fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
 
+        if return_stat_map:
+            return stat_map
```

### Comparing `neurocaps-0.8.9/neurocaps/analysis/merge.py` & `neurocaps-0.9.0/neurocaps/analysis/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Merge subject timeseries dictionaries or pickle files to the first dictionary or pickle file in the list.
     Repetition times from the same subject and run are merged together. The combined dicitonary will only include subjects
     that are present in all dictionaries.
 
     Parameters
     ----------
 
-    subject_timeseries_list: dict
+    subject_timeseries_list: list[dict] or list[str]
         The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
         the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
         ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
         must consist of the timeseries associated with that run.
     return_combined_dict: bool, default=True,
         Returns the merged dictionaries if True
     return_reduced_dicts: bool, default=False
```

### Comparing `neurocaps-0.8.9/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.0/neurocaps/extraction/timeseriesextractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import json, os, re, sys, warnings
 from typing import Union
 from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
-import re, os, warnings, json, sys
 
 class TimeseriesExtractor(_TimeseriesExtractorGetter):
     def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
                  parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}, use_confounds: bool=True, confound_names: list[str]=None, fd_threshold: float=None,
                  n_acompcor_separate: int=None, dummy_scans: int=None):
         """Timeseries Extractor Class
         
@@ -295,15 +295,14 @@
         Parameters
         ----------
         output_dir : str
             Directory to save the file to.
         file_name : str
             Name of the file without the "pkl" extension.
         """
-
         import pickle
 
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
         
         with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
@@ -329,15 +328,15 @@
             Whether to show figires or not to show figures
         output_dir : str
             Directory to save the file to.
         file_name : str
             Name of the file with the extension to signify the file type.
         kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include "dpi" and "figsize". If output_dir is not None and no inputs for dpi and format are given,
-            dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (8,6).
+            dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (11,5).
 
         Raises
         ------
         ValueError
             If both `roi_indx` and `region` are specified.
         AssertionError
             If `file_name` does not contain an extension to signify the file type.
@@ -373,15 +372,15 @@
         
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
             assert "." in file_name, "`file_name` must be specified if `output_dir` is specified and it must contain an extension to signify the file type."
 
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                         figsize= kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (15, 5))
+                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (11, 5))
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
         # Obtain the column indices associated with the rois; add logic for roi_indx == 0 since it would be recognized as False
```

### Comparing `neurocaps-0.8.9/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.0/neurocaps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.9
+Version: 0.9.0
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,15 +18,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
+Requires-Dist: nibabel
 Requires-Dist: nilearn==0.10.2
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
 **Still in beta but stable.**
 
@@ -104,14 +107,15 @@
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
+# Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
 from neurocaps.analysis import CAP
 
 """If an asterisk '*' is after a name, all confounds starting with the 
 term preceding the parameter will be used. in this case, all parameters 
 starting with cosine will be used."""
@@ -155,41 +159,47 @@
                             subplots=True)
 
 cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+```python
+
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
-
 ```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
 **DataFrame Output:**
 | Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
 | 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
 | 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
 | 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
 | 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
+```python
+cap_analysis.caps2surf(fwhm=1)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.8.9/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.0/neurocaps.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,13 +15,15 @@
 neurocaps/_utils/_timeseriesextractor_internals/__init__.py
 neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
 neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
 neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
 neurocaps/analysis/__init__.py
 neurocaps/analysis/cap.py
 neurocaps/analysis/merge.py
+neurocaps/analysis/standardize.py
 neurocaps/extraction/__init__.py
 neurocaps/extraction/timeseriesextractor.py
 tests/test_CAP.py
 tests/test_TimeseriesExtractor.py
 tests/test_TimeseriesExtractor_additional.py
-tests/test_merge_dicts.py
+tests/test_merge_dicts.py
+tests/test_standardize.py
```

### Comparing `neurocaps-0.8.9/pyproject.toml` & `neurocaps-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.8.9"
+version = "0.9.0"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
@@ -22,15 +22,18 @@
     "Development Status :: 4 - Beta"
 ]
 dependencies = ["numpy",
                 "pandas",
                 "matplotlib",
                 "seaborn",
                 "kneed",
+                "nibabel",
                 "nilearn == 0.10.2",
+                "surfplot",
+                "neuromaps",
                 "pybids; platform_system != 'Windows'"
                 ]
 
 [project.urls]
 Homepage = "https://github.com/donishadsmith/neurocaps"  
 
 [tool.distutils.bdist_wheel]
```

### Comparing `neurocaps-0.8.9/tests/test_CAP.py` & `neurocaps-0.9.0/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.0/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.0/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.9/tests/test_merge_dicts.py` & `neurocaps-0.9.0/tests/test_merge_dicts.py`

 * *Files identical despite different names*


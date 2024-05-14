# Comparing `tmp/neurocaps-0.9.0.tar.gz` & `tmp/neurocaps-0.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.0.tar", last modified: Tue May 14 03:01:07 2024, max compression
+gzip compressed data, was "neurocaps-0.9.0.post1.tar", last modified: Tue May 14 03:49:34 2024, max compression
```

## Comparing `neurocaps-0.9.0.tar` & `neurocaps-0.9.0.post1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 02:59:55.000000 neurocaps-0.9.0/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15007 2024-05-14 03:01:07.000000 neurocaps-0.9.0/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14053 2024-05-14 02:59:55.000000 neurocaps-0.9.0/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    55573 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/merge.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/analysis/standardize.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29237 2024-05-14 02:59:55.000000 neurocaps-0.9.0/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15007 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 03:01:06.000000 neurocaps-0.9.0/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1319 2024-05-14 02:59:55.000000 neurocaps-0.9.0/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 03:01:07.000000 neurocaps-0.9.0/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:01:07.000000 neurocaps-0.9.0/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_merge_dicts.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 02:59:56.000000 neurocaps-0.9.0/tests/test_standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15014 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14055 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    55726 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/analysis/merge.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/analysis/standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29237 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15014 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 03:49:34.000000 neurocaps-0.9.0.post1/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/tests/test_merge_dicts.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 03:49:10.000000 neurocaps-0.9.0.post1/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.0/LICENSE.md` & `neurocaps-0.9.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/PKG-INFO` & `neurocaps-0.9.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0
+Version: 0.9.0.post1
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -191,15 +191,16 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 cap_analysis.caps2surf(fwhm=1)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.0/README.md` & `neurocaps-0.9.0.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,16 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 cap_analysis.caps2surf(fwhm=1)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.0/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.0.post1/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.9.0.post1/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.0.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/analysis/cap.py` & `neurocaps-0.9.0.post1/neurocaps/analysis/cap.py`

 * *Files 1% similar despite different names*

```diff
@@ -831,17 +831,20 @@
                 sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
                 sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
                 p = Plot(lh, rh)
 
                 # Add base layer
                 p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
 
+                plot_min = -1 if round(atlas_fdata.min()) == 0 else round(atlas_fdata.min())
+                plot_max = 1 if round(atlas_fdata.max()) == 0 else round(atlas_fdata.max())
+
                 # Add stat map layer
                 p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
-                            color_range=(round(atlas_fdata.min()), round(atlas_fdata.max())))
+                            color_range=(plot_min,plot_max))
 
                 # Color bar
                 kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
                         decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"])
                 fig = p.build(cbar_kws=kws)
                 fig_name = f"{group} - {cap}"
                 fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])
```

### Comparing `neurocaps-0.9.0/neurocaps/analysis/merge.py` & `neurocaps-0.9.0.post1/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/analysis/standardize.py` & `neurocaps-0.9.0.post1/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.0.post1/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.0.post1/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0
+Version: 0.9.0.post1
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -191,15 +191,16 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 cap_analysis.caps2surf(fwhm=1)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/6241b4b7-f5ae-4bfa-99b2-9e801d5b9422)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.0/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.0.post1/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/pyproject.toml` & `neurocaps-0.9.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.9.0"
+version = "0.9.0post1"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.9.0/tests/test_CAP.py` & `neurocaps-0.9.0.post1/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.0.post1/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.0.post1/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/tests/test_merge_dicts.py` & `neurocaps-0.9.0.post1/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0/tests/test_standardize.py` & `neurocaps-0.9.0.post1/tests/test_standardize.py`

 * *Files identical despite different names*


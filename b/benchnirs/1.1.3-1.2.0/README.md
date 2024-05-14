# Comparing `tmp/benchnirs-1.1.3.tar.gz` & `tmp/benchnirs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchnirs-1.1.3.tar", last modified: Thu Nov  2 20:54:40 2023, max compression
+gzip compressed data, was "benchnirs-1.2.0.tar", last modified: Tue May 14 13:39:38 2024, max compression
```

## Comparing `benchnirs-1.1.3.tar` & `benchnirs-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 20:54:40.859445 benchnirs-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    35083 2023-11-02 20:54:33.000000 benchnirs-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10452 2023-11-02 20:54:40.859445 benchnirs-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9913 2023-11-02 20:54:33.000000 benchnirs-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-02 20:54:40.859445 benchnirs-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-11-02 20:54:33.000000 benchnirs-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 20:54:40.856445 benchnirs-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 20:54:40.857445 benchnirs-1.1.3/src/benchnirs/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-11-02 20:54:33.000000 benchnirs-1.1.3/src/benchnirs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27685 2023-11-02 20:54:33.000000 benchnirs-1.1.3/src/benchnirs/learn.py
--rw-rw-rw-   0 root         (0) root         (0)    25059 2023-11-02 20:54:33.000000 benchnirs-1.1.3/src/benchnirs/load.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2023-11-02 20:54:33.000000 benchnirs-1.1.3/src/benchnirs/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2023-11-02 20:54:33.000000 benchnirs-1.1.3/src/benchnirs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 20:54:40.858445 benchnirs-1.1.3/src/benchnirs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10452 2023-11-02 20:54:40.000000 benchnirs-1.1.3/src/benchnirs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      327 2023-11-02 20:54:40.000000 benchnirs-1.1.3/src/benchnirs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-02 20:54:40.000000 benchnirs-1.1.3/src/benchnirs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-11-02 20:54:40.000000 benchnirs-1.1.3/src/benchnirs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-02 20:54:40.000000 benchnirs-1.1.3/src/benchnirs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.836725 benchnirs-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-14 13:39:29.000000 benchnirs-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11603 2024-05-14 13:39:38.836725 benchnirs-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-14 13:39:29.000000 benchnirs-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:39:38.836725 benchnirs-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-14 13:39:29.000000 benchnirs-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.833725 benchnirs-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.835725 benchnirs-1.2.0/src/benchnirs/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48933 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/learn.py
+-rw-rw-rw-   0 root         (0) root         (0)    25059 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.836725 benchnirs-1.2.0/src/benchnirs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11603 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/top_level.txt
```

### Comparing `benchnirs-1.1.3/LICENSE` & `benchnirs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchnirs-1.1.3/PKG-INFO` & `benchnirs-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.1.3
+Version: 1.2.0
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,15 @@
 
 **Features**
 - loading of open access datasets
 - signal processing and feature extraction on fNIRS data
 - training, optimisation and evaluation of machine learning models (including deep learning)
 - production of training graphs, metrics and other useful figures for evaluation
 - benchmarking and comparison of machine learning models
+- supervised, self-supervised and transfer learning
 - much more!
 
 
 ## Documentation
 The documentation of the framework with examples can be found [here](https://hanbnrd.gitlab.io/benchnirs).
 
 
@@ -94,16 +95,16 @@
 > ```bash
 > pip install --upgrade benchnirs
 > ```
 
 
 ## Running main scripts
 - [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
 - [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
 - [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
 - [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
 
 
 ## Example
 An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
@@ -118,14 +119,25 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Extra scripts: n-back tailored
+- `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
+- `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
+- `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+
+
+## Extra scripts: transfer learning
+- `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+- `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
+
+
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
 - adding support for new **open access datasets**
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
```

### Comparing `benchnirs-1.1.3/README.md` & `benchnirs-1.2.0/src/benchnirs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: benchnirs
+Version: 1.2.0
+Summary: Benchmarking framework for machine learning with fNIRS
+Home-page: https://gitlab.com/HanBnrd/benchnirs
+Author: Johann Benerradi
+Author-email: johann.benerradi@gmail.com
+License: GNU GPLv3+
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 > Benchmarking framework for machine learning with fNIRS
 
 **Quick links**  
@@ -24,14 +40,15 @@
 
 **Features**
 - loading of open access datasets
 - signal processing and feature extraction on fNIRS data
 - training, optimisation and evaluation of machine learning models (including deep learning)
 - production of training graphs, metrics and other useful figures for evaluation
 - benchmarking and comparison of machine learning models
+- supervised, self-supervised and transfer learning
 - much more!
 
 
 ## Documentation
 The documentation of the framework with examples can be found [here](https://hanbnrd.gitlab.io/benchnirs).
 
 
@@ -78,16 +95,16 @@
 > ```bash
 > pip install --upgrade benchnirs
 > ```
 
 
 ## Running main scripts
 - [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
 - [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
 - [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
 - [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
 
 
 ## Example
 An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
@@ -102,14 +119,25 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Extra scripts: n-back tailored
+- `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
+- `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
+- `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+
+
+## Extra scripts: transfer learning
+- `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+- `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
+
+
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
 - adding support for new **open access datasets**
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
@@ -186,7 +214,9 @@
 > 	volume={8},
 > 	number={12},
 > 	pages={1486},
 > 	year={2019},
 > 	publisher={Multidisciplinary Digital Publishing Institute}
 > }
 > ```
+
+
```

### Comparing `benchnirs-1.1.3/setup.py` & `benchnirs-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="benchnirs",
-    version="1.1.3",
+    version="1.2.0",
     author="Johann Benerradi",
     author_email="johann.benerradi@gmail.com",
     description="Benchmarking framework for machine learning with fNIRS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/HanBnrd/benchnirs",
     license='GNU GPLv3+',
```

### Comparing `benchnirs-1.1.3/src/benchnirs/load.py` & `benchnirs-1.2.0/src/benchnirs/load.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.1.3/src/benchnirs/process.py` & `benchnirs-1.2.0/src/benchnirs/process.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-def process_epochs(mne_epochs, tmax=None, tslide=None, reject_criteria=None):
+def process_epochs(mne_epochs, tmax=None, tslide=None, sort=False,
+                   reject_criteria=None):
     """
     Perform processing on epochs including baseline cropping, bad epoch
     removal, label extraction and  unit conversion.
 
     Parameters
     ----------
     mne_epochs : MNE Epochs object
@@ -14,14 +15,18 @@
         initial end time.
 
     tslide : float | None
         Size of the sliding window in seconds. Will crop the epochs if ``tmax``
         is not a multiple of ``tslide``. Defaults to ``None`` for no window
         sliding.
 
+    sort : boolean
+        Whether to sort channels by type (all HbO, all HbR). Defaults to
+        ``False`` for no sorting.
+
     reject_criteria : list of floats | None
         List of the 2 peak-to-peak rejection thresholds for HbO and HbR
         channels respectively in uM. Defaults to ``None`` for no rejection.
 
     Returns
     -------
     nirs : array of shape (n_epochs, n_channels, n_times)
@@ -45,14 +50,18 @@
         epochs.drop_bad(reject=reject)
         epochs.verbose = original_verbose
 
     # Extract data
     labels = epochs.events[:, 2] - 1  # start at 0
     groups = epochs.metadata['Subject_ID'].to_numpy() - 1  # start at 0
     nirs_epochs = epochs.pick_types(stim=False, fnirs=True)
+    if sort:
+        hbo_chs = epochs.copy().pick_types(stim=False, fnirs='hbo').ch_names
+        hbr_chs = epochs.copy().pick_types(stim=False, fnirs='hbr').ch_names
+        nirs_epochs.reorder_channels(hbo_chs + hbr_chs)
     nirs = nirs_epochs.get_data()
     nirs *= 1e6  # convert from M to uM
 
     # Create sliding window
     if tslide is not None:
         sliding_size = int(tslide * nirs_epochs.info['sfreq'])
         r = nirs.shape[-1] % sliding_size
```

### Comparing `benchnirs-1.1.3/src/benchnirs/viz.py` & `benchnirs-1.2.0/src/benchnirs/viz.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.1.3/src/benchnirs.egg-info/PKG-INFO` & `benchnirs-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: benchnirs
-Version: 1.1.3
-Summary: Benchmarking framework for machine learning with fNIRS
-Home-page: https://gitlab.com/HanBnrd/benchnirs
-Author: Johann Benerradi
-Author-email: johann.benerradi@gmail.com
-License: GNU GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 > Benchmarking framework for machine learning with fNIRS
 
 **Quick links**  
@@ -40,14 +24,15 @@
 
 **Features**
 - loading of open access datasets
 - signal processing and feature extraction on fNIRS data
 - training, optimisation and evaluation of machine learning models (including deep learning)
 - production of training graphs, metrics and other useful figures for evaluation
 - benchmarking and comparison of machine learning models
+- supervised, self-supervised and transfer learning
 - much more!
 
 
 ## Documentation
 The documentation of the framework with examples can be found [here](https://hanbnrd.gitlab.io/benchnirs).
 
 
@@ -94,16 +79,16 @@
 > ```bash
 > pip install --upgrade benchnirs
 > ```
 
 
 ## Running main scripts
 - [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
 - [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
 - [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
 - [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
 
 
 ## Example
 An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
@@ -118,14 +103,25 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Extra scripts: n-back tailored
+- `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
+- `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
+- `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+
+
+## Extra scripts: transfer learning
+- `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
+- `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
+
+
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
 - adding support for new **open access datasets**
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
@@ -202,9 +198,7 @@
 > 	volume={8},
 > 	number={12},
 > 	pages={1486},
 > 	year={2019},
 > 	publisher={Multidisciplinary Digital Publishing Institute}
 > }
 > ```
-
-
```


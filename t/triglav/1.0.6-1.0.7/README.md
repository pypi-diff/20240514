# Comparing `tmp/triglav-1.0.6.tar.gz` & `tmp/triglav-1.0.7.tar.gz`

## Comparing `triglav-1.0.6.tar` & `triglav-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 triglav-1.0.6/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 triglav-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 triglav-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 triglav-1.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 triglav-1.0.6/.github/workflows/draft-pdf.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 triglav-1.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 triglav-1.0.6/docs/API.md
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 triglav-1.0.6/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0   137872 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/01_random_dataset.ipynb
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/README.md
--rw-r--r--   0        0        0   162145 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/16S_CD_stability.ipynb
--rw-r--r--   0        0        0   571249 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/16S_end_to_end.ipynb
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/stability.py
--rw-r--r--   0        0        0  1481934 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/ESV.table
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/metadata.csv
--rw-r--r--   0        0        0   507476 2020-02-02 00:00:00.000000 triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/rdp.out.tmp
--rw-r--r--   0        0        0   340299 2020-02-02 00:00:00.000000 triglav-1.0.6/paper/Figure 1.pdf
--rw-r--r--   0        0        0   313401 2020-02-02 00:00:00.000000 triglav-1.0.6/paper/Figure 2.pdf
--rw-r--r--   0        0        0    16736 2020-02-02 00:00:00.000000 triglav-1.0.6/paper/paper.bib
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 triglav-1.0.6/paper/paper.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 triglav-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 triglav-1.0.6/tests/test_triglav.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 triglav-1.0.6/tests/data/expected_output.csv
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 triglav-1.0.6/triglav/__init__.py
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 triglav-1.0.6/triglav/triglav.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 triglav-1.0.6/.gitignore
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 triglav-1.0.6/LICENSE
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 triglav-1.0.6/README.md
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 triglav-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 triglav-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 triglav-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 triglav-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 triglav-1.0.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 triglav-1.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 triglav-1.0.7/docs/API.md
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 triglav-1.0.7/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0   137872 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/01_random_dataset.ipynb
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/README.md
+-rw-r--r--   0        0        0   162145 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/16S_CD_stability.ipynb
+-rw-r--r--   0        0        0   571249 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/16S_end_to_end.ipynb
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/stability.py
+-rw-r--r--   0        0        0  1481934 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/ESV.table
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/metadata.csv
+-rw-r--r--   0        0        0   507476 2020-02-02 00:00:00.000000 triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/rdp.out.tmp
+-rw-r--r--   0        0        0   340299 2020-02-02 00:00:00.000000 triglav-1.0.7/paper/Figure 1.pdf
+-rw-r--r--   0        0        0   313401 2020-02-02 00:00:00.000000 triglav-1.0.7/paper/Figure 2.pdf
+-rw-r--r--   0        0        0    16736 2020-02-02 00:00:00.000000 triglav-1.0.7/paper/paper.bib
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 triglav-1.0.7/paper/paper.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 triglav-1.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 triglav-1.0.7/tests/test_triglav.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 triglav-1.0.7/tests/data/expected_output.csv
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 triglav-1.0.7/triglav/__init__.py
+-rw-r--r--   0        0        0    37778 2020-02-02 00:00:00.000000 triglav-1.0.7/triglav/triglav.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 triglav-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 triglav-1.0.7/LICENSE
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 triglav-1.0.7/README.md
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 triglav-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 triglav-1.0.7/PKG-INFO
```

### Comparing `triglav-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `triglav-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `triglav-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/.github/workflows/ci.yml` & `triglav-1.0.7/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,24 @@
     branches: [ main, dev ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9, 3.10, 3.11]
+        python-version: [3.10, 3.11, 3.12]
 
     steps:
     - uses: actions/checkout@v2
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniforge-variant: Mambaforge
         miniforge-version: latest
         activate-environment: Triglav
         channel-priority: strict
-        environment-file: environment.yml
         use-mamba: true
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest pytest-cov
         pip install .
```

### Comparing `triglav-1.0.6/.github/workflows/python-publish.yml` & `triglav-1.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/docs/API.md` & `triglav-1.0.7/docs/API.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/docs/CONTRIBUTING.md` & `triglav-1.0.7/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/01_random_dataset.ipynb` & `triglav-1.0.7/notebooks/01_random_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/README.md` & `triglav-1.0.7/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/16S_CD_stability.ipynb` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/16S_CD_stability.ipynb`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/16S_end_to_end.ipynb` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/16S_end_to_end.ipynb`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/stability.py` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/stability.py`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/ESV.table` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/ESV.table`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/metadata.csv` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/metadata.csv`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/notebooks/Diseased-Gut-Analysis/Diseased Gut/rdp.out.tmp` & `triglav-1.0.7/notebooks/Diseased-Gut-Analysis/Diseased Gut/rdp.out.tmp`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/paper/Figure 1.pdf` & `triglav-1.0.7/paper/Figure 1.pdf`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/paper/Figure 2.pdf` & `triglav-1.0.7/paper/Figure 2.pdf`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/paper/paper.bib` & `triglav-1.0.7/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/paper/paper.md` & `triglav-1.0.7/paper/paper.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/tests/test_triglav.py` & `triglav-1.0.7/tests/test_triglav.py`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/triglav/triglav.py` & `triglav-1.0.7/triglav/triglav.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         clf = ExtraTreesClassifier(
             self.n_estimators,
             min_samples_split=int(X_stacked.shape[0] * self.min_samples_split),
             max_features=1,
         ).fit(X_stacked, y_f)
 
         L = clf.apply(X)
-        L = OneHotEncoder(sparse=False).fit_transform(L)
+        L = OneHotEncoder(sparse_output=False).fit_transform(L)
         S = np.dot(L, L.T)
         S = S / 1024
         S = 1 - S
         return np.sqrt(S)
 
 
 ##################################################################################
```

### Comparing `triglav-1.0.6/.gitignore` & `triglav-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/LICENSE` & `triglav-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `triglav-1.0.6/README.md` & `triglav-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Triglav - Feature Selection Using Iterative Refinement
 
 [![CI](https://github.com/jrudar/Triglav/actions/workflows/ci.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/ci.yml)
-[![Draft PDF](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml)
 
 ## Overview
 
 Triglav (named after the Slavic god of divination) attempts to discover
 all relevant features using an iterative refinement approach. This
 approach is based after the method introduced in Boruta with several
 modifications:
```

### Comparing `triglav-1.0.6/pyproject.toml` & `triglav-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "triglav"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
-    {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
+    {name = "Josip Rudar", email = "joe.rudar@inspection.gc.ca"},
     {name = "Peter Kruczkiewicz"},
     {name = "G. Brian Golding"},
     {name = "Oliver Lung"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
 description = "Triglav: Iterative Refinement and Selection of Stable Features Using Shapley Values"
 keywords = [
     "ecology",
     "multivariate statistics",
     "feature selection",
     "stability selection"
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "matplotlib >= 3.4.3",
-    "numpy == 1.23.5",
+    "numpy >= 1.26",
     "scikit-learn >= 1.0.1",
     "statsmodels >= 0.12.0",
     "shap >= 0.40.0",
     "sage-importance >= 0.0.5",
     "scipy >= 1.7.3",
     "joblib >= 1.1.0",
     "imbalanced-learn >= 0.10.1"
```

### Comparing `triglav-1.0.6/PKG-INFO` & `triglav-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: triglav
-Version: 1.0.6
+Version: 1.0.7
 Summary: Triglav: Iterative Refinement and Selection of Stable Features Using Shapley Values
 Project-URL: Homepage, https://github.com/jrudar/Triglav
 Project-URL: Repository, https://github.com/jrudar/Triglav.git
 Project-URL: Bug Tracker, https://github.com/jrudar/Triglav/issues
 Author: Peter Kruczkiewicz, G. Brian Golding, Oliver Lung
-Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
+Author-email: Josip Rudar <joe.rudar@inspection.gc.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
         
         Copyright (c) 2023 Josip Rudar, Peter Kruczkiewicz, Oliver Lung, G.Brian Golding, Mehrdad Hajibabaei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,23 +33,22 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Requires-Dist: imbalanced-learn>=0.10.1
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: matplotlib>=3.4.3
-Requires-Dist: numpy==1.23.5
+Requires-Dist: numpy>=1.26
 Requires-Dist: sage-importance>=0.0.5
 Requires-Dist: scikit-learn>=1.0.1
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: shap>=0.40.0
 Requires-Dist: statsmodels>=0.12.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
@@ -60,15 +59,14 @@
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Triglav - Feature Selection Using Iterative Refinement
 
 [![CI](https://github.com/jrudar/Triglav/actions/workflows/ci.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/ci.yml)
-[![Draft PDF](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml)
 
 ## Overview
 
 Triglav (named after the Slavic god of divination) attempts to discover
 all relevant features using an iterative refinement approach. This
 approach is based after the method introduced in Boruta with several
 modifications:
```


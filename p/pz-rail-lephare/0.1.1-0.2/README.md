# Comparing `tmp/pz_rail_lephare-0.1.1.tar.gz` & `tmp/pz_rail_lephare-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_lephare-0.1.1.tar", last modified: Wed Apr 17 15:05:27 2024, max compression
+gzip compressed data, was "pz_rail_lephare-0.2.tar", last modified: Tue May 14 21:31:25 2024, max compression
```

## Comparing `pz_rail_lephare-0.1.1.tar` & `pz_rail_lephare-0.2.tar`

### file list

```diff
@@ -1,43 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/examples/LePhare_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.899948 pz_rail_lephare-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/estimation/algos/lephare.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/estimation/algos/lsst.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/rail/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/lephare/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/rail/lephare/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/tests/lephare/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.931851 pz_rail_lephare-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.923851 pz_rail_lephare-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.923851 pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.923851 pz_rail_lephare-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.923851 pz_rail_lephare-0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    30020 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/examples/LePhare_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   156144 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/examples/data/output_table_conv_test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/examples/data/output_table_conv_train.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/examples/small_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:31:25.931851 pz_rail_lephare-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.919851 pz_rail_lephare-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.919851 pz_rail_lephare-0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.919851 pz_rail_lephare-0.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/src/rail/estimation/algos/lephare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/src/rail/estimation/algos/lsst.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/src/rail/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/src/rail/lephare/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/src/rail/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-14 21:31:25.000000 pz_rail_lephare-0.2/src/rail/lephare/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/tests/data/lsst.para
+-rw-r--r--   0 runner    (1001) docker     (127)   156144 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/tests/data/output_table_conv_test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/tests/data/output_table_conv_train.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:31:25.927851 pz_rail_lephare-0.2/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 21:31:19.000000 pz_rail_lephare-0.2/tests/lephare/test_algos.py
```

### Comparing `pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_lephare-0.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/pull_request_template.md` & `pz_rail_lephare-0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/workflows/linting.yml` & `pz_rail_lephare-0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_lephare-0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/workflows/smoke-test.yml` & `pz_rail_lephare-0.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_lephare-0.2/.github/workflows/testing-and-coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
-        python -m pytest tests --cov=lephare --cov-report=xml
+        python -m pytest tests -m "not slow" --cov=lephare --cov-report=xml
     - name: Upload coverage report to codecov
       uses: codecov/codecov-action@v3
```

### Comparing `pz_rail_lephare-0.1.1/.gitignore` & `pz_rail_lephare-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.pre-commit-config.yaml` & `pz_rail_lephare-0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/.prepare_project.sh` & `pz_rail_lephare-0.2/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/LICENSE` & `pz_rail_lephare-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_lephare-0.1.1/PKG-INFO` & `pz_rail_lephare-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-lephare
-Version: 0.1.1
+Version: 0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -42,15 +42,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # pz-rail-lephare
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-lephare)
-[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
+[![PyPI](https://img.shields.io/pypi/v/pz-rail-lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
 
 ## RAIL LePHARE
 
 This package allows users to run the [LePHARE code](https://github.com/lephare-photoz/lephare/) 
 through [RAIL](https://github.com/LSSTDESC/RAIL). 
 It can be installed via pip with the following command. 
 Full documentation is available at the main [LePHARE documentation](https://lephare.readthedocs.io/en/latest/index.html).
```

### Comparing `pz_rail_lephare-0.1.1/README.md` & `pz_rail_lephare-0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pz-rail-lephare
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-lephare)
-[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
+[![PyPI](https://img.shields.io/pypi/v/pz-rail-lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
 
 ## RAIL LePHARE
 
 This package allows users to run the [LePHARE code](https://github.com/lephare-photoz/lephare/) 
 through [RAIL](https://github.com/LSSTDESC/RAIL). 
 It can be installed via pip with the following command. 
 Full documentation is available at the main [LePHARE documentation](https://lephare.readthedocs.io/en/latest/index.html).
```

### Comparing `pz_rail_lephare-0.1.1/examples/LePhare_demo.ipynb` & `pz_rail_lephare-0.2/examples/LePhare_demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999425551470589%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'Note that in the parlance of the Creation Module, "*

 * *            '"degraders" is any post-processing that occurs to the "true" sample generated by the '*

 * *            'create Engine.  This can include adding photometric errors, applying quality cuts, '*

 * *            "introducing systematic biases, etc. \\n')], delete: [6]}}, 4: {'source': {insert: "*

 * *            "[(2, 'from rail.creation.degraders.lsst_error_model import LSSTErrorModel\\n'), (3, "*

 * *            "'from rail […]*

```diff
@@ -21,15 +21,15 @@
             "source": [
                 "This notebook is built on the main rail Goldenspike example in order to demonstrate adding in the rail_relphare wrapper.\n",
                 "\n",
                 "This notebook demonstrates how to use a the various RAIL Modules to draw synthetic samples of fluxes by color, apply physical effects to them, train photo-Z estimators on the samples, test and validate the preformance of those estimators, and to use the RAIL summarization modules to obtain n(z) estimates based on the p(z) estimates.\n",
                 "\n",
                 "**Creation** \n",
                 "\n",
-                "Note that in the parlance of the Creation Module, \"degradation\" is any post-processing that occurs to the \"true\" sample generated by the create Engine.  This can include adding photometric errors, applying quality cuts, introducing systematic biases, etc. \n",
+                "Note that in the parlance of the Creation Module, \"degraders\" is any post-processing that occurs to the \"true\" sample generated by the create Engine.  This can include adding photometric errors, applying quality cuts, introducing systematic biases, etc. \n",
                 "\n",
                 "In this notebook, we will draw both test and training samples from a RAIL Engine object. Then we will demonstrate how to use RAIL degraders to apply effects to those samples.\n",
                 "\n",
                 "**Training and Estimation** \n",
                 "\n",
                 "The RAIL Informer modules \"train\" or \"inform\" models used to estimate p(z) given band fluxes (and potentially other information).\n",
                 "\n",
@@ -73,20 +73,20 @@
             "execution_count": null,
             "id": "material-funeral",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Various rail modules\n",
                 "import rail\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
-                "from rail.creation.degradation.spectroscopic_degraders import (\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.spectroscopic_degraders import (\n",
                 "    InvRedshiftIncompleteness,\n",
                 "    LineConfusion,\n",
                 ")\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
                 "from rail.creation.engines.flowEngine import FlowModeler, FlowCreator, FlowPosterior\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.core.util_stages import ColumnMapper, TableConverter\n",
                 "\n",
                 "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator\n",
                 "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator\n",
```

### Comparing `pz_rail_lephare-0.1.1/pyproject.toml` & `pz_rail_lephare-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 testpaths = [
     "tests",
 ]
 addopts = [
     "--cov=rail",
     "--cov-report=html"
 ]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+]
 
 [tool.pylint]
 disable = [
     "abstract-method",
     "invalid-name",
     "too-many-statements",
     "missing-module-docstring",
```

### Comparing `pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/PKG-INFO` & `pz_rail_lephare-0.2/src/pz_rail_lephare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-lephare
-Version: 0.1.1
+Version: 0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -42,15 +42,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # pz-rail-lephare
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-lephare)
-[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
+[![PyPI](https://img.shields.io/pypi/v/pz-rail-lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
 
 ## RAIL LePHARE
 
 This package allows users to run the [LePHARE code](https://github.com/lephare-photoz/lephare/) 
 through [RAIL](https://github.com/LSSTDESC/RAIL). 
 It can be installed via pip with the following command. 
 Full documentation is available at the main [LePHARE documentation](https://lephare.readthedocs.io/en/latest/index.html).
```

### Comparing `pz_rail_lephare-0.1.1/src/rail/estimation/algos/lephare.py` & `pz_rail_lephare-0.2/src/rail/estimation/algos/lephare.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from rail.estimation.estimator import CatEstimator, CatInformer
 from rail.core.common_params import SHARED_PARAMS
 from ceci.config import StageParameter as Param
 import os
 import lephare as lp
 import numpy as np
+from astropy.table import Table
 import qp
+import importlib
 
 
 class LephareInformer(CatInformer):
     """Inform stage for LephareEstimator
 
     This class will set templates and filters required for photoz estimation.
     """
@@ -21,117 +23,70 @@
         nzbins=SHARED_PARAMS,
         nondetect_val=SHARED_PARAMS,
         mag_limits=SHARED_PARAMS,
         bands=SHARED_PARAMS,
         err_bands=SHARED_PARAMS,
         ref_band=SHARED_PARAMS,
         redshift_col=SHARED_PARAMS,
-        lephare_config_file=Param(
-            str,
-            "{}/{}".format(os.path.dirname(os.path.abspath(__file__)), "lsst.para"),
-            msg="Path to the lephare config in .para format",
-        ),
-        star_sed=Param(
-            str,
-            "$LEPHAREDIR/examples/STAR_MOD_ALL.list",
-            msg="Path to text file containing list of star SED templates",
-        ),
-        qso_sed=Param(
-            str,
-            "$LEPHAREDIR/sed/QSO/SALVATO09/AGN_MOD.list",
-            msg="Path to text file containing list of galaxy SED templates",
-        ),
-        gal_sed=Param(
-            str,
-            "$LEPHAREDIR/examples/COSMOS_MOD.list",
-            msg="Path to text file containing list of quasar SED templates",
-        ),
-        star_mag_dict=Param(
+        lephare_config=Param(
             dict,
-            dict(
-                lib_ascii="YES",
+            lp.read_config(
+                "{}/{}".format(os.path.dirname(os.path.abspath(__file__)), "lsst.para")
             ),
-            msg="Dictionary of values sent to MagGal for stars",
+            msg="The lephare config keymap.",
+        ),
+        star_config=Param(
+            dict,
+            dict(LIB_ASCII=lp.keyword("LIB_ASCII", "YES")),
+            msg="Star config overrides.",
         ),
-        gal_mag_dict=Param(
+        gal_config=Param(
             dict,
             dict(
-                lib_ascii="YES",
-                mod_extinc="18,26,26,33,26,33,26,33",
-                extinc_law=(
+                LIB_ASCII=lp.keyword("LIB_ASCII", "YES"),
+                MOD_EXTINC=lp.keyword("MOD_EXTINC", "18,26,26,33,26,33,26,33"),
+                EXTINC_LAW=lp.keyword(
+                    "EXTINC_LAW",
                     "SMC_prevot.dat,SB_calzetti.dat,"
-                    "SB_calzetti_bump1.dat,SB_calzetti_bump2.dat"
+                    "SB_calzetti_bump1.dat,SB_calzetti_bump2.dat",
                 ),
-                em_lines="EMP_UV",
-                em_dispersion="0.5,0.75,1.,1.5,2.",
+                EM_LINES=lp.keyword("EM_LINES", "EMP_UV"),
+                EM_DISPERSION=lp.keyword("EM_DISPERSION", "0.5,0.75,1.,1.5,2."),
             ),
-            msg="Dictionary of values sent to MagGal for galaxies",
+            msg="Galaxy config overrides.",
         ),
-        qso_mag_dict=Param(
+        qso_config=Param(
             dict,
             dict(
-                lib_ascii="YES",
-                mod_extinc="0,1000",
-                eb_v="0.,0.1,0.2,0.3",
-                extinc_law="SB_calzetti.dat",
+                LIB_ASCII=lp.keyword("LIB_ASCII", "YES"),
+                MOD_EXTINC=lp.keyword("MOD_EXTINC", "0,1000"),
+                EB_V=lp.keyword("EB_V", "0.,0.1,0.2,0.3"),
+                EXTINC_LAW=lp.keyword("EXTINC_LAW", "SB_calzetti.dat"),
             ),
-            msg="Dictionary of values sent to MagGal for quasars",
+            msg="QSO config overrides.",
         ),
     )
 
     def __init__(self, args, comm=None):
         """Init function, init config stuff (COPIED from rail_bpz)"""
         CatInformer.__init__(self, args, comm=comm)
-        self.lephare_config = lp.read_config(self.config["lephare_config_file"])
+        self.lephare_config = self.config["lephare_config"]
+        # We create a run directory with the informer name
+        self.run_dir = _set_run_dir(self.config["name"])
 
     def _set_config(self, lephare_config):
         """Update the lephare config
 
         Parameters
         ==========
         lepahre_config : `dict`
             A dictionary of the lephare config keywords.
         """
         self.lephare_config = lephare_config
 
-    def _create_filter_library(self):
-        """Make the filter library files in lephare format"""
-        # load filters from config file
-        filterLib = lp.FilterSvc.from_config(self.config["lephare_config_file"])
-        # Get location to store filter files
-        filter_output = os.path.join(
-            os.environ["LEPHAREWORK"], "filt", self.lephare_config["FILTER_FILE"].value
-        )
-        # Write filter files
-        lp.write_output_filter(
-            filter_output + ".dat", filter_output + ".doc", filterLib
-        )
-
-    def _create_sed_library(self):
-        """Make the SED binary library files in lephare format.
-
-        We separately create the star, quasar and galaxy libraries.
-        """
-        sedlib = lp.Sedtolib(config_keymap=self.lephare_config)
-        sedlib.run(typ="STAR", star_sed=self.config["star_sed"])
-        sedlib.run(typ="GAL", gal_sed=self.config["gal_sed"])
-        sedlib.run(typ="QSO", qso_sed=self.config["qso_sed"])
-
-    def _create_mag_library(self):
-        """Make the magnitudes library file in lephare format.
-
-        We separately create the star, quasar and galaxy libraries.
-
-        TODO: replace hardcoded config options with class config options.
-        """
-        maglib = lp.MagGal(config_keymap=self.lephare_config)
-        maglib.run(typ="STAR", **self.config["star_mag_dict"])
-        maglib.run(typ="GAL", **self.config["gal_mag_dict"])
-        maglib.run(typ="QSO", **self.config["qso_mag_dict"])
-
     def run(self):
         """Run rail_lephare inform stage.
 
         This informer takes the config and templates and makes the inputs
         required for the run.
 
         In addition to the three lephare stages making the filter, sed, and
@@ -144,134 +99,209 @@
         else:  # pragma: no cover
             training_data = self.get_data("input")
 
         # Get number of sources
         ngal = len(training_data[self.config.ref_band])
 
         # The three main lephare specific inform tasks
-        self._create_filter_library()
-        self._create_sed_library()
-        self._create_mag_library()
+        lp.prepare(
+            self.lephare_config,
+            star_config=self.config["star_config"],
+            gal_config=self.config["gal_config"],
+            qso_config=self.config["qso_config"],
+        )
 
         # Spectroscopic redshifts
         self.szs = training_data[self.config.redshift_col]
 
+        # Run auto adapt on training sample
+        input = _rail_to_lephare_input(
+            training_data, self.config.bands, self.config.err_bands
+        )
+        if self.config["lephare_config"]["AUTO_ADAPT"].value == "YES":
+            a0, a1 = lp.calculate_offsets(self.config["lephare_config"], input)
+            offsets = [a0, a1]
+        else:
+            offsets = None
+        # We must make a string dictionary to allow pickling and saving
+        config_text_dict = dict()
+        for k in self.config["lephare_config"]:
+            config_text_dict[k] = self.config["lephare_config"][k].value
         # Give principle inform config 'model' to instance.
-        self.model = dict(lephare_config_file=self.config["lephare_config_file"])
+        self.model = dict(
+            lephare_config=config_text_dict, offsets=offsets, run_dir=self.run_dir
+        )
         self.add_data("model", self.model)
 
 
 class LephareEstimator(CatEstimator):
     """LePhare-base CatEstimator"""
 
     name = "LephareEstimator"
     config_options = CatEstimator.config_options.copy()
 
     # Add Lephare-specific configuration options here
     config_options.update(
-        zmin=SHARED_PARAMS,
-        zmax=SHARED_PARAMS,
-        nzbins=SHARED_PARAMS,
         nondetect_val=SHARED_PARAMS,
         mag_limits=SHARED_PARAMS,
         bands=SHARED_PARAMS,
         ref_band=SHARED_PARAMS,
         err_bands=SHARED_PARAMS,
         redshift_col=SHARED_PARAMS,
-        lephare_config_file=Param(
+        lephare_config=Param(
+            dict,
+            lp.read_config(
+                "{}/{}".format(os.path.dirname(os.path.abspath(__file__)), "lsst.para")
+            ),
+            msg="The lephare config keymap.",
+        ),
+        output_keys=Param(
+            list,
+            ["Z_BEST", "ZQ_BEST", "MOD_STAR"],
+            msg="The output keys to add to ancil. These must be in the output para file.",
+        ),
+        offsets=Param(
+            list,
+            [],
+            msg=(
+                "The offsets to apply to photometry. If empty "
+                "autoadapt will be run if that key is set in the config."
+            ),
+        ),
+        run_dir=Param(
             str,
-            "{}/{}".format(os.path.dirname(os.path.abspath(__file__)), "lsst.para"),
-            msg="Path to the lephare config in .para format",
+            "None",
+            msg=(
+                "Override for the LEPHAREWORK directory. If None we load it "
+                "from the model which is set during the inform stage. This "
+                "is to facilitate manually moving intermediate files."
+            ),
         ),
     )
 
     def __init__(self, args, comm=None):
         CatEstimator.__init__(self, args, comm=comm)
-        self.lephare_config = lp.read_config(self.config["lephare_config_file"])
+        self.lephare_config = self.config["lephare_config"]
         self.photz = lp.PhotoZ(self.lephare_config)
-
-    def _estimate_pdf(self, onesource):
-        """Return the pdf of a single source.
-
-        Do we want to resample on RAIL z grid?
-        """
-        # Check this is the best way to access pdf
-        pdf = onesource.pdfmap[11]  # 11 = Bayesian galaxy redshift
-        # return the PDF as an array alongside lephare native zgrid
-        return np.array(pdf.vPDF), np.array(pdf.xaxis)
-
-        # Default local parameters
-        self.config_file = "{}/{}".format(
-            os.path.dirname(os.path.abspath(__file__)), "lsst.para"
-        )
-        self.lephare_config = lp.read_config(self.config_file)
-        self.photz = lp.PhotoZ(self.lephare_config)
-        print("init")
-
-    # def open_model(self, **kwargs):
-    #     CatEstimator.open_model(self, **kwargs)
-    #     self.modeldict = self.model
-
-    def _estimate_pdf(self, onesource):
-        """Return the pdf of a single source.
-
-        Do we want to resample on RAIL z grid?
-        """
-        # Check this is the best way to access pdf
-        pdf = onesource.pdfmap[11]  # 11 = Bayesian galaxy redshift
-        # return the PDF as an array alongside lephare native zgrid
-        return np.array(pdf.vPDF), np.array(pdf.xaxis)
+        Z_STEP = self.lephare_config["Z_STEP"].value
+        self.zstep = float(Z_STEP.split(",")[0])
+        self.zmin = float(Z_STEP.split(",")[1])
+        self.zmax = float(Z_STEP.split(",")[2])
+        self.nzbins = int((self.zmax - self.zmin) / self.zstep)
+        CatEstimator.open_model(self, **self.config)
+
+        if self.config["run_dir"] == "None":
+            self.run_dir = self.model["run_dir"]
+        else:
+            self.run_dir = self.config["run_dir"]
+        _update_lephare_env(None, self.run_dir)
 
     def _process_chunk(self, start, end, data, first):
-        """Process an individual chunk of sources using lephare
+        """Process an individual chunk of sources using lephare. 
 
         Run the equivalent of zphota and get the PDF for every source.
         """
-        # write the results of estimation for this chunk of data
-        self.zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins)
-
-        nz = len(self.zgrid)
-        ng = data["redshift"].shape[0]
-        flux = np.array([data["mag_{}_lsst".format(b)] for b in "ugrizy"]).T
-        flux_err = np.array([data["mag_err_{}_lsst".format(b)] for b in "ugrizy"]).T
-        zspec = data["redshift"]
+        # Create the lephare input table
+        input = _rail_to_lephare_input(data, self.config.bands, self.config.err_bands)
+        # Set the desired offsets estimate config overide lephare config overide inform offsets
+        if self.config["offsets"]:
+            offsets = self.config["offsets"]
+        elif self.config["lephare_config"]["AUTO_ADAPT"].value == "YES":
+            a0, a1 = lp.calculate_offsets(self.config["lephare_config"], input)
+            offsets = [a0, a1]
+        elif not self.config["offsets"]:
+            offsets = self.model["offsets"]
+        output, pdfs, zgrid = lp.process(self.lephare_config, input, offsets=offsets)
+        self.zgrid = zgrid
 
-        pdfs = []  # np.zeros((ng, nz))
+        ng = data[self.config.bands[0]].shape[0]
         zmode = np.zeros(ng)
         zmean = np.zeros(ng)
-        zgrid = self.zgrid
 
-        # Loop over all ng galaxies!
-        srclist = []
         for i in range(ng):
-            oneObj = lp.onesource(i, self.photz.gridz)
-            oneObj.readsource(str(i), flux[i], flux_err[i], 63, zspec[i], " ")
-            self.photz.prep_data(oneObj)
-            srclist.append(oneObj)
-
-        # Run autoadapt to improve zero points
-        a0, a1 = self.photz.run_autoadapt(srclist)
-        offsets = ",".join(np.array(a0).astype(str))
-        offsets = "# Offsets from auto-adapt: " + offsets + "\n"
-        print(offsets)
-
-        photozlist = []
-        for i in range(ng):
-            oneObj = lp.onesource(i, self.photz.gridz)
-            oneObj.readsource(str(i), flux[i], flux_err[i], 63, zspec[i], " ")
-            self.photz.prep_data(oneObj)
-            photozlist.append(oneObj)
-
-        self.photz.run_photoz(photozlist, a0, a1)
-
-        for i in range(ng):
-            pdf, zgrid = self._estimate_pdf(photozlist[i])
-            pdfs.append(pdf)
             # Take median in case multiple probability densities are equal
             zmode[i] = np.median(
                 zgrid[np.where(pdfs[i] == np.max(pdfs[i]))[0].astype(int)]
             )
             zmean[i] = (zgrid * pdfs[i]).sum() / pdfs[i].sum()
 
         qp_dstn = qp.Ensemble(qp.interp, data=dict(xvals=zgrid, yvals=np.array(pdfs)))
-        qp_dstn.set_ancil(dict(zmode=zmode, zmean=zmean))
+        ancil = dict(zmode=zmode, zmean=zmean)
+        # Add the requested outputs.
+        for c in self.config["output_keys"]:
+            ancil[c] = np.array(output[c])
+        qp_dstn.set_ancil(ancil)
         self._do_chunk_output(qp_dstn, start, end, first)
+
+
+def _rail_to_lephare_input(data, mag_cols, mag_err_cols):
+    """Take the rail data input and convert it to that expected by lephare
+
+    Parameters
+    ==========
+    data : pandas
+        The RAIL input data chunk
+
+    Returns
+    =======
+    input : astropy.table.Table
+        The lephare input
+
+
+    """
+    ng = data["redshift"].shape[0]
+    # Make input catalogue in standard lephare format
+    input = Table()
+    try:
+        input["id"] = data["id"]
+    except KeyError:
+        input["id"] = np.arange(ng)
+    # Add all available magnitudes
+    for n in np.arange(len(mag_cols)):
+        input[mag_cols[n]] = data[mag_cols[n]].T
+        input[mag_err_cols[n]] = data[mag_err_cols[n]].T
+    # Set context to use all bands
+    input["context"] = np.sum([2**n for n in np.arange(ng)])
+    input["zspec"] = data["redshift"]
+    input["string_data"] = " "
+    return input
+
+
+def _update_lephare_env(lepharedir, lepharework):
+    """Update the environment variables and reset the lephare package.
+
+    We may be using the same Python session to run inform with different
+    settings. These produce intermediate files which are distinct and we must
+    use different runs.
+
+    This simple function updates the environment variables and reloads lephare
+    to ensure they are properly used.
+    """
+    if lepharedir is not None:
+        os.environ["LEPHAREDIR"] = lepharedir
+    if lepharework is not None:
+        os.environ["LEPHAREWORK"] = lepharework
+    importlib.reload(lp)
+
+
+def _set_run_dir(name=None, full_path=None):
+    """Create a named run if it doesn't exist otherwise set it to existing.
+
+    lephare has the functionality to set a timed or named run. In general we
+    must ensure that each inform run has a distinct run to ensure that
+    intermediate files are not overwritten.
+
+    Parameters
+    ==========
+    name : str
+        The name to set the run. If not set we use a default timestamped run.
+    full_path : str
+        If set we create a run directory wherever the user sets it.
+    """
+    if name is None:
+        run_directory = lp.dm.create_new_run()
+    elif full_path:
+        run_directory = full_path
+    else:
+        run_directory = os.path.realpath(f"{lp.dm.lephare_work_dir}/../{name}")
+    _update_lephare_env(lp.LEPHAREDIR, run_directory)
+    return run_directory
```

### Comparing `pz_rail_lephare-0.1.1/src/rail/estimation/algos/lsst.para` & `pz_rail_lephare-0.2/src/rail/estimation/algos/lsst.para`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ##############################################################################################
 ###########               CREATION OF LIBRARIES FROM SEDs List                   #############
 ########### Run : $ZPHOTDIR/source/sedtolib -t (S/Q/G) -c zphot.para             #############
 ##############################################################################################
 #
 #-------------------    STELLAR LIBRARY (ASCII SEDs)        ---------------------------       
-STAR_SED        STAR_SWIRE.list         # STAR list (full path)
+STAR_SED        sed/STAR/STAR_MOD_ALL.list         # STAR list (full path)
 STAR_LIB	LSST_STAR_BIN 		# Binary STAR LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 STAR_FSCALE	3.432E-09		# Arbitrary Flux Scale 
 #
 #-------------------    QSO LIBRARY (ASCII SEDs)            ---------------------------  
-QSO_SED		AGN_LONSDALE.list       # QSO list (full path)
+QSO_SED		sed/QSO/SALVATO09/AGN_MOD.list       # QSO list (full path)
 QSO_LIB		LSST_QSO_BIN 			# Binary QSO LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 QSO_FSCALE	1.			# Arbitrary Flux Scale 
 #
 #-------------------  GALAXY LIBRARY (ASCII or BINARY SEDs) ---------------------------
-GAL_SED		 CE_MOD.list            # GALAXMuzzin09_SEDY list (full path)
+GAL_SED		 examples/COSMOS_MOD.list            # GALAXMuzzin09_SEDY list (full path)
 GAL_LIB	         LSST_GAL_BIN 	                # Binary GAL LIBRARY (-> $ZPHOTWORK/lib_bin/*)
 GAL_FSCALE      1.                      # Arbitrary Flux Scale
 #SEL_AGE 	/data/zphot_vers25_03_03/sed/GAL/HYPERZ/AGE_GISSEL_HZ.dat	# List of Age for GISSEL(full path)
 AGE_RANGE  0.,15.e9                                     # Age Min-Max in yr
 
 
 #
@@ -60,15 +60,15 @@
 #
 #------------------   MAG + Z_STEP + COSMO + EXTINCTION   -----------------------------
 MAGTYPE         AB		# Magnitude type (AB or VEGA)
 ZGRID_TYPE      0               # Define the kind of redshift grid (0: linear ; 1: dz*(1+z)) 
 Z_STEP 		0.01,0.,7. 	# dz, zmin, zmax 
 COSMOLOGY	70,0.3,0.7	# H0,om0,lbd0    (if lb0>0->om0+lbd0=1)
 MOD_EXTINC 	0,0		# model range for extinction 
-EXTINC_LAW	SB_calzetti.dat	# ext. law (in  $ZPHOTDIR/ext/*)
+EXTINC_LAW	SMC_prevot.dat,SB_calzetti.dat,SB_calzetti_bump1.dat,SB_calzetti_bump2.dat	# ext. law (in  $ZPHOTDIR/ext/*)
 EB_V            0.,0.05,0.1,0.15,0.2,0.25,0.3,0.35,0.4,0.5 # E(B-V) (<50 values)
 EM_LINES        EMP_UV          # [NO/EMP_UV/EMP_SFR/PHYS] choice between emission line prescription  
 EM_DISPERSION   0.5,0.75,1.,1.5,2. # Dispersion allowed in the emission line flux factor
 ADD_DUSTEM      NO               # Add the dust emission in templates when missing 
 #
 #------------------     ASCII OUTPUT FILES OPTION       -------------------------------
 LIB_ASCII       NO		# Writing Output in ASCII file (-> working directory)
```


# Comparing `tmp/casanovo-4.1.0.tar.gz` & `tmp/casanovo-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casanovo-4.1.0.tar", last modified: Fri Feb 16 08:34:48 2024, max compression
+gzip compressed data, was "casanovo-4.2.0.tar", last modified: Tue May 14 18:35:18 2024, max compression
```

## Comparing `casanovo-4.1.0.tar` & `casanovo-4.2.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.472007 casanovo-4.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.460007 casanovo-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.464007 casanovo-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-16 08:34:33.000000 casanovo-4.1.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-16 08:34:33.000000 casanovo-4.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-16 08:34:33.000000 casanovo-4.1.0/.github/workflows/screenshots.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-16 08:34:33.000000 casanovo-4.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-16 08:34:33.000000 casanovo-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-16 08:34:33.000000 casanovo-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-16 08:34:33.000000 casanovo-4.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-16 08:34:33.000000 casanovo-4.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-16 08:34:33.000000 casanovo-4.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-16 08:34:33.000000 casanovo-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-16 08:34:33.000000 casanovo-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-16 08:34:33.000000 casanovo-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-16 08:34:48.472007 casanovo-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-16 08:34:33.000000 casanovo-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.464007 casanovo-4.1.0/casanovo/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/casanovo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.464007 casanovo-4.1.0/casanovo/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/data/ms_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.468007 casanovo-4.1.0/casanovo/denovo/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/denovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/denovo/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/denovo/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    40933 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/denovo/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/denovo/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-16 08:34:33.000000 casanovo-4.1.0/casanovo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.472007 casanovo-4.1.0/casanovo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-16 08:34:48.000000 casanovo-4.1.0/casanovo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-16 08:34:33.000000 casanovo-4.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.468007 casanovo-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.468007 casanovo-4.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/images/configure-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25705 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/images/evaluate-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/images/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25790 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/images/sequence-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39035 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/images/train-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-16 08:34:33.000000 casanovo-4.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-16 08:34:33.000000 casanovo-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.468007 casanovo-4.1.0/sample_data/
--rw-r--r--   0 runner    (1001) docker     (127)   283201 2024-02-16 08:34:33.000000 casanovo-4.1.0/sample_data/sample_preprocessed_spectra.mgf
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 08:34:48.472007 casanovo-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.468007 casanovo-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-16 08:34:33.000000 casanovo-4.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-02-16 08:34:33.000000 casanovo-4.1.0/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 08:34:48.472007 casanovo-4.1.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-16 08:34:33.000000 casanovo-4.1.0/tests/unit_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-02-16 08:34:33.000000 casanovo-4.1.0/tests/unit_tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-02-16 08:34:33.000000 casanovo-4.1.0/tests/unit_tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.248824 casanovo-4.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.232823 casanovo-4.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.236823 casanovo-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 18:35:06.000000 casanovo-4.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 18:35:06.000000 casanovo-4.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 18:35:06.000000 casanovo-4.2.0/.github/workflows/screenshots.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 18:35:06.000000 casanovo-4.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 18:35:06.000000 casanovo-4.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 18:35:06.000000 casanovo-4.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 18:35:06.000000 casanovo-4.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-05-14 18:35:06.000000 casanovo-4.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-14 18:35:06.000000 casanovo-4.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-14 18:35:06.000000 casanovo-4.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-14 18:35:06.000000 casanovo-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 18:35:06.000000 casanovo-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 18:35:18.244824 casanovo-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-14 18:35:06.000000 casanovo-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.236823 casanovo-4.2.0/casanovo/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/casanovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.240823 casanovo-4.2.0/casanovo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/data/ms_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.240823 casanovo-4.2.0/casanovo/denovo/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/denovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/denovo/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/denovo/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42041 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/denovo/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/denovo/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 18:35:06.000000 casanovo-4.2.0/casanovo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.244824 casanovo-4.2.0/casanovo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 18:35:18.000000 casanovo-4.2.0/casanovo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 18:35:06.000000 casanovo-4.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.240823 casanovo-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15862 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/file_formats.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.244824 casanovo-4.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/images/configure-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25705 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/images/evaluate-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25632 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/images/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25790 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/images/sequence-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39035 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/images/train-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-14 18:35:06.000000 casanovo-4.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-14 18:35:06.000000 casanovo-4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.244824 casanovo-4.2.0/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   283201 2024-05-14 18:35:06.000000 casanovo-4.2.0/sample_data/sample_preprocessed_spectra.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:35:18.248824 casanovo-4.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.244824 casanovo-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-14 18:35:06.000000 casanovo-4.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-14 18:35:06.000000 casanovo-4.2.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:35:18.244824 casanovo-4.2.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-14 18:35:06.000000 casanovo-4.2.0/tests/unit_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-14 18:35:06.000000 casanovo-4.2.0/tests/unit_tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22116 2024-05-14 18:35:06.000000 casanovo-4.2.0/tests/unit_tests/test_unit.py
```

### Comparing `casanovo-4.1.0/.github/workflows/lint.yml` & `casanovo-4.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/.github/workflows/publish.yml` & `casanovo-4.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/.github/workflows/screenshots.yml` & `casanovo-4.2.0/.github/workflows/screenshots.yml`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/.github/workflows/tests.yml` & `casanovo-4.2.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - dev
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        os: [ubuntu-latest, windows-latest, macos-13]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python 3.10
       uses: actions/setup-python@v5
       with:
         python-version: "3.10"
```

### Comparing `casanovo-4.1.0/.gitignore` & `casanovo-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/CHANGELOG.md` & `casanovo-4.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [4.2.0] - 2024-05-14
+
+### Added
+
+- A deprecation warning will be issued when deprecated config options are used in the config file or in the model weights file.
+
+### Changed
+
+- Config option `max_iters` has been renamed to `cosine_schedule_period_iters` to better reflect that it controls the number of iterations for the cosine half period of the learning rate.
+
+### Fixed
+
+- Fix beam search caching failure when multiple beams have an equal predicted peptide score by breaking ties randomly.
+- The mzTab output file now has proper line endings regardless of platform, fixing the extra `\r` found when run on Windows.
+
 ## [4.1.0] - 2024-02-16
 
 ### Changed
 
 - Instead of having to specify `train_from_scratch` in the config file, training will proceed from an existing model weights file if this is given as an argument to `casanovo train`.
 
 ### Fixed
@@ -229,15 +244,16 @@
 
 ## [1.0.0] - 2022-01-28
 
 ### Added
 
 - Initial Casanovo version.
 
-[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v4.1.0...HEAD
+[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v4.2.0...HEAD
+[4.2.0]: https://github.com/Noble-Lab/casanovo/compare/v4.1.0...v4.2.0
 [4.1.0]: https://github.com/Noble-Lab/casanovo/compare/v4.0.1...v4.1.0
 [4.0.1]: https://github.com/Noble-Lab/casanovo/compare/v4.0.0...v4.0.1
 [4.0.0]: https://github.com/Noble-Lab/casanovo/compare/v3.5.0...v4.0.0
 [3.5.0]: https://github.com/Noble-Lab/casanovo/compare/v3.4.0...v3.5.0
 [3.4.0]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...v3.4.0
 [3.3.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
 [3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.1.0...v3.2.0
```

### Comparing `casanovo-4.1.0/CODE_OF_CONDUCT.md` & `casanovo-4.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/CONTRIBUTING.md` & `casanovo-4.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/LICENSE` & `casanovo-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/PKG-INFO` & `casanovo-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanovo
-Version: 4.1.0
+Version: 4.2.0
 Summary: De novo mass spectrometry peptide sequencing with a transformer model
 Author-email: Melih Yilmaz <melih@cs.washington.edu>, "William E. Fondrie" <fondriew@gmail.com>, Wout Bittremieux <wout.bittremieux@uantwerpen.be>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Noble-Lab/casanovo
 Project-URL: Documentation, https://casanovo.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Noble-Lab/casanovo/issues
 Project-URL: Discussion Board, https://github.com/Noble-Lab/casanovo/discussions
```

### Comparing `casanovo-4.1.0/README.md` & `casanovo-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/casanovo.py` & `casanovo-4.2.0/casanovo/casanovo.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/config.py` & `casanovo-4.2.0/casanovo/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """Parse the YAML configuration."""
 
 import logging
 import shutil
+import warnings
 from pathlib import Path
 from typing import Optional, Dict, Callable, Tuple, Union
 
 import yaml
 
 from . import utils
 
 logger = logging.getLogger("casanovo")
 
 
+# FIXME: This contains deprecated config options to be removed in the next major
+#  version update.
+_config_deprecated = dict(
+    every_n_train_steps="val_check_interval",
+    max_iters="cosine_schedule_period_iters",
+)
+
+
 class Config:
     """The Casanovo configuration options.
 
     If a parameter is missing from a user's configuration file, the default
     value is assumed.
 
     Parameters
@@ -52,15 +61,15 @@
         dim_intensity=int,
         max_length=int,
         residues=dict,
         n_log=int,
         tb_summarywriter=str,
         train_label_smoothing=float,
         warmup_iters=int,
-        max_iters=int,
+        cosine_schedule_period_iters=int,
         learning_rate=float,
         weight_decay=float,
         train_batch_size=int,
         predict_batch_size=int,
         n_beams=int,
         top_match=int,
         max_epochs=int,
@@ -80,14 +89,23 @@
             self._params = yaml.safe_load(f_in)
 
         if config_file is None:
             self._user_config = {}
         else:
             with Path(config_file).open() as f_in:
                 self._user_config = yaml.safe_load(f_in)
+                # Remap deprecated config entries.
+                for old, new in _config_deprecated.items():
+                    if old in self._user_config:
+                        self._user_config[new] = self._user_config.pop(old)
+                        warnings.warn(
+                            f"Deprecated config option '{old}' remapped to "
+                            f"'{new}'",
+                            DeprecationWarning,
+                        )
                 # Check for missing entries in config file.
                 config_missing = self._params.keys() - self._user_config.keys()
                 if len(config_missing) > 0:
                     raise KeyError(
                         "Missing expected config option(s): "
                         f"{', '.join(config_missing)}"
                     )
```

### Comparing `casanovo-4.1.0/casanovo/config.yaml` & `casanovo-4.2.0/casanovo/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,109 @@
 ###
 # Casanovo configuration.
 # Blank entries are interpreted as "None".
 ###
 
 ###
-# The following parameters can be modified when running inference or
-# when fine-tuning an existing Casanovo model.
+# The following parameters can be modified when running inference or when
+# fine-tuning an existing Casanovo model.
 ###
 
-# Max absolute difference allowed with respect to observed precursor m/z
+# Max absolute difference allowed with respect to observed precursor m/z.
 # Predictions outside the tolerance range are assigned a negative peptide score.
 precursor_mass_tol: 50  # ppm
-# Isotopes to consider when comparing predicted and observed precursor m/z's
+# Isotopes to consider when comparing predicted and observed precursor m/z's.
 isotope_error_range: [0, 1]
-# The minimum length of predicted peptides
+# The minimum length of predicted peptides.
 min_peptide_len: 6
-# Number of spectra in one inference batch
+# Number of spectra in one inference batch.
 predict_batch_size: 1024
-# Number of beams used in beam search
+# Number of beams used in beam search.
 n_beams: 1
-# Number of PSMs for each spectrum
+# Number of PSMs for each spectrum.
 top_match: 1
 # The hardware accelerator to use. Must be one of:
-# "cpu", "gpu", "tpu", "ipu", "hpu", "mps", or "auto"
+# "cpu", "gpu", "tpu", "ipu", "hpu", "mps", or "auto".
 accelerator: "auto"
-# The devices to use. Can be set to a positive number int,
-# or the value -1 to indicate all available devices should be used,
-# If left empty, the appropriate number will be automatically
-# selected for automatic selected on the chosen accelerator.
+# The devices to use. Can be set to a positive number int, or the value -1 to
+# indicate all available devices should be used. If left empty, the appropriate
+# number will be automatically selected for based on the chosen accelerator.
 devices:
 
 ###
 # The following parameters should only be modified if you are training a new
 # Casanovo model from scratch.
 ###
 
-# Random seed to ensure reproducible results
+# Random seed to ensure reproducible results.
 random_seed: 454
 
 # OUTPUT OPTIONS
-# Logging frequency in training steps
+# Logging frequency in training steps.
 n_log: 1
-# Tensorboard directory to use for keeping track of training metrics
+# Tensorboard directory to use for keeping track of training metrics.
 tb_summarywriter:
-# Save the top k model checkpoints during training. -1 saves all, and
-# leaving this field empty saves none.
+# Save the top k model checkpoints during training. -1 saves all, and leaving
+# this field empty saves none.
 save_top_k: 5
-# Path to saved checkpoints
+# Path to saved checkpoints.
 model_save_folder_path: ""
-# Model validation and checkpointing frequency in training steps
+# Model validation and checkpointing frequency in training steps.
 val_check_interval: 50_000
 
 # SPECTRUM PROCESSING OPTIONS
-# Number of the most intense peaks to retain, any remaining peaks are discarded
+# Number of the most intense peaks to retain, any remaining peaks are discarded.
 n_peaks: 150
-# Min peak m/z allowed, peaks with smaller m/z are discarded
+# Min peak m/z allowed, peaks with smaller m/z are discarded.
 min_mz: 50.0
-# Max peak m/z allowed, peaks with larger m/z are discarded
+# Max peak m/z allowed, peaks with larger m/z are discarded.
 max_mz: 2500.0
-# Min peak intensity allowed, less intense peaks are discarded
+# Min peak intensity allowed, less intense peaks are discarded.
 min_intensity: 0.01
-# Max absolute m/z difference allowed when removing the precursor peak
+# Max absolute m/z difference allowed when removing the precursor peak.
 remove_precursor_tol: 2.0  # Da
-# Max precursor charge allowed, spectra with larger charge are skipped
+# Max precursor charge allowed, spectra with larger charge are skipped.
 max_charge: 10
 
 # MODEL ARCHITECTURE OPTIONS
-# Dimensionality of latent representations, i.e. peak embeddings
+# Dimensionality of latent representations, i.e. peak embeddings.
 dim_model: 512
-# Number of attention heads
+# Number of attention heads.
 n_head: 8
-# Dimensionality of fully connected layers
+# Dimensionality of fully connected layers.
 dim_feedforward: 1024
-# Number of transformer layers in spectrum encoder and peptide decoder
+# Number of transformer layers in spectrum encoder and peptide decoder.
 n_layers: 9
-# Dropout rate for model weights
+# Dropout rate for model weights.
 dropout: 0.0
-# Number of dimensions to use for encoding peak intensity
-# Projected up to ``dim_model`` by default and summed with the peak m/z encoding
+# Number of dimensions to use for encoding peak intensity.
+# Projected up to `dim_model` by default and summed with the peak m/z encoding.
 dim_intensity:
-# Max decoded peptide length
+# Max decoded peptide length.
 max_length: 100
-# Number of warmup iterations for learning rate scheduler
+# The number of iterations for the linear warm-up of the learning rate.
 warmup_iters: 100_000
-# Max number of iterations for learning rate scheduler
-max_iters: 600_000
-# Learning rate for weight updates during training
+# The number of iterations for the cosine half period of the learning rate.
+cosine_schedule_period_iters: 600_000
+# Learning rate for weight updates during training.
 learning_rate: 5e-4
-# Regularization term for weight updates
+# Regularization term for weight updates.
 weight_decay: 1e-5
-# Amount of label smoothing when computing the training loss
+# Amount of label smoothing when computing the training loss.
 train_label_smoothing: 0.01
 
 # TRAINING/INFERENCE OPTIONS
-# Number of spectra in one training batch
+# Number of spectra in one training batch.
 train_batch_size: 32
-# Max number of training epochs
+# Max number of training epochs.
 max_epochs: 30
-# Number of validation steps to run before training begins
+# Number of validation steps to run before training begins.
 num_sanity_val_steps: 0
-# Calculate peptide and amino acid precision during training. this
-# is expensive, so we recommend against it.
+# Calculate peptide and amino acid precision during training.
+# This is expensive, so we recommend against it.
 calculate_precision: False
 
 # AMINO ACID AND MODIFICATION VOCABULARY
 residues:
   "G": 57.021464
   "A": 71.037114
   "S": 87.032028
```

### Comparing `casanovo-4.1.0/casanovo/data/datasets.py` & `casanovo-4.2.0/casanovo/data/datasets.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/data/ms_io.py` & `casanovo-4.2.0/casanovo/data/ms_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             )
             self._run_map[filename] = i
 
     def save(self) -> None:
         """
         Export the spectrum identifications to the mzTab file.
         """
-        with open(self.filename, "w") as f:
+        with open(self.filename, "w", newline="") as f:
             writer = csv.writer(f, delimiter="\t", lineterminator=os.linesep)
             # Write metadata.
             for row in self.metadata:
                 writer.writerow(["MTD", *row])
             # Write PSMs.
             writer.writerow(
                 [
```

### Comparing `casanovo-4.1.0/casanovo/denovo/dataloaders.py` & `casanovo-4.2.0/casanovo/denovo/dataloaders.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/denovo/evaluate.py` & `casanovo-4.2.0/casanovo/denovo/evaluate.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/denovo/model.py` & `casanovo-4.2.0/casanovo/denovo/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """A de novo peptide sequencing model."""
 
 import collections
 import heapq
 import logging
+import warnings
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import depthcharge.masses
 import einops
 import torch
 import numpy as np
 import lightning.pytorch as pl
 from torch.utils.tensorboard import SummaryWriter
 from depthcharge.components import ModelMixin, PeptideDecoder, SpectrumEncoder
 
 from . import evaluate
+from .. import config
 from ..data import ms_io
 
 logger = logging.getLogger("casanovo")
 
 
 class Spec2Pep(pl.LightningModule, ModelMixin):
     """
@@ -42,15 +44,15 @@
     dim_intensity : Optional[int]
         The number of features to use for encoding peak intensity. The remaining
         (``dim_model - dim_intensity``) are reserved for encoding the m/z value.
         If ``None``, the intensity will be projected up to ``dim_model`` using a
         linear layer, then summed with the m/z encoding for each peak.
     max_length : int
         The maximum peptide length to decode.
-    residues: Union[Dict[str, float], str]
+    residues : Union[Dict[str, float], str]
         The amino acid dictionary and their masses. By default ("canonical) this
         is only the 20 canonical amino acids, with cysteine carbamidomethylated.
         If "massivekb", this dictionary will include the modifications found in
         MassIVE-KB. Additionally, a dictionary can be used to specify a custom
         collection of amino acids and masses.
     max_charge : int
         The maximum precursor charge to consider.
@@ -61,32 +63,32 @@
         Take into account the error introduced by choosing a non-monoisotopic
         peak for fragmentation by not penalizing predicted precursor m/z's that
         fit the specified isotope error:
         `abs(calc_mz - (precursor_mz - isotope * 1.00335 / precursor_charge))
         < precursor_mass_tol`
     min_peptide_len : int
         The minimum length of predicted peptides.
-    n_beams: int
+    n_beams : int
         Number of beams used during beam search decoding.
-    top_match: int
+    top_match : int
         Number of PSMs to return for each spectrum.
     n_log : int
         The number of epochs to wait between logging messages.
-    tb_summarywriter: Optional[str]
+    tb_summarywriter : Optional[str]
         Folder path to record performance metrics during training. If ``None``,
         don't use a ``SummaryWriter``.
-    train_label_smoothing: float
+    train_label_smoothing : float
         Smoothing factor when calculating the training loss.
-    warmup_iters: int
-        The number of warm up iterations for the learning rate scheduler.
-    max_iters: int
-        The total number of iterations for the learning rate scheduler.
-    out_writer: Optional[str]
+    warmup_iters : int
+        The number of iterations for the linear warm-up of the learning rate.
+    cosine_schedule_period_iters : int
+        The number of iterations for the cosine half period of the learning rate.
+    out_writer : Optional[str]
         The output writer for the prediction results.
-    calculate_precision: bool
+    calculate_precision : bool
         Calculate the validation set precision during training.
         This is expensive.
     **kwargs : Dict
         Additional keyword arguments passed to the Adam optimizer.
     """
 
     def __init__(
@@ -107,15 +109,15 @@
         top_match: int = 1,
         n_log: int = 10,
         tb_summarywriter: Optional[
             torch.utils.tensorboard.SummaryWriter
         ] = None,
         train_label_smoothing: float = 0.01,
         warmup_iters: int = 100_000,
-        max_iters: int = 600_000,
+        cosine_schedule_period_iters: int = 600_000,
         out_writer: Optional[ms_io.MztabWriter] = None,
         calculate_precision: bool = False,
         **kwargs: Dict,
     ):
         super().__init__()
         self.save_hyperparameters()
 
@@ -140,15 +142,23 @@
         self.softmax = torch.nn.Softmax(2)
         self.celoss = torch.nn.CrossEntropyLoss(
             ignore_index=0, label_smoothing=train_label_smoothing
         )
         self.val_celoss = torch.nn.CrossEntropyLoss(ignore_index=0)
         # Optimizer settings.
         self.warmup_iters = warmup_iters
-        self.max_iters = max_iters
+        self.cosine_schedule_period_iters = cosine_schedule_period_iters
+        # `kwargs` will contain additional arguments as well as unrecognized
+        # arguments, including deprecated ones. Remove the deprecated ones.
+        for k in config._config_deprecated:
+            kwargs.pop(k, None)
+            warnings.warn(
+                f"Deprecated hyperparameter '{k}' removed from the model.",
+                DeprecationWarning,
+            )
         self.opt_kwargs = kwargs
 
         # Data properties.
         self.max_length = max_length
         self.residues = residues
         self.precursor_mass_tol = precursor_mass_tol
         self.isotope_error_range = isotope_error_range
@@ -468,15 +478,17 @@
     def _cache_finished_beams(
         self,
         tokens: torch.Tensor,
         scores: torch.Tensor,
         step: int,
         beams_to_cache: torch.Tensor,
         beam_fits_precursor: torch.Tensor,
-        pred_cache: Dict[int, List[Tuple[float, np.ndarray, torch.Tensor]]],
+        pred_cache: Dict[
+            int, List[Tuple[float, float, np.ndarray, torch.Tensor]]
+        ],
     ):
         """
         Cache terminated beams.
 
         Parameters
         ----------
         tokens : torch.Tensor of shape (n_spectra * n_beams, max_length)
@@ -489,19 +501,21 @@
             Index of the current decoding step.
         beams_to_cache : torch.Tensor of shape (n_spectra * n_beams)
             Boolean tensor indicating whether the current beams are ready for
             caching.
         beam_fits_precursor: torch.Tensor of shape (n_spectra * n_beams)
             Boolean tensor indicating whether the beams are within the
             precursor m/z tolerance.
-        pred_cache : Dict[int, List[Tuple[float, np.ndarray, torch.Tensor]]]
+        pred_cache : Dict[
+                int, List[Tuple[float, float, np.ndarray, torch.Tensor]]
+        ]
             Priority queue with finished beams for each spectrum, ordered by
             peptide score. For each finished beam, a tuple with the (negated)
-            peptide score, amino acid-level scores, and the predicted tokens is
-            stored.
+            peptide score, a random tie-breaking float, the amino acid-level
+            scores, and the predicted tokens is stored.
         """
         for i in range(len(beams_to_cache)):
             if not beams_to_cache[i]:
                 continue
             # Find the starting index of the spectrum.
             spec_idx = i // self.n_beams
             # FIXME: The next 3 lines are very similar as what's done in
@@ -534,15 +548,20 @@
             # the number of beams elements).
             if len(pred_cache[spec_idx]) < self.n_beams:
                 heapadd = heapq.heappush
             else:
                 heapadd = heapq.heappushpop
             heapadd(
                 pred_cache[spec_idx],
-                (peptide_score, aa_scores, torch.clone(pred_peptide)),
+                (
+                    peptide_score,
+                    np.random.random_sample(),
+                    aa_scores,
+                    torch.clone(pred_peptide),
+                ),
             )
 
     def _get_topk_beams(
         self,
         tokens: torch.tensor,
         scores: torch.tensor,
         finished_beams: torch.tensor,
@@ -632,25 +651,30 @@
         )
         scores = einops.rearrange(scores, "B L V S -> (B S) L V")
         tokens = einops.rearrange(tokens, "B L S -> (B S) L")
         return tokens, scores
 
     def _get_top_peptide(
         self,
-        pred_cache: Dict[int, List[Tuple[float, np.ndarray, torch.Tensor]]],
+        pred_cache: Dict[
+            int, List[Tuple[float, float, np.ndarray, torch.Tensor]]
+        ],
     ) -> Iterable[List[Tuple[float, np.ndarray, str]]]:
         """
         Return the peptide with the highest confidence score for each spectrum.
 
         Parameters
         ----------
-        pred_cache : Dict[int, List[Tuple[float, np.ndarray, torch.Tensor]]]
+        pred_cache : Dict[
+                int, List[Tuple[float, float, np.ndarray, torch.Tensor]]
+        ]
             Priority queue with finished beams for each spectrum, ordered by
             peptide score. For each finished beam, a tuple with the peptide
-            score, amino acid-level scores, and the predicted tokens is stored.
+            score, a random tie-breaking float, the amino acid-level scores,
+            and the predicted tokens is stored.
 
         Returns
         -------
         pred_peptides : Iterable[List[Tuple[float, np.ndarray, str]]]
             For each spectrum, a list with the top peptide prediction(s). A
             peptide predictions consists of a tuple with the peptide score,
             the amino acid scores, and the predicted peptide sequence.
@@ -659,15 +683,15 @@
             if len(peptides) > 0:
                 yield [
                     (
                         pep_score,
                         aa_scores,
                         "".join(self.decoder.detokenize(pred_tokens)),
                     )
-                    for pep_score, aa_scores, pred_tokens in heapq.nlargest(
+                    for pep_score, _, aa_scores, pred_tokens in heapq.nlargest(
                         self.top_match, peptides
                     )
                 ]
             else:
                 yield []
 
     def _forward_step(
@@ -956,47 +980,53 @@
         -------
         Tuple[torch.optim.Optimizer, Dict[str, Any]]
             The initialized Adam optimizer and its learning rate scheduler.
         """
         optimizer = torch.optim.Adam(self.parameters(), **self.opt_kwargs)
         # Apply learning rate scheduler per step.
         lr_scheduler = CosineWarmupScheduler(
-            optimizer, warmup=self.warmup_iters, max_iters=self.max_iters
+            optimizer, self.warmup_iters, self.cosine_schedule_period_iters
         )
         return [optimizer], {"scheduler": lr_scheduler, "interval": "step"}
 
 
 class CosineWarmupScheduler(torch.optim.lr_scheduler._LRScheduler):
     """
-    Learning rate scheduler with linear warm up followed by cosine shaped decay.
+    Learning rate scheduler with linear warm-up followed by cosine shaped decay.
 
     Parameters
     ----------
     optimizer : torch.optim.Optimizer
         Optimizer object.
-    warmup : int
-        The number of warm up iterations.
-    max_iters : torch.optim
-        The total number of iterations.
+    warmup_iters : int
+        The number of iterations for the linear warm-up of the learning rate.
+    cosine_schedule_period_iters : int
+        The number of iterations for the cosine half period of the learning rate.
     """
 
     def __init__(
-        self, optimizer: torch.optim.Optimizer, warmup: int, max_iters: int
+        self,
+        optimizer: torch.optim.Optimizer,
+        warmup_iters: int,
+        cosine_schedule_period_iters: int,
     ):
-        self.warmup, self.max_iters = warmup, max_iters
+        self.warmup_iters = warmup_iters
+        self.cosine_schedule_period_iters = cosine_schedule_period_iters
         super().__init__(optimizer)
 
     def get_lr(self):
         lr_factor = self.get_lr_factor(epoch=self.last_epoch)
         return [base_lr * lr_factor for base_lr in self.base_lrs]
 
     def get_lr_factor(self, epoch):
-        lr_factor = 0.5 * (1 + np.cos(np.pi * epoch / self.max_iters))
-        if epoch <= self.warmup:
-            lr_factor *= epoch / self.warmup
+        lr_factor = 0.5 * (
+            1 + np.cos(np.pi * epoch / self.cosine_schedule_period_iters)
+        )
+        if epoch <= self.warmup_iters:
+            lr_factor *= epoch / self.warmup_iters
         return lr_factor
 
 
 def _calc_mass_error(
     calc_mz: float, obs_mz: float, charge: int, isotope: int = 0
 ) -> float:
     """
```

### Comparing `casanovo-4.1.0/casanovo/denovo/model_runner.py` & `casanovo-4.2.0/casanovo/denovo/model_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,16 @@
 
     def initialize_model(self, train: bool) -> None:
         """Initialize the Casanovo model.
 
         Parameters
         ----------
         train : bool
-            Determines whether to set the model up for model training
-            or evaluation / inference.
+            Determines whether to set the model up for model training or
+            evaluation / inference.
         """
         model_params = dict(
             dim_model=self.config.dim_model,
             n_head=self.config.n_head,
             dim_feedforward=self.config.dim_feedforward,
             n_layers=self.config.n_layers,
             dropout=self.config.dropout,
@@ -222,34 +222,34 @@
             min_peptide_len=self.config.min_peptide_len,
             n_beams=self.config.n_beams,
             top_match=self.config.top_match,
             n_log=self.config.n_log,
             tb_summarywriter=self.config.tb_summarywriter,
             train_label_smoothing=self.config.train_label_smoothing,
             warmup_iters=self.config.warmup_iters,
-            max_iters=self.config.max_iters,
+            cosine_schedule_period_iters=self.config.cosine_schedule_period_iters,
             lr=self.config.learning_rate,
             weight_decay=self.config.weight_decay,
             out_writer=self.writer,
             calculate_precision=self.config.calculate_precision,
         )
 
-        # Reconfigurable non-architecture related parameters for a loaded model
+        # Reconfigurable non-architecture related parameters for a loaded model.
         loaded_model_params = dict(
             max_length=self.config.max_length,
             precursor_mass_tol=self.config.precursor_mass_tol,
             isotope_error_range=self.config.isotope_error_range,
             n_beams=self.config.n_beams,
             min_peptide_len=self.config.min_peptide_len,
             top_match=self.config.top_match,
             n_log=self.config.n_log,
             tb_summarywriter=self.config.tb_summarywriter,
             train_label_smoothing=self.config.train_label_smoothing,
             warmup_iters=self.config.warmup_iters,
-            max_iters=self.config.max_iters,
+            cosine_schedule_period_iters=self.config.cosine_schedule_period_iters,
             lr=self.config.learning_rate,
             weight_decay=self.config.weight_decay,
             out_writer=self.writer,
             calculate_precision=self.config.calculate_precision,
         )
 
         if self.model_filename is None:
@@ -296,15 +296,15 @@
                     self.model_filename,
                     map_location=device,
                     **model_params,
                 )
             except RuntimeError:
                 raise RuntimeError(
                     "Weights file incompatible with the current version of "
-                    "Casanovo. "
+                    "Casanovo."
                 )
 
     def initialize_data_module(
         self,
         train_index: Optional[AnnotatedSpectrumIndex] = None,
         valid_index: Optional[AnnotatedSpectrumIndex] = None,
         test_index: Optional[
```

### Comparing `casanovo-4.1.0/casanovo/utils.py` & `casanovo-4.2.0/casanovo/utils.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo/version.py` & `casanovo-4.2.0/casanovo/version.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/casanovo.egg-info/PKG-INFO` & `casanovo-4.2.0/casanovo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanovo
-Version: 4.1.0
+Version: 4.2.0
 Summary: De novo mass spectrometry peptide sequencing with a transformer model
 Author-email: Melih Yilmaz <melih@cs.washington.edu>, "William E. Fondrie" <fondriew@gmail.com>, Wout Bittremieux <wout.bittremieux@uantwerpen.be>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Noble-Lab/casanovo
 Project-URL: Documentation, https://casanovo.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Noble-Lab/casanovo/issues
 Project-URL: Discussion Board, https://github.com/Noble-Lab/casanovo/discussions
```

### Comparing `casanovo-4.1.0/casanovo.egg-info/SOURCES.txt` & `casanovo-4.2.0/casanovo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 docs/CHANGELOG.md
 docs/CODE_OF_CONDUCT.md
 docs/CONTRIBUTING.md
 docs/Makefile
 docs/conf.py
 docs/environment.yaml
 docs/faq.md
+docs/file_formats.md
 docs/getting_started.md
 docs/index.md
 docs/make.bat
 docs/images/configure-help.svg
 docs/images/evaluate-help.svg
 docs/images/help.svg
 docs/images/sequence-help.svg
```

### Comparing `casanovo-4.1.0/docs/CHANGELOG.md` & `casanovo-4.2.0/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [4.2.0] - 2024-05-14
+
+### Added
+
+- A deprecation warning will be issued when deprecated config options are used in the config file or in the model weights file.
+
+### Changed
+
+- Config option `max_iters` has been renamed to `cosine_schedule_period_iters` to better reflect that it controls the number of iterations for the cosine half period of the learning rate.
+
+### Fixed
+
+- Fix beam search caching failure when multiple beams have an equal predicted peptide score by breaking ties randomly.
+- The mzTab output file now has proper line endings regardless of platform, fixing the extra `\r` found when run on Windows.
+
 ## [4.1.0] - 2024-02-16
 
 ### Changed
 
 - Instead of having to specify `train_from_scratch` in the config file, training will proceed from an existing model weights file if this is given as an argument to `casanovo train`.
 
 ### Fixed
@@ -229,15 +244,16 @@
 
 ## [1.0.0] - 2022-01-28
 
 ### Added
 
 - Initial Casanovo version.
 
-[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v4.1.0...HEAD
+[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v4.2.0...HEAD
+[4.2.0]: https://github.com/Noble-Lab/casanovo/compare/v4.1.0...v4.2.0
 [4.1.0]: https://github.com/Noble-Lab/casanovo/compare/v4.0.1...v4.1.0
 [4.0.1]: https://github.com/Noble-Lab/casanovo/compare/v4.0.0...v4.0.1
 [4.0.0]: https://github.com/Noble-Lab/casanovo/compare/v3.5.0...v4.0.0
 [3.5.0]: https://github.com/Noble-Lab/casanovo/compare/v3.4.0...v3.5.0
 [3.4.0]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...v3.4.0
 [3.3.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
 [3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.1.0...v3.2.0
```

### Comparing `casanovo-4.1.0/docs/CODE_OF_CONDUCT.md` & `casanovo-4.2.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/CONTRIBUTING.md` & `casanovo-4.2.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/Makefile` & `casanovo-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/conf.py` & `casanovo-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/faq.md` & `casanovo-4.2.0/docs/faq.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,48 +30,48 @@
 You can avoid this error by explicitly specifying the model file using the `--model` parameter.
 
 ## GPU Troubleshooting
 
 **Casanovo is very slow even when running on the GPU. How can I speed it up?**
 
 It is highly recommended to run Casanovo on the GPU to get the maximum performance.
-If Casanovo is slow despite that your system has a GPU, the GPU might not be configured correctly for Casanovo.
+If Casanovo is slow despite your system having a GPU, then the GPU might not be configured correctly.
 A quick test to verify that Casanovo is using your (CUDA-enabled) GPU is to run `watch nvidia-smi` in your terminal.
-If Casanovo has access to the GPU, you should see it listed in the bottom process table and the "Volatile GPU-Util" column at the top right should show activity while Casanovo is processing the data.
+If Casanovo has access to the GPU, then you should see it listed in the bottom process table, and the "Volatile GPU-Util" column at the top right should show activity while Casanovo is processing the data.
 
-If Casanovo is not listed in the `nvidia-smi` output, it is not using your GPU.
+If Casanovo is not listed in the `nvidia-smi` output, then it is not using your GPU.
 This is commonly caused by an incompatibility between your NVIDIA drivers and Pytorch.
-Although Pytorch is installed automatically when installing Casanovo, in this case we recommend to reinstall it manually according to the following steps:
+Although Pytorch is installed automatically when installing Casanovo, in this case we recommend reinstalling it manually according to the following steps:
 
 1. Uninstall the current version of Pytorch: `pip uninstall torch`
 2. Install the latest version of the NVIDIA drivers using the [official CUDA Toolkit](https://developer.nvidia.com/cuda-downloads). If supported by your system, an easy alternative can be conda using `conda install -c nvidia cuda-toolkit`.
 3. Install the latest version of Pytorch according to the [instructions on the Pytorch website](https://pytorch.org/get-started/locally/).
 
 Try to run Casanovo again and use `watch nvidia-smi` to inspect whether it can use the GPU now.
-If this is still not yet the case, please [open an issue on GitHub](https://github.com/Noble-Lab/casanovo/issues/new).
-Include full information about your system set-up, the installed CUDA toolkit and Pytorch versions, and the troubleshooting steps you have performed.
+If this is still not the case, please [open an issue on GitHub](https://github.com/Noble-Lab/casanovo/issues/new).
+Include full information about your system setup, the installed CUDA toolkit and Pytorch versions, and the troubleshooting steps you have performed.
 
-**I get a "CUDA out of memory" error when trying to run Casanovo. Help!**
+**Why do I get a "CUDA out of memory" error when trying to run Casanovo?**
 
 This means that there was not enough (free) memory available on your GPU to run Casanovo, which is especially likely to happen when you are using a smaller, consumer-grade GPU.
-We recommend trying to decrease the `train_batch_size` or `predict_batch_size` options in the [config file](https://github.com/Noble-Lab/casanovo/blob/main/casanovo/config.yaml) (depending on whether the error occurred during `train` or `denovo` mode) to reduce the number of spectra that are processed simultaneously.
+Depending on whether the error occurred during `train` or `denovo` mode, we recommend decreasing the `train_batch_size` or `predict_batch_size` options, respectively, in the [config file](https://github.com/Noble-Lab/casanovo/blob/main/casanovo/config.yaml) to reduce the number of spectra that are processed simultaneously.
 Additionally, we recommend shutting down any other processes that may be running on the GPU, so that Casanovo can exclusively use the GPU.
 
 **How can I run Casanovo on a specific GPU device?**
 
 You can control which GPU(s) Casanovo uses by setting the `devices` option in the [configuration file](https://github.com/Noble-Lab/casanovo/blob/main/casanovo/config.yaml).
-Analogously, this setting also controls the number of cores to use when running on a CPU only (which can be specified using the `accelerator` option).
+This setting also controls the number of cores to use when running on a CPU only (which can be specified using the `accelerator` option).
 
 By default, Casanovo will automatically try to use the maximum number of devices available.
-I.e., if your system has multiple GPUs, Casanovo will utilize all of those for maximum efficiency.
+I.e., if your system has multiple GPUs, then Casanovo will use all of them for maximum efficiency.
 Alternatively, you can select a specific GPU by specifying the GPU number as the value for `devices`.
 For example, if you have a four-GPU system, when specifying `devices: 1` in your config file Casanovo will only use the GPU with identifier `1`.
 
 The config file functionality only allows specifying a single GPU, by setting its id under `devices`, or all GPUs, by setting `devices: -1`.
-If you want more fine-grained control to use some but not all GPUs on a multi-GPU system, the `CUDA_VISIBLE_DEVICES` environment variable can be used instead.
+If you want more fine-grained control to use some but not all GPUs on a multi-GPU system, then the `CUDA_VISIBLE_DEVICES` environment variable can be used instead.
 For example, by setting `CUDA_VISIBLE_DEVICES=1,3`, only GPUs `1` and `3` will be visible to Casanovo, and specifying `devices: -1` will allow it to utilize both of these.
 
 Note that when using `CUDA_VISIBLE_DEVICES`, the GPU numbers (potentially to be specified under `devices`) are reset to consecutively increase from `0`.
 
 **I see "NotImplementedError: The operator 'aten::index.Tensor'..." when using a Mac with an Apple Silicon chip.**
 
 Casanovo can leverage Apple's Metal Performance Shaders (MPS) on newer Mac computers, which requires that the `PYTORCH_ENABLE_MPS_FALLBACK` is set to `1`:
@@ -82,15 +82,15 @@
 
 This will need to be set with each new shell session, or you can add it to your `.bashrc` / `.zshrc` to set this environment variable by default.
 
 ## Training Casanovo
 
 **Where can I find the data that Casanovo was trained on?**
 
-The [Casanovo results reported](https://doi.org/10.1101/2023.01.03.522621) were obtained by training on two different datasets: (i) a commonly used nine-species benchmark dataset, and (ii) a large-scale training dataset derived from the MassIVE Knowledge Base (MassIVE-KB).
+The [reported Casanovo results](https://doi.org/10.1101/2023.01.03.522621) were obtained by training on two different datasets: (i) a commonly used nine-species benchmark dataset, and (ii) a large-scale training dataset derived from the MassIVE Knowledge Base (MassIVE-KB).
 
 All data for the _nine-species benchmark_ is available as annotated MGF files [on MassIVE](https://doi.org/doi:10.25345/C52V2CK8J).
 Using these data, Casanovo was trained in a cross-validated fashion, training on eight species and testing on the remaining species.
 
 The _MassIVE-KB training data_ was derived from PSMs used to compile the MassIVE-KB v1 spectral library and consists of 30 million PSMs.
 These PSMs were obtained by collecting up to the top 100 PSMs for each of the precursors (as defined by a peptidoform and charge) included in MassIVE-KB.
 To compile this dataset yourself, on the [MassIVE website](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp), go to [MassIVE Knowledge Base](https://massive.ucsd.edu/ProteoSAFe/static/massive-kb-libraries.jsp) > [Human HCD Spectral Library](https://massive.ucsd.edu/ProteoSAFe/status.jsp?task=82c0124b6053407fa41ba98f53fd8d89) > [All Candidate library spectra](https://massive.ucsd.edu/ProteoSAFe/result.jsp?task=82c0124b6053407fa41ba98f53fd8d89&view=candidate_library_spectra) > Download.
@@ -100,55 +100,69 @@
 The _non-enzymatic dataset_, used to train a non-tryptic version of Casanovo, was created by selecting PSMs with a uniform distribution of amino acids at the C-terminal peptide positions from two datasets: MassIVE-KB and PROSPECT.
 Training, validation, and test splits for the non-enzymatic dataset are available as annotated MGF files [on MassIVE](https://doi.org/doi:10.25345/C5KS6JG0W).
 
 **How do I know which model to use after training Casanovo?**
 
 By default, Casanovo saves a snapshot of the model weights after every 50,000 training steps.
 Note that the number of samples that are processed during a single training step depends on the batch size.
-Therefore, when using the default training batch size of 32, this corresponds to saving a model snapshot after every 1.6 million training samples.
+Therefore, the default training batch size of 32 corresponds to saving a model snapshot after every 1.6 million training samples.
 You can optionally modify the snapshot (and validation) frequency in the [config file](https://github.com/Noble-Lab/casanovo/blob/main/casanovo/config.yaml) (parameter `val_check_interval`), depending on your dataset size.
-Note that taking very frequent model snapshots will result in somewhat slower training time because Casanovo will evaluate its performance on the validation data for every snapshot.
+Note that taking very frequent model snapshots will result in slower training time because Casanovo will evaluate its performance on the validation data for every snapshot.
 
 When saving a model snapshot, Casanovo will use the validation data to compute performance measures (training loss, validation loss, amino acid precision, and peptide precision) and print this information to the console and log file.
-After your training job is finished, you can identify the best performing model that achieves the maximum peptide and amino acid precision from the log file and use the corresponding model snapshot.
+After your training job is finished, you can identify the model that achieves the maximum peptide and amino acid precision from the log file and use the corresponding model snapshot.
 
 **Even though I added new post-translational modifications to the configuration file, Casanovo didn't identify those peptides.**
 
 Casanovo can only make predictions using post-translational modifications (PTMs) that were included when training the model.
 If you want to add new types of PTMs, then you will need to retrain the model.
 
 The [`config.yaml` configuration file](https://github.com/Noble-Lab/casanovo/blob/main/casanovo/config.yaml) contains all amino acids and PTMs that Casanovo knows.
 By default, this includes oxidation of methionine, deamidation of asparagine and glutamine, N-terminal acetylation, N-terminal carbamylation, and an N-terminal loss of ammonia.
 (Additionally, cysteines are _always_ considered to be carbamidomethylated.)
 Simply making changes to the `residues` alphabet in the configuration file is insufficient to identify new types of PTMs with Casanovo, however.
 This is indicated by the fact that this option is not marked with `(I)` in the configuration file, which indicates options that can be modified during inference.
-Al remaining options require training a new Casanovo model.
+All remaining options require training a new Casanovo model.
 
 Therefore, to learn the spectral signature of previously unknown PTMs, a new Casanovo version needs to be _trained_.
 To include new PTMs in Casanovo, you need to:
 1. Update the `residues` alphabet in the configuration file accordingly.
 2. Compile a large training dataset that includes those PTMs and format this as an annotated MGF file. Note that you can include some or all of the data that was originally used to train Casanovo (see above), in addition to the data that includes your new types of PTMs.
 3. Train a new version of Casanovo on this dataset.
 
 It is unfortunately not possible to finetune a pre-trained Casanovo model to add new types of PTMs.
 Instead, such a model must be trained from scratch.
 
 **How can I change the learning rate schedule used during training?**
 
-By default, Casanovo uses a learning rate schedule that combines linear warm up followed by a cosine wave shaped decay (as implemented in `CosineWarmupScheduler` in `casanovo/denovo/model.py`) during training.
+By default, Casanovo uses a learning rate schedule that combines linear warm up followed by a cosine decay (as implemented in `CosineWarmupScheduler` in `casanovo/denovo/model.py`) during training.
 To use a different learning rate schedule, you can specify an alternative learning rate scheduler as follows (in the `lr_scheduler` variable in function `Spec2Pep.configure_optimizers` in `casanovo/denovo/model.py`):
 
 ```
 lr_scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, total_iters=self.warmup_iters)
 ```
 
 You can use any of the scheduler classes available in [`torch.optim.lr_scheduler`](https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate) or implement your custom learning rate schedule similar to `CosineWarmupScheduler`.
 
 ## Miscellaneous
 
+**Can I use Casanovo to sequence antibodies?**
+
+Yes, antibody sequencing is one of the popular uses for de novo sequencing technology.
+[This article](https://academic.oup.com/bib/article/24/1/bbac542/6955273) carried out a systematic comparison of six de novo sequencing tools (Novor, pNovo 3, DeepNovo, SMSNet, PointNovo and Casanovo).  Casanovo fared very well in this comparison: "Casanovo exhibits the highest number of correct peptide predictions compared with all other de novo algorithms across all enzymes demonstrating the advantage of using transformers for peptide sequencing. Furthermore, Casanovo predicts amino acids with overall superior precision."
+
+In practice, you may want to try providing your Casanovo output file to the [Stitch software](https://github.com/snijderlab/stitch), which performs template-based assembly of de novo peptide reads to reconstruct antibody sequences ([Schulte and Snyder 2024](https://www.biorxiv.org/content/10.1101/2024.02.20.581155v1)).
+
+**Where can I find Casanovo model weights trained on the nine-species benchmark?**
+
+You can find the Casanovo weights corresponding to the nine-species benchmark [on Zenodo](https://doi.org/10.5281/zenodo.10694984), compatible with Casanovo v4.x.x.
+These weights correspond to training and validation on eight species using the default configurations, with the remaining species held out for testing, as indicated by the file names.
+Note that these weights are only intended for evaluation purposes on this specific benchmark dataset.
+For general-purpose usage of Casanovo, use its [default weights](https://casanovo.readthedocs.io/en/latest/getting_started.html#download-model-weights) instead, as these will give significantly improved performance.
+
 **How can I generate a precision–coverage curve?**
 
 You can evaluate a trained Casanovo model compared to ground-truth peptide labels using a precision–coverage curve.
 
 1. Run Casanovo in sequencing or evaluation mode on your MS/MS data, [as described here](https://casanovo.readthedocs.io/en/latest/getting_started.html#running-casanovo).
 2. Collect the ground-truth peptide labels as well as the peptide labels predicted by Casanovo. Note that Casanovo might not report a peptide for every spectrum if the spectra are invalid (e.g. not enough peaks), so make sure that both pieces of information are correctly linked to each other (using the `spectra_ref` column in the mzTab output file produced by Casanovo).
 3. Use the following script to plot a precision–coverage curve:
```

### Comparing `casanovo-4.1.0/docs/getting_started.md` & `casanovo-4.2.0/docs/getting_started.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,16 @@
 All auxiliary data, model, and training-related parameters can be specified in a YAML configuration file. 
 To generate a YAML file containing the current Casanovo defaults, run:
 ```sh
 casanovo configure
 ```
 ![`casanovo configure --help`](images/configure-help.svg)
 
-When using Casanovo to sequence peptides from mass spectra or evaluate a previous model's performance, you can change some of the parameters in this file, indicated with "(I)" in the file. 
-The other parameters will not have an effect unless you are training a new Casanovo model.
-
+When using Casanovo to sequence peptides from mass spectra or evaluate a previous model's performance, you can change some of the parameters in the first section of this file.
+Parameters in the second section will not have an effect unless you are training a new Casanovo model.
 
 ### Download model weights
 
 Using Casanovo to sequence peptides from new mass spectra, Casanovo needs compatible pretrained model weights to make its predictions.
 By default, Casanovo will try to download the latest compatible model weights from GitHub when it is run. 
 
 However, our model weights are uploaded with new Casanovo versions on the [Releases page](https://github.com/Noble-Lab/casanovo/releases) under the "Assets" for each release (file extension: `.ckpt`).
```

### Comparing `casanovo-4.1.0/docs/images/configure-help.svg` & `casanovo-4.2.0/docs/images/configure-help.svg`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/images/evaluate-help.svg` & `casanovo-4.2.0/docs/images/evaluate-help.svg`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/images/sequence-help.svg` & `casanovo-4.2.0/docs/images/sequence-help.svg`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/images/train-help.svg` & `casanovo-4.2.0/docs/images/train-help.svg`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/docs/index.md` & `casanovo-4.2.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 
 ```{toctree}
 ---
 hidden: true
 maxdepth: 1
 ---
 Getting Started <getting_started.md>
+File Formats <file_formats.md>
 FAQs <faq.md>
 Contributing <CONTRIBUTING.md>
 Code of Conduct <CODE_OF_CONDUCT.md>
 Changelog <CHANGELOG.md>
 ```
```

### Comparing `casanovo-4.1.0/docs/make.bat` & `casanovo-4.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/pyproject.toml` & `casanovo-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/sample_data/sample_preprocessed_spectra.mgf` & `casanovo-4.2.0/sample_data/sample_preprocessed_spectra.mgf`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/tests/conftest.py` & `casanovo-4.2.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     """A config file for a tiny model."""
     cfg = {
         "n_head": 2,
         "dim_feedforward": 10,
         "n_layers": 1,
         "train_label_smoothing": 0.01,
         "warmup_iters": 1,
-        "max_iters": 1,
+        "cosine_schedule_period_iters": 1,
         "max_epochs": 20,
         "val_check_interval": 1,
         "model_save_folder_path": str(tmp_path),
         "accelerator": "cpu",
         "precursor_mass_tol": 5,
         "isotope_error_range": [0, 1],
         "min_peptide_len": 6,
```

### Comparing `casanovo-4.1.0/tests/test_integration.py` & `casanovo-4.2.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `casanovo-4.1.0/tests/unit_tests/test_config.py` & `casanovo-4.2.0/tests/unit_tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,7 +33,19 @@
         cfg = yaml.safe_load(f_in)
         # Insert invalid config option.
         cfg["random_seed_"] = 354
         yaml.safe_dump(cfg, f_out)
 
     with pytest.raises(KeyError):
         Config(filename)
+
+
+def test_deprecated(tmp_path, tiny_config):
+    filename = str(tmp_path / "config_deprecated.yml")
+    with open(tiny_config, "r") as f_in, open(filename, "w") as f_out:
+        cfg = yaml.safe_load(f_in)
+        # Insert deprecated config option.
+        cfg["max_iters"] = 1
+        yaml.safe_dump(cfg, f_out)
+
+    with pytest.warns(DeprecationWarning):
+        Config(filename)
```

### Comparing `casanovo-4.1.0/tests/unit_tests/test_runner.py` & `casanovo-4.2.0/tests/unit_tests/test_runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,25 +58,25 @@
         runner.train([mgf_small], [mgf_small])
         runner.trainer.save_checkpoint(ckpt)
 
     # Try changing model arch:
     other_config = Config(tiny_config)
     other_config.n_layers = 50  # lol
     other_config.n_beams = 12
-    other_config.max_iters = 2
+    other_config.cosine_schedule_period_iters = 2
     with torch.device("meta"):
         # Now load the weights into a new model
         # The device should be meta for all the weights.
         runner = ModelRunner(config=other_config, model_filename=str(ckpt))
         runner.initialize_model(train=False)
 
     obs_layers = runner.model.encoder.transformer_encoder.num_layers
     assert obs_layers == 1  # Match the original arch.
     assert runner.model.n_beams == 12  # Match the config
-    assert runner.model.max_iters == 2  # Match the config
+    assert runner.model.cosine_schedule_period_iters == 2  # Match the config
     assert next(runner.model.parameters()).device == torch.device("meta")
 
     # If the Trainer correctly moves the weights to the accelerator,
     # then it should fail if the weights are on the "meta" device.
     with torch.device("meta"):
         with ModelRunner(other_config, model_filename=str(ckpt)) as runner:
             with pytest.raises(NotImplementedError) as err:
@@ -95,14 +95,42 @@
             runner.evaluate([mgf_small])
 
     # Should work:
     with ModelRunner(config=config, model_filename=str(ckpt)) as runner:
         runner.evaluate([mgf_small])
 
 
+def test_save_and_load_weights_deprecated(tmp_path, mgf_small, tiny_config):
+    """Test saving and loading weights with deprecated config options."""
+    config = Config(tiny_config)
+    config.max_epochs = 1
+    config.cosine_schedule_period_iters = 5
+    ckpt = tmp_path / "test.ckpt"
+
+    with ModelRunner(config=config) as runner:
+        runner.train([mgf_small], [mgf_small])
+        runner.trainer.save_checkpoint(ckpt)
+
+    # Replace the new config option with the deprecated one.
+    ckpt_data = torch.load(ckpt)
+    ckpt_data["hyper_parameters"]["max_iters"] = 5
+    del ckpt_data["hyper_parameters"]["cosine_schedule_period_iters"]
+    torch.save(ckpt_data, str(ckpt))
+
+    # Inference.
+    with ModelRunner(config=config, model_filename=str(ckpt)) as runner:
+        runner.initialize_model(train=False)
+        assert runner.model.cosine_schedule_period_iters == 5
+    # Fine-tuning.
+    with ModelRunner(config=config, model_filename=str(ckpt)) as runner:
+        with pytest.warns(DeprecationWarning):
+            runner.train([mgf_small], [mgf_small])
+            assert "max_iters" not in runner.model.opt_kwargs
+
+
 def test_calculate_precision(tmp_path, mgf_small, tiny_config):
     """Test that this parameter is working correctly."""
     config = Config(tiny_config)
     config.n_layers = 1
     config.max_epochs = 1
     config.calculate_precision = False
     config.tb_summarywriter = str(tmp_path)
```

### Comparing `casanovo-4.1.0/tests/unit_tests/test_unit.py` & `casanovo-4.2.0/tests/unit_tests/test_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         step,
         finished_beams & ~discarded_beams,
         beam_fits_precursor,
         pred_cache,
     )
     # Verify that the correct peptides have been cached.
     correct_cached = 0
-    for _, _, pep in pred_cache[0]:
+    for _, _, _, pep in pred_cache[0]:
         if torch.equal(pep, torch.tensor([4, 14, 4, 13])):
             correct_cached += 1
         elif torch.equal(pep, torch.tensor([4, 14, 4, 18])):
             correct_cached += 1
         elif torch.equal(pep, torch.tensor([4, 14, 4])):
             correct_cached += 1
         else:
@@ -216,21 +216,21 @@
             )
     assert correct_cached == 1
 
     # Test _get_top_peptide().
     # Return the candidate peptide with the highest score
     test_cache = collections.OrderedDict((i, []) for i in range(batch))
     heapq.heappush(
-        test_cache[0], (0.93, 4 * [0.93], torch.tensor([4, 14, 4, 19]))
+        test_cache[0], (0.93, 0.1, 4 * [0.93], torch.tensor([4, 14, 4, 19]))
     )
     heapq.heappush(
-        test_cache[0], (0.95, 4 * [0.95], torch.tensor([4, 14, 4, 13]))
+        test_cache[0], (0.95, 0.2, 4 * [0.95], torch.tensor([4, 14, 4, 13]))
     )
     heapq.heappush(
-        test_cache[0], (0.94, 4 * [0.94], torch.tensor([4, 14, 4, 4]))
+        test_cache[0], (0.94, 0.3, 4 * [0.94], torch.tensor([4, 14, 4, 4]))
     )
 
     assert list(model._get_top_peptide(test_cache))[0][0][-1] == "PEPK"
     # Test that an empty predictions is returned when no beams have been
     # finished.
     empty_cache = collections.OrderedDict((i, []) for i in range(batch))
     assert len(list(model._get_top_peptide(empty_cache))[0]) == 0
@@ -292,15 +292,15 @@
     beam_fits_precursor = torch.BoolTensor([False, True, True, False])
 
     model._cache_finished_beams(
         tokens, scores, step, finished_beams, beam_fits_precursor, pred_cache
     )
     # Verify predictions with matching/non-matching precursor m/z.
     positive_score = negative_score = 0
-    for peptide_score, _, _ in pred_cache[0]:
+    for peptide_score, _, _, _ in pred_cache[0]:
         positive_score += peptide_score >= 0
         negative_score += peptide_score < 0
     assert positive_score == 2
     assert negative_score == 2
 
     # Test using a single beam only.
     model = Spec2Pep(n_beams=1, residues="massivekb", min_peptide_len=2)
@@ -431,15 +431,15 @@
     batch = 2  # B
     beam = model.n_beams  # S
     model.decoder.reverse = True
     length = model.max_length + 1  # L
     vocab = model.decoder.vocab_size + 1  # V
     step = 4
 
-    # Initialize dummyy scores and tokens.
+    # Initialize dummy scores and tokens.
     scores = torch.full(
         size=(batch, length, vocab, beam), fill_value=torch.nan
     )
     scores = einops.rearrange(scores, "B L V S -> (B S) L V")
     tokens = torch.zeros(batch * beam, length, dtype=torch.int64)
 
     # Simulate non-zero amino acid-level probability scores.
@@ -463,14 +463,45 @@
             [4, 14, 4, 28, 0],
             [4, 14, 4, 1, 3],
         ]
     )
 
     assert torch.equal(new_tokens[:, : step + 1], expected_tokens)
 
+    # Test that duplicate peptide scores don't lead to a conflict in the cache.
+    model = Spec2Pep(n_beams=5, residues="massivekb", min_peptide_len=3)
+    batch = 2  # B
+    beam = model.n_beams  # S
+    model.decoder.reverse = True
+    length = model.max_length + 1  # L
+    vocab = model.decoder.vocab_size + 1  # V
+    step = 4
+
+    # Simulate beams with identical amino acid scores but different tokens.
+    scores = torch.zeros(size=(batch * beam, length, vocab))
+    scores[: batch * beam, : step + 1, :] = torch.rand(1)
+    tokens = torch.zeros(batch * beam, length, dtype=torch.int64)
+    tokens[: batch * beam, :step] = torch.randint(
+        1, vocab, (batch * beam, step)
+    )
+
+    pred_cache = collections.OrderedDict((i, []) for i in range(batch))
+    model._cache_finished_beams(
+        tokens,
+        scores,
+        step,
+        torch.ones(batch * beam, dtype=torch.bool),
+        torch.ones(batch * beam, dtype=torch.bool),
+        pred_cache,
+    )
+    for beam_i, preds in pred_cache.items():
+        assert len(preds) == beam
+        peptide_scores = [pep[0] for pep in preds]
+        assert np.allclose(peptide_scores, peptide_scores[0])
+
 
 def test_eval_metrics():
     """
     Test peptide and amino acid-level evaluation metrics.
     Predicted AAs are considered correct if they are <0.1Da from the
     corresponding ground truth AA with either a suffix or prefix <0.5Da from
     the ground truth. A peptide prediction is correct if all its AA are correct
```


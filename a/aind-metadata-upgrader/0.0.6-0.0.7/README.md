# Comparing `tmp/aind-metadata-upgrader-0.0.6.tar.gz` & `tmp/aind_metadata_upgrader-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-metadata-upgrader-0.0.6.tar", last modified: Fri Mar 22 15:38:59 2024, max compression
+gzip compressed data, was "aind_metadata_upgrader-0.0.7.tar", last modified: Tue May 14 19:33:19 2024, max compression
```

## Comparing `aind-metadata-upgrader-0.0.6.tar` & `aind_metadata_upgrader-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.933670 aind-metadata-upgrader-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.933670 aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.933670 aind-metadata-upgrader-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.937670 aind-metadata-upgrader-0.0.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.937670 aind-metadata-upgrader-0.0.6/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.937670 aind-metadata-upgrader-0.0.6/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.933670 aind-metadata-upgrader-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.937670 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 15:38:45.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/base_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/data_description_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/processing_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-22 15:38:59.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-22 15:38:59.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:38:59.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-22 15:38:59.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 15:38:59.000000 aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.937670 aind-metadata-upgrader-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.933670 aind-metadata-upgrader-0.0.6/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.10.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.11.0_wrong_funder.json
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0_no_creation.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0_wrong_field.json
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2_funding_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2_wrong_field.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:38:59.941670 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.0.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.2.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.2.5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.3.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_other_no_notes.json
--rw-r--r--   0 runner    (1001) docker     (127)    29239 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/test_data_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-03-22 15:38:44.000000 aind-metadata-upgrader-0.0.6/tests/test_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.702986 aind_metadata_upgrader-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.710986 aind_metadata_upgrader-0.0.7/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.710986 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 19:33:09.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/base_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/data_description_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22691 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/procedures_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/processing_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-14 19:33:19.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-14 19:33:19.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:33:19.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 19:33:19.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 19:33:19.000000 aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.710986 aind_metadata_upgrader-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.714986 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.10.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.11.0_wrong_funder.json
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0_no_creation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0_wrong_field.json
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2_funding_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2_wrong_field.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.714986 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.2.5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.3.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_other_no_notes.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.706986 aind_metadata_upgrader-0.0.7/tests/resources/procedures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.714986 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/652505_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/656376_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/665259_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/674182_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/675376_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/679811_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/689238_procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/U19_examples/698034_procedures.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/609281.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/609281_invalid_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/652504_U19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/652742.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/653980.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/664644.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/667825.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/676909.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/676909_test_craniotomy_size.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/699835_U19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/class_model_examples/699835_U19_new_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:19.718986 aind_metadata_upgrader-0.0.7/tests/resources/procedures/log_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/resources/procedures/log_files/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29239 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/test_data_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/test_procedures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-14 19:33:08.000000 aind_metadata_upgrader-0.0.7/tests/test_utils.py
```

### Comparing `aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_upgrader-0.0.7/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.github/workflows/init.yml` & `aind_metadata_upgrader-0.0.7/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.github/workflows/tag_and_publish.yml` & `aind_metadata_upgrader-0.0.7/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.github/workflows/test_and_lint.yml` & `aind_metadata_upgrader-0.0.7/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/.gitignore` & `aind_metadata_upgrader-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/LICENSE` & `aind_metadata_upgrader-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/PKG-INFO` & `aind_metadata_upgrader-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-metadata-upgrader
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aind-data-schema==0.31.8
+Requires-Dist: pydantic<2.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

### Comparing `aind-metadata-upgrader-0.0.6/README.md` & `aind_metadata_upgrader-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/Makefile` & `aind_metadata_upgrader-0.0.7/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/make.bat` & `aind_metadata_upgrader-0.0.7/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/source/_static/dark-logo.svg` & `aind_metadata_upgrader-0.0.7/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/source/_static/favicon.ico` & `aind_metadata_upgrader-0.0.7/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/source/_static/light-logo.svg` & `aind_metadata_upgrader-0.0.7/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/doc_template/source/conf.py` & `aind_metadata_upgrader-0.0.7/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/pyproject.toml` & `aind_metadata_upgrader-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    'aind-data-schema==0.31.8'
+    'aind-data-schema==0.31.8',
+    'pydantic<2.7'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
```

### Comparing `aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/base_upgrade.py` & `aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/base_upgrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module to contain base code to upgrade old models"""
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from typing import Any, Type, Union
 
 from aind_data_schema.base import AindModel
 from pydantic.fields import PydanticUndefined
 
 
 class BaseModelUpgrade(ABC):
@@ -54,12 +54,7 @@
             try:
                 attr_default = getattr(self.model_class.model_fields.get(field_name), "default")
                 if attr_default == PydanticUndefined:
                     return None
                 return attr_default
             except AttributeError:
                 return None
-
-    @abstractmethod
-    def upgrade(self, **kwargs) -> AindModel:
-        """Upgrades the old model into the current version"""
-        raise NotImplementedError  # "pragma: no cover"
```

### Comparing `aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/data_description_upgrade.py` & `aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/data_description_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Module to contain code to upgrade old data description models"""
 
 from copy import deepcopy
 from datetime import datetime
-from typing import Any, Optional, Union, List
+from typing import Any, List, Optional, Union
 
 import semver
 from aind_data_schema.base import AindModel
 from aind_data_schema.core.data_description import (
     DataDescription,
     DataLevel,
     Funding,
 )
 from aind_data_schema.models.modalities import Modality
 from aind_data_schema.models.organizations import Organization
-from aind_data_schema.models.platforms import Platform
 from aind_data_schema.models.pid_names import PIDName
+from aind_data_schema.models.platforms import Platform
 
 from aind_metadata_upgrader.base_upgrade import BaseModelUpgrade
 
 
 class ModalityUpgrade:
     """Handle upgrades for Modality models."""
```

### Comparing `aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader/processing_upgrade.py` & `aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader/processing_upgrade.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/src/aind_metadata_upgrader.egg-info/PKG-INFO` & `aind_metadata_upgrader-0.0.7/src/aind_metadata_upgrader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-metadata-upgrader
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aind-data-schema==0.31.8
+Requires-Dist: pydantic<2.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.10.0.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.10.0.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.11.0_wrong_funder.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.11.0_wrong_funder.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0_no_creation.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0_no_creation.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.3.0_wrong_field.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.3.0_wrong_field.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.4.0.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.4.0.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.0.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.0.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2_funding_map.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2_funding_map.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_data_description/data_description_0.6.2_wrong_field.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_data_description/data_description_0.6.2_wrong_field.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.0.1.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.0.1.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.1.0.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.1.0.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.2.1.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.2.1.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.2.5.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.2.5.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_0.3.1.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_0.3.1.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/resources/ephys_processing/processing_other_no_notes.json` & `aind_metadata_upgrader-0.0.7/tests/resources/ephys_processing/processing_other_no_notes.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-upgrader-0.0.6/tests/test_data_description.py` & `aind_metadata_upgrader-0.0.7/tests/test_data_description.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     DataLevel,
     Funding,
     Group,
     RelatedData,
 )
 from aind_data_schema.models.modalities import Modality
 from aind_data_schema.models.organizations import Organization
-from aind_data_schema.models.platforms import Platform
 from aind_data_schema.models.pid_names import PIDName
+from aind_data_schema.models.platforms import Platform
 from pydantic import ValidationError
 from pydantic import __version__ as pyd_version
 
 from aind_metadata_upgrader.data_description_upgrade import (
     DataDescriptionUpgrade,
     FundingUpgrade,
     InstitutionUpgrade,
-    ModalityUpgrade,
     InvestigatorsUpgrade,
+    ModalityUpgrade,
 )
 
 DATA_DESCRIPTION_FILES_PATH = Path(__file__).parent / "resources" / "ephys_data_description"
 PYD_VERSION = re.match(r"(\d+.\d+).\d+", pyd_version).group(1)
 
 
 class TestDataDescriptionUpgrade(unittest.TestCase):
```

### Comparing `aind-metadata-upgrader-0.0.6/tests/test_processing.py` & `aind_metadata_upgrader-0.0.7/tests/test_processing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import json
 import os
 import re
 import unittest
 from pathlib import Path
 from typing import List
 
+from aind_data_schema.base import AindGeneric
 from aind_data_schema.core.processing import (
     DataProcess,
     PipelineProcess,
     Processing,
 )
-from aind_data_schema.base import AindGeneric
 from pydantic import __version__ as pyd_version
 
 from aind_metadata_upgrader.processing_upgrade import (
     DataProcessUpgrade,
     ProcessingUpgrade,
 )
```


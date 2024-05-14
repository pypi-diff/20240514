# Comparing `tmp/volkswagencarnet-4.4.9.tar.gz` & `tmp/volkswagencarnet-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volkswagencarnet-4.4.9.tar", last modified: Tue Jun 23 13:37:00 2020, max compression
+gzip compressed data, was "volkswagencarnet-5.0.0b1.tar", last modified: Tue May 14 13:31:17 2024, max compression
```

## Comparing `volkswagencarnet-4.4.9.tar` & `volkswagencarnet-5.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (116)      532 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      407 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1014 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)      774 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1379 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/validate.yml
--rw-r--r--   0 runner    (1001) docker     (116)    11356 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4599 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17802 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (116)       42 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      896 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/tests/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      511 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    50553 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/volkswagencarnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.641037 volkswagencarnet-5.0.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/snyk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/testrelease.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/validate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/validate_pr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34876 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/credentials.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/dummy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/mock_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/fixtures/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/dummy_cookies.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14352 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/selectivestatus_by_app.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer_without_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_utilities_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_vehicle_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/volkswagencarnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45931 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49000 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146387 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/top_level.txt
```

### Comparing `volkswagencarnet-4.4.9/.github/release-drafter.yml` & `volkswagencarnet-5.0.0b1/.github/release-drafter.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 name-template: "v$RESOLVED_VERSION 🌈"
 tag-template: "v$RESOLVED_VERSION"
+change-template: "- #$NUMBER $TITLE @$AUTHOR"
+sort-direction: ascending
 categories:
   - title: "🚀 Features"
     labels:
       - "feature"
       - "enhancement"
+
   - title: "🐛 Bug Fixes"
     labels:
       - "fix"
       - "bugfix"
       - "bug"
+
   - title: "🧰 Maintenance"
-    label: "chore"
-change-template: "- $TITLE @$AUTHOR (#$NUMBER)"
+    labels:
+      - "dependencies"
+      - "refactoring"
+      - "tests"
+
 version-resolver:
   major:
     labels:
       - "major"
   minor:
     labels:
       - "minor"
```

### Comparing `volkswagencarnet-4.4.9/.github/workflows/validate.yml` & `volkswagencarnet-5.0.0b1/.github/workflows/validate.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
+# This workflow will install Python dependencies, run tests and ruff with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Validate
 
 #on: [push]
 #on: [push, pull_request]
 on:
@@ -10,37 +10,54 @@
     branches:
       - master
   push:
     branches:
       - master
 
 jobs:
-  build:
+  ruff:
+    name: Ruff
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v4
+
+      - name: Check ruff
+        uses: chartboost/ruff-action@v1
+        with:
+          args: 'format --diff'
+
+  test-n-build:
+    name: Test and Build
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8]
+        python-version: ["3.11", "3.12"]
 
     steps:
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install flake8 pytest
+          pip install pytest build twine setuptools setuptools_scm
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+          if [ -f requirements-test.txt ]; then pip install -r requirements-test.txt; fi
 
-      - name: Lint with flake8
-        run: |
-          # stop the build if there are Python syntax errors or undefined names
-          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
       - name: Test with pytest
         run: |
           pytest
+
+      - name: Test build package
+        run: |
+          python -m build --outdir dist/
+          python -m twine check dist/*
+          python -m setuptools_scm --strip-dev
```

### Comparing `volkswagencarnet-4.4.9/PKG-INFO` & `volkswagencarnet-5.0.0b1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,182 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 4.4.9
-Summary: Communicate with Volkswagen WeConnect
+Version: 5.0.0b1
+Summary: Communicate with Volkswagen Connect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
-License: UNKNOWN
-Description: # Volkswagen Carnet
-        
-        [![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/robinostlund)
-        
-        ![Python package](https://github.com/robinostlund/volkswagencarnet/workflows/Python%20package/badge.svg)
-        ![Upload Python Package](https://github.com/robinostlund/volkswagencarnet/workflows/Upload%20Python%20Package/badge.svg)
-        
-        ![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet?label=Downloads)
-        ![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet?label=Downloads%20)
-        ![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet?label=Downloads%20)
-        
-        ![Latest PyPi Version](https://img.shields.io/pypi/v/volkswagencarnet?label=Latest%20PyPi%20Version)
-        ![Latest Github Tag](https://img.shields.io/github/v/tag/robinostlund/volkswagencarnet?label=Latest%20Github%20Tag)
-        
-        ## Information
-        
-        Retrieve statistics about your Volkswagen from the Volkswagen Carnet online service
-        
-        No licence, public domain, no guarantees, feel free to use for anything. Please contribute improvements/bugfixes etc.
-        
-        ## Thanks to
-        
-        - [Wez3](https://github.com/wez3)
-        - [Reneboer](https://github.com/reneboer)
-        - [Tubalainen](https://github.com/tubalainen)
-        
-        For supporting and helping in this project.
-        
-        ## Other related repositories
-        
-        - [HomeAssistant Component](https://github.com/robinostlund/homeassistant-volkswagencarnet) a custom component for Home Assistant
-        - [VolkswagenCarnetClient](https://github.com/robinostlund/volkswagencarnet-client) a cli version of this library
-        
-        ## Installation
-        
-        ```sh
-        [venv-python3] user@localhost:~
-        $ pip install volkswagencarnet
-        ```
-        
-        ### Example
-        
-        ```python
-        #!/usr/bin/env python3
-        import volkswagencarnet
-        import pprint
-        import asyncio
-        import logging
-        
-        from aiohttp import ClientSession
-        
-        logging.basicConfig(level=logging.DEBUG)
-        
-        VW_USERNAME='test@example.com'
-        VW_PASSWORD='mysecretpassword
-        
-        
-        COMPONENTS = {
-            'sensor': 'sensor',
-            'binary_sensor': 'binary_sensor',
-            'lock': 'lock',
-            'device_tracker': 'device_tracker',
-            'switch': 'switch',
-            'climate': 'climate'
-        }
-        
-        RESOURCES = [
-            'position',
-            'distance',
-            'electric_climatisation',
-            'combustion_climatisation',
-            'window_heater',
-            'combustion_engine_heating',
-            'charging',
-            'adblue_level',
-            'battery_level',
-            'fuel_level',
-            'service_inspection',
-            'oil_inspection',
-            'last_connected',
-            'charging_time_left',
-            'electric_range',
-            'combustion_range',
-            'combined_range',
-            'charge_max_ampere',
-            'climatisation_target_temperature',
-            'external_power',
-            'parking_light',
-            'climatisation_without_external_power',
-            'door_locked',
-            'trunk_locked',
-            'request_in_progress',
-            'windows_closed',
-            'trip_last_average_speed',
-            'trip_last_average_electric_consumption',
-            'trip_last_average_fuel_consumption',
-            'trip_last_duration',
-            'trip_last_length'
-        ]
-        
-        def is_enabled(attr):
-            """Return true if the user has enabled the resource."""
-            return attr in RESOURCES
-        
-        async def main():
-            """Main method."""
-            async with ClientSession() as session:
-                connection = volkswagencarnet.Connection(session, VW_USERNAME, VW_PASSWORD)
-                if await connection._login():
-                    if await connection.update(request_data=False):
-                        # Print overall state
-                        pprint.pprint(connection._state)
-        
-                        # Print vehicles
-                        for vehicle in connection.vehicles:
-                            pprint.pprint(vehicle)
-        
-                        # get all instruments
-                        instruments = set()
-                        for vehicle in connection.vehicles:
-                            dashboard = vehicle.dashboard(mutable=True)
-        
-                            for instrument in (
-                                    instrument
-                                    for instrument in dashboard.instruments
-                                    if instrument.component in COMPONENTS
-                                    and is_enabled(instrument.slug_attr)):
-        
-                                instruments.add(instrument)
-        
-                        # Output all supported instruments
-                        for instrument in instruments:
-                            print(f'name: {instrument.full_name}')
-                            print(f'str_state: {instrument.str_state}')
-                            print(f'state: {instrument.state}')
-                            print(f'supported: {instrument.is_supported}')
-                            print(f'attr: {instrument.attr}')
-                            print(f'attributes: {instrument.attributes}')
-        
-        if __name__ == "__main__":
-            loop = asyncio.get_event_loop()
-            # loop.run(main())
-            loop.run_until_complete(main())
-        ```
-        
-Platform: UNKNOWN
-Provides: volkswagencarnet
+License: GPLv3
+Project-URL: Bug Tracker, https://github.com/robinostlund/volkswagencarnet/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: lxml
+Requires-Dist: beautifulsoup4
+Requires-Dist: aiohttp
+Requires-Dist: pyjwt
+
+# Volkswagen Carnet
+
+[![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/robinostlund)
+
+![Release](https://img.shields.io/github/workflow/status/robinostlund/volkswagencarnet/Release)
+![PyPi](https://img.shields.io/pypi/v/volkswagencarnet)
+![Version](https://img.shields.io/github/v/release/robinostlund/volkswagencarnet)
+![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)
+![Known Vulnerabilities](https://snyk.io/test/github/robinostlund/volkswagencarnet/badge.svg)
+[![CodeQL](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml)
+[![codecov](https://codecov.io/gh/robinostlund/volkswagencarnet/branch/master/graph/badge.svg?token=NH1Q1GH4I3)](https://codecov.io/gh/robinostlund/volkswagencarnet)
+
+
+![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet)
+![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet)
+![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet)
+
+## Help Wanted
+
+As i don't have a car with Volkswagen Connect anymore i would appreciate if it would be possible to get help to keep this repository maintained. So if you feel that you have some time over and is interested in helping out with this. Please feel to contact me! Thanks
+
+## Information
+
+Retrieve statistics about your Volkswagen from the Volkswagen Carnet online service
+
+No licence, public domain, no guarantees, feel free to use for anything. Please contribute improvements/bugfixes etc.
+
+## Thanks to
+
+- [Wez3](https://github.com/wez3)
+- [Reneboer](https://github.com/reneboer)
+- [Tubalainen](https://github.com/tubalainen)
+- [JohNan](https://github.com/JohNan)
+- [milkboy](https://github.com/milkboy)
+
+For supporting and helping in this project.
+
+## Other related repositories
+
+- [HomeAssistant Component](https://github.com/robinostlund/homeassistant-volkswagencarnet) a custom component for Home Assistant
+
+## Installation
+
+```sh
+[venv-python3] user@localhost:~
+$ pip install volkswagencarnet
+```
+
+### Example
+
+```python
+#!/usr/bin/env python3
+from volkswagencarnet.vw_connection import Connection
+import pprint
+import asyncio
+import logging
+
+from aiohttp import ClientSession
+
+logging.basicConfig(level=logging.DEBUG)
+
+VW_USERNAME='test@example.com'
+VW_PASSWORD='mysecretpassword'
+
+
+COMPONENTS = {
+    'sensor': 'sensor',
+    'binary_sensor': 'binary_sensor',
+    'lock': 'lock',
+    'device_tracker': 'device_tracker',
+    'switch': 'switch',
+    'climate': 'climate'
+}
+
+RESOURCES = [
+    'position',
+    'distance',
+    'electric_climatisation',
+    'combustion_climatisation',
+    'window_heater',
+    'combustion_engine_heating',
+    'charging',
+    'adblue_level',
+    'battery_level',
+    'fuel_level',
+    'service_inspection',
+    'oil_inspection',
+    'last_connected',
+    'charging_time_left',
+    'electric_range',
+    'combustion_range',
+    'combined_range',
+    'charge_max_ampere',
+    'climatisation_target_temperature',
+    'external_power',
+    'parking_light',
+    'climatisation_without_external_power',
+    'door_locked',
+    'trunk_locked',
+    'request_in_progress',
+    'windows_closed',
+    'sunroof_closed',
+    'trip_last_average_speed',
+    'trip_last_average_electric_consumption',
+    'trip_last_average_fuel_consumption',
+    'trip_last_duration',
+    'trip_last_length'
+]
+
+def is_enabled(attr):
+    """Return true if the user has enabled the resource."""
+    return attr in RESOURCES
+
+async def main():
+    """Main method."""
+    async with ClientSession(headers={'Connection': 'keep-alive'}) as session:
+        connection = Connection(session, VW_USERNAME, VW_PASSWORD)
+        if await connection.doLogin():
+            if await connection.update():
+                # Print overall state
+                pprint.pprint(connection._state)
+
+                # Print vehicles
+                for vehicle in connection.vehicles:
+                    pprint.pprint(vehicle)
+
+                # get all instruments
+                instruments = set()
+                for vehicle in connection.vehicles:
+                    dashboard = vehicle.dashboard(mutable=True)
+
+                    for instrument in (
+                            instrument
+                            for instrument in dashboard.instruments
+                            if instrument.component in COMPONENTS
+                            and is_enabled(instrument.slug_attr)):
+
+                        instruments.add(instrument)
+
+                # Output all supported instruments
+                for instrument in instruments:
+                    print(f'name: {instrument.full_name}')
+                    print(f'str_state: {instrument.str_state}')
+                    print(f'state: {instrument.state}')
+                    print(f'supported: {instrument.is_supported}')
+                    print(f'attr: {instrument.attr}')
+                    print(f'attributes: {instrument.attributes}')
+
+if __name__ == "__main__":
+    loop = asyncio.get_event_loop()
+    # loop.run(main())
+    loop.run_until_complete(main())
+```
+
+## Development
+I'd strongly advise installing the git pre-commit hook using `pre-commit install`. See [pre-commit.com](https://pre-commit.com/) for details.
+Some basic checks are performed before you commit the code, so code style issues
+will be visible and fixable before creating the PR. Git pre-commit hooks can
+always be skipped using the `--no-verify` flag to `git commit`, if there
+is something preventing you from actually fixing the reported (and non-auto-fixed) issues.
+
+Decent test coverage for any new or changed code is also much appreciated :)
```

### Comparing `volkswagencarnet-4.4.9/README.md` & `volkswagencarnet-5.0.0b1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 # Volkswagen Carnet
 
 [![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/robinostlund)
 
-![Python package](https://github.com/robinostlund/volkswagencarnet/workflows/Python%20package/badge.svg)
-![Upload Python Package](https://github.com/robinostlund/volkswagencarnet/workflows/Upload%20Python%20Package/badge.svg)
+![Release](https://img.shields.io/github/workflow/status/robinostlund/volkswagencarnet/Release)
+![PyPi](https://img.shields.io/pypi/v/volkswagencarnet)
+![Version](https://img.shields.io/github/v/release/robinostlund/volkswagencarnet)
+![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)
+![Known Vulnerabilities](https://snyk.io/test/github/robinostlund/volkswagencarnet/badge.svg)
+[![CodeQL](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml)
+[![codecov](https://codecov.io/gh/robinostlund/volkswagencarnet/branch/master/graph/badge.svg?token=NH1Q1GH4I3)](https://codecov.io/gh/robinostlund/volkswagencarnet)
+
+
+![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet)
+![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet)
+![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet)
 
-![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet?label=Downloads)
-![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet?label=Downloads%20)
-![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet?label=Downloads%20)
+## Help Wanted
 
-![Latest PyPi Version](https://img.shields.io/pypi/v/volkswagencarnet?label=Latest%20PyPi%20Version)
-![Latest Github Tag](https://img.shields.io/github/v/tag/robinostlund/volkswagencarnet?label=Latest%20Github%20Tag)
+As i don't have a car with Volkswagen Connect anymore i would appreciate if it would be possible to get help to keep this repository maintained. So if you feel that you have some time over and is interested in helping out with this. Please feel to contact me! Thanks
 
 ## Information
 
 Retrieve statistics about your Volkswagen from the Volkswagen Carnet online service
 
 No licence, public domain, no guarantees, feel free to use for anything. Please contribute improvements/bugfixes etc.
 
 ## Thanks to
 
 - [Wez3](https://github.com/wez3)
 - [Reneboer](https://github.com/reneboer)
 - [Tubalainen](https://github.com/tubalainen)
+- [JohNan](https://github.com/JohNan)
+- [milkboy](https://github.com/milkboy)
 
 For supporting and helping in this project.
 
 ## Other related repositories
 
 - [HomeAssistant Component](https://github.com/robinostlund/homeassistant-volkswagencarnet) a custom component for Home Assistant
-- [VolkswagenCarnetClient](https://github.com/robinostlund/volkswagencarnet-client) a cli version of this library
 
 ## Installation
 
 ```sh
 [venv-python3] user@localhost:~
 $ pip install volkswagencarnet
 ```
 
 ### Example
 
 ```python
 #!/usr/bin/env python3
-import volkswagencarnet
+from volkswagencarnet.vw_connection import Connection
 import pprint
 import asyncio
 import logging
 
 from aiohttp import ClientSession
 
 logging.basicConfig(level=logging.DEBUG)
 
 VW_USERNAME='test@example.com'
-VW_PASSWORD='mysecretpassword
+VW_PASSWORD='mysecretpassword'
 
 
 COMPONENTS = {
     'sensor': 'sensor',
     'binary_sensor': 'binary_sensor',
     'lock': 'lock',
     'device_tracker': 'device_tracker',
@@ -87,31 +95,32 @@
     'external_power',
     'parking_light',
     'climatisation_without_external_power',
     'door_locked',
     'trunk_locked',
     'request_in_progress',
     'windows_closed',
+    'sunroof_closed',
     'trip_last_average_speed',
     'trip_last_average_electric_consumption',
     'trip_last_average_fuel_consumption',
     'trip_last_duration',
     'trip_last_length'
 ]
 
 def is_enabled(attr):
     """Return true if the user has enabled the resource."""
     return attr in RESOURCES
 
 async def main():
     """Main method."""
-    async with ClientSession() as session:
-        connection = volkswagencarnet.Connection(session, VW_USERNAME, VW_PASSWORD)
-        if await connection._login():
-            if await connection.update(request_data=False):
+    async with ClientSession(headers={'Connection': 'keep-alive'}) as session:
+        connection = Connection(session, VW_USERNAME, VW_PASSWORD)
+        if await connection.doLogin():
+            if await connection.update():
                 # Print overall state
                 pprint.pprint(connection._state)
 
                 # Print vehicles
                 for vehicle in connection.vehicles:
                     pprint.pprint(vehicle)
 
@@ -138,7 +147,16 @@
                     print(f'attributes: {instrument.attributes}')
 
 if __name__ == "__main__":
     loop = asyncio.get_event_loop()
     # loop.run(main())
     loop.run_until_complete(main())
 ```
+
+## Development
+I'd strongly advise installing the git pre-commit hook using `pre-commit install`. See [pre-commit.com](https://pre-commit.com/) for details.
+Some basic checks are performed before you commit the code, so code style issues
+will be visible and fixable before creating the PR. Git pre-commit hooks can
+always be skipped using the `--no-verify` flag to `git commit`, if there
+is something preventing you from actually fixing the reported (and non-auto-fixed) issues.
+
+Decent test coverage for any new or changed code is also much appreciated :)
```

### Comparing `volkswagencarnet-4.4.9/utilities.py` & `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,137 @@
-from datetime import date, datetime
-from base64 import b64encode
-from string import ascii_letters as letters, digits
-from sys import argv
-from os import environ as env
-from os.path import join, dirname, expanduser
-from itertools import product
+"""Common utility functions."""
+
+from datetime import datetime
 import json
 import logging
 import re
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def read_config():
-    """Read config from file."""
-    for directory, filename in product(
-        [
-            dirname(argv[0]),
-            expanduser("~"),
-            env.get("XDG_CONFIG_HOME", join(expanduser("~"), ".config")),
-        ],
-        ["vw.conf", ".vw.conf"],
-    ):
-        try:
-            config = join(directory, filename)
-            _LOGGER.debug("checking for config file %s", config)
-            with open(config) as config:
-                return dict(
-                    x.split(": ")
-                    for x in config.read().strip().splitlines()
-                    if not x.startswith("#")
-                )
-        except (IOError, OSError):
-            continue
-    return {}
-
-
-def json_loads(s):
+def json_loads(s) -> object:
+    """Load JSON from string and parse timestamps."""
     return json.loads(s, object_hook=obj_parser)
 
 
-def obj_parser(obj):
+def obj_parser(obj: dict) -> dict:
     """Parse datetime."""
     for key, val in obj.items():
         try:
             obj[key] = datetime.strptime(val, "%Y-%m-%dT%H:%M:%S%z")
         except (TypeError, ValueError):
-            pass
+            """The value was not a date."""  # pylint: disable=pointless-string-statement
     return obj
 
 
-def find_path(src, path):
-    """Simple navigation of a hierarchical dict structure using XPATH-like syntax.
+def find_path_in_dict(src: dict | list, path: str | list) -> object:
+    """Return data at path in dictionary source.
+
+    Simple navigation of a hierarchical dict structure using XPATH-like syntax.
 
-    >>> find_path(dict(a=1), 'a')
+    >>> find_path_in_dict(dict(a=1), 'a')
     1
 
-    >>> find_path(dict(a=1), '')
+    >>> find_path_in_dict(dict(a=1), '')
     {'a': 1}
 
-    >>> find_path(dict(a=None), 'a')
+    >>> find_path_in_dict(dict(a=None), 'a')
 
 
-    >>> find_path(dict(a=1), 'b')
+    >>> find_path_in_dict(dict(a=1), 'b')
     Traceback (most recent call last):
     ...
     KeyError: 'b'
 
-    >>> find_path(dict(a=dict(b=1)), 'a.b')
+    >>> find_path_in_dict(dict(a=dict(b=1)), 'a.b')
     1
 
-    >>> find_path(dict(a=dict(b=1)), 'a')
+    >>> find_path_in_dict(dict(a=dict(b=1)), 'a')
     {'b': 1}
 
-    >>> find_path(dict(a=dict(b=1)), 'a.c')
+    >>> find_path_in_dict(dict(a=dict(b=1)), 'a.c')
     Traceback (most recent call last):
     ...
     KeyError: 'c'
 
     """
     if not path:
         return src
     if isinstance(path, str):
         path = path.split(".")
-    return find_path(src[path[0]], path[1:])
+    if isinstance(src, list):
+        try:
+            f = float(path[0])
+            if f.is_integer() and len(src) > 0:
+                return find_path_in_dict(src[int(f)], path[1:])
+            raise KeyError("Key not found")
+        except ValueError as valerr:
+            raise KeyError(f"{path[0]} should be an integer") from valerr
+        except IndexError as idxerr:
+            raise KeyError("Index out of range") from idxerr
+    return find_path_in_dict(src[path[0]], path[1:])
+
+
+def find_path(src: dict | list, path: str | list) -> object:
+    """Return data at path in source."""
+    try:
+        return find_path_in_dict(src, path)
+    except KeyError:
+        _LOGGER.error(
+            "Dictionary path: %s is no longer present. Dictionary: %s", path, src
+        )
+        return None
 
 
 def is_valid_path(src, path):
-    """
+    """Check if path exists in source.
+
     >>> is_valid_path(dict(a=1), 'a')
     True
 
     >>> is_valid_path(dict(a=1), '')
     True
 
     >>> is_valid_path(dict(a=1), None)
     True
 
     >>> is_valid_path(dict(a=1), 'b')
     False
+
+    >>> is_valid_path({"a": [{"b": True}, {"c": True}]}, 'a.0.b')
+    True
+
+    >>> is_valid_path({"a": [{"b": True}, {"c": True}]}, 'a.1.b')
+    False
     """
     try:
-        find_path(src, path)
-        return True
+        find_path_in_dict(src, path)
     except KeyError:
         return False
+    else:
+        return True
 
 
-def camel2slug(s):
+def camel2slug(s: str) -> str:
     """Convert camelCase to camel_case.
 
     >>> camel2slug('fooBar')
     'foo_bar'
+
+    Should not produce "__" in case input contains something like "Foo_Bar"
     """
-    return re.sub("([A-Z])", "_\\1", s).lower().lstrip("_")
+    return re.sub("((?<!_)[A-Z])", "_\\1", s).lower().strip("_ \n\t\r")
+
+
+def make_url(url: str, **kwargs: str) -> str:
+    """Replace placeholders in a URL with given keyword arguments."""
+
+    # Replace both `{key}` and `$key` in the URL
+    for key, value in kwargs.items():
+        placeholder1 = f"{{{key}}}"
+        placeholder2 = f"${key}"
+        url = url.replace(placeholder1, str(value)).replace(placeholder2, str(value))
+
+    # Check if any unreplaced placeholders remain
+    if "{" in url or "}" in url:
+        raise ValueError("Not all placeholders were replaced in the URL")
+    return url
```

### Comparing `volkswagencarnet-4.4.9/volkswagencarnet.egg-info/PKG-INFO` & `volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,182 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 4.4.9
-Summary: Communicate with Volkswagen WeConnect
+Version: 5.0.0b1
+Summary: Communicate with Volkswagen Connect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
-License: UNKNOWN
-Description: # Volkswagen Carnet
-        
-        [![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/robinostlund)
-        
-        ![Python package](https://github.com/robinostlund/volkswagencarnet/workflows/Python%20package/badge.svg)
-        ![Upload Python Package](https://github.com/robinostlund/volkswagencarnet/workflows/Upload%20Python%20Package/badge.svg)
-        
-        ![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet?label=Downloads)
-        ![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet?label=Downloads%20)
-        ![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet?label=Downloads%20)
-        
-        ![Latest PyPi Version](https://img.shields.io/pypi/v/volkswagencarnet?label=Latest%20PyPi%20Version)
-        ![Latest Github Tag](https://img.shields.io/github/v/tag/robinostlund/volkswagencarnet?label=Latest%20Github%20Tag)
-        
-        ## Information
-        
-        Retrieve statistics about your Volkswagen from the Volkswagen Carnet online service
-        
-        No licence, public domain, no guarantees, feel free to use for anything. Please contribute improvements/bugfixes etc.
-        
-        ## Thanks to
-        
-        - [Wez3](https://github.com/wez3)
-        - [Reneboer](https://github.com/reneboer)
-        - [Tubalainen](https://github.com/tubalainen)
-        
-        For supporting and helping in this project.
-        
-        ## Other related repositories
-        
-        - [HomeAssistant Component](https://github.com/robinostlund/homeassistant-volkswagencarnet) a custom component for Home Assistant
-        - [VolkswagenCarnetClient](https://github.com/robinostlund/volkswagencarnet-client) a cli version of this library
-        
-        ## Installation
-        
-        ```sh
-        [venv-python3] user@localhost:~
-        $ pip install volkswagencarnet
-        ```
-        
-        ### Example
-        
-        ```python
-        #!/usr/bin/env python3
-        import volkswagencarnet
-        import pprint
-        import asyncio
-        import logging
-        
-        from aiohttp import ClientSession
-        
-        logging.basicConfig(level=logging.DEBUG)
-        
-        VW_USERNAME='test@example.com'
-        VW_PASSWORD='mysecretpassword
-        
-        
-        COMPONENTS = {
-            'sensor': 'sensor',
-            'binary_sensor': 'binary_sensor',
-            'lock': 'lock',
-            'device_tracker': 'device_tracker',
-            'switch': 'switch',
-            'climate': 'climate'
-        }
-        
-        RESOURCES = [
-            'position',
-            'distance',
-            'electric_climatisation',
-            'combustion_climatisation',
-            'window_heater',
-            'combustion_engine_heating',
-            'charging',
-            'adblue_level',
-            'battery_level',
-            'fuel_level',
-            'service_inspection',
-            'oil_inspection',
-            'last_connected',
-            'charging_time_left',
-            'electric_range',
-            'combustion_range',
-            'combined_range',
-            'charge_max_ampere',
-            'climatisation_target_temperature',
-            'external_power',
-            'parking_light',
-            'climatisation_without_external_power',
-            'door_locked',
-            'trunk_locked',
-            'request_in_progress',
-            'windows_closed',
-            'trip_last_average_speed',
-            'trip_last_average_electric_consumption',
-            'trip_last_average_fuel_consumption',
-            'trip_last_duration',
-            'trip_last_length'
-        ]
-        
-        def is_enabled(attr):
-            """Return true if the user has enabled the resource."""
-            return attr in RESOURCES
-        
-        async def main():
-            """Main method."""
-            async with ClientSession() as session:
-                connection = volkswagencarnet.Connection(session, VW_USERNAME, VW_PASSWORD)
-                if await connection._login():
-                    if await connection.update(request_data=False):
-                        # Print overall state
-                        pprint.pprint(connection._state)
-        
-                        # Print vehicles
-                        for vehicle in connection.vehicles:
-                            pprint.pprint(vehicle)
-        
-                        # get all instruments
-                        instruments = set()
-                        for vehicle in connection.vehicles:
-                            dashboard = vehicle.dashboard(mutable=True)
-        
-                            for instrument in (
-                                    instrument
-                                    for instrument in dashboard.instruments
-                                    if instrument.component in COMPONENTS
-                                    and is_enabled(instrument.slug_attr)):
-        
-                                instruments.add(instrument)
-        
-                        # Output all supported instruments
-                        for instrument in instruments:
-                            print(f'name: {instrument.full_name}')
-                            print(f'str_state: {instrument.str_state}')
-                            print(f'state: {instrument.state}')
-                            print(f'supported: {instrument.is_supported}')
-                            print(f'attr: {instrument.attr}')
-                            print(f'attributes: {instrument.attributes}')
-        
-        if __name__ == "__main__":
-            loop = asyncio.get_event_loop()
-            # loop.run(main())
-            loop.run_until_complete(main())
-        ```
-        
-Platform: UNKNOWN
-Provides: volkswagencarnet
+License: GPLv3
+Project-URL: Bug Tracker, https://github.com/robinostlund/volkswagencarnet/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: lxml
+Requires-Dist: beautifulsoup4
+Requires-Dist: aiohttp
+Requires-Dist: pyjwt
+
+# Volkswagen Carnet
+
+[![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/robinostlund)
+
+![Release](https://img.shields.io/github/workflow/status/robinostlund/volkswagencarnet/Release)
+![PyPi](https://img.shields.io/pypi/v/volkswagencarnet)
+![Version](https://img.shields.io/github/v/release/robinostlund/volkswagencarnet)
+![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)
+![Known Vulnerabilities](https://snyk.io/test/github/robinostlund/volkswagencarnet/badge.svg)
+[![CodeQL](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/robinostlund/volkswagencarnet/actions/workflows/codeql-analysis.yml)
+[![codecov](https://codecov.io/gh/robinostlund/volkswagencarnet/branch/master/graph/badge.svg?token=NH1Q1GH4I3)](https://codecov.io/gh/robinostlund/volkswagencarnet)
+
+
+![Downloads a day](https://img.shields.io/pypi/dd/volkswagencarnet)
+![Downloads a week](https://img.shields.io/pypi/dw/volkswagencarnet)
+![Downloads a month](https://img.shields.io/pypi/dm/volkswagencarnet)
+
+## Help Wanted
+
+As i don't have a car with Volkswagen Connect anymore i would appreciate if it would be possible to get help to keep this repository maintained. So if you feel that you have some time over and is interested in helping out with this. Please feel to contact me! Thanks
+
+## Information
+
+Retrieve statistics about your Volkswagen from the Volkswagen Carnet online service
+
+No licence, public domain, no guarantees, feel free to use for anything. Please contribute improvements/bugfixes etc.
+
+## Thanks to
+
+- [Wez3](https://github.com/wez3)
+- [Reneboer](https://github.com/reneboer)
+- [Tubalainen](https://github.com/tubalainen)
+- [JohNan](https://github.com/JohNan)
+- [milkboy](https://github.com/milkboy)
+
+For supporting and helping in this project.
+
+## Other related repositories
+
+- [HomeAssistant Component](https://github.com/robinostlund/homeassistant-volkswagencarnet) a custom component for Home Assistant
+
+## Installation
+
+```sh
+[venv-python3] user@localhost:~
+$ pip install volkswagencarnet
+```
+
+### Example
+
+```python
+#!/usr/bin/env python3
+from volkswagencarnet.vw_connection import Connection
+import pprint
+import asyncio
+import logging
+
+from aiohttp import ClientSession
+
+logging.basicConfig(level=logging.DEBUG)
+
+VW_USERNAME='test@example.com'
+VW_PASSWORD='mysecretpassword'
+
+
+COMPONENTS = {
+    'sensor': 'sensor',
+    'binary_sensor': 'binary_sensor',
+    'lock': 'lock',
+    'device_tracker': 'device_tracker',
+    'switch': 'switch',
+    'climate': 'climate'
+}
+
+RESOURCES = [
+    'position',
+    'distance',
+    'electric_climatisation',
+    'combustion_climatisation',
+    'window_heater',
+    'combustion_engine_heating',
+    'charging',
+    'adblue_level',
+    'battery_level',
+    'fuel_level',
+    'service_inspection',
+    'oil_inspection',
+    'last_connected',
+    'charging_time_left',
+    'electric_range',
+    'combustion_range',
+    'combined_range',
+    'charge_max_ampere',
+    'climatisation_target_temperature',
+    'external_power',
+    'parking_light',
+    'climatisation_without_external_power',
+    'door_locked',
+    'trunk_locked',
+    'request_in_progress',
+    'windows_closed',
+    'sunroof_closed',
+    'trip_last_average_speed',
+    'trip_last_average_electric_consumption',
+    'trip_last_average_fuel_consumption',
+    'trip_last_duration',
+    'trip_last_length'
+]
+
+def is_enabled(attr):
+    """Return true if the user has enabled the resource."""
+    return attr in RESOURCES
+
+async def main():
+    """Main method."""
+    async with ClientSession(headers={'Connection': 'keep-alive'}) as session:
+        connection = Connection(session, VW_USERNAME, VW_PASSWORD)
+        if await connection.doLogin():
+            if await connection.update():
+                # Print overall state
+                pprint.pprint(connection._state)
+
+                # Print vehicles
+                for vehicle in connection.vehicles:
+                    pprint.pprint(vehicle)
+
+                # get all instruments
+                instruments = set()
+                for vehicle in connection.vehicles:
+                    dashboard = vehicle.dashboard(mutable=True)
+
+                    for instrument in (
+                            instrument
+                            for instrument in dashboard.instruments
+                            if instrument.component in COMPONENTS
+                            and is_enabled(instrument.slug_attr)):
+
+                        instruments.add(instrument)
+
+                # Output all supported instruments
+                for instrument in instruments:
+                    print(f'name: {instrument.full_name}')
+                    print(f'str_state: {instrument.str_state}')
+                    print(f'state: {instrument.state}')
+                    print(f'supported: {instrument.is_supported}')
+                    print(f'attr: {instrument.attr}')
+                    print(f'attributes: {instrument.attributes}')
+
+if __name__ == "__main__":
+    loop = asyncio.get_event_loop()
+    # loop.run(main())
+    loop.run_until_complete(main())
+```
+
+## Development
+I'd strongly advise installing the git pre-commit hook using `pre-commit install`. See [pre-commit.com](https://pre-commit.com/) for details.
+Some basic checks are performed before you commit the code, so code style issues
+will be visible and fixable before creating the PR. Git pre-commit hooks can
+always be skipped using the `--no-verify` flag to `git commit`, if there
+is something preventing you from actually fixing the reported (and non-auto-fixed) issues.
+
+Decent test coverage for any new or changed code is also much appreciated :)
```


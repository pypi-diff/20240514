# Comparing `tmp/pyfolio_reloaded-0.9.7.tar.gz` & `tmp/pyfolio_reloaded-0.9.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfolio_reloaded-0.9.7.tar", last modified: Tue May 14 19:21:38 2024, max compression
+gzip compressed data, was "pyfolio_reloaded-0.9.7.dev2.tar", last modified: Mon May 13 15:45:20 2024, max compression
```

## Comparing `pyfolio_reloaded-0.9.7.tar` & `pyfolio_reloaded-0.9.7.dev2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.492608 pyfolio_reloaded-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.464608 pyfolio_reloaded-0.9.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.464608 pyfolio_reloaded-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/workflows/conda_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/workflows/test_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.github/workflows/unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19255 2024-05-14 19:21:38.492608 pyfolio_reloaded-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/WHATSNEW.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/build_and_deploy_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.460608 pyfolio_reloaded-0.9.7/conda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.464608 pyfolio_reloaded-0.9.7/conda/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/conda/recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.464608 pyfolio_reloaded-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.464608 pyfolio_reloaded-0.9.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/source/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:21:38.492608 pyfolio_reloaded-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.460608 pyfolio_reloaded-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.468608 pyfolio_reloaded-0.9.7/src/pyfolio/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/deprecate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.476608 pyfolio_reloaded-0.9.7/src/pyfolio/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  2409115 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/results.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1053570 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/sector_mappings_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   603437 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/single_stock_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  2066435 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/slippage_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3787905 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/examples/zipline_algo_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/interesting_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/ipycompat.py
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/perf_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)    62330 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/round_trips.py
--rw-r--r--   0 runner    (1001) docker     (127)    44741 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/tears.py
--rw-r--r--   0 runner    (1001) docker     (127)    36354 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/txn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/src/pyfolio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.488608 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19255 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 19:21:38.000000 pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.484608 pyfolio_reloaded-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_capacity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:38.488608 pyfolio_reloaded-0.9.7/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)    25231 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/factor_loadings.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/factor_returns.csv
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/intercepts.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/positions.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/residuals.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/returns.csv
--rw-r--r--   0 runner    (1001) docker     (127)   171201 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_LMCAP.csv
--rw-r--r--   0 runner    (1001) docker     (127)   176341 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_LT_MOMENTUM.csv
--rw-r--r--   0 runner    (1001) docker     (127)   176325 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_MACDSignal.csv
--rw-r--r--   0 runner    (1001) docker     (127)   176472 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_VLTY.csv
--rw-r--r--   0 runner    (1001) docker     (127)   163470 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_caps.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14737 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_gross_lev.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72979 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_pos.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    16393 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_returns.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    79854 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_sectors.csv
--rw-r--r--   0 runner    (1001) docker     (127)   168354 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_shares_held.csv
--rw-r--r--   0 runner    (1001) docker     (127)   139637 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_txn.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   162991 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_data/test_volumes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_perf_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_round_trips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_tears.py
--rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-14 19:21:33.000000 pyfolio_reloaded-0.9.7/tests/test_txn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/conda_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/test_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/WHATSNEW.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/build_and_deploy_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/conda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/conda/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/conda/recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/deprecate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.547405 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  2409115 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/results.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1053570 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/sector_mappings_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   603437 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/single_stock_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2066435 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/slippage_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3787905 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/zipline_algo_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/interesting_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/ipycompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62305 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44741 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/tears.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36354 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/txn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.559404 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.555405 pyfolio_reloaded-0.9.7.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_capacity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.559404 pyfolio_reloaded-0.9.7.dev2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    25231 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_loadings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_returns.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/intercepts.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/positions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/residuals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/returns.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   171201 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LMCAP.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176341 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LT_MOMENTUM.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176325 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_MACDSignal.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176472 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_VLTY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   163470 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_caps.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14737 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_gross_lev.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72979 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_pos.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16393 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_returns.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    79854 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_sectors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   168354 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_shares_held.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   139637 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_txn.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   162991 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_volumes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_tears.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_txn.py
```

### Comparing `pyfolio_reloaded-0.9.7/.github/dependabot.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/.github/workflows/build_wheels.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/build_wheels.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 name: PyPI
 
 on:
   workflow_dispatch:
     inputs:
-      target:
-        type: choice
-        description: 'Package Index'
+      publish_to_pypi:
+        description: 'Publish to PyPI?'
         required: true
-        default: 'PYPI'
-        options: [ 'TESTPYPI', 'PYPI' ]
+        type: string
+        default: 'false'
 
 jobs:
   dist:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
@@ -20,15 +19,14 @@
         python-version: [ "3.10" ]
 
     steps:
       - name: Checkout pyfolio
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
-          ref: 0.9.7
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Build wheels
@@ -48,20 +46,20 @@
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
       - name: publish to testpypi
-        if: ${{ github.event.inputs.target  == 'TESTPYPI' }}
         uses: pypa/gh-action-pypi-publish@release/v1
+        if: ${{ inputs.publish_to_pypi == 'false' }}
         with:
           user: __token__
           password: ${{ secrets.TESTPYPI_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
 
       - name: publish to pypi
-        if: ${{ github.event.inputs.target  == 'PYPI' }}
         uses: pypa/gh-action-pypi-publish@release/v1
+        if: ${{ inputs.publish_to_pypi == 'true' }}
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pyfolio_reloaded-0.9.7/.github/workflows/conda_package.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/conda_package.yml`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/.github/workflows/test_wheels.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/test_wheels.yml`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/.github/workflows/unit_tests.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/unit_tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
       - main
   pull_request:
     branches:
       - main
 
 jobs:
   build:
-    name: Unit Tests for ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest , windows-latest, macos-latest ]
         python-version: [ '3.9', '3.10', '3.11', '3.12']
     steps:
```

### Comparing `pyfolio_reloaded-0.9.7/.gitignore` & `pyfolio_reloaded-0.9.7.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/LICENSE` & `pyfolio_reloaded-0.9.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/PKG-INFO` & `pyfolio_reloaded-0.9.7.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfolio-reloaded
-Version: 0.9.7
+Version: 0.9.7.dev2
 Summary: Performance and risk analysis of financial portfolios with Python
 Author: Quantopian Inc
 Author-email: pm@ml4trading.io
 Maintainer: Stefan Jansen
 Maintainer-email: pm@ml4trading.io
 License:                                  Apache License
                                    Version 2.0, January 2004
```

### Comparing `pyfolio_reloaded-0.9.7/README.md` & `pyfolio_reloaded-0.9.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/WHATSNEW.md` & `pyfolio_reloaded-0.9.7.dev2/WHATSNEW.md`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/conda/recipe/meta.yaml` & `pyfolio_reloaded-0.9.7.dev2/conda/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/docs/Makefile` & `pyfolio_reloaded-0.9.7.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/docs/deploy.py` & `pyfolio_reloaded-0.9.7.dev2/docs/deploy.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/docs/make.bat` & `pyfolio_reloaded-0.9.7.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/docs/source/api-reference.rst` & `pyfolio_reloaded-0.9.7.dev2/docs/source/api-reference.rst`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/docs/source/conf.py` & `pyfolio_reloaded-0.9.7.dev2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/pyproject.toml` & `pyfolio_reloaded-0.9.7.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
   docs/source/conf.py
 \)
 '''
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{39,310}-pandas{13,14,15}, py{39,310, 311,312}-pandas{20,21,22}
+envlist = py39-pandas{11,12},py{39,310}-pandas{13,14,15}, py{39,310, 311,312}-pandas{20,21,22}
 isolated_build = True
 skip_missing_interpreters = True
 minversion = 3.23.0
 
 [gh-actions]
 python =
     3.9: py39
@@ -150,14 +150,16 @@
 usedevelop = True
 setenv =
     MPLBACKEND = Agg
 
 changedir = tmp
 extras = test
 deps =
+    pandas11: pandas>=1.1.0,<1.2
+    pandas12: pandas>=1.2.0,<1.3
     pandas13: pandas>=1.3.0,<1.4
     pandas14: pandas>=1.4.0,<1.5
     pandas15: pandas>=1.5.0,<1.6
     pandas20: pandas>=2.0,<2.1
     pandas21: pandas>=2.1,<2.2
     pandas22: pandas>=2.2,<2.3
```

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/__init__.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/capacity.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/capacity.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/deprecate.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/results.pickle` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/results.pickle`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/sector_mappings_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/sector_mappings_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/single_stock_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/single_stock_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/slippage_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/slippage_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/examples/zipline_algo_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/zipline_algo_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/interesting_periods.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/interesting_periods.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/ipycompat.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/ipycompat.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/perf_attrib.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/perf_attrib.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/plotting.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -807,15 +807,15 @@
 
     cum_rets = ep.cum_returns(returns, 1.0)
 
     y_axis_formatter = FuncFormatter(utils.two_dec_places)
     ax.yaxis.set_major_formatter(FuncFormatter(y_axis_formatter))
 
     if factor_returns is not None:
-        cum_factor_returns = ep.cum_returns(factor_returns.loc[cum_rets.index], 1.0)
+        cum_factor_returns = ep.cum_returns(factor_returns[cum_rets.index], 1.0)
         cum_factor_returns.plot(
             lw=2,
             color="gray",
             label=factor_returns.name,
             alpha=0.60,
             ax=ax,
             **kwargs,
@@ -1373,15 +1373,15 @@
         returns
         if live_start_date is None
         else returns.loc[returns.index < live_start_date]
     )
     is_weekly = ep.aggregate_returns(is_returns, "weekly")
     is_monthly = ep.aggregate_returns(is_returns, "monthly")
     sns.boxplot(
-        data=[is_returns.values, is_weekly.values, is_monthly.values],
+        data=[is_returns, is_weekly, is_monthly],
         palette=["#4c72B0", "#55A868", "#CCB974"],
         ax=ax,
         **kwargs,
     )
 
     if live_start_date is not None:
         oos_returns = returns.loc[returns.index >= live_start_date]
```

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/pos.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/pos.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/round_trips.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/round_trips.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/tears.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/tears.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/timeseries.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/txn.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/txn.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio/utils.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/utils.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/PKG-INFO` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfolio-reloaded
-Version: 0.9.7
+Version: 0.9.7.dev2
 Summary: Performance and risk analysis of financial portfolios with Python
 Author: Quantopian Inc
 Author-email: pm@ml4trading.io
 Maintainer: Stefan Jansen
 Maintainer-email: pm@ml4trading.io
 License:                                  Apache License
                                    Version 2.0, January 2004
```

### Comparing `pyfolio_reloaded-0.9.7/src/pyfolio_reloaded.egg-info/SOURCES.txt` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_capacity.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_capacity.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/factor_loadings.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_loadings.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/factor_returns.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_returns.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/positions.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/positions.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/residuals.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/residuals.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/returns.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/returns.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_LMCAP.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LMCAP.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_LT_MOMENTUM.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LT_MOMENTUM.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_MACDSignal.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_MACDSignal.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_VLTY.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_VLTY.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_caps.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_caps.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_gross_lev.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_gross_lev.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_pos.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_pos.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_returns.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_returns.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_sectors.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_sectors.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_shares_held.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_shares_held.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_txn.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_txn.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_data/test_volumes.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_volumes.csv`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_perf_attrib.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_perf_attrib.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_pos.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_pos.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_round_trips.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_round_trips.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_tears.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_tears.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             parse_dates=True,
         )
     )
 
     @parameterized.expand(
         [
             ({},),
-            ({"slippage": 1},),
+            # ({"slippage": 1},),
             ({"live_start_date": test_returns.index[-20]},),
             ({"round_trips": True},),
             ({"hide_positions": True},),
             ({"cone_std": 1},),
             ({"bootstrap": True},),
         ]
     )
```

### Comparing `pyfolio_reloaded-0.9.7/tests/test_timeseries.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyfolio_reloaded-0.9.7/tests/test_txn.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_txn.py`

 * *Files identical despite different names*


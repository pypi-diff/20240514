# Comparing `tmp/dodata-0.4.9.tar.gz` & `tmp/dodata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodata-0.4.9.tar", last modified: Thu Apr 11 17:27:19 2024, max compression
+gzip compressed data, was "dodata-0.5.0.tar", last modified: Mon Apr 29 13:52:17 2024, max compression
```

## Comparing `dodata-0.4.9.tar` & `dodata-0.5.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.968827 dodata-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.940827 dodata-0.4.9/.changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 17:27:09.000000 dodata-0.4.9/.changelog.d/changelog_template.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-11 17:27:09.000000 dodata-0.4.9/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.940827 dodata-0.4.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.940827 dodata-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/workflows/require-labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-11 17:27:09.000000 dodata-0.4.9/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-11 17:27:09.000000 dodata-0.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-11 17:27:09.000000 dodata-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-11 17:27:09.000000 dodata-0.4.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 17:27:09.000000 dodata-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 17:27:09.000000 dodata-0.4.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-11 17:27:19.968827 dodata-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-11 17:27:09.000000 dodata-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.944826 dodata-0.4.9/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1810 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/component_cutback.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.944826 dodata-0.4.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   360904 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/images/device_die_wafer.png
--rw-r--r--   0 runner    (1001) docker     (127)    34153 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/images/schema.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12822 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/images/wafer22.png
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    75026 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/resistance.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/rings.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 17:27:09.000000 dodata-0.4.9/docs/spirals.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.968827 dodata-0.4.9/dodata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-11 17:27:19.000000 dodata-0.4.9/dodata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-11 17:27:19.000000 dodata-0.4.9/dodata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:27:19.000000 dodata-0.4.9/dodata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 17:27:19.000000 dodata-0.4.9/dodata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 17:27:19.000000 dodata-0.4.9/dodata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.936827 dodata-0.4.9/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.936827 dodata-0.4.9/notebooks/dodata_tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.948827 dodata-0.4.9/notebooks/dodata_tutorials/cutback/
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/1_generate_layout.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/2_generate_measurement_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/3_upload_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/4_download_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/5_delete.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/generate_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/cutback/generic.lyp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.952827 dodata-0.4.9/notebooks/dodata_tutorials/resistance/
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/1_generate_layout.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/2_generate_measurement_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20591 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/3_upload_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/4_download_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/5_delete.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/generate_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/resistance/test_chip.lyp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.952827 dodata-0.4.9/notebooks/dodata_tutorials/rings/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/1_generate_layout.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/2_generate_measurement_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28560 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/3_upload_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12822 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/4_download_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/5_delete.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/generate_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/rings/generic.lyp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.956827 dodata-0.4.9/notebooks/dodata_tutorials/spirals/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/1_generate_layout.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/2_generate_measurement_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24733 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/3_upload_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/4_download_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/5_delete.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/loss_measurements.lyp
--rw-r--r--   0 runner    (1001) docker     (127)    24171 2024-04-11 17:27:09.000000 dodata-0.4.9/notebooks/dodata_tutorials/spirals/test_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-11 17:27:09.000000 dodata-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:27:19.968827 dodata-0.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.936827 dodata-0.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.936827 dodata-0.4.9/src/doplaydo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.956827 dodata-0.4.9/src/doplaydo/dodata/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.956827 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.956827 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/fsr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/iv_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/power_envelope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.960827 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/cutback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/iv_sheet_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/loss_cutback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.960827 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/aggregate_loss_cutback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.964827 dodata-0.4.9/src/doplaydo/dodata/api/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/analysis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/api_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/device_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/die.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/api/wafer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.964827 dodata-0.4.9/src/doplaydo/dodata/db/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/device_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/die.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/db/wafer.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:09.000000 dodata-0.4.9/src/doplaydo/dodata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:27:19.968827 dodata-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_analysis_device_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_analysis_die.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_analysis_die_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_analysis_plot_device_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_analysis_wafer.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_devicedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-11 17:27:09.000000 dodata-0.4.9/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.091863 dodata-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.071863 dodata-0.5.0/.changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-29 13:52:02.000000 dodata-0.5.0/.changelog.d/changelog_template.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-29 13:52:02.000000 dodata-0.5.0/.coverage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.071863 dodata-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.071863 dodata-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/workflows/require-labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-29 13:52:02.000000 dodata-0.5.0/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-29 13:52:02.000000 dodata-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 13:52:02.000000 dodata-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-29 13:52:02.000000 dodata-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 13:52:02.000000 dodata-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 13:52:02.000000 dodata-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 13:52:17.091863 dodata-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-29 13:52:02.000000 dodata-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.071863 dodata-0.5.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1810 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/component_cutback.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.075863 dodata-0.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   360904 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/images/device_die_wafer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34153 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/images/schema.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12822 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/images/wafer22.png
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    75026 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/resistance.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/rings.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 13:52:02.000000 dodata-0.5.0/docs/spirals.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.087863 dodata-0.5.0/dodata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 13:52:17.000000 dodata-0.5.0/dodata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 13:52:17.000000 dodata-0.5.0/dodata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:52:17.000000 dodata-0.5.0/dodata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 13:52:17.000000 dodata-0.5.0/dodata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 13:52:17.000000 dodata-0.5.0/dodata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.067863 dodata-0.5.0/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.067863 dodata-0.5.0/notebooks/dodata_tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.075863 dodata-0.5.0/notebooks/dodata_tutorials/cutback/
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/1_generate_layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/2_generate_measurement_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/3_upload_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/4_download_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/5_delete.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/generate_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/cutback/generic.lyp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.079863 dodata-0.5.0/notebooks/dodata_tutorials/resistance/
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/1_generate_layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/2_generate_measurement_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30860 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/3_upload_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/4_download_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/5_delete.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/generate_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/resistance/test_chip.lyp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.079863 dodata-0.5.0/notebooks/dodata_tutorials/rings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/1_generate_layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/2_generate_measurement_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28583 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/3_upload_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12822 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/4_download_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/5_delete.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/generate_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41092 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/rings/generic.lyp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.079863 dodata-0.5.0/notebooks/dodata_tutorials/spirals/
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/1_generate_layout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/2_generate_measurement_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24733 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/3_upload_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/4_download_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/5_delete.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/loss_measurements.lyp
+-rw-r--r--   0 runner    (1001) docker     (127)    24171 2024-04-29 13:52:02.000000 dodata-0.5.0/notebooks/dodata_tutorials/spirals/test_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-29 13:52:02.000000 dodata-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:52:17.091863 dodata-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.067863 dodata-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.067863 dodata-0.5.0/src/doplaydo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.079863 dodata-0.5.0/src/doplaydo/dodata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.079863 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.083863 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/fsr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/iv_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/power_envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.083863 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/cutback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/iv_sheet_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/loss_cutback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.083863 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/aggregate_loss_cutback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.083863 dodata-0.5.0/src/doplaydo/dodata/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/analysis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/device_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/die.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/api/wafer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.083863 dodata-0.5.0/src/doplaydo/dodata/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/device_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/die.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/db/wafer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:02.000000 dodata-0.5.0/src/doplaydo/dodata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:52:17.087863 dodata-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_analysis_device_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_analysis_die.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_analysis_die_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_analysis_plot_device_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_analysis_wafer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_devicedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 13:52:02.000000 dodata-0.5.0/tests/test_upload.py
```

### Comparing `dodata-0.4.9/.coverage` & `dodata-0.5.0/.coverage`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.github/release-drafter.yml` & `dodata-0.5.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.github/workflows/pages.yml` & `dodata-0.5.0/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.github/workflows/release-drafter.yml` & `dodata-0.5.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.github/workflows/release.yml` & `dodata-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.github/workflows/test_code.yml` & `dodata-0.5.0/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/.pre-commit-config.yaml` & `dodata-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/CHANGELOG.md` & `dodata-0.5.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # Changelog
 
 <!-- towncrier release notes start -->
 
-## [0.4.9](https://github.com/doplaydo/DoData_SDK/releases/v0.4.9) - 2024-04-11
+## [0.5.0](https://github.com/doplaydo/DoData_SDK/releases/v0.5.0) - 2024-04-29
 
 No significant changes.
 
 
-## [0.4.8](https://github.com/doplaydo/DoData_SDK/releases/v0.4.8) - 2024-03-12
-
-No significant changes.
-
-
-## [0.4.7](https://github.com/doplaydo/DoData_SDK/releases/v0.4.7) - 2024-03-12
-
-No significant changes.
-
-
-## [0.4.6](https://github.com/doplaydo/DoData_SDK/releases/v0.4.6) - 2024-03-06
-
-No significant changes.
+## 0.4.10
 
+- improve docs
+    - less points in resistance generation
+    - add wafer compare examples. Add plotly to dependencies.
+    - add device variation factor on sheet resistance and spirals demos
+- improve wafer_plot
+    * add filter by percentile to wafer plots
+    * support scientific notation with arbitrary number of decimals, and different die label font sizes
 
 ## 0.4.5
 
 - update to gdsfactory 7.17.0
 
 ## 0.4.4
```

### Comparing `dodata-0.4.9/LICENSE` & `dodata-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/PKG-INFO` & `dodata-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodata
-Version: 0.4.9
+Version: 0.5.0
 Summary: Software Development Kit - SDK for DoData
 Author-email: DoPlayDo <contact@doplaydo.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 DoPlayDo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,15 @@
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: sqlmodel>=0.0.14
 Requires-Dist: tqdm
 Provides-Extra: demos
 Requires-Dist: gdsfactory==7.17.0; extra == "demos"
 Requires-Dist: jupyterlab; extra == "demos"
+Requires-Dist: plotly; extra == "demos"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: towncrier; extra == "dev"
 Requires-Dist: tbump; extra == "dev"
@@ -64,15 +65,15 @@
 Requires-Dist: types-setuptools; extra == "maintainer"
 Requires-Dist: types-docutils; extra == "maintainer"
 Requires-Dist: types-Pygments; extra == "maintainer"
 Requires-Dist: pylsp-mypy; extra == "maintainer"
 Requires-Dist: python-lsp-server[all]; extra == "maintainer"
 Requires-Dist: python-lsp-ruff; extra == "maintainer"
 
-# DoData python library 0.4.9
+# DoData python library 0.5.0
 
 DoData offers a state-of-the-art data storage solution tailored specifically for chip design. Designed to seamlessly integrate into your workflow, the platform provides a scalable solution for storing, managing, and analyzing your chip data files.
 
 ![](https://i.imgur.com/ZwIWS08.png)
 
 ## Installation
```

### Comparing `dodata-0.4.9/README.md` & `dodata-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# DoData python library 0.4.9
+# DoData python library 0.5.0
 
 DoData offers a state-of-the-art data storage solution tailored specifically for chip design. Designed to seamlessly integrate into your workflow, the platform provides a scalable solution for storing, managing, and analyzing your chip data files.
 
 ![](https://i.imgur.com/ZwIWS08.png)
 
 ## Installation
```

### Comparing `dodata-0.4.9/docs/_config.yml` & `dodata-0.5.0/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/docs/_toc.yml` & `dodata-0.5.0/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/docs/images/device_die_wafer.png` & `dodata-0.5.0/docs/images/device_die_wafer.png`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/docs/images/schema.svg` & `dodata-0.5.0/docs/images/schema.svg`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/docs/images/wafer22.png` & `dodata-0.5.0/docs/images/wafer22.png`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/docs/logo.png` & `dodata-0.5.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/dodata.egg-info/PKG-INFO` & `dodata-0.5.0/dodata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodata
-Version: 0.4.9
+Version: 0.5.0
 Summary: Software Development Kit - SDK for DoData
 Author-email: DoPlayDo <contact@doplaydo.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 DoPlayDo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,15 @@
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: sqlmodel>=0.0.14
 Requires-Dist: tqdm
 Provides-Extra: demos
 Requires-Dist: gdsfactory==7.17.0; extra == "demos"
 Requires-Dist: jupyterlab; extra == "demos"
+Requires-Dist: plotly; extra == "demos"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: towncrier; extra == "dev"
 Requires-Dist: tbump; extra == "dev"
@@ -64,15 +65,15 @@
 Requires-Dist: types-setuptools; extra == "maintainer"
 Requires-Dist: types-docutils; extra == "maintainer"
 Requires-Dist: types-Pygments; extra == "maintainer"
 Requires-Dist: pylsp-mypy; extra == "maintainer"
 Requires-Dist: python-lsp-server[all]; extra == "maintainer"
 Requires-Dist: python-lsp-ruff; extra == "maintainer"
 
-# DoData python library 0.4.9
+# DoData python library 0.5.0
 
 DoData offers a state-of-the-art data storage solution tailored specifically for chip design. Designed to seamlessly integrate into your workflow, the platform provides a scalable solution for storing, managing, and analyzing your chip data files.
 
 ![](https://i.imgur.com/ZwIWS08.png)
 
 ## Installation
```

### Comparing `dodata-0.4.9/dodata.egg-info/SOURCES.txt` & `dodata-0.5.0/dodata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/1_generate_layout.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/1_generate_layout.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/2_generate_measurement_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/2_generate_measurement_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/3_upload_measurements.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/3_upload_measurements.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/4_download_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/4_download_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/5_delete.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/5_delete.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/generate_layout.py` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/generate_layout.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/cutback/generic.lyp` & `dodata-0.5.0/notebooks/dodata_tutorials/cutback/generic.lyp`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/1_generate_layout.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/1_generate_layout.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/2_generate_measurement_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/2_generate_measurement_data.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903534658185337%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, '        resistance: in Ohms.\\n'), (11, 'i = "*

 * *            "np.linspace(0, 100, 21)\\n')], delete: [12, 6, 4]}}, 6: {'source': {insert: [(1, "*

 * *            '\'wafers = ["2eq221eqewq2", "334abd342zuq", "6d4c615ff105"]\\n\')], delete: [1]}}, 8: '*

 * *            '{\'source\': {insert: [(0, \'wafers_path = Path("wafers")\\n\'), (8, \'    '*

 * *            "wafer_per_cent_variation = 0.20  # 20% variation\\n'), (9, '    "*

 * *            'wafer_variation_factor = 1 + wafer_per_cent […]*

```diff
@@ -44,23 +44,22 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def iv_resistance(resistance, current) -> np.ndarray:\n",
                 "    \"\"\"Returns IV.\n",
                 "\n",
                 "    Args:\n",
-                "        resistance: in Ohms\n",
+                "        resistance: in Ohms.\n",
                 "        current: electrical intensity in A.\n",
-                "\n",
                 "    \"\"\"\n",
                 "    v = resistance * current\n",
                 "    return v\n",
                 "\n",
                 "\n",
-                "i = np.linspace(0, 100, 79)\n",
+                "i = np.linspace(0, 100, 21)\n",
                 "v = iv_resistance(resistance=30, current=i)\n",
                 "\n",
                 "plt.figure(figsize=(10, 6))\n",
                 "plt.plot(i, v)\n",
                 "plt.title(\"Resistance\")\n",
                 "plt.xlabel(\"Current (A)\")\n",
                 "plt.ylabel(\"V\")\n",
@@ -103,15 +102,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "c7b873fc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "wafer_definitions = Path(\"wafer_definitions.json\")\n",
-                "wafers = [\"6d4c615ff105\"]\n",
+                "wafers = [\"2eq221eqewq2\", \"334abd342zuq\", \"6d4c615ff105\"]\n",
                 "dies = [\n",
                 "    {\"x\": x, \"y\": y}\n",
                 "    for y in range(-2, 3)\n",
                 "    for x in range(-2, 3)\n",
                 "    if not (abs(y) == 2 and abs(x) == 2)\n",
                 "]\n",
                 "\n",
@@ -135,36 +134,51 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f3cf4dcc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cwd = Path(\".\")\n",
+                "wafers_path = Path(\"wafers\")\n",
                 "\n",
                 "metadata = {\"measurement_type\": \"Spectral MEAS\", \"temperature\": 25}\n",
                 "\n",
                 "length = 20\n",
                 "ohms_per_square = 100\n",
                 "\n",
-                "\n",
                 "for wafer in wafers:\n",
+                "    wafer_per_cent_variation = 0.20  # 20% variation\n",
+                "    wafer_variation_factor = 1 + wafer_per_cent_variation * (2 * np.random.rand() - 1)\n",
+                "\n",
                 "    for die in dies:\n",
                 "        die = f\"{(die['x'])}_{(die['y'])}\"\n",
                 "        for (_, row), (_, device_row) in zip(df.iterrows(), df.iterrows()):\n",
                 "            cell_id = row[\"cell\"]\n",
-                "            resistance = ohms_per_square * row[\"width_um\"] * length * 1e-12\n",
-                "            top_cell_id = \"resistance\"\n",
-                "            device_id = (\n",
-                "                f\"{top_cell_id}_{cell_id}_{device_row['x']}_{device_row['y']}\"\n",
+                "            basic_resistance = ohms_per_square * row[\"width_um\"] * length * 1e-12\n",
+                "            device_per_cent_variation = 0.05  # 5% variation\n",
+                "            device_variation_factor = 1 + device_per_cent_variation * (\n",
+                "                2 * np.random.rand() - 1\n",
                 "            )\n",
+                "            resistance = (\n",
+                "                basic_resistance * wafer_variation_factor * device_variation_factor\n",
+                "            )\n",
+                "\n",
+                "            # Special resistance cases (open and short circuits)\n",
+                "            rand_num = np.random.rand()\n",
+                "            if rand_num < 0.05:\n",
+                "                resistance = 3000  # 5% with infinite resistance (open circuit)\n",
+                "            elif rand_num < 0.08:  # Additional 3% (total 8% chance)\n",
+                "                resistance = 0  # 3% with zero resistance (short circuit)\n",
+                "\n",
+                "            top_cell_id = \"resistance\"\n",
+                "            device_id = f\"{top_cell_id}_{cell_id}_{device_row['x']}_{device_row['y']}\"\n",
                 "            v = iv_resistance(resistance=resistance, current=i)\n",
                 "            noise = 5e-2 * np.random.rand(len(v)) * v  # add 5% noise\n",
                 "            v += noise\n",
-                "            dirpath = cwd / wafer / die / device_id\n",
+                "            dirpath = wafers_path / wafer / die / device_id\n",
                 "            dirpath.mkdir(exist_ok=True, parents=True)\n",
                 "            data_file = dirpath / \"data.json\"\n",
                 "            metadata_file = dirpath / \"attributes.json\"\n",
                 "            metadata_file.write_text(json.dumps(metadata))\n",
                 "\n",
                 "            d = {\n",
                 "                \"v\": v,\n",
@@ -246,20 +260,26 @@
                 "p = np.polyfit(i2, v2, deg=1)\n",
                 "print(f\"Sheet resistance {p[0]:.2f}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b016b639",
+            "id": "f2d9d682",
             "metadata": {},
             "outputs": [],
-            "source": [
-                "p"
-            ]
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5d08c214",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/3_upload_measurements.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/3_upload_measurements.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672596067617254%*

 * *Differences: {"'cells'": "{0: {'id': '68e7c0eb', 'source': {insert: [(0, '# Upload Measurement Data and run "*

 * *            "Analysis\\n')], delete: [0]}}, 1: {'id': '30a16d0e', 'source': {insert: [(5, 'import "*

 * *            "getpass')], delete: [7, 6, 5]}}, 2: {'id': '39025f78'}, 3: {'id': '8d70639d', "*

 * *            "'source': ['username = getpass.getuser()\\n', 'PROJECT_ID = "*

 * *            'f"spirals-{username}"\\n\', \'MEASUREMENTS_PATH = Path("6d4c615ff105/")\\n\', '*

 * *            "'PROJECT_ID']}, 4: {'id': '337aa355'}, 5: […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "324eaab3",
+            "id": "68e7c0eb",
             "metadata": {},
             "source": [
-                "# Upload measurements and run analysis\n",
+                "# Upload Measurement Data and run Analysis\n",
                 "\n",
                 "Now you will post your measurement data and analysis to the database via the API.\n",
                 "\n",
                 "**If you are running the tutorials in DoLab, the following instructions are not necessary and you can skip directly to the next cell.**\n",
                 "\n",
                 "You will need to authenticate to the database with your username and password. To make this easy,  you can create a file called `.env` in this folder and complete it with your organization's URL and authentication information as follows:\n",
                 "\n",
@@ -25,80 +25,80 @@
                 "\n",
                 "If you haven't defined a `.env` file or saved your credentials to your environment variables, you will be prompted for your credentials now."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "131ce11e",
+            "id": "30a16d0e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import doplaydo.dodata as dd\n",
                 "import pandas as pd\n",
                 "from pathlib import Path\n",
                 "from tqdm.auto import tqdm\n",
                 "import requests\n",
-                "import getpass\n",
-                "\n",
-                "username = getpass.getuser()"
+                "import getpass"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e14eba7a",
+            "id": "39025f78",
             "metadata": {},
             "source": [
                 "Let's now create a project. \n",
                 "\n",
                 "In normal circumstances, everyone will be sharing and contributing to a project. In this demo, however, we want to *keep your project separate* from other users for clarity, so we will append your username to the project name. This way you can also safely delete and recreate projects without creating issues for others. If you prefer though, you can change the `PROJECT_ID` to anything you like. Just be sure to update it in the subsequent notebooks of this tutorial as well."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6144eb85",
+            "id": "8d70639d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "PROJECT_ID = f\"resistance-{username}\"\n",
-                "MEASUREMENTS_PATH = Path(\"6d4c615ff105/\")"
+                "username = getpass.getuser()\n",
+                "PROJECT_ID = f\"spirals-{username}\"\n",
+                "MEASUREMENTS_PATH = Path(\"6d4c615ff105/\")\n",
+                "PROJECT_ID"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e4e8e119",
+            "id": "337aa355",
             "metadata": {},
             "source": [
                 "Lets delete the project if it already exists so that you can start fresh."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "96eaf9b3",
+            "id": "c8d226b3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.delete(PROJECT_ID).text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bcee9154",
+            "id": "814a129c",
             "metadata": {},
             "source": [
                 "## New project\n",
                 "\n",
                 "You can create the project, upload the design manifest, and upload the wafer definitions through the Webapp as well as programmatically using this notebook"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "774500ef",
+            "id": "207cd8ec",
             "metadata": {},
             "source": [
                 "### Upload Project\n",
                 "\n",
                 "You can create a new project and extract all cells & devices below for the `RidgeLoss` and `RibLoss`\n",
                 "\n",
                 "The expressions are regex expressions. For intro and testing your regexes you can check out [regex101](https://regex101.com)\n",
@@ -109,163 +109,169 @@
                 "\n",
                 "Whitelists take precedence over blacklists, so if you define both, it uses only the whitelist."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "695b1865",
+            "id": "0746daec",
             "metadata": {},
             "outputs": [],
             "source": [
                 "cell_extraction = [\n",
                 "    dd.project.Extraction(\n",
-                "        cell_id=\"resistance\",\n",
-                "        cell_white_list=[\"^resistance\"],\n",
+                "        cell_id=\"RibLoss\",\n",
+                "        cell_white_list=[\"^cutback_rib\"],\n",
+                "        min_hierarchy_lvl=0,\n",
+                "        max_hierarchy_lvl=0,\n",
+                "    ),\n",
+                "    dd.project.Extraction(\n",
+                "        cell_id=\"RidgeLoss\",\n",
+                "        cell_white_list=[\"^cutback_ridge\"],\n",
                 "        min_hierarchy_lvl=0,\n",
                 "        max_hierarchy_lvl=0,\n",
                 "    ),\n",
                 "]\n",
                 "\n",
                 "dd.project.create(\n",
                 "    project_id=PROJECT_ID,\n",
                 "    eda_file=\"test_chip.gds\",\n",
-                "    lyp_file=\"test_chip.lyp\",\n",
+                "    lyp_file=\"loss_measurements.lyp\",\n",
                 "    cell_extractions=cell_extraction,\n",
                 ").text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "63d5a0cc",
+            "id": "724d33f5",
             "metadata": {},
             "source": [
                 "### Upload Design Manifest\n",
                 "\n",
                 "The design manifest is a CSV file that includes all the cell names, the cell settings, a list of analysis to trigger, and a list of settings for each analysis."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fffbb4b7",
+            "id": "5902d5ad",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm = pd.read_csv(\"design_manifest.csv\")\n",
                 "dm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "355452eb",
+            "id": "3b214d19",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm = dm.drop(columns=[\"analysis\", \"analysis_parameters\"])\n",
                 "dm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0e650acd",
+            "id": "31577dc7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm.to_csv(\"design_manifest_without_analysis.csv\", index=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c79178e4",
+            "id": "1aa5a8b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.upload_design_manifest(\n",
                 "    project_id=PROJECT_ID, filepath=\"design_manifest_without_analysis.csv\"\n",
                 ").text"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cb52f953",
+            "id": "db40bd55",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.download_design_manifest(\n",
                 "    project_id=PROJECT_ID, filepath=\"design_manifest_downloaded.csv\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "edd1d6cc",
+            "id": "d50a9b23",
             "metadata": {},
             "source": [
                 "### Upload Wafer Definitions\n",
                 "\n",
                 "The wafer definition is a JSON file where you can define the wafer names and die names and location for each wafer."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bfea5fcb",
+            "id": "8181b418",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.upload_wafer_definitions(\n",
                 "    project_id=PROJECT_ID, filepath=\"wafer_definitions.json\"\n",
                 ").text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "13f73719",
+            "id": "9c9c71d0",
             "metadata": {},
             "source": [
                 "## Upload data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cfda4e1b",
+            "id": "eddc6cdb",
             "metadata": {},
             "source": [
                 "Your Tester can output the data in JSON files. It does not need to be Python."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "26377b7f",
+            "id": "b0cc0012",
             "metadata": {},
             "source": [
                 "You can get all paths which have measurement data within the test path."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8348da4c",
+            "id": "91f386d5",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "outputs": [],
             "source": [
                 "data_files = list(MEASUREMENTS_PATH.glob(\"**/data.json\"))\n",
                 "print(data_files[0].parts)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "baf7d7d6",
+            "id": "bb7859dc",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "source": [
                 " You should define a plotting per measurement type in python. Your plots can evolve over time even for the same measurement type.\n",
                 "\n",
                 "Required:\n",
@@ -296,58 +302,56 @@
                 "\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7765dc0d",
+            "id": "38478f45",
             "metadata": {},
             "outputs": [],
             "source": [
-                "measurement_type = dd.api.device_data.PlottingKwargs(\n",
-                "    x_name=\"i\",\n",
-                "    y_name=\"v\",\n",
-                "    x_col=\"i\",\n",
-                "    y_col=[\"v\"],  # can also be a string for a single value\n",
-                "    # y_col=\"v\",\n",
+                "spectrum_measurement_type = dd.api.device_data.PlottingKwargs(\n",
+                "    x_name=\"wavelength\",\n",
+                "    y_name=\"output_power\",\n",
+                "    x_col=\"wavelength\",\n",
+                "    # y_col=[\"output_power\"],  # can also be a string for a single value\n",
+                "    y_col=\"output_power\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "47655f38",
+            "id": "3eee0823",
             "metadata": {},
             "source": [
                 "### Upload measurements\n",
                 "\n",
                 "You can now upload measurement data.\n",
                 "\n",
                 "This is a bare bones example, in a production setting, you can also add validation, logging, and error handling to ensure a smooth operation.\n",
                 "\n",
                 "Every measurement you upload will trigger all the analysis that you defined in the design manifest."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "28205616",
+            "id": "2f37ca4d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "wafer_set = set()\n",
-                "die_set = set()\n",
                 "NUMBER_OF_THREADS = 1 if \"127\" in dd.settings.dodata_url else dd.settings.n_threads\n",
                 "NUMBER_OF_THREADS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c4ff8f0f",
+            "id": "3370ba1a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "if NUMBER_OF_THREADS == 1:\n",
                 "    for path in tqdm(data_files):\n",
                 "        wafer_id = path.parts[0]\n",
                 "        die_x, die_y = path.parts[1].split(\"_\")\n",
@@ -355,26 +359,24 @@
                 "        r = dd.api.device_data.upload(\n",
                 "            file=path,\n",
                 "            project_id=PROJECT_ID,\n",
                 "            wafer_id=wafer_id,\n",
                 "            die_x=die_x,\n",
                 "            die_y=die_y,\n",
                 "            device_id=path.parts[2],\n",
-                "            data_type=\"measurement\",\n",
-                "            plotting_kwargs=measurement_type,\n",
+                "            data_type=\"measurement\",  # can also be \"simulation\"\n",
+                "            plotting_kwargs=spectrum_measurement_type,\n",
                 "        )\n",
-                "        wafer_set.add(wafer_id)\n",
-                "        die_set.add(path.parts[2])\n",
                 "        r.raise_for_status()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "940660d3",
+            "id": "d515538c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "data_files = list(MEASUREMENTS_PATH.glob(\"**/data.json\"))\n",
                 "project_ids = []\n",
                 "device_ids = []\n",
                 "die_ids = []\n",
@@ -391,23 +393,23 @@
                 "    wafer_id = path.parts[0]\n",
                 "\n",
                 "    device_ids.append(device_id)\n",
                 "    die_ids.append(die_id)\n",
                 "    die_xs.append(die_x)\n",
                 "    die_ys.append(die_y)\n",
                 "    wafer_ids.append(wafer_id)\n",
-                "    plotting_kwargs.append(measurement_type)\n",
+                "    plotting_kwargs.append(spectrum_measurement_type)\n",
                 "    project_ids.append(PROJECT_ID)\n",
                 "    data_types.append(\"measurement\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bbbf759b",
+            "id": "772a6aa0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "if NUMBER_OF_THREADS > 1:\n",
                 "    dd.device_data.upload_multi(\n",
                 "        files=data_files,\n",
                 "        project_ids=project_ids,\n",
@@ -420,306 +422,452 @@
                 "        progress_bar=True,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f419dc2d",
+            "id": "0ad0cc7a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "wafer_set = set(wafer_ids)\n",
                 "die_set = set(die_ids)\n",
                 "\n",
                 "print(wafer_set)\n",
                 "print(die_set)\n",
                 "print(len(die_set))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8b714fdd",
+            "id": "52579f5a",
             "metadata": {},
             "source": [
                 "## Analysis\n",
                 "\n",
-                "You can run analysis at 3 different levels. For example to extract:\n",
+                "You can run analysis at 3 different levels. For example to calculate:\n",
                 "\n",
                 "1. Device: averaged power envelope over certain number of samples.\n",
                 "2. Die: fit the propagation loss as a function of length.\n",
                 "3. Wafer: Define the Upper and Lower Spec limits for Known Good Die (KGD)\n",
                 "\n",
-                "![](https://i.imgur.com/ZwIWS08.png)\n",
-                "\n"
+                "![](https://i.imgur.com/ZwIWS08.png)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9e338f0d",
+            "id": "2685ea64",
             "metadata": {},
             "source": [
                 "To upload custom analysis functions to the DoData server, follow these simplified guidelines:\n",
                 "\n",
                 "- Input:\n",
-                "  - Begin with a unique identifier (device_data_pkey, die_pkey, wafer_pkey) as the first argument.\n",
+                "  - Begin with a unique identifier (device_data_id, die_id, wafer_id) as the first argument.\n",
                 "  - Add necessary keyword arguments for the analysis.\n",
                 "\n",
                 "- Output: Dictionary\n",
                 "  - output: Return a simple, one-level dictionary. All values must be serializable. Avoid using numpy or pandas; convert to lists if needed.\n",
                 "  - summary_plot: Provide a summary plot, either as a matplotlib figure or io.BytesIO object.\n",
                 "  - attributes: Add a serializable dictionary of the analysis settings.\n",
-                "  - device_data_pkey/die_pkey/wafer_pkey: Include the used identifier (device_data_pkey, die_pkey, wafer_pkey).\n"
+                "  - device_data_id/die_id/wafer_id: Include the used identifier (device_data_id, die_id, wafer_id).\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "76bf5a3a",
+            "id": "93b0cd0c",
             "metadata": {},
             "source": [
-                "### Device analysis\n",
+                "### Device Analysis\n",
                 "\n",
                 "You can either trigger analysis automatically by defining it in the design manifest, using the UI or using the Python DoData library.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "845c1e26",
+            "id": "6d3fd20d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from IPython.display import Code, display, Image\n",
                 "import doplaydo.dodata as dd\n",
                 "\n",
-                "display(Code(dd.config.Path.analysis_functions_device_iv_resistance))"
+                "display(Code(dd.config.Path.analysis_functions_device_power_envelope))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "93a5037d",
+            "id": "662c646b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
                 "    0\n",
                 "]\n",
                 "device_data.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "77edfda8",
+            "id": "ef086354",
             "metadata": {},
             "outputs": [],
             "source": [
+                "analysis_function_id = \"device_power_envelope\"\n",
+                "\n",
                 "response = dd.api.analysis_functions.validate(\n",
-                "    analysis_function_id=\"device_iv\",\n",
-                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
+                "    analysis_function_id=analysis_function_id,\n",
+                "    function_path=dd.config.Path.analysis_functions_device_power_envelope,\n",
                 "    test_model_pkey=device_data.pkey,\n",
                 "    target_model_name=\"device_data\",\n",
-                "    parameters=dict(min_i=50),\n",
+                "    parameters=dict(n=10),\n",
                 ")\n",
                 "Image(response.content)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b830c79d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "response = dd.api.analysis_functions.validate(\n",
-                "    analysis_function_id=\"device_iv\",\n",
-                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
-                "    test_model_pkey=device_data.pkey,\n",
-                "    target_model_name=\"device_data\",\n",
-                "    parameters=dict(wrong_variable=50),\n",
-                ")\n",
-                "print(response.text)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "d2195dd1",
+            "id": "fce41ff1",
             "metadata": {},
             "outputs": [],
             "source": [
+                "analysis_function_id = \"device_power_envelope\"\n",
+                "\n",
                 "dd.api.analysis_functions.validate_and_upload(\n",
-                "    analysis_function_id=\"device_iv\",\n",
-                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
+                "    analysis_function_id=analysis_function_id,\n",
+                "    function_path=dd.config.Path.analysis_functions_device_power_envelope,\n",
                 "    test_model_pkey=device_data.pkey,\n",
                 "    target_model_name=\"device_data\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6ea9f999",
+            "id": "e92bcbad",
             "metadata": {},
             "source": [
                 "### Die Analysis\n",
                 "\n",
-                "You can define a state for all device data available and trigger on that state.\n",
-                "\n",
-                "In the following example you will trigger a die analysis for 300, 500 and 800nm wide waveguides."
+                "You can trigger a die analysis for 300, 500 and 800nm wide waveguides."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7aac7d19",
+            "id": "0d4e1dc6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Code(dd.config.Path.analysis_functions_die_sheet_resistance)"
+                "Code(dd.config.Path.analysis_functions_die_loss_cutback)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a18a204b",
+            "metadata": {},
+            "source": [
+                "Lets find a die pkey for this project, so that we can trigger the die analysis on it."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7b0a8b2e",
+            "id": "aae6c7f0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
                 "    0\n",
                 "]\n",
                 "device_data.die.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "21cf85be",
+            "id": "23d60a04",
             "metadata": {},
             "outputs": [],
             "source": [
                 "die_pkey = device_data.die.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "10ed6342",
+            "id": "6f859562",
             "metadata": {},
             "outputs": [],
             "source": [
                 "response = dd.api.analysis_functions.validate(\n",
-                "    analysis_function_id=\"die_iv_sheet_resistance\",\n",
-                "    function_path=dd.config.Path.analysis_functions_die_sheet_resistance,\n",
+                "    analysis_function_id=\"die_loss_cutback\",\n",
+                "    function_path=dd.config.Path.analysis_functions_die_loss_cutback,\n",
                 "    test_model_pkey=die_pkey,\n",
                 "    target_model_name=\"die\",\n",
                 ")\n",
-                "print(response.headers)\n",
                 "Image(response.content)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c065cbc",
+            "id": "b339c418",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.api.analysis_functions.validate_and_upload(\n",
-                "    analysis_function_id=\"die_iv_sheet_resistance\",\n",
-                "    function_path=dd.config.Path.analysis_functions_die_sheet_resistance,\n",
+                "    analysis_function_id=\"die_loss_cutback\",\n",
+                "    function_path=dd.config.Path.analysis_functions_die_loss_cutback,\n",
                 "    test_model_pkey=die_pkey,\n",
                 "    target_model_name=\"die\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2f1aa23a",
+            "id": "79a7b5ce",
             "metadata": {},
             "outputs": [],
             "source": [
                 "database_dies = []\n",
-                "analysis_function_id = \"die_iv_sheet_resistance\"\n",
-                "widths_um = dm.width_um.unique()\n",
-                "widths_um"
+                "widths_um = [0.3, 0.5, 0.8]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eef585d3",
+            "id": "c7f166dc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lengths_um = dm.length_um.unique()\n",
-                "lengths_um"
+                "NUMBER_OF_THREADS = dd.settings.n_threads"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d05c2bcb",
+            "id": "20e3bd08",
             "metadata": {},
             "outputs": [],
             "source": [
-                "length_um = lengths_um[0]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4164f73c",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "analysis_function_id = \"die_iv_sheet_resistance\"\n",
-                "parameters = [{\"width_key\": \"width_um\", \"length_key\": \"length_um\"}] * len(wafer_set)\n",
+                "widths_um = [0.3, 0.5, 0.8]\n",
+                "parameters = [{\"value\": width_um, \"key\": \"width_um\"} for width_um in widths_um]\n",
                 "\n",
                 "dd.analysis.trigger_die_multi(\n",
                 "    project_id=PROJECT_ID,\n",
-                "    analysis_function_id=analysis_function_id,\n",
+                "    analysis_function_id=\"die_loss_cutback\",\n",
                 "    wafer_ids=wafer_set,\n",
                 "    die_xs=die_xs,\n",
                 "    die_ys=die_ys,\n",
-                "    progress_bar=True,\n",
                 "    parameters=parameters,\n",
+                "    progress_bar=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "775faf5e",
+            "id": "73c1c731",
             "metadata": {},
             "outputs": [],
             "source": [
                 "plots = dd.analysis.get_die_analysis_plots(\n",
                 "    project_id=PROJECT_ID, wafer_id=wafer_ids[0], die_x=0, die_y=0\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8653e5c1",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "len(plots)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8209822f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "display(plots[0])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "4d4a3ca7",
+            "metadata": {},
+            "source": [
+                "### Wafer Analysis\n",
+                "\n",
+                "Lets Define the Upper and Lower Spec limits for Known Good Die (KGD).\n",
+                "\n",
+                "For example:\n",
+                "\n",
+                "waveguide width (nm) | Lower Spec Limit (dB/cm) | Upper Spec limit (dB/cm)\n",
+                "----------------| -------------------------| ------------------------\n",
+                "300 |  0 | 3.13\n",
+                "500 |  0 | 2.31\n",
+                "800 |  0 | 1.09\n",
+                "\n",
+                "As for waveguide loss you can define no minimum loss (0 dB/cm) and you only define the maximum accepted loss (Upper Spec Limit)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "af4522d5",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "Code(dd.config.Path.analysis_functions_wafer_loss_cutback)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "81c2c0ec",
+            "metadata": {},
+            "source": [
+                "Lets find a wafer pkey for this project, so that we can trigger the wafer analysis on it."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "153a6df4",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
+                "    0\n",
+                "]\n",
+                "wafer_pkey = device_data.die.wafer.pkey\n",
+                "wafer_pkey"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "35cc8bdc",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "response = dd.api.analysis_functions.validate(\n",
+                "    analysis_function_id=\"wafer_loss_cutback\",\n",
+                "    function_path=dd.config.Path.analysis_functions_wafer_loss_cutback,\n",
+                "    test_model_pkey=wafer_pkey,\n",
+                "    target_model_name=\"wafer\",\n",
+                "    parameters={\n",
+                "        \"key\": \"width_um\",\n",
+                "        \"value\": 0.3,\n",
+                "        \"upper_spec\": 3.13,\n",
+                "        \"lower_spec\": 0,\n",
+                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
+                "        \"metric\": \"propagation_loss_dB_cm\",\n",
+                "    },\n",
+                ")\n",
+                "Image(response.content)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8a9399a8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dd.api.analysis_functions.validate_and_upload(\n",
+                "    analysis_function_id=\"wafer_loss_cutback\",\n",
+                "    function_path=dd.config.Path.analysis_functions_wafer_loss_cutback,\n",
+                "    test_model_pkey=wafer_pkey,\n",
+                "    target_model_name=\"wafer\",\n",
+                "    parameters={\n",
+                "        \"key\": \"width_um\",\n",
+                "        \"value\": 0.3,\n",
+                "        \"lower_spec\": 0,\n",
+                "        \"upper_spec\": 3.13,\n",
+                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
+                "        \"metric\": \"propagation_loss_dB_cm\",\n",
+                "    },\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6f6b5e32",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "widths_um = [0.3, 0.5, 0.8]\n",
+                "maximum_loss_per_width = {\n",
+                "    0.3: 3.13,\n",
+                "    0.5: 2.31,\n",
+                "    0.8: 1.09,\n",
+                "}\n",
+                "parameters = [\n",
+                "    {\n",
+                "        \"key\": \"width_um\",\n",
+                "        \"value\": width_um,\n",
+                "        \"upper_spec\": maximum_loss_per_width[width_um],\n",
+                "        \"lower_spec\": 0,\n",
+                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
+                "        \"metric\": \"propagation_loss_dB_cm\",\n",
+                "    }\n",
+                "    for width_um in widths_um\n",
+                "]\n",
+                "\n",
+                "for wafer in tqdm(wafer_set):\n",
+                "    for params in parameters:\n",
+                "        r = dd.analysis.trigger_wafer(\n",
+                "            project_id=PROJECT_ID,\n",
+                "            wafer_id=wafer,\n",
+                "            analysis_function_id=\"wafer_loss_cutback\",\n",
+                "            parameters=params,\n",
+                "        )\n",
+                "        if r.status_code != 200:\n",
+                "            raise requests.HTTPError(r.text)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8341c707",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plots = dd.analysis.get_wafer_analysis_plots(\n",
+                "    project_id=PROJECT_ID, wafer_id=wafer_ids[0], target_model=\"wafer\"\n",
                 ")\n",
                 "len(plots)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3bfcaaf7",
+            "id": "b74e1fe0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "for plot in plots:\n",
                 "    display(plot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b6e189ed",
+            "id": "b31a45b5",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/4_download_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/4_download_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/5_delete.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/5_delete.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/generate_layout.py` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/generate_layout.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/resistance/test_chip.lyp` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/test_chip.lyp`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/1_generate_layout.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/1_generate_layout.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/2_generate_measurement_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/2_generate_measurement_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/3_upload_measurements.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/3_upload_measurements.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999763794406651%*

 * *Differences: {"'cells'": "{55: {'source': {insert: [(8, '    ],\\n'), (9, '    limit=1,\\n')], delete: [8]}}}"}*

```diff
@@ -829,15 +829,16 @@
                 "    [\n",
                 "        dd.Project.project_id == PROJECT_ID,\n",
                 "        dd.or_(\n",
                 "            dd.Device.device_id == device_data20.device.device_id,\n",
                 "            dd.Device.device_id == device_data10.device.device_id,\n",
                 "            dd.Device.device_id == device_data5.device.device_id,\n",
                 "        ),\n",
-                "    ]\n",
+                "    ],\n",
+                "    limit=1,\n",
                 ")\n",
                 "device_data_pkeys = [d.pkey for d in device_data_objects]\n",
                 "params = [dict(height=-0.02)] * len(device_data_objects)\n",
                 "analyses = dd.api.analysis.trigger_device_data_multi(\n",
                 "    device_data_pkeys=device_data_pkeys,\n",
                 "    analysis_function_id=\"device_fsr\",\n",
                 "    parameters=params,\n",
```

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/4_download_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/4_download_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/5_delete.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/5_delete.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/generate_layout.py` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/generate_layout.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/rings/generic.lyp` & `dodata-0.5.0/notebooks/dodata_tutorials/rings/generic.lyp`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/1_generate_layout.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/1_generate_layout.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/2_generate_measurement_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/2_generate_measurement_data.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996153578390421%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, '    peak_power: float, center_wavelength: float, "*

 * *            'bandwidth_1dB, wavelength\\n\'), (3, \'    """Calculate the response of a Gaussian '*

 * *            "grating coupler.\\n'), (5, '    Args:\\n'), (6, '        peak_power: The peak power "*

 * *            "of the response.\\n'), (7, '        center_wavelength: The center wavelength of the "*

 * *            "grating coupler.\\n'), (8, '        bandwidth_1dB: The 1 dB bandwidth of the "*

 * *            "coupler.\\n'), (9 […]*

```diff
@@ -43,47 +43,45 @@
             "id": "08f8de0e",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "outputs": [],
             "source": [
                 "def gaussian_grating_coupler_response(\n",
-                "    peak_power, center_wavelength, bandwidth_1dB, wavelength\n",
+                "    peak_power: float, center_wavelength: float, bandwidth_1dB, wavelength\n",
                 "):\n",
-                "    \"\"\"\n",
-                "    Calculate the response of a Gaussian grating coupler.\n",
+                "    \"\"\"Calculate the response of a Gaussian grating coupler.\n",
                 "\n",
-                "    Parameters:\n",
-                "    - peak_power: The peak power of the response.\n",
-                "    - center_wavelength: The center wavelength of the grating coupler.\n",
-                "    - bandwidth_1dB: The 1 dB bandwidth of the coupler.\n",
-                "    - wavelength: The wavelength at which the response is evaluated.\n",
+                "    Args:\n",
+                "        peak_power: The peak power of the response.\n",
+                "        center_wavelength: The center wavelength of the grating coupler.\n",
+                "        bandwidth_1dB: The 1 dB bandwidth of the coupler.\n",
+                "        wavelength: The wavelength at which the response is evaluated.\n",
                 "\n",
                 "    Returns:\n",
                 "    - The power of the grating coupler response at the given wavelength.\n",
                 "    \"\"\"\n",
                 "    # Convert 1 dB bandwidth to standard deviation (sigma)\n",
                 "    sigma = bandwidth_1dB / (2 * np.sqrt(2 * np.log(10)))\n",
                 "\n",
                 "    # Gaussian response calculation\n",
                 "    response = peak_power * np.exp(\n",
                 "        -0.5 * ((wavelength - center_wavelength) / sigma) ** 2\n",
                 "    )\n",
-                "\n",
                 "    return response\n",
                 "\n",
                 "\n",
                 "nm = 1e-3\n",
                 "# Parameters\n",
                 "peak_power = 1.0\n",
                 "center_wavelength = 1550 * nm  # Center wavelength in micrometers\n",
                 "bandwidth_1dB = 100 * nm\n",
                 "\n",
                 "# Wavelength range: 100 nm around the center wavelength, converted to micrometers\n",
-                "wavelength_range = np.linspace(center_wavelength - 0.05, center_wavelength + 0.05, 150)\n",
+                "wavelength_range = np.linspace(center_wavelength - 0.05, center_wavelength + 0.05, 121)\n",
                 "\n",
                 "# Calculate the response for each wavelength\n",
                 "responses = [\n",
                 "    gaussian_grating_coupler_response(peak_power, center_wavelength, bandwidth_1dB, wl)\n",
                 "    for wl in wavelength_range\n",
                 "]\n",
                 "\n",
@@ -170,44 +168,49 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "14c13dd3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "cwd = Path(\".\")\n",
-                "\n",
                 "metadata = {\"measurement_type\": \"Spectral MEAS\", \"temperature\": 25}\n",
-                "\n",
                 "noise_peak_to_peak_dB = 1\n",
                 "grating_coupler_loss_dB = 3\n",
                 "\n",
                 "for wafer in wafers:\n",
+                "    wafer_per_cent_variation = 0.20  # 20% variation\n",
+                "    wafer_variation_factor = 1 + wafer_per_cent_variation * (2 * np.random.rand() - 1)\n",
+                "\n",
                 "    for die in dies:\n",
                 "        die = f\"{(die['x'])}_{(die['y'])}\"\n",
                 "        for (_, row), (_, device_row) in zip(df.iterrows(), df.iterrows()):\n",
                 "            cell_id = row[\"cell\"]\n",
                 "            if \"ridge\" in cell_id:\n",
                 "                continue\n",
                 "            top_cell_id = \"RibLoss\" if \"rib\" in cell_id else \"RidgeLoss\"\n",
-                "            device_id = (\n",
-                "                f\"{top_cell_id}_{cell_id}_{device_row['x']}_{device_row['y']}\"\n",
-                "            )\n",
+                "            device_id = f\"{top_cell_id}_{cell_id}_{device_row['x']}_{device_row['y']}\"\n",
                 "            dirpath = cwd / wafer / die / device_id\n",
                 "            dirpath.mkdir(exist_ok=True, parents=True)\n",
                 "            data_file = dirpath / \"data.json\"\n",
                 "            metadata_file = dirpath / \"attributes.json\"\n",
                 "            metadata_file.write_text(json.dumps(metadata))\n",
                 "            loss_dB = (\n",
                 "                np.polyval(loss_vs_width_model, row[\"width_um\"])\n",
                 "                * row[\"length_um\"]\n",
                 "                * 1e-6\n",
                 "                * 1e2\n",
                 "            )  # convert um to cm\n",
                 "            loss_dB += 2 * grating_coupler_loss_dB\n",
                 "            peak_power = 10 ** (-loss_dB / 10)\n",
+                "            device_per_cent_variation = 0.05  # 5% variation\n",
+                "            device_variation_factor = 1 + device_per_cent_variation * (\n",
+                "                2 * np.random.rand() - 1\n",
+                "            )\n",
+                "            peak_power *= wafer_variation_factor * device_variation_factor\n",
+                "\n",
                 "            output_power = [\n",
                 "                gaussian_grating_coupler_response(\n",
                 "                    peak_power, center_wavelength, bandwidth_1dB, wl\n",
                 "                )\n",
                 "                for wl in wavelength_range\n",
                 "            ]\n",
                 "            output_power *= 10 ** (\n",
```

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/3_upload_measurements.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/resistance/3_upload_measurements.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9633582406713722%*

 * *Differences: {"'cells'": "{0: {'id': '324eaab3', 'source': {insert: [(0, '# Upload measurements and run "*

 * *            "analysis\\n')], delete: [0]}}, 1: {'id': '131ce11e', 'source': {insert: [(5, 'import "*

 * *            "getpass\\n'), (6, 'import matplotlib.pyplot as plt\\n'), (7, '\\n'), (8, 'username = "*

 * *            "getpass.getuser()')], delete: [5]}}, 2: {'id': 'e14eba7a'}, 3: {'id': '6144eb85', "*

 * *            '\'source\': [\'PROJECT_ID = f"resistance-{username}"\\n\', \'\\n\', '*

 * *            '\'MEASUREMENTS_PATHS = lis […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "68e7c0eb",
+            "id": "324eaab3",
             "metadata": {},
             "source": [
-                "# Upload Measurement Data and run Analysis\n",
+                "# Upload measurements and run analysis\n",
                 "\n",
                 "Now you will post your measurement data and analysis to the database via the API.\n",
                 "\n",
                 "**If you are running the tutorials in DoLab, the following instructions are not necessary and you can skip directly to the next cell.**\n",
                 "\n",
                 "You will need to authenticate to the database with your username and password. To make this easy,  you can create a file called `.env` in this folder and complete it with your organization's URL and authentication information as follows:\n",
                 "\n",
@@ -25,80 +25,83 @@
                 "\n",
                 "If you haven't defined a `.env` file or saved your credentials to your environment variables, you will be prompted for your credentials now."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "30a16d0e",
+            "id": "131ce11e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import doplaydo.dodata as dd\n",
                 "import pandas as pd\n",
                 "from pathlib import Path\n",
                 "from tqdm.auto import tqdm\n",
                 "import requests\n",
-                "import getpass"
+                "import getpass\n",
+                "import matplotlib.pyplot as plt\n",
+                "\n",
+                "username = getpass.getuser()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "39025f78",
+            "id": "e14eba7a",
             "metadata": {},
             "source": [
                 "Let's now create a project. \n",
                 "\n",
                 "In normal circumstances, everyone will be sharing and contributing to a project. In this demo, however, we want to *keep your project separate* from other users for clarity, so we will append your username to the project name. This way you can also safely delete and recreate projects without creating issues for others. If you prefer though, you can change the `PROJECT_ID` to anything you like. Just be sure to update it in the subsequent notebooks of this tutorial as well."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8d70639d",
+            "id": "6144eb85",
             "metadata": {},
             "outputs": [],
             "source": [
-                "username = getpass.getuser()\n",
-                "PROJECT_ID = f\"spirals-{username}\"\n",
-                "MEASUREMENTS_PATH = Path(\"6d4c615ff105/\")\n",
-                "PROJECT_ID"
+                "PROJECT_ID = f\"resistance-{username}\"\n",
+                "\n",
+                "MEASUREMENTS_PATHS = list(Path(\"wafers\").glob(\"*\"))\n",
+                "MEASUREMENTS_PATHS"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "337aa355",
+            "id": "e4e8e119",
             "metadata": {},
             "source": [
                 "Lets delete the project if it already exists so that you can start fresh."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c8d226b3",
+            "id": "96eaf9b3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.delete(PROJECT_ID).text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "814a129c",
+            "id": "bcee9154",
             "metadata": {},
             "source": [
                 "## New project\n",
                 "\n",
                 "You can create the project, upload the design manifest, and upload the wafer definitions through the Webapp as well as programmatically using this notebook"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "207cd8ec",
+            "id": "774500ef",
             "metadata": {},
             "source": [
                 "### Upload Project\n",
                 "\n",
                 "You can create a new project and extract all cells & devices below for the `RidgeLoss` and `RibLoss`\n",
                 "\n",
                 "The expressions are regex expressions. For intro and testing your regexes you can check out [regex101](https://regex101.com)\n",
@@ -109,169 +112,167 @@
                 "\n",
                 "Whitelists take precedence over blacklists, so if you define both, it uses only the whitelist."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0746daec",
+            "id": "695b1865",
             "metadata": {},
             "outputs": [],
             "source": [
                 "cell_extraction = [\n",
                 "    dd.project.Extraction(\n",
-                "        cell_id=\"RibLoss\",\n",
-                "        cell_white_list=[\"^cutback_rib\"],\n",
-                "        min_hierarchy_lvl=0,\n",
-                "        max_hierarchy_lvl=0,\n",
-                "    ),\n",
-                "    dd.project.Extraction(\n",
-                "        cell_id=\"RidgeLoss\",\n",
-                "        cell_white_list=[\"^cutback_ridge\"],\n",
+                "        cell_id=\"resistance\",\n",
+                "        cell_white_list=[\"^resistance\"],\n",
                 "        min_hierarchy_lvl=0,\n",
                 "        max_hierarchy_lvl=0,\n",
                 "    ),\n",
                 "]\n",
                 "\n",
                 "dd.project.create(\n",
                 "    project_id=PROJECT_ID,\n",
                 "    eda_file=\"test_chip.gds\",\n",
-                "    lyp_file=\"loss_measurements.lyp\",\n",
+                "    lyp_file=\"test_chip.lyp\",\n",
                 "    cell_extractions=cell_extraction,\n",
                 ").text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "724d33f5",
+            "id": "63d5a0cc",
             "metadata": {},
             "source": [
                 "### Upload Design Manifest\n",
                 "\n",
                 "The design manifest is a CSV file that includes all the cell names, the cell settings, a list of analysis to trigger, and a list of settings for each analysis."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5902d5ad",
+            "id": "fffbb4b7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm = pd.read_csv(\"design_manifest.csv\")\n",
                 "dm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3b214d19",
+            "id": "355452eb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm = dm.drop(columns=[\"analysis\", \"analysis_parameters\"])\n",
                 "dm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "31577dc7",
+            "id": "0e650acd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dm.to_csv(\"design_manifest_without_analysis.csv\", index=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1aa5a8b0",
+            "id": "c79178e4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.upload_design_manifest(\n",
                 "    project_id=PROJECT_ID, filepath=\"design_manifest_without_analysis.csv\"\n",
                 ").text"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "db40bd55",
+            "id": "cb52f953",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.download_design_manifest(\n",
                 "    project_id=PROJECT_ID, filepath=\"design_manifest_downloaded.csv\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d50a9b23",
+            "id": "edd1d6cc",
             "metadata": {},
             "source": [
                 "### Upload Wafer Definitions\n",
                 "\n",
                 "The wafer definition is a JSON file where you can define the wafer names and die names and location for each wafer."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8181b418",
+            "id": "bfea5fcb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.project.upload_wafer_definitions(\n",
                 "    project_id=PROJECT_ID, filepath=\"wafer_definitions.json\"\n",
                 ").text"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9c9c71d0",
+            "id": "13f73719",
             "metadata": {},
             "source": [
                 "## Upload data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "eddc6cdb",
+            "id": "cfda4e1b",
             "metadata": {},
             "source": [
                 "Your Tester can output the data in JSON files. It does not need to be Python."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b0cc0012",
+            "id": "26377b7f",
             "metadata": {},
             "source": [
                 "You can get all paths which have measurement data within the test path."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "91f386d5",
+            "id": "8348da4c",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "outputs": [],
             "source": [
-                "data_files = list(MEASUREMENTS_PATH.glob(\"**/data.json\"))\n",
+                "data_files = [\n",
+                "    file\n",
+                "    for MEASUREMENTS_PATH in MEASUREMENTS_PATHS\n",
+                "    for file in MEASUREMENTS_PATH.glob(\"**/data.json\")\n",
+                "]\n",
                 "print(data_files[0].parts)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bb7859dc",
+            "id": "baf7d7d6",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "source": [
                 " You should define a plotting per measurement type in python. Your plots can evolve over time even for the same measurement type.\n",
                 "\n",
                 "Required:\n",
@@ -302,114 +303,117 @@
                 "\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "38478f45",
+            "id": "7765dc0d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "spectrum_measurement_type = dd.api.device_data.PlottingKwargs(\n",
-                "    x_name=\"wavelength\",\n",
-                "    y_name=\"output_power\",\n",
-                "    x_col=\"wavelength\",\n",
-                "    # y_col=[\"output_power\"],  # can also be a string for a single value\n",
-                "    y_col=\"output_power\",\n",
+                "measurement_type = dd.api.device_data.PlottingKwargs(\n",
+                "    x_name=\"i\",\n",
+                "    y_name=\"v\",\n",
+                "    x_col=\"i\",\n",
+                "    y_col=[\"v\"],  # can also be a string for a single value\n",
+                "    # y_col=\"v\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3eee0823",
+            "id": "47655f38",
             "metadata": {},
             "source": [
                 "### Upload measurements\n",
                 "\n",
                 "You can now upload measurement data.\n",
                 "\n",
                 "This is a bare bones example, in a production setting, you can also add validation, logging, and error handling to ensure a smooth operation.\n",
                 "\n",
                 "Every measurement you upload will trigger all the analysis that you defined in the design manifest."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2f37ca4d",
+            "id": "28205616",
             "metadata": {},
             "outputs": [],
             "source": [
+                "wafer_set = set()\n",
+                "die_set = set()\n",
                 "NUMBER_OF_THREADS = 1 if \"127\" in dd.settings.dodata_url else dd.settings.n_threads\n",
                 "NUMBER_OF_THREADS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3370ba1a",
+            "id": "c4ff8f0f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "if NUMBER_OF_THREADS == 1:\n",
                 "    for path in tqdm(data_files):\n",
-                "        wafer_id = path.parts[0]\n",
-                "        die_x, die_y = path.parts[1].split(\"_\")\n",
+                "        wafer_id = path.parts[1]\n",
+                "        die_x, die_y = path.parts[2].split(\"_\")\n",
                 "\n",
                 "        r = dd.api.device_data.upload(\n",
                 "            file=path,\n",
                 "            project_id=PROJECT_ID,\n",
                 "            wafer_id=wafer_id,\n",
                 "            die_x=die_x,\n",
                 "            die_y=die_y,\n",
-                "            device_id=path.parts[2],\n",
-                "            data_type=\"measurement\",  # can also be \"simulation\"\n",
-                "            plotting_kwargs=spectrum_measurement_type,\n",
+                "            device_id=path.parts[3],\n",
+                "            data_type=\"measurement\",\n",
+                "            plotting_kwargs=measurement_type,\n",
                 "        )\n",
+                "        wafer_set.add(wafer_id)\n",
+                "        die_set.add(path.parts[2])\n",
                 "        r.raise_for_status()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d515538c",
+            "id": "940660d3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_files = list(MEASUREMENTS_PATH.glob(\"**/data.json\"))\n",
                 "project_ids = []\n",
                 "device_ids = []\n",
                 "die_ids = []\n",
                 "die_xs = []\n",
                 "die_ys = []\n",
                 "wafer_ids = []\n",
                 "plotting_kwargs = []\n",
                 "data_types = []\n",
                 "\n",
                 "for path in data_files:\n",
-                "    device_id = path.parts[2]\n",
-                "    die_id = path.parts[1]\n",
+                "    device_id = path.parts[3]\n",
+                "    die_id = path.parts[2]\n",
                 "    die_x, die_y = die_id.split(\"_\")\n",
-                "    wafer_id = path.parts[0]\n",
+                "    wafer_id = path.parts[1]\n",
                 "\n",
                 "    device_ids.append(device_id)\n",
                 "    die_ids.append(die_id)\n",
                 "    die_xs.append(die_x)\n",
                 "    die_ys.append(die_y)\n",
                 "    wafer_ids.append(wafer_id)\n",
-                "    plotting_kwargs.append(spectrum_measurement_type)\n",
+                "    plotting_kwargs.append(measurement_type)\n",
                 "    project_ids.append(PROJECT_ID)\n",
                 "    data_types.append(\"measurement\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "772a6aa0",
+            "id": "bbbf759b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "if NUMBER_OF_THREADS > 1:\n",
                 "    dd.device_data.upload_multi(\n",
                 "        files=data_files,\n",
                 "        project_ids=project_ids,\n",
@@ -422,452 +426,656 @@
                 "        progress_bar=True,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0ad0cc7a",
+            "id": "f419dc2d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "wafer_set = set(wafer_ids)\n",
                 "die_set = set(die_ids)\n",
                 "\n",
                 "print(wafer_set)\n",
                 "print(die_set)\n",
                 "print(len(die_set))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "52579f5a",
+            "id": "8b714fdd",
             "metadata": {},
             "source": [
                 "## Analysis\n",
                 "\n",
-                "You can run analysis at 3 different levels. For example to calculate:\n",
+                "You can run analysis at 3 different levels. For example to extract:\n",
                 "\n",
                 "1. Device: averaged power envelope over certain number of samples.\n",
                 "2. Die: fit the propagation loss as a function of length.\n",
                 "3. Wafer: Define the Upper and Lower Spec limits for Known Good Die (KGD)\n",
                 "\n",
-                "![](https://i.imgur.com/ZwIWS08.png)"
+                "![](https://i.imgur.com/ZwIWS08.png)\n",
+                "\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2685ea64",
+            "id": "9e338f0d",
             "metadata": {},
             "source": [
                 "To upload custom analysis functions to the DoData server, follow these simplified guidelines:\n",
                 "\n",
                 "- Input:\n",
-                "  - Begin with a unique identifier (device_data_id, die_id, wafer_id) as the first argument.\n",
+                "  - Begin with a unique identifier (device_data_pkey, die_pkey, wafer_pkey) as the first argument.\n",
                 "  - Add necessary keyword arguments for the analysis.\n",
                 "\n",
                 "- Output: Dictionary\n",
                 "  - output: Return a simple, one-level dictionary. All values must be serializable. Avoid using numpy or pandas; convert to lists if needed.\n",
                 "  - summary_plot: Provide a summary plot, either as a matplotlib figure or io.BytesIO object.\n",
                 "  - attributes: Add a serializable dictionary of the analysis settings.\n",
-                "  - device_data_id/die_id/wafer_id: Include the used identifier (device_data_id, die_id, wafer_id).\n"
+                "  - device_data_pkey/die_pkey/wafer_pkey: Include the used identifier (device_data_pkey, die_pkey, wafer_pkey).\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "93b0cd0c",
+            "id": "76bf5a3a",
             "metadata": {},
             "source": [
-                "### Device Analysis\n",
+                "### Device analysis\n",
                 "\n",
                 "You can either trigger analysis automatically by defining it in the design manifest, using the UI or using the Python DoData library.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6d3fd20d",
+            "id": "845c1e26",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from IPython.display import Code, display, Image\n",
                 "import doplaydo.dodata as dd\n",
                 "\n",
-                "display(Code(dd.config.Path.analysis_functions_device_power_envelope))"
+                "display(Code(dd.config.Path.analysis_functions_device_iv_resistance))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "662c646b",
+            "id": "93a5037d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
                 "    0\n",
                 "]\n",
                 "device_data.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef086354",
+            "id": "77edfda8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "analysis_function_id = \"device_power_envelope\"\n",
-                "\n",
                 "response = dd.api.analysis_functions.validate(\n",
-                "    analysis_function_id=analysis_function_id,\n",
-                "    function_path=dd.config.Path.analysis_functions_device_power_envelope,\n",
+                "    analysis_function_id=\"device_iv\",\n",
+                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
                 "    test_model_pkey=device_data.pkey,\n",
                 "    target_model_name=\"device_data\",\n",
-                "    parameters=dict(n=10),\n",
+                "    parameters=dict(min_i=50),\n",
                 ")\n",
                 "Image(response.content)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fce41ff1",
+            "id": "b830c79d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "response = dd.api.analysis_functions.validate(\n",
+                "    analysis_function_id=\"device_iv\",\n",
+                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
+                "    test_model_pkey=device_data.pkey,\n",
+                "    target_model_name=\"device_data\",\n",
+                "    parameters=dict(wrong_variable=50),\n",
+                ")\n",
+                "print(response.text)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d2195dd1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "analysis_function_id = \"device_power_envelope\"\n",
-                "\n",
                 "dd.api.analysis_functions.validate_and_upload(\n",
-                "    analysis_function_id=analysis_function_id,\n",
-                "    function_path=dd.config.Path.analysis_functions_device_power_envelope,\n",
+                "    analysis_function_id=\"device_iv\",\n",
+                "    function_path=dd.config.Path.analysis_functions_device_iv_resistance,\n",
                 "    test_model_pkey=device_data.pkey,\n",
                 "    target_model_name=\"device_data\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e92bcbad",
+            "id": "6ea9f999",
             "metadata": {},
             "source": [
                 "### Die Analysis\n",
                 "\n",
-                "You can trigger a die analysis for 300, 500 and 800nm wide waveguides."
+                "You can define a state for all device data available and trigger on that state.\n",
+                "\n",
+                "In the following example you will trigger a die analysis for 300, 500 and 800nm wide waveguides."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0d4e1dc6",
+            "id": "7aac7d19",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Code(dd.config.Path.analysis_functions_die_loss_cutback)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a18a204b",
-            "metadata": {},
-            "source": [
-                "Lets find a die pkey for this project, so that we can trigger the die analysis on it."
+                "Code(dd.config.Path.analysis_functions_die_sheet_resistance)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "aae6c7f0",
+            "id": "7b0a8b2e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
                 "    0\n",
                 "]\n",
                 "device_data.die.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "23d60a04",
+            "id": "21cf85be",
             "metadata": {},
             "outputs": [],
             "source": [
                 "die_pkey = device_data.die.pkey"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6f859562",
+            "id": "10ed6342",
             "metadata": {},
             "outputs": [],
             "source": [
                 "response = dd.api.analysis_functions.validate(\n",
-                "    analysis_function_id=\"die_loss_cutback\",\n",
-                "    function_path=dd.config.Path.analysis_functions_die_loss_cutback,\n",
+                "    analysis_function_id=\"die_iv_sheet_resistance\",\n",
+                "    function_path=dd.config.Path.analysis_functions_die_sheet_resistance,\n",
                 "    test_model_pkey=die_pkey,\n",
                 "    target_model_name=\"die\",\n",
                 ")\n",
+                "print(response.headers)\n",
                 "Image(response.content)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b339c418",
+            "id": "6c065cbc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dd.api.analysis_functions.validate_and_upload(\n",
-                "    analysis_function_id=\"die_loss_cutback\",\n",
-                "    function_path=dd.config.Path.analysis_functions_die_loss_cutback,\n",
+                "    analysis_function_id=\"die_iv_sheet_resistance\",\n",
+                "    function_path=dd.config.Path.analysis_functions_die_sheet_resistance,\n",
                 "    test_model_pkey=die_pkey,\n",
                 "    target_model_name=\"die\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "79a7b5ce",
+            "id": "2f1aa23a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "database_dies = []\n",
-                "widths_um = [0.3, 0.5, 0.8]"
+                "analysis_function_id = \"die_iv_sheet_resistance\"\n",
+                "widths_um = dm.width_um.unique()\n",
+                "widths_um"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "eef585d3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "lengths_um = dm.length_um.unique()\n",
+                "lengths_um"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c7f166dc",
+            "id": "d05c2bcb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "NUMBER_OF_THREADS = dd.settings.n_threads"
+                "length_um = lengths_um[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "20e3bd08",
+            "id": "4164f73c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "widths_um = [0.3, 0.5, 0.8]\n",
-                "parameters = [{\"value\": width_um, \"key\": \"width_um\"} for width_um in widths_um]\n",
+                "analysis_function_id = \"die_iv_sheet_resistance\"\n",
+                "parameters = [{\"width_key\": \"width_um\", \"length_key\": \"length_um\"}] * len(wafer_set)\n",
                 "\n",
                 "dd.analysis.trigger_die_multi(\n",
                 "    project_id=PROJECT_ID,\n",
-                "    analysis_function_id=\"die_loss_cutback\",\n",
+                "    analysis_function_id=analysis_function_id,\n",
                 "    wafer_ids=wafer_set,\n",
                 "    die_xs=die_xs,\n",
                 "    die_ys=die_ys,\n",
-                "    parameters=parameters,\n",
                 "    progress_bar=True,\n",
+                "    parameters=parameters,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "73c1c731",
+            "id": "775faf5e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "plots = dd.analysis.get_die_analysis_plots(\n",
                 "    project_id=PROJECT_ID, wafer_id=wafer_ids[0], die_x=0, die_y=0\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "8653e5c1",
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                ")\n",
                 "len(plots)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8209822f",
+            "id": "3bfcaaf7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "display(plots[0])"
+                "for plot in plots:\n",
+                "    display(plot)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4d4a3ca7",
+            "id": "3c0401f9",
             "metadata": {},
             "source": [
-                "### Wafer Analysis\n",
+                "## Wafer analysis\n",
                 "\n",
                 "Lets Define the Upper and Lower Spec limits for Known Good Die (KGD).\n",
                 "\n",
-                "For example:\n",
-                "\n",
-                "waveguide width (nm) | Lower Spec Limit (dB/cm) | Upper Spec limit (dB/cm)\n",
-                "----------------| -------------------------| ------------------------\n",
-                "300 |  0 | 3.13\n",
-                "500 |  0 | 2.31\n",
-                "800 |  0 | 1.09\n",
-                "\n",
-                "As for waveguide loss you can define no minimum loss (0 dB/cm) and you only define the maximum accepted loss (Upper Spec Limit)\n"
+                "Lets find a wafer pkey for this project, so that we can trigger the die analysis on it."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "af4522d5",
+            "id": "38aa9509",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Code(dd.config.Path.analysis_functions_wafer_loss_cutback)"
+                "device_id"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "81c2c0ec",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b4e71b56",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Lets find a wafer pkey for this project, so that we can trigger the wafer analysis on it."
+                "device_data_objects = dd.get_data_objects_by_query(\n",
+                "    [\n",
+                "        dd.Project.project_id == PROJECT_ID,\n",
+                "        dd.Device.device_id == device_data.device.device_id,\n",
+                "    ],\n",
+                "    limit=1,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "153a6df4",
+            "id": "b6e189ed",
             "metadata": {},
             "outputs": [],
             "source": [
-                "device_data, df = dd.get_data_by_query([dd.Project.project_id == PROJECT_ID], limit=1)[\n",
-                "    0\n",
-                "]\n",
-                "wafer_pkey = device_data.die.wafer.pkey\n",
-                "wafer_pkey"
+                "wafer_pkey = device_data_objects[0].die.wafer.pkey\n",
+                "wafer_id = device_data_objects[0].die.wafer.wafer_id\n",
+                "wafer_id"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "35cc8bdc",
+            "id": "76cee641",
             "metadata": {},
             "outputs": [],
             "source": [
+                "upper_spec = 1e-8\n",
+                "lower_spec = 1e-12\n",
+                "parameters = {\n",
+                "    \"upper_spec\": upper_spec,\n",
+                "    \"lower_spec\": lower_spec,\n",
+                "    \"analysis_function_id\": \"die_iv_sheet_resistance\",\n",
+                "    \"metric\": \"sheet_resistance\",\n",
+                "    \"key\": None,\n",
+                "    \"scientific_notation\": True,\n",
+                "    \"decimal_places\": 1,\n",
+                "    \"fontsize_die\": 15,\n",
+                "    \"percentile_low\": 10,\n",
+                "    \"percentile_high\": 90,\n",
+                "}\n",
+                "\n",
                 "response = dd.api.analysis_functions.validate(\n",
                 "    analysis_function_id=\"wafer_loss_cutback\",\n",
                 "    function_path=dd.config.Path.analysis_functions_wafer_loss_cutback,\n",
                 "    test_model_pkey=wafer_pkey,\n",
                 "    target_model_name=\"wafer\",\n",
-                "    parameters={\n",
-                "        \"key\": \"width_um\",\n",
-                "        \"value\": 0.3,\n",
-                "        \"upper_spec\": 3.13,\n",
-                "        \"lower_spec\": 0,\n",
-                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
-                "        \"metric\": \"propagation_loss_dB_cm\",\n",
-                "    },\n",
+                "    parameters=parameters,\n",
                 ")\n",
                 "Image(response.content)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8a9399a8",
+            "id": "af87516b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dd.api.analysis_functions.validate_and_upload(\n",
+                "response = dd.api.analysis_functions.validate_and_upload(\n",
                 "    analysis_function_id=\"wafer_loss_cutback\",\n",
                 "    function_path=dd.config.Path.analysis_functions_wafer_loss_cutback,\n",
                 "    test_model_pkey=wafer_pkey,\n",
                 "    target_model_name=\"wafer\",\n",
-                "    parameters={\n",
-                "        \"key\": \"width_um\",\n",
-                "        \"value\": 0.3,\n",
-                "        \"lower_spec\": 0,\n",
-                "        \"upper_spec\": 3.13,\n",
-                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
-                "        \"metric\": \"propagation_loss_dB_cm\",\n",
-                "    },\n",
+                "    parameters=parameters,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6f6b5e32",
+            "id": "cc03b4d8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "widths_um = [0.3, 0.5, 0.8]\n",
-                "maximum_loss_per_width = {\n",
-                "    0.3: 3.13,\n",
-                "    0.5: 2.31,\n",
-                "    0.8: 1.09,\n",
-                "}\n",
-                "parameters = [\n",
-                "    {\n",
-                "        \"key\": \"width_um\",\n",
-                "        \"value\": width_um,\n",
-                "        \"upper_spec\": maximum_loss_per_width[width_um],\n",
-                "        \"lower_spec\": 0,\n",
-                "        \"analysis_function_id\": \"die_loss_cutback\",\n",
-                "        \"metric\": \"propagation_loss_dB_cm\",\n",
-                "    }\n",
-                "    for width_um in widths_um\n",
-                "]\n",
+                "parameters_list = [parameters]\n",
                 "\n",
                 "for wafer in tqdm(wafer_set):\n",
-                "    for params in parameters:\n",
+                "    for params in parameters_list:\n",
                 "        r = dd.analysis.trigger_wafer(\n",
                 "            project_id=PROJECT_ID,\n",
                 "            wafer_id=wafer,\n",
                 "            analysis_function_id=\"wafer_loss_cutback\",\n",
                 "            parameters=params,\n",
                 "        )\n",
                 "        if r.status_code != 200:\n",
                 "            raise requests.HTTPError(r.text)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8341c707",
+            "id": "1ac4bc68",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for wafer_id in wafer_set:\n",
+                "    plots = dd.analysis.get_wafer_analysis_plots(\n",
+                "        project_id=PROJECT_ID, wafer_id=wafer_id, target_model=\"wafer\"\n",
+                "    )\n",
+                "    for plot in plots:\n",
+                "        display(plot)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "51953e78",
+            "metadata": {},
+            "source": [
+                "## Wafer and Die comparison\n",
+                "\n",
+                "You can compare any dies or wafers, as another type of aggregated analysis"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3f4a27d6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plots = dd.analysis.get_wafer_analysis_plots(\n",
-                "    project_id=PROJECT_ID, wafer_id=wafer_ids[0], target_model=\"wafer\"\n",
+                "filter_clauses = [dd.Project.project_id == PROJECT_ID]\n",
+                "wafers = dd.db.wafer.get_wafers_by_query(filter_clauses)\n",
+                "wafer_pkeys = set([w.pkey for w in wafers])\n",
+                "wafer_pkeys"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0bfdd252",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "wafer_ids = {w.wafer_id for w in wafers}\n",
+                "wafer_ids"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "894c074c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "analysis_function_id = \"die_iv_sheet_resistance\"\n",
+                "filter_clauses = [dd.AnalysisFunction.analysis_function_id == analysis_function_id]\n",
+                "analyses_per_wafer = {}\n",
+                "\n",
+                "for wafer_id in wafer_ids:\n",
+                "    analyses_per_wafer[wafer_id] = dd.db.analysis.get_analyses_for_wafer(\n",
+                "        project_id=PROJECT_ID,\n",
+                "        wafer_id=wafer_id,\n",
+                "        target_model=\"die\",\n",
+                "        filter_clauses=filter_clauses,\n",
+                "    )"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "58d97274",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df = pd.DataFrame(\n",
+                "    [\n",
+                "        {\n",
+                "            \"die_pkey\": analysis.die_pkey,  # Correct access to die_pkey\n",
+                "            \"sheet_resistance\": analysis.output[\n",
+                "                \"sheet_resistance\"\n",
+                "            ],  # Correct access to sheet_resistance\n",
+                "            \"wafer_id\": wafer_id,  # Wafer key as part of the data\n",
+                "        }\n",
+                "        for wafer_id, analyses in analyses_per_wafer.items()  # First iterate over dict items\n",
+                "        for analysis in analyses  # Then iterate over each analysis in the list of analyses\n",
+                "    ]\n",
                 ")\n",
-                "len(plots)"
+                "df.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b74e1fe0",
+            "id": "88cc8f7f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for plot in plots:\n",
-                "    display(plot)"
+                "dict(analyses_per_wafer[wafer_id][0])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "59d87383",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def remove_outliers(df, column_name=\"sheet_resistance\"):\n",
+                "    Q1 = df[column_name].quantile(0.25)\n",
+                "    Q3 = df[column_name].quantile(0.75)\n",
+                "    IQR = Q3 - Q1\n",
+                "    lower_bound = Q1 - 1.5 * IQR\n",
+                "    upper_bound = Q3 + 1.5 * IQR\n",
+                "    return df[(df[column_name] >= lower_bound) & (df[column_name] <= upper_bound)]\n",
+                "\n",
+                "\n",
+                "filtered_df = remove_outliers(df)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "63844d43",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def remove_outliers(df, column_name=\"sheet_resistance\", min_val=None, max_val=None):\n",
+                "    \"\"\"Remove outliers from a DataFrame based on a column value.\"\"\"\n",
+                "    if min_val is not None:\n",
+                "        df = df[df[column_name] >= min_val]\n",
+                "    if max_val is not None:\n",
+                "        df = df[df[column_name] <= max_val]\n",
+                "    return df\n",
+                "\n",
+                "\n",
+                "filtered_df = remove_outliers(df, min_val=1e-15, max_val=1e-3)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4513686d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "filtered_df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "dfbf8385",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import plotly.express as px\n",
+                "\n",
+                "fig = px.box(\n",
+                "    df,\n",
+                "    x=\"wafer_id\",\n",
+                "    y=\"sheet_resistance\",\n",
+                "    title=\"Box Plot without Removing Outliers\",\n",
+                "    color=\"wafer_id\",  # This line will assign a different color to each box based on 'wafer_pkey'\n",
+                ")\n",
+                "fig.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "20b6ef49",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fig = px.box(\n",
+                "    filtered_df,\n",
+                "    x=\"wafer_id\",\n",
+                "    y=\"sheet_resistance\",\n",
+                "    title=\"Box Plot after Removing Outliers\",\n",
+                "    color=\"wafer_id\",  # This line will assign a different color to each box based on 'wafer_pkey'\n",
+                ")\n",
+                "fig.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "58131110",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import plotly.express as px\n",
+                "\n",
+                "# Assuming 'filtered_df' is your DataFrame that has been filtered to remove outliers.\n",
+                "fig = px.box(\n",
+                "    filtered_df,\n",
+                "    x=\"wafer_id\",\n",
+                "    y=\"sheet_resistance\",\n",
+                "    color=\"wafer_id\",  # Assign a different color to each box based on 'wafer_pkey'.\n",
+                "    title=\"Box Plot after Removing Outliers\",\n",
+                "    category_orders={\n",
+                "        \"wafer_id\": sorted(filtered_df[\"wafer_id\"].unique())\n",
+                "    },  # Sort the x-axis categories\n",
+                ")\n",
+                "\n",
+                "# Update the style of the boxes to resemble Seaborn's aesthetic and add transparency\n",
+                "fig.update_traces(marker=dict(opacity=0.6), line=dict(width=2), boxmean=True)\n",
+                "\n",
+                "# Update layout for a cleaner look, akin to Seaborn, and add grid lines\n",
+                "fig.update_layout(\n",
+                "    template=\"simple_white\",\n",
+                "    xaxis_title=\"Wafer ID\",\n",
+                "    yaxis_title=\"Sheet Resistance\",\n",
+                "    plot_bgcolor=\"rgba(0,0,0,0)\",  # Transparent background\n",
+                "    yaxis=dict(\n",
+                "        gridcolor=\"rgba(128,128,128,0.5)\",  # Light gray grid lines with transparency\n",
+                "        showgrid=True,  # Ensure grid lines are shown\n",
+                "        zerolinecolor=\"rgba(128,128,128,0.5)\",  # Light gray zero line with transparency\n",
+                "    ),\n",
+                "    xaxis=dict(\n",
+                "        gridcolor=\"rgba(128,128,128,0.5)\",  # Light gray grid lines with transparency\n",
+                "        showgrid=True,  # Ensure grid lines are shown\n",
+                "        zerolinecolor=\"rgba(128,128,128,0.5)\",  # Light gray zero line with transparency\n",
+                "    ),\n",
+                ")\n",
+                "\n",
+                "fig.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b31a45b5",
+            "id": "e2b5af48",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/4_download_data.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/4_download_data.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/5_delete.ipynb` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/5_delete.ipynb`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/loss_measurements.lyp` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/loss_measurements.lyp`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/notebooks/dodata_tutorials/spirals/test_chip.py` & `dodata-0.5.0/notebooks/dodata_tutorials/spirals/test_chip.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/pyproject.toml` & `dodata-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,21 @@
   "tqdm"
 ]
 description = "Software Development Kit - SDK for DoData"
 license = {file = "LICENSE"}
 name = "dodata"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.4.9"
+version = "0.5.0"
 
 [project.optional-dependencies]
 demos = [
   "gdsfactory==7.17.0",
-  "jupyterlab"
+  "jupyterlab",
+  "plotly"
 ]
 dev = [
   "ruff",
   "mypy",
   "pre-commit",
   "pytest",
   "towncrier",
@@ -179,15 +180,15 @@
 src = "src/doplaydo/dodata/__init__.py"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.tbump.version]
-current = "0.4.9"  # bump this
+current = "0.5.0"  # bump this
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `dodata-0.4.9/src/doplaydo/dodata/__init__.py` & `dodata-0.5.0/src/doplaydo/dodata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from .db.common import attribute_filter, analysis_filter
 from .db.device_data import get_data_by_query, get_data_objects_by_query
 
 from .api.device_data import get_data_by_pkey
 from .api import analysis, cell, device, device_data, project
 
-__version__ = "0.4.9"
+__version__ = "0.5.0"
 
 # ruff: noqa: D101
 __all__ = [
     "Analysis",
     "AnalysisFunction",
     "AnalysisFunctionTargetModel",
     "Cell",
```

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/fsr.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/fsr.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/iv_resistance.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/iv_resistance.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/device_data/power_envelope.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/device_data/power_envelope.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/aggregate.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/aggregate.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/cutback.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/cutback.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/iv_sheet_resistance.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/iv_sheet_resistance.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/die/loss_cutback.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/die/loss_cutback.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data_id.py` & `dodata-0.5.0/src/doplaydo/dodata/analysis_functions/wafer/aggregate_device_data_id.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/analysis.py` & `dodata-0.5.0/src/doplaydo/dodata/api/analysis.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/analysis_functions.py` & `dodata-0.5.0/src/doplaydo/dodata/api/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/cell.py` & `dodata-0.5.0/src/doplaydo/dodata/api/cell.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/device.py` & `dodata-0.5.0/src/doplaydo/dodata/api/device.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/device_data.py` & `dodata-0.5.0/src/doplaydo/dodata/api/device_data.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/die.py` & `dodata-0.5.0/src/doplaydo/dodata/api/die.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/project.py` & `dodata-0.5.0/src/doplaydo/dodata/api/project.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/api/wafer.py` & `dodata-0.5.0/src/doplaydo/dodata/api/wafer.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/config.py` & `dodata-0.5.0/src/doplaydo/dodata/config.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/db/analysis.py` & `dodata-0.5.0/src/doplaydo/dodata/db/analysis.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/db/common.py` & `dodata-0.5.0/src/doplaydo/dodata/db/common.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/db/device_data.py` & `dodata-0.5.0/src/doplaydo/dodata/db/device_data.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/db/die.py` & `dodata-0.5.0/src/doplaydo/dodata/db/die.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/src/doplaydo/dodata/db/wafer.py` & `dodata-0.5.0/src/doplaydo/dodata/db/wafer.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,20 +26,24 @@
     session = get_session()
     statement = _get_wafer_joined_query()
 
     for clause in clauses:
         statement = statement.where(clause)
 
     _wafers = session.exec(statement).all()
-
     return _wafers
 
 
 def get_by_id(project_id: str, wafer_id: str) -> Sequence[m.Wafer]:
-    """Get a wafer by project name and wafer name."""
+    """Get a wafer by project name and wafer name.
+
+    Args:
+        project_id: The project name.
+        wafer_id: The wafer name.
+    """
     return get_wafers_by_query(
         [m.Project.project_id == project_id, m.Wafer.wafer_id == wafer_id]
     )
 
 
 def get_by_pkey(wafer_pkey: int) -> m.Wafer:
     """Get a wafer by its unique pkey."""
@@ -50,20 +54,25 @@
 
     return _wafers[0]
 
 
 def get_wafer_dies(
     wafer_id: str, project_id: str, clauses: list[ColumnElement[bool] | bool]
 ) -> Sequence[m.Die]:
-    """Return a list of filtered wafer dies."""
+    """Return a list of filtered wafer dies.
+
+    Args:
+        wafer_id: The wafer name.
+        project_id: The project name.
+        clauses: A list of sqlalchemy clauses to filter the dies.
+    """
     session = get_session()
     statement = _get_die_joined_query()
 
     clauses.append(m.Project.project_id == project_id)
     clauses.append(m.Wafer.wafer_id == wafer_id)
 
     for clause in clauses:
         statement = statement.where(clause)
 
     _dies = session.exec(statement).all()
-
     return _dies
```

### Comparing `dodata-0.4.9/src/doplaydo/dodata/engine.py` & `dodata-0.5.0/src/doplaydo/dodata/engine.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_analysis_device_data.py` & `dodata-0.5.0/tests/test_analysis_device_data.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_analysis_die.py` & `dodata-0.5.0/tests/test_analysis_die.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_analysis_die_multi.py` & `dodata-0.5.0/tests/test_analysis_die_multi.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_analysis_wafer.py` & `dodata-0.5.0/tests/test_analysis_wafer.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_devicedata.py` & `dodata-0.5.0/tests/test_devicedata.py`

 * *Files identical despite different names*

### Comparing `dodata-0.4.9/tests/test_upload.py` & `dodata-0.5.0/tests/test_upload.py`

 * *Files identical despite different names*


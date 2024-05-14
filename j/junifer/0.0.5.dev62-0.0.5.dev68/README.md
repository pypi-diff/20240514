# Comparing `tmp/junifer-0.0.5.dev62.tar.gz` & `tmp/junifer-0.0.5.dev68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.5.dev62.tar", last modified: Tue May 14 11:06:13 2024, max compression
+gzip compressed data, was "junifer-0.0.5.dev68.tar", last modified: Tue May 14 13:17:02 2024, max compression
```

## Comparing `junifer-0.0.5.dev62.tar` & `junifer-0.0.5.dev68.tar`

### file list

```diff
@@ -1,457 +1,464 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.178114 junifer-0.0.5.dev62/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.114115 junifer-0.0.5.dev62/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 11:06:13.178114 junifer-0.0.5.dev62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.106115 junifer-0.0.5.dev62/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.118115 junifer-0.0.5.dev62/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.122115 junifer-0.0.5.dev62/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.122115 junifer-0.0.5.dev62/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.122115 junifer-0.0.5.dev62/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/115.doc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/161.feature
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/273.feature
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/323.feature
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/324.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/330.doc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/331.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/332.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/336.removal
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/339.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/changes/newsfragments/340.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/extending/preprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.126115 junifer-0.0.5.dev62/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.130115 junifer-0.0.5.dev62/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/yamls/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.130115 junifer-0.0.5.dev62/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 11:06:12.000000 junifer-0.0.5.dev62/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.130115 junifer-0.0.5.dev62/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.130115 junifer-0.0.5.dev62/junifer/api/queue_context/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/htcondor_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/queue_context_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.130115 junifer-0.0.5.dev62/junifer/api/queue_context/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/queue_context/tests/test_htcondor_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/afni/run_afni_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/res/ants/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/ants/ResampleImage
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/ants/antsApplyTransforms
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/ants/antsApplyTransformsToPoints
--rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/ants/run_ants_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/res/fsl/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/fsl/applywarp
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/fsl/flirt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/fsl/img2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/fsl/run_fsl_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/fsl/std2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/run_conda.bash
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/run_conda.zsh
--rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/run_venv.bash
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/res/run_venv.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.134115 junifer-0.0.5.dev62/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.138115 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.138115 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.138115 junifer-0.0.5.dev62/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.106115 junifer-0.0.5.dev62/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.142114 junifer-0.0.5.dev62/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.106115 junifer-0.0.5.dev62/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.142114 junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    65345 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/template_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.142114 junifer-0.0.5.dev62/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/tests/test_template_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/dmcc13_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_dmcc13_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.146114 junifer-0.0.5.dev62/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.110115 junifer-0.0.5.dev62/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 11:06:09.000000 junifer-0.0.5.dev62/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-14 11:06:09.000000 junifer-0.0.5.dev62/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 11:06:09.000000 junifer-0.0.5.dev62/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 11:06:09.000000 junifer-0.0.5.dev62/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-14 11:06:09.000000 junifer-0.0.5.dev62/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.150115 junifer-0.0.5.dev62/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.154115 junifer-0.0.5.dev62/junifer/markers/complexity/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/sample_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.154115 junifer-0.0.5.dev62/junifer/markers/complexity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_sample_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/complexity/weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.154115 junifer-0.0.5.dev62/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/_afni_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/_junifer_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.154115 junifer-0.0.5.dev62/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.158115 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.158115 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.158115 junifer-0.0.5.dev62/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/_afni_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/_junifer_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.158115 junifer-0.0.5.dev62/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.158115 junifer-0.0.5.dev62/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.162114 junifer-0.0.5.dev62/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/_afni_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/_fsl_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/_nilearn_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/smoothing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/smoothing/tests/test_smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/tests/test_preprocess_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/warping/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/warping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/warping/_ants_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/warping/_fsl_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/warping/space_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.166114 junifer-0.0.5.dev62/junifer/preprocess/warping/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/preprocess/warping/tests/test_space_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.170114 junifer-0.0.5.dev62/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.174114 junifer-0.0.5.dev62/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.174114 junifer-0.0.5.dev62/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.174114 junifer-0.0.5.dev62/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 11:06:13.000000 junifer-0.0.5.dev62/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:06:13.178114 junifer-0.0.5.dev62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:06:13.174114 junifer-0.0.5.dev62/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_dmcc13_benchmark_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-14 11:06:08.000000 junifer-0.0.5.dev62/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.203605 junifer-0.0.5.dev68/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.143605 junifer-0.0.5.dev68/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.143605 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.147606 junifer-0.0.5.dev68/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 13:17:02.199605 junifer-0.0.5.dev68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.147606 junifer-0.0.5.dev68/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.131605 junifer-0.0.5.dev68/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.147606 junifer-0.0.5.dev68/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.147606 junifer-0.0.5.dev68/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.147606 junifer-0.0.5.dev68/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.151605 junifer-0.0.5.dev68/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.151605 junifer-0.0.5.dev68/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.151605 junifer-0.0.5.dev68/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/115.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/161.feature
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/273.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/323.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/324.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/330.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/331.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/332.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/336.removal
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/339.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/340.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/changes/newsfragments/342.misc
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.155605 junifer-0.0.5.dev68/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/extending/preprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.155605 junifer-0.0.5.dev68/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.155605 junifer-0.0.5.dev68/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.155605 junifer-0.0.5.dev68/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.155605 junifer-0.0.5.dev68/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.159605 junifer-0.0.5.dev68/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.159605 junifer-0.0.5.dev68/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/yamls/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.159605 junifer-0.0.5.dev68/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.159605 junifer-0.0.5.dev68/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16142 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.159605 junifer-0.0.5.dev68/junifer/api/queue_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/htcondor_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/queue_context_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/queue_context/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/queue_context/tests/test_htcondor_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/afni/run_afni_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/res/ants/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/ants/ResampleImage
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/ants/antsApplyTransforms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/ants/antsApplyTransformsToPoints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/ants/run_ants_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/res/freesurfer/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/freesurfer/mri_binarize
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/freesurfer/mri_mc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/freesurfer/mri_pretess
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/freesurfer/mris_convert
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/freesurfer/run_freesurfer_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.163605 junifer-0.0.5.dev68/junifer/api/res/fsl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/fsl/applywarp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/fsl/flirt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/fsl/img2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/fsl/run_fsl_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/fsl/std2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/run_conda.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/run_conda.zsh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/run_venv.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/res/run_venv.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.167605 junifer-0.0.5.dev68/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.135605 junifer-0.0.5.dev68/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.171605 junifer-0.0.5.dev68/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.135605 junifer-0.0.5.dev68/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.171605 junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65345 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/template_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.171605 junifer-0.0.5.dev68/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/tests/test_template_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/dmcc13_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_dmcc13_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.175605 junifer-0.0.5.dev68/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.135605 junifer-0.0.5.dev68/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 13:16:58.000000 junifer-0.0.5.dev68/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-14 13:16:58.000000 junifer-0.0.5.dev68/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 13:16:58.000000 junifer-0.0.5.dev68/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 13:16:58.000000 junifer-0.0.5.dev68/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-14 13:16:58.000000 junifer-0.0.5.dev68/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.179605 junifer-0.0.5.dev68/junifer/markers/complexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/sample_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.183605 junifer-0.0.5.dev68/junifer/markers/complexity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_sample_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/complexity/weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.183605 junifer-0.0.5.dev68/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/_afni_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/_junifer_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.183605 junifer-0.0.5.dev68/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.183605 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/_afni_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/_junifer_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.187605 junifer-0.0.5.dev68/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/_afni_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/_fsl_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/_nilearn_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/smoothing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/smoothing/tests/test_smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/tests/test_preprocess_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/warping/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/warping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/warping/_ants_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/warping/_fsl_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/warping/space_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.191605 junifer-0.0.5.dev68/junifer/preprocess/warping/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/preprocess/warping/tests/test_space_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.195605 junifer-0.0.5.dev68/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.199605 junifer-0.0.5.dev68/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.199605 junifer-0.0.5.dev68/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.199605 junifer-0.0.5.dev68/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 13:17:02.000000 junifer-0.0.5.dev68/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:17:02.203605 junifer-0.0.5.dev68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:02.199605 junifer-0.0.5.dev68/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_dmcc13_benchmark_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-14 13:16:57.000000 junifer-0.0.5.dev68/tox.ini
```

### Comparing `junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.5.dev68/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/ci-docs.yml` & `junifer-0.0.5.dev68/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/ci.yml` & `junifer-0.0.5.dev68/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/docs-preview.yml` & `junifer-0.0.5.dev68/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/docs.yml` & `junifer-0.0.5.dev68/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/lint.yml` & `junifer-0.0.5.dev68/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.github/workflows/pypi.yml` & `junifer-0.0.5.dev68/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.gitignore` & `junifer-0.0.5.dev68/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/.pre-commit-config.yaml` & `junifer-0.0.5.dev68/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/LICENSE.md` & `junifer-0.0.5.dev68/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/PKG-INFO` & `junifer-0.0.5.dev68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev62
+Version: 0.0.5.dev68
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev62/README.md` & `junifer-0.0.5.dev68/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/codecov.yml` & `junifer-0.0.5.dev68/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/conda-env.yml` & `junifer-0.0.5.dev68/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/Makefile` & `junifer-0.0.5.dev68/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/_static/css/custom.css` & `junifer-0.0.5.dev68/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/_templates/versions.html` & `junifer-0.0.5.dev68/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/builtin.rst` & `junifer-0.0.5.dev68/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/changes/contributors.inc` & `junifer-0.0.5.dev68/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/conf.py` & `junifer-0.0.5.dev68/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/contribution.rst` & `junifer-0.0.5.dev68/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/coordinates.rst` & `junifer-0.0.5.dev68/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/datagrabber.rst` & `junifer-0.0.5.dev68/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/dependencies.rst` & `junifer-0.0.5.dev68/docs/extending/dependencies.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/extension.rst` & `junifer-0.0.5.dev68/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/index.rst` & `junifer-0.0.5.dev68/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/marker.rst` & `junifer-0.0.5.dev68/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/masks.rst` & `junifer-0.0.5.dev68/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/parcellations.rst` & `junifer-0.0.5.dev68/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/extending/preprocessor.rst` & `junifer-0.0.5.dev68/docs/extending/preprocessor.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/faq.rst` & `junifer-0.0.5.dev68/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/help.rst` & `junifer-0.0.5.dev68/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/images/junifer_logo.png` & `junifer-0.0.5.dev68/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/index.rst` & `junifer-0.0.5.dev68/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/installation.rst` & `junifer-0.0.5.dev68/docs/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -159,7 +159,40 @@
 
 Or, alternatively, you can execute this command which will update the
 ``~/.bashrc`` for you:
 
 .. code-block:: bash
 
   junifer setup ants-docker | grep "PATH=" | xargs | >> ~/.bashrc
+
+FreeSurfer
+----------
+
+To install FreeSurfer, you can always follow the `FreeSurfer official instructions
+<https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall>`_. Additionally, you can
+also follow the following steps to install and configure the FreeSurfer Docker container
+in your local system.
+
+1. Install Docker. You can follow the
+   `Docker official instructions <https://docs.docker.com/get-docker/>`_.
+2. Pull the FreeSurfer Docker image from
+   `Docker Hub FreeSurfer <https://hub.docker.com/r/freesurfer/freesurfer>`_:
+
+.. code-block:: bash
+
+  docker pull freesurfer/freesurfer
+
+3. Add the Junifer FreeSurfer scripts to your PATH environment variable. Run the
+   following command:
+
+.. code-block:: bash
+
+  junifer setup freesurfer-docker
+
+Take the last line and copy it to your ``.bashrc`` or ``.zshrc`` file.
+
+Or, alternatively, you can execute this command which will update the
+``~/.bashrc`` for you:
+
+.. code-block:: bash
+
+  junifer setup freesurfer-docker | grep "PATH=" | xargs | >> ~/.bashrc
```

### Comparing `junifer-0.0.5.dev62/docs/links.inc` & `junifer-0.0.5.dev68/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/maintaining.rst` & `junifer-0.0.5.dev68/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.5.dev68/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/starting.rst` & `junifer-0.0.5.dev68/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/data.rst` & `junifer-0.0.5.dev68/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/datagrabber.rst` & `junifer-0.0.5.dev68/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/datareader.rst` & `junifer-0.0.5.dev68/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/index.rst` & `junifer-0.0.5.dev68/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/marker.rst` & `junifer-0.0.5.dev68/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/pipeline.rst` & `junifer-0.0.5.dev68/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/preprocess.rst` & `junifer-0.0.5.dev68/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/understanding/storage.rst` & `junifer-0.0.5.dev68/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/using/codeless.rst` & `junifer-0.0.5.dev68/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/using/index.rst` & `junifer-0.0.5.dev68/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/using/masks.rst` & `junifer-0.0.5.dev68/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/using/queueing.rst` & `junifer-0.0.5.dev68/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/using/running.rst` & `junifer-0.0.5.dev68/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/docs/whats_new.rst` & `junifer-0.0.5.dev68/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/norun_hcpfc_pearson.py` & `junifer-0.0.5.dev68/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/norun_ukbvm_gmd.py` & `junifer-0.0.5.dev68/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/run_compute_parcel_mean.py` & `junifer-0.0.5.dev68/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.5.dev68/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/run_ets_rss_marker.py` & `junifer-0.0.5.dev68/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/run_junifer_julearn.py` & `junifer-0.0.5.dev68/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/run_run_gmd_mean.py` & `junifer-0.0.5.dev68/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/yamls/gmd_mean.yaml` & `junifer-0.0.5.dev68/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.5.dev68/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/cli.py` & `junifer-0.0.5.dev68/junifer/api/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -584,7 +584,33 @@
         docker pull antsx/ants
 
     3. Add this line to the ~/.bashrc or ~/.zshrc file:
 
     export PATH="$PATH:{ants_wrappers_path}"
     """
     click.secho(msg, fg="blue")
+
+
+@setup.command("freesurfer-docker")
+def freesurfer_docker() -> None:  # pragma: no cover
+    """Configure FreeSurfer-Docker wrappers."""
+    import junifer
+
+    pkg_path = Path(junifer.__path__[0])  # type: ignore
+    fs_wrappers_path = pkg_path / "api" / "res" / "freesurfer"
+    msg = f"""
+    Installation instructions for FreeSurfer-Docker wrappers:
+
+    1. Install Docker: https://docs.docker.com/get-docker/
+
+    2. Get the FreeSurfer-Docker image by running this on the command line:
+
+        docker pull freesurfer/freesurfer
+
+    3. Get license from: https://surfer.nmr.mgh.harvard.edu/registration.html .
+       You can skip this step if you already have one.
+
+    4. Add this line to the ~/.bashrc or ~/.zshrc file:
+
+    export PATH="$PATH:{fs_wrappers_path}"
+    """
+    click.secho(msg, fg="blue")
```

### Comparing `junifer-0.0.5.dev62/junifer/api/decorators.py` & `junifer-0.0.5.dev68/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/functions.py` & `junifer-0.0.5.dev68/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/parser.py` & `junifer-0.0.5.dev68/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/queue_context/gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev68/junifer/api/queue_context/gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/queue_context/htcondor_adapter.py` & `junifer-0.0.5.dev68/junifer/api/queue_context/htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/queue_context/queue_context_adapter.py` & `junifer-0.0.5.dev68/junifer/api/queue_context/queue_context_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev68/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/queue_context/tests/test_htcondor_adapter.py` & `junifer-0.0.5.dev68/junifer/api/queue_context/tests/test_htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.5.dev68/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/res/ants/run_ants_docker.sh` & `junifer-0.0.5.dev68/junifer/api/res/ants/run_ants_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/res/fsl/run_fsl_docker.sh` & `junifer-0.0.5.dev68/junifer/api/res/fsl/run_fsl_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/res/run_conda.bash` & `junifer-0.0.5.dev68/junifer/api/res/run_conda.bash`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/res/run_conda.zsh` & `junifer-0.0.5.dev68/junifer/api/res/run_conda.zsh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/tests/test_api_utils.py` & `junifer-0.0.5.dev68/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/tests/test_cli.py` & `junifer-0.0.5.dev68/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/tests/test_functions.py` & `junifer-0.0.5.dev68/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/tests/test_parser.py` & `junifer-0.0.5.dev68/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/api/utils.py` & `junifer-0.0.5.dev68/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.5.dev68/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.5.dev68/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/__init__.py` & `junifer-0.0.5.dev68/junifer/data/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/coordinates.py` & `junifer-0.0.5.dev68/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.5.dev68/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/masks.py` & `junifer-0.0.5.dev68/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/parcellations.py` & `junifer-0.0.5.dev68/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/template_spaces.py` & `junifer-0.0.5.dev68/junifer/data/template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/tests/test_coordinates.py` & `junifer-0.0.5.dev68/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/tests/test_data_utils.py` & `junifer-0.0.5.dev68/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/tests/test_masks.py` & `junifer-0.0.5.dev68/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/tests/test_parcellations.py` & `junifer-0.0.5.dev68/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/tests/test_template_spaces.py` & `junifer-0.0.5.dev68/junifer/data/tests/test_template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/data/utils.py` & `junifer-0.0.5.dev68/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/__init__.py` & `junifer-0.0.5.dev68/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.5.dev68/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/base.py` & `junifer-0.0.5.dev68/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/datalad_base.py` & `junifer-0.0.5.dev68/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/dmcc13_benchmark.py` & `junifer-0.0.5.dev68/junifer/datagrabber/dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.5.dev68/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/multiple.py` & `junifer-0.0.5.dev68/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/pattern.py` & `junifer-0.0.5.dev68/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.5.dev68/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_dmcc13_benchmark.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.5.dev68/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datagrabber/utils.py` & `junifer-0.0.5.dev68/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datareader/default.py` & `junifer-0.0.5.dev68/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.5.dev68/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.5.dev68/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.5.dev68/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.5.dev68/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev68/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev68/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/__init__.py` & `junifer-0.0.5.dev68/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/base.py` & `junifer-0.0.5.dev68/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/collection.py` & `junifer-0.0.5.dev68/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/__init__.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/complexity_base.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/complexity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/hurst_exponent.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/multiscale_entropy_auc.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/perm_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/range_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/range_entropy_auc.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/sample_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_hurst_exponent.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_perm_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_range_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_range_entropy_auc.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_sample_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/tests/test_weighted_perm_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/tests/test_weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/complexity/weighted_perm_entropy.py` & `junifer-0.0.5.dev68/junifer/markers/complexity/weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/ets_rss.py` & `junifer-0.0.5.dev68/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/_afni_falff.py` & `junifer-0.0.5.dev68/junifer/markers/falff/_afni_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/_junifer_falff.py` & `junifer-0.0.5.dev68/junifer/markers/falff/_junifer_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/falff_base.py` & `junifer-0.0.5.dev68/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/parcel_aggregation.py` & `junifer-0.0.5.dev68/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/_afni_reho.py` & `junifer-0.0.5.dev68/junifer/markers/reho/_afni_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/_junifer_reho.py` & `junifer-0.0.5.dev68/junifer/markers/reho/_junifer_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/reho_base.py` & `junifer-0.0.5.dev68/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/sphere_aggregation.py` & `junifer-0.0.5.dev68/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.5.dev68/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_collection.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.5.dev68/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/markers/utils.py` & `junifer-0.0.5.dev68/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/onthefly/read_transform.py` & `junifer-0.0.5.dev68/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.5.dev68/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.5.dev68/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/registry.py` & `junifer-0.0.5.dev68/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/singleton.py` & `junifer-0.0.5.dev68/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.5.dev68/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.5.dev68/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.5.dev68/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.5.dev68/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.5.dev68/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/utils.py` & `junifer-0.0.5.dev68/junifer/pipeline/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,29 +33,32 @@
     ------
     ValueError
         If ``name`` is invalid.
     RuntimeError
         If ``name`` is mandatory and is not found.
 
     """
-    valid_ext_dependencies = ("afni", "fsl", "ants")
+    valid_ext_dependencies = ("afni", "fsl", "ants", "freesurfer")
     if name not in valid_ext_dependencies:
         raise_error(
             "Invalid value for `name`, should be one of: "
             f"{valid_ext_dependencies}"
         )
     # Check for afni
     if name == "afni":
         found = _check_afni(**kwargs)
     # Check for fsl
     elif name == "fsl":
         found = _check_fsl(**kwargs)
     # Check for ants
     elif name == "ants":
         found = _check_ants(**kwargs)
+    # Check for freesurfer
+    elif name == "freesurfer":
+        found = _check_freesurfer(**kwargs)
 
     # Check if the dependency is mandatory in case it's not found
     if not found and not optional:
         raise_error(
             msg=(
                 f"{name} is not installed but is "
                 "required by one of the pipeline steps"
@@ -241,7 +244,67 @@
         if not all_commands_found:
             warn_with_log(
                 "ANTs is installed but some of the required commands "
                 "were not found. These are the results: "
                 f"{commands_found_results}"
             )
     return ants_found
+
+
+def _check_freesurfer(commands: Optional[List[str]] = None) -> bool:
+    """Check if FreeSurfer is present in the system.
+
+    Parameters
+    ----------
+    commands : list of str, optional
+        The commands to specifically check for from FreeSurfer. If None, only
+        the basic FreeSurfer help would be looked up, else, would also
+        check for specific commands (default None).
+
+    Returns
+    -------
+    bool
+        Whether FreeSurfer is found or not.
+
+    """
+    completed_process = subprocess.run(
+        "recon-all -help",
+        stdin=subprocess.DEVNULL,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.STDOUT,
+        shell=True,  # is unsafe but kept for resolution via PATH
+        check=False,
+    )
+    fs_found = completed_process.returncode == 0
+
+    # Check for specific commands
+    if fs_found and commands is not None:
+        if not isinstance(commands, list):
+            commands = [commands]
+        # Store command found results
+        commands_found_results = {}
+        # Set all commands found flag to True
+        all_commands_found = True
+        # Check commands' existence
+        for command in commands:
+            command_process = subprocess.run(
+                [command],
+                stdin=subprocess.DEVNULL,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.STDOUT,
+                shell=True,  # is unsafe but kept for resolution via PATH
+                check=False,
+            )
+            command_found = command_process.returncode == 0
+            commands_found_results[command] = (
+                "found" if command_found else "not found"
+            )
+            # Set flag to trigger warning
+            all_commands_found = all_commands_found and command_found
+        # One or more commands were missing
+        if not all_commands_found:
+            warn_with_log(
+                "FreeSurfer is installed but some of the required commands "
+                "were not found. These are the results: "
+                f"{commands_found_results}"
+            )
+    return fs_found
```

### Comparing `junifer-0.0.5.dev62/junifer/pipeline/workdir_manager.py` & `junifer-0.0.5.dev68/junifer/pipeline/workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/base.py` & `junifer-0.0.5.dev68/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.5.dev68/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.5.dev68/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/smoothing/_afni_smoothing.py` & `junifer-0.0.5.dev68/junifer/preprocess/smoothing/_afni_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/smoothing/_fsl_smoothing.py` & `junifer-0.0.5.dev68/junifer/preprocess/smoothing/_fsl_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/smoothing/_nilearn_smoothing.py` & `junifer-0.0.5.dev68/junifer/preprocess/smoothing/_nilearn_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/smoothing/smoothing.py` & `junifer-0.0.5.dev68/junifer/preprocess/smoothing/smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/smoothing/tests/test_smoothing.py` & `junifer-0.0.5.dev68/junifer/preprocess/smoothing/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.5.dev68/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/warping/_ants_warper.py` & `junifer-0.0.5.dev68/junifer/preprocess/warping/_ants_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/warping/_fsl_warper.py` & `junifer-0.0.5.dev68/junifer/preprocess/warping/_fsl_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/warping/space_warper.py` & `junifer-0.0.5.dev68/junifer/preprocess/warping/space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/preprocess/warping/tests/test_space_warper.py` & `junifer-0.0.5.dev68/junifer/preprocess/warping/tests/test_space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/stats.py` & `junifer-0.0.5.dev68/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/base.py` & `junifer-0.0.5.dev68/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/hdf5.py` & `junifer-0.0.5.dev68/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/pandas_base.py` & `junifer-0.0.5.dev68/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/sqlite.py` & `junifer-0.0.5.dev68/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.5.dev68/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.5.dev68/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.5.dev68/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.5.dev68/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/tests/test_utils.py` & `junifer-0.0.5.dev68/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/storage/utils.py` & `junifer-0.0.5.dev68/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.5.dev68/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/datagrabbers.py` & `junifer-0.0.5.dev68/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/registry.py` & `junifer-0.0.5.dev68/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.5.dev68/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.5.dev68/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.5.dev68/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.5.dev68/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/testing/utils.py` & `junifer-0.0.5.dev68/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/tests/test_stats.py` & `junifer-0.0.5.dev68/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/utils/helpers.py` & `junifer-0.0.5.dev68/junifer/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/utils/logging.py` & `junifer-0.0.5.dev68/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/utils/tests/test_fs.py` & `junifer-0.0.5.dev68/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/utils/tests/test_helpers.py` & `junifer-0.0.5.dev68/junifer/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer/utils/tests/test_logging.py` & `junifer-0.0.5.dev68/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/junifer.egg-info/PKG-INFO` & `junifer-0.0.5.dev68/junifer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev62
+Version: 0.0.5.dev68
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev62/junifer.egg-info/SOURCES.txt` & `junifer-0.0.5.dev68/junifer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 docs/changes/newsfragments/324.bugfix
 docs/changes/newsfragments/330.doc
 docs/changes/newsfragments/331.bugfix
 docs/changes/newsfragments/332.bugfix
 docs/changes/newsfragments/336.removal
 docs/changes/newsfragments/339.bugfix
 docs/changes/newsfragments/340.bugfix
+docs/changes/newsfragments/342.misc
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/dependencies.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
@@ -134,14 +135,19 @@
 junifer/api/res/afni/3dReHo
 junifer/api/res/afni/afni
 junifer/api/res/afni/run_afni_docker.sh
 junifer/api/res/ants/ResampleImage
 junifer/api/res/ants/antsApplyTransforms
 junifer/api/res/ants/antsApplyTransformsToPoints
 junifer/api/res/ants/run_ants_docker.sh
+junifer/api/res/freesurfer/mri_binarize
+junifer/api/res/freesurfer/mri_mc
+junifer/api/res/freesurfer/mri_pretess
+junifer/api/res/freesurfer/mris_convert
+junifer/api/res/freesurfer/run_freesurfer_docker.sh
 junifer/api/res/fsl/applywarp
 junifer/api/res/fsl/flirt
 junifer/api/res/fsl/img2imgcoord
 junifer/api/res/fsl/run_fsl_docker.sh
 junifer/api/res/fsl/std2imgcoord
 junifer/api/tests/test_api_utils.py
 junifer/api/tests/test_cli.py
```

### Comparing `junifer-0.0.5.dev62/junifer.egg-info/requires.txt` & `junifer-0.0.5.dev68/junifer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/pyproject.toml` & `junifer-0.0.5.dev68/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_bids_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.5.dev68/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_dmcc13_benchmark_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_dmcc13_benchmark_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.5.dev68/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev62/tox.ini` & `junifer-0.0.5.dev68/tox.ini`

 * *Files identical despite different names*


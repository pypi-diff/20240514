# Comparing `tmp/cdflib-1.3.0.tar.gz` & `tmp/cdflib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.3.0.tar", last modified: Fri May 10 22:42:45 2024, max compression
+gzip compressed data, was "cdflib-1.3.1.tar", last modified: Tue May 14 19:35:04 2024, max compression
```

## Comparing `cdflib-1.3.0.tar` & `cdflib-1.3.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.333941 cdflib-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.325941 cdflib-1.3.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-10 22:42:36.000000 cdflib-1.3.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.325941 cdflib-1.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-10 22:42:36.000000 cdflib-1.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 22:42:36.000000 cdflib-1.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 22:42:36.000000 cdflib-1.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.321941 cdflib-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.325941 cdflib-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 22:42:36.000000 cdflib-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-10 22:42:36.000000 cdflib-1.3.0/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-10 22:42:36.000000 cdflib-1.3.0/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 22:42:36.000000 cdflib-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-10 22:42:36.000000 cdflib-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 22:42:36.000000 cdflib-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 22:42:36.000000 cdflib-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 22:42:36.000000 cdflib-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-10 22:42:45.333941 cdflib-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 22:42:36.000000 cdflib-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.325941 cdflib-1.3.0/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 22:42:36.000000 cdflib-1.3.0/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-10 22:42:36.000000 cdflib-1.3.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.325941 cdflib-1.3.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:36.000000 cdflib-1.3.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 22:42:36.000000 cdflib-1.3.0/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.329941 cdflib-1.3.0/cdflib/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/_gzip_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    84441 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (127)   106363 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    70305 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.329941 cdflib-1.3.0/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39388 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    49368 2024-05-10 22:42:36.000000 cdflib-1.3.0/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.333941 cdflib-1.3.0/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 22:42:45.000000 cdflib-1.3.0/cdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 22:42:36.000000 cdflib-1.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.329941 cdflib-1.3.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.329941 cdflib-1.3.0/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-10 22:42:36.000000 cdflib-1.3.0/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-10 22:42:36.000000 cdflib-1.3.0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 22:42:36.000000 cdflib-1.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 22:42:36.000000 cdflib-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 22:42:45.337941 cdflib-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.333941 cdflib-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9711 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19626 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:42:45.333941 cdflib-1.3.0/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (127)   125566 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    67164 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-05-10 22:42:36.000000 cdflib-1.3.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 22:42:36.000000 cdflib-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.381893 cdflib-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.369893 cdflib-1.3.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-14 19:34:55.000000 cdflib-1.3.1/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.369893 cdflib-1.3.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 19:34:55.000000 cdflib-1.3.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 19:34:55.000000 cdflib-1.3.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 19:34:55.000000 cdflib-1.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.365893 cdflib-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.369893 cdflib-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 19:34:55.000000 cdflib-1.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-14 19:34:55.000000 cdflib-1.3.1/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-14 19:34:55.000000 cdflib-1.3.1/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 19:34:55.000000 cdflib-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-14 19:34:55.000000 cdflib-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 19:34:55.000000 cdflib-1.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-14 19:34:55.000000 cdflib-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 19:34:55.000000 cdflib-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 19:35:04.381893 cdflib-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 19:34:55.000000 cdflib-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.373893 cdflib-1.3.1/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 19:34:55.000000 cdflib-1.3.1/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-14 19:34:55.000000 cdflib-1.3.1/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.373893 cdflib-1.3.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:34:55.000000 cdflib-1.3.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 19:34:55.000000 cdflib-1.3.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.373893 cdflib-1.3.1/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/_gzip_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84457 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106555 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70305 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.373893 cdflib-1.3.1/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39388 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50624 2024-05-14 19:34:55.000000 cdflib-1.3.1/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.377893 cdflib-1.3.1/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 19:35:04.000000 cdflib-1.3.1/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 19:34:55.000000 cdflib-1.3.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.377893 cdflib-1.3.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.377893 cdflib-1.3.1/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-14 19:34:55.000000 cdflib-1.3.1/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-14 19:34:55.000000 cdflib-1.3.1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 19:34:55.000000 cdflib-1.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 19:34:55.000000 cdflib-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-14 19:35:04.381893 cdflib-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.377893 cdflib-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18368 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9711 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19626 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:04.377893 cdflib-1.3.1/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)   125566 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    67164 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-05-14 19:34:55.000000 cdflib-1.3.1/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-14 19:34:55.000000 cdflib-1.3.1/tox.ini
```

### Comparing `cdflib-1.3.0/.circleci/config.yml` & `cdflib-1.3.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/.devcontainer/devcontainer.json` & `cdflib-1.3.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/.github/workflows/pypi-build.yaml` & `cdflib-1.3.1/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/.pre-commit-config.yaml` & `cdflib-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/.readthedocs.yml` & `cdflib-1.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/LICENSE` & `cdflib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/PKG-INFO` & `cdflib-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.3.0
+Version: 1.3.1
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.21
 Provides-Extra: tests
 Requires-Dist: astropy; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: pytest>=3.9; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: xarray; extra == "tests"
+Requires-Dist: h5netcdf; extra == "tests"
 Requires-Dist: netcdf4; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: astropy; extra == "docs"
 Requires-Dist: xarray; extra == "docs"
 Requires-Dist: netcdf4; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
```

### Comparing `cdflib-1.3.0/README.md` & `cdflib-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/asv.conf.json` & `cdflib-1.3.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/benchmarks/benchmarks.py` & `cdflib-1.3.1/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/CDFLeapSeconds.txt` & `cdflib-1.3.1/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/cdfread.py` & `cdflib-1.3.1/cdflib/cdfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1735,15 +1735,15 @@
         if squeeze_needed:
             ret = np.squeeze(ret, axis=(ret.ndim - 1))
             if dimensions is not None:
                 dimensions.pop()
 
         # Put the data into system byte order
         if self._convert_option() != "=":
-            ret = ret.byteswap().newbyteorder()
+            ret = ret.view(ret.dtype.newbyteorder()).byteswap()
 
         if self._majority == "Column_major":
             if dimensions is not None:
                 axes = [0] + list(range(len(dimensions), 0, -1))
             else:
                 axes = None
             ret = np.transpose(ret, axes=axes)
```

### Comparing `cdflib-1.3.0/cdflib/cdfwrite.py` & `cdflib-1.3.1/cdflib/cdfwrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -2281,15 +2281,14 @@
         Returns
         -------
         recs : int
             The number of records generated by converting indata
         odata : byte stream
             The stream of bytes to write to the CDF file
         """
-
         recSize = self._datatype_size(data_type, num_elems) * num_values
         # List or Tuple data
         if isinstance(indata, list) or isinstance(indata, tuple):
             if (num_values != 1) and (len(indata) != num_values):
                 raise Exception("Use numpy for inputting multidimensional arrays")
             size = len(indata)
             if data_type == self.CDF_CHAR or data_type == self.CDF_UCHAR:
@@ -2389,18 +2388,21 @@
                             complex_data.append(indata[x].real)
                             complex_data.append(indata[x].imag)
                     else:
                         complex_data.append(indata.real)
                         complex_data.append(indata.imag)
                     indata = complex_data
                 form = tofrom + str(recs * num_values * num_elems) + dt_string
-                if recs * num_values * num_elems > 1:
-                    return recs, struct.pack(form, *indata)
-                else:
-                    return recs, struct.pack(form, indata)
+                try:
+                    if recs * num_values * num_elems > 1:
+                        return recs, struct.pack(form, *indata)
+                    else:
+                        return recs, struct.pack(form, indata)
+                except struct.error:
+                    raise ValueError("Unable to convert data to CDF format, data " "object cannot be of type string.")
 
     def _num_values(self, zVar: bool, varNum: int) -> int:
         """
         Determines the number of values in a record.
         Set zVar=True if this is a zvariable.
         """
         values = 1
```

### Comparing `cdflib-1.3.0/cdflib/dataclasses.py` & `cdflib-1.3.1/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/epochs.py` & `cdflib-1.3.1/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/epochs_astropy.py` & `cdflib-1.3.1/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/s3.py` & `cdflib-1.3.1/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/utils.py` & `cdflib-1.3.1/cdflib/utils.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.3.1/cdflib/xarray/cdf_to_xarray.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.3.1/cdflib/xarray/xarray_to_cdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
     41: np.int8(-128),
     44: np.float32(-1e31),
     45: np.float64(-1e31),
     51: np.str_(" "),
     52: np.str_(" "),
 }
 
+# Regular expression to match valid ISTP variable/attribute names
+ISTP_COMPLIANT_NAME = re.compile(r"^[A-Za-z][A-Za-z0-9_]*$")
+
 
 class ISTPError(Exception):
     """
     Exception raised for ISTP Compliance Errors
     """
 
     def __init__(self, message: str = ""):
@@ -160,15 +163,15 @@
         cdf_data_type = "CDF_UINT1"
     elif numpy_data_type == np.uint16:
         cdf_data_type = "CDF_UINT2"
     elif numpy_data_type == np.uint32:
         cdf_data_type = "CDF_UINT4"
     elif numpy_data_type == np.uint64:
         cdf_data_type = "CDF_UINT8"
-    elif numpy_data_type == np.complex_:
+    elif numpy_data_type == np.complex128:
         cdf_data_type = "CDF_EPOCH16"
     elif numpy_data_type.type in (np.str_, np.bytes_):
         element_size = int(numpy_data_type.str[2:])  # The length of the longest string in the numpy array
     elif var.dtype == object:  # This commonly means we either have multidimensional arrays of strings or datetime objects
         if _is_datetime_array(var.data):
             cdf_data_type = "CDF_TIME_TT2000"
         else:
@@ -464,14 +467,40 @@
     return depend_0_list, time_varying_dimensions
 
 
 def _verify_monotonically_increasing(epoch_data: npt.NDArray) -> np.bool_:
     return np.all(epoch_data[1:] > epoch_data[:-1])
 
 
+def _validate_varatt_names(dataset: xr.Dataset, terminate_on_warning: bool) -> None:
+    for var_name in dataset.variables:
+        if not ISTP_COMPLIANT_NAME.match(str(var_name)):
+            _warn_or_except(
+                f"Invalid ISTP variable name: {str(var_name)}",
+                terminate_on_warning,
+            )
+
+    # Check attributes in the dataset
+    for attr_name in dataset.attrs:
+        if not ISTP_COMPLIANT_NAME.match(str(attr_name)):
+            _warn_or_except(
+                f"Invalid ISTP global attribute name: {str(attr_name)}",
+                terminate_on_warning,
+            )
+
+    # Check attributes of each variable
+    for var in dataset.variables:
+        for attr_name in dataset[var].attrs:
+            if not ISTP_COMPLIANT_NAME.match(str(attr_name)):
+                _warn_or_except(
+                    f"Invalid ISTP variable attribute name: {str(attr_name)}",
+                    terminate_on_warning,
+                )
+
+
 def _add_depend_variables_to_dataset(
     dataset: xr.Dataset,
     dim_vars: List[str],
     depend_0_vars: List[str],
     time_varying_dimensions: List[str],
     terminate_on_warning: bool = False,
     auto_fix_depends: bool = True,
@@ -988,14 +1017,17 @@
     # Make a deep copy of the data before continuing
     dataset = xarray_dataset.copy()
 
     if nan_to_fillval:
         _convert_nans_to_fillval(dataset)
 
     if istp:
+        # This checks all the variable and attribute names to ensure they are ISTP compliant.
+        _validate_varatt_names(dataset, terminate_on_warning)
+
         # This creates a list of suspected or confirmed label variables
         _label_checker(dataset, terminate_on_warning)
 
         # This creates a list of suspected or confirmed dimension variables
         dim_vars = _dimension_checker(dataset, terminate_on_warning)
 
         # This creates a list of suspected or confirmed record variables
```

### Comparing `cdflib-1.3.0/cdflib.egg-info/PKG-INFO` & `cdflib-1.3.1/cdflib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.3.0
+Version: 1.3.1
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.21
 Provides-Extra: tests
 Requires-Dist: astropy; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: pytest>=3.9; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: xarray; extra == "tests"
+Requires-Dist: h5netcdf; extra == "tests"
 Requires-Dist: netcdf4; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: astropy; extra == "docs"
 Requires-Dist: xarray; extra == "docs"
 Requires-Dist: netcdf4; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
```

### Comparing `cdflib-1.3.0/cdflib.egg-info/SOURCES.txt` & `cdflib-1.3.1/cdflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/Makefile` & `cdflib-1.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/changelog.rst` & `cdflib-1.3.1/doc/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 =========
 Changelog
 =========
 
+1.3.1
+=====
+General Updates
+---------------
+- Added tox to serve as the unit testing infrastructure, and changed which unit tests were run (see the github actions to see what exactly is running)
+- Added tests to check future versions of numpy and astropy
+- Added back in the remote data unit tests
+
+xarray_to_cdf
+-------------
+- Added an ISTP check to determine is attribute and variable names are compliant
+
+cdfwrite
+---------
+- Clearer error message surrounding data type conversions to CDF data types
+
 1.3.0
 =====
 General Updates
 ---------------
 - Added .devcontainer to support development of cdflib on github
 - Renamed the master branch to "main"
 - Added netcdf4 to the test dependencies
```

### Comparing `cdflib-1.3.0/doc/conf.py` & `cdflib-1.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/index.rst` & `cdflib-1.3.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/make.bat` & `cdflib-1.3.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/modules/cdfepoch.rst` & `cdflib-1.3.1/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/modules/cdfread.rst` & `cdflib-1.3.1/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/doc/modules/cdfwrite.rst` & `cdflib-1.3.1/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/meta.yaml` & `cdflib-1.3.1/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 {% set name = "cdflib" %}
-{% set version = "1.3.0" %}
+{% set version = "1.3.1" %}
 
 package:
   name: "{{ name|lower }}"
   version: "{{ version }}"
 
 source:
   git_url: https://github.com/MAVENSDC/cdflib.git
   git_depth: 20
-  git_rev: 1.3.0
+  git_rev: 1.3.1
 
 build:
   number: 0
   script: "{{ PYTHON }} -m pip install . -vv"
 
 requirements:
   build:
```

### Comparing `cdflib-1.3.0/mypy.ini` & `cdflib-1.3.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/setup.cfg` & `cdflib-1.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -11,39 +11,41 @@
 	PDS
 	GSFC
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Utilities
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
-python_requires = >= 3.6
+python_requires = >= 3.8
 include_package_data = True
 packages = find:
 install_requires = 
-	numpy
+	numpy >= 1.21
 
 [options.extras_require]
 tests = 
 	astropy
 	hypothesis
 	pytest >= 3.9
 	pytest-cov
 	pytest-remotedata
 	xarray
+	h5netcdf
 	netcdf4
 docs = 
 	astropy
 	xarray
 	netcdf4
 	sphinx
 	sphinx-automodapi
```

### Comparing `cdflib-1.3.0/tests/test_astropy_epochs.py` & `cdflib-1.3.1/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/test_cdfread.py` & `cdflib-1.3.1/tests/test_cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/test_cdfwrite.py` & `cdflib-1.3.1/tests/test_cdfwrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Any, Dict
 
 import numpy as np
+import pytest
 
 from cdflib import cdfread, cdfwrite
 
 R = Path(__file__).parent
 fnbasic = "testing.cdf"
 
 
@@ -626,7 +627,15 @@
 
     # Open the file to read
     reader = cdf_read(fn)
 
     # Test CDF info
     var = reader.varget("Variable1")
     assert var[3] == 3
+
+
+def test_convert_data_error(tmp_path):
+    indata = int(-9223372036854775808)
+    cdf = cdfwrite.CDF(tmp_path / "test.cdf", cdf_spec={"rDim_sizes": [1]})
+    with pytest.raises(ValueError):
+        # Data from list of strings with dimension "epoch"
+        cdf._convert_data(51, 1, 1, indata)
```

### Comparing `cdflib-1.3.0/tests/test_epochs.py` & `cdflib-1.3.1/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/test_xarray_reader_writer.py` & `cdflib-1.3.1/tests/test_xarray_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf` & `cdflib-1.3.1/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.3.1/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.3.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.3.1/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*


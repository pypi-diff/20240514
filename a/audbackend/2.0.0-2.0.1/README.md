# Comparing `tmp/audbackend-2.0.0.tar.gz` & `tmp/audbackend-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audbackend-2.0.0.tar", last modified: Fri May 10 06:59:47 2024, max compression
+gzip compressed data, was "audbackend-2.0.1.tar", last modified: Tue May 14 10:50:55 2024, max compression
```

## Comparing `audbackend-2.0.0.tar` & `audbackend-2.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.059556 audbackend-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 06:59:40.000000 audbackend-2.0.0/.coveragerc.Linux
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-10 06:59:40.000000 audbackend-2.0.0/.coveragerc.Windows
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 06:59:40.000000 audbackend-2.0.0/.coveragerc.macOS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.047556 audbackend-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.047556 audbackend-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-10 06:59:40.000000 audbackend-2.0.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-10 06:59:40.000000 audbackend-2.0.0/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-10 06:59:40.000000 audbackend-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-10 06:59:40.000000 audbackend-2.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 06:59:40.000000 audbackend-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-10 06:59:40.000000 audbackend-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 06:59:40.000000 audbackend-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-10 06:59:40.000000 audbackend-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-10 06:59:40.000000 audbackend-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-10 06:59:47.059556 audbackend-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-10 06:59:40.000000 audbackend-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/core/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/backend/artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    33083 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/backend/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/core/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/interface/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/interface/maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    22076 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/interface/unversioned.py
--rw-r--r--   0 runner    (1001) docker     (127)    31608 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/interface/versioned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.051556 audbackend-2.0.0/audbackend/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-10 06:59:40.000000 audbackend-2.0.0/audbackend/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.059556 audbackend-2.0.0/audbackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-10 06:59:47.000000 audbackend-2.0.0/audbackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-10 06:59:47.000000 audbackend-2.0.0/audbackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:59:47.000000 audbackend-2.0.0/audbackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 06:59:47.000000 audbackend-2.0.0/audbackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 06:59:47.000000 audbackend-2.0.0/audbackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.055556 audbackend-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.055556 audbackend-2.0.0/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/api-src/audbackend.backend.rst
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/api-src/audbackend.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/api-src/audbackend.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/developer-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/legacy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-10 06:59:40.000000 audbackend-2.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-10 06:59:40.000000 audbackend-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 06:59:40.000000 audbackend-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:59:47.059556 audbackend-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.059556 audbackend-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/bad_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:59:47.059556 audbackend-2.0.0/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/misc/cleanup_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/singlefolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_backend_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_backend_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_backend_filesystem_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_interface_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    27976 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_interface_unversioned.py
--rw-r--r--   0 runner    (1001) docker     (127)    40415 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_interface_versioned.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_legacy_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 06:59:40.000000 audbackend-2.0.0/tests/test_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.846904 audbackend-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 10:50:49.000000 audbackend-2.0.1/.coveragerc.Linux
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 10:50:49.000000 audbackend-2.0.1/.coveragerc.Windows
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 10:50:49.000000 audbackend-2.0.1/.coveragerc.macOS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.830904 audbackend-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.834904 audbackend-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-14 10:50:49.000000 audbackend-2.0.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 10:50:49.000000 audbackend-2.0.1/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-14 10:50:49.000000 audbackend-2.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-14 10:50:49.000000 audbackend-2.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 10:50:49.000000 audbackend-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 10:50:49.000000 audbackend-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-14 10:50:49.000000 audbackend-2.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-14 10:50:49.000000 audbackend-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 10:50:49.000000 audbackend-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-14 10:50:55.846904 audbackend-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-14 10:50:49.000000 audbackend-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.834904 audbackend-2.0.1/audbackend/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.838904 audbackend-2.0.1/audbackend/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.838904 audbackend-2.0.1/audbackend/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.838904 audbackend-2.0.1/audbackend/core/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/backend/artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33083 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/backend/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.838904 audbackend-2.0.1/audbackend/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/interface/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/interface/maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22076 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/interface/unversioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31608 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/interface/versioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.838904 audbackend-2.0.1/audbackend/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 10:50:49.000000 audbackend-2.0.1/audbackend/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.846904 audbackend-2.0.1/audbackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-14 10:50:55.000000 audbackend-2.0.1/audbackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-14 10:50:55.000000 audbackend-2.0.1/audbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:50:55.000000 audbackend-2.0.1/audbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 10:50:55.000000 audbackend-2.0.1/audbackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 10:50:55.000000 audbackend-2.0.1/audbackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.842904 audbackend-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.842904 audbackend-2.0.1/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/api-src/audbackend.backend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/api-src/audbackend.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/api-src/audbackend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/developer-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-14 10:50:49.000000 audbackend-2.0.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-14 10:50:49.000000 audbackend-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 10:50:49.000000 audbackend-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:50:55.846904 audbackend-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.842904 audbackend-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/bad_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:50:55.842904 audbackend-2.0.1/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/misc/cleanup_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/singlefolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_backend_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_backend_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_backend_filesystem_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_interface_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27976 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_interface_unversioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40415 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_interface_versioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_legacy_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 10:50:49.000000 audbackend-2.0.1/tests/test_repository.py
```

### Comparing `audbackend-2.0.0/.github/workflows/doc.yml` & `audbackend-2.0.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/.github/workflows/linter.yml` & `audbackend-2.0.1/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/.github/workflows/publish.yml` & `audbackend-2.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/.github/workflows/test.yml` & `audbackend-2.0.1/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         os: [ ubuntu-latest, windows-latest, macOS-latest ]
         python-version: [ '3.10' ]
         include:
           - os: ubuntu-latest
             python-version: '3.8'
           - os: ubuntu-latest
             python-version: '3.9'
+          - os: ubuntu-latest
+            python-version: '3.11'
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
```

### Comparing `audbackend-2.0.0/.pre-commit-config.yaml` & `audbackend-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/CHANGELOG.rst` & `audbackend-2.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 2.0.1 (2024-05-14)
+--------------------------
+
+* Added: support for Python 3.11
+* Fixed: ensure execution time of
+  ``audbackend.interface.Maven.ls()``
+  is independent of repository size
+  on all backends
+
+
 Version 2.0.0 (2024-05-10)
 --------------------------
 
 * Added: ``audbackend.interface`` sub-module
   including an backend interface base class
   ``audbackend.interface.Base``,
   and the three interfaces
```

### Comparing `audbackend-2.0.0/CONTRIBUTING.rst` & `audbackend-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/LICENSE` & `audbackend-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/PKG-INFO` & `audbackend-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbackend
-Version: 2.0.0
+Version: 2.0.1
 Summary: Backends to access Artifactory and local file system
 Author-email: Johannes Wagner <jwagner@audeering.com>, Hagen Wierstorf <hwierstorf@audeering.com>
 License: MIT License
         
         Copyright (c) 2021 audEERING GmbH and Contributors
         
         Authors:
@@ -38,23 +38,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: audeer>=1.20.0
 Requires-Dist: pywin32; sys_platform == "win32"
 Provides-Extra: artifactory
-Requires-Dist: dohq-artifactory>=0.9.0; extra == "artifactory"
+Requires-Dist: dohq-artifactory>=0.10.0; extra == "artifactory"
 Provides-Extra: all
-Requires-Dist: dohq-artifactory>=0.9.0; extra == "all"
+Requires-Dist: dohq-artifactory>=0.10.0; extra == "all"
 
 ==========
 audbackend
 ==========
 
 |tests| |coverage| |docs| |python-versions| |license|
```

### Comparing `audbackend-2.0.0/README.rst` & `audbackend-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/__init__.py` & `audbackend-2.0.1/audbackend/__init__.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/api.py` & `audbackend-2.0.1/audbackend/core/api.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/backend/artifactory.py` & `audbackend-2.0.1/audbackend/core/backend/artifactory.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/backend/base.py` & `audbackend-2.0.1/audbackend/core/backend/base.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/backend/filesystem.py` & `audbackend-2.0.1/audbackend/core/backend/filesystem.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/conftest.py` & `audbackend-2.0.1/audbackend/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/errors.py` & `audbackend-2.0.1/audbackend/core/errors.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/interface/base.py` & `audbackend-2.0.1/audbackend/core/interface/base.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/interface/maven.py` & `audbackend-2.0.1/audbackend/core/interface/maven.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,33 +164,37 @@
         """  # noqa: E501
         if path.endswith("/"):  # find files under sub-path
             paths = self.backend.ls(
                 path,
                 suppress_backend_errors=suppress_backend_errors,
             )
             # Files are also stored as sub-folder,
-            # e.g. `/file/version/file-version.ext`,
+            # e.g. `.../<name>/<version>/<name>-<version><ext>`,
             # so we need to skip those
             sub_paths = len(path.split("/")) - 2
             if sub_paths > 0:
                 paths = [
                     path for path in paths if len(path.split(self.sep)) > 3 + sub_paths
                 ]
 
         else:  # find versions of path
             root, file = self.split(path)
+            name, ext = self._split_ext(file)
 
+            # Look inside `<root>/<name>/`
+            # for available versions.
+            # It will return entries in the form
+            # `<root>/<name>/<version>/<name>-<version><ext>`
             paths = self.backend.ls(
-                root,
+                self.backend.join(root, name, self.sep),
                 suppress_backend_errors=suppress_backend_errors,
             )
 
-            # filter for '/root/version/file'
+            # filter for '<root>/<name>/<version>/<name>-x.x.x<ext>'
             depth = root.count("/") + 2
-            name, ext = self._split_ext(file)
             match = re.compile(rf"{name}-\d+\.\d+.\d+{ext}")
             paths = [
                 p
                 for p in paths
                 if (p.count("/") == depth and match.match(os.path.basename(p)))
             ]
 
@@ -204,27 +208,28 @@
                     raise BackendError(ex)
 
         if not paths:
             return []
 
         paths_and_versions = []
         for p in paths:
+            # Split into
+            # ["", ..., <name>, <version>, <name>-<version><ext>]
             tokens = p.split(self.sep)
-
-            name = tokens[-1]
             version = tokens[-2]
 
             if version:
-                base = tokens[-3]
-                ext = name[len(base) + len(version) + 1 :]
-                name = f"{base}{ext}"
-                path = self.sep.join(tokens[:-3])
+                root = self.sep.join(tokens[:-3])
+                name = tokens[-3]
+                name_version_ext = tokens[-1]
+
+                ext = name_version_ext[len(name) + len(version) + 1 :]
+                file = f"{name}{ext}"
 
-                path = self.sep + path
-                path = self.join(path, name)
+                path = self.join(self.sep, root, file)
 
                 if not pattern or fnmatch.fnmatch(os.path.basename(path), pattern):
                     paths_and_versions.append((path, version))
 
         paths_and_versions = sorted(paths_and_versions)
 
         if latest_version:
```

### Comparing `audbackend-2.0.0/audbackend/core/interface/unversioned.py` & `audbackend-2.0.1/audbackend/core/interface/unversioned.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/interface/versioned.py` & `audbackend-2.0.1/audbackend/core/interface/versioned.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/repository.py` & `audbackend-2.0.1/audbackend/core/repository.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend/core/utils.py` & `audbackend-2.0.1/audbackend/core/utils.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/audbackend.egg-info/PKG-INFO` & `audbackend-2.0.1/audbackend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbackend
-Version: 2.0.0
+Version: 2.0.1
 Summary: Backends to access Artifactory and local file system
 Author-email: Johannes Wagner <jwagner@audeering.com>, Hagen Wierstorf <hwierstorf@audeering.com>
 License: MIT License
         
         Copyright (c) 2021 audEERING GmbH and Contributors
         
         Authors:
@@ -38,23 +38,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: audeer>=1.20.0
 Requires-Dist: pywin32; sys_platform == "win32"
 Provides-Extra: artifactory
-Requires-Dist: dohq-artifactory>=0.9.0; extra == "artifactory"
+Requires-Dist: dohq-artifactory>=0.10.0; extra == "artifactory"
 Provides-Extra: all
-Requires-Dist: dohq-artifactory>=0.9.0; extra == "all"
+Requires-Dist: dohq-artifactory>=0.10.0; extra == "all"
 
 ==========
 audbackend
 ==========
 
 |tests| |coverage| |docs| |python-versions| |license|
```

### Comparing `audbackend-2.0.0/audbackend.egg-info/SOURCES.txt` & `audbackend-2.0.1/audbackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/api-src/audbackend.rst` & `audbackend-2.0.1/docs/api-src/audbackend.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/conf.py` & `audbackend-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/developer-guide.rst` & `audbackend-2.0.1/docs/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/index.rst` & `audbackend-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/install.rst` & `audbackend-2.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/legacy.rst` & `audbackend-2.0.1/docs/legacy.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/docs/usage.rst` & `audbackend-2.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/pyproject.toml` & `audbackend-2.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,30 +20,31 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering',
 ]
 dependencies = [
     'audeer >=1.20.0',
     'pywin32; sys_platform == "win32"',
 ]
 # Get version dynamically from git
 # (needs setuptools_scm tools config below)
 dynamic = ['version']
 
 [project.optional-dependencies]
 artifactory = [
-    'dohq-artifactory >=0.9.0',
+    'dohq-artifactory >=0.10.0',
 ]
 all = [
-    'dohq-artifactory >=0.9.0',
+    'dohq-artifactory >=0.10.0',
 ]
 
 
 [project.urls]
 repository = 'https://github.com/audeering/audbackend/'
 documentation = 'https://audeering.github.io/audbackend/'
```

### Comparing `audbackend-2.0.0/tests/bad_file_system.py` & `audbackend-2.0.1/tests/bad_file_system.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/conftest.py` & `audbackend-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/misc/cleanup_artifactory.py` & `audbackend-2.0.1/tests/misc/cleanup_artifactory.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/singlefolder.py` & `audbackend-2.0.1/tests/singlefolder.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_api.py` & `audbackend-2.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_backend_artifactory.py` & `audbackend-2.0.1/tests/test_backend_artifactory.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_backend_base.py` & `audbackend-2.0.1/tests/test_backend_base.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_backend_filesystem.py` & `audbackend-2.0.1/tests/test_backend_filesystem.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_interface_maven.py` & `audbackend-2.0.1/tests/test_interface_maven.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_interface_unversioned.py` & `audbackend-2.0.1/tests/test_interface_unversioned.py`

 * *Files identical despite different names*

### Comparing `audbackend-2.0.0/tests/test_interface_versioned.py` & `audbackend-2.0.1/tests/test_interface_versioned.py`

 * *Files identical despite different names*


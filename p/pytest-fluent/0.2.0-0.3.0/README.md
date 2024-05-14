# Comparing `tmp/pytest-fluent-0.2.0.tar.gz` & `tmp/pytest_fluent-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-fluent-0.2.0.tar", last modified: Mon Jun 26 12:57:57 2023, max compression
+gzip compressed data, was "pytest_fluent-0.3.0.tar", last modified: Tue May 14 08:51:32 2024, max compression
```

## Comparing `pytest-fluent-0.2.0.tar` & `pytest_fluent-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.697304 pytest-fluent-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.681304 pytest-fluent-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.681304 pytest-fluent-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 12:57:57.697304 pytest-fluent-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.685304 pytest-fluent-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.685304 pytest-fluent-0.2.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/usage/stage_settings.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 12:57:57.697304 pytest-fluent-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.673304 pytest-fluent-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.685304 pytest-fluent-0.2.0/src/pytest_fluent/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/additional_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/content_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.689304 pytest-fluent-0.2.0/src/pytest_fluent/data/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/data/default.stage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/data/schema.stage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/setting_file_loader_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/src/pytest_fluent/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.689304 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 12:57:57.000000 pytest-fluent-0.2.0/src/pytest_fluent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.693304 pytest-fluent-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.697304 pytest-fluent-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/data/complex.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/data/default.json
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/data/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_additional_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_addoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_content_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_ini_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_reporting_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tests/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-26 12:57:28.000000 pytest-fluent-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/usage/stage_settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.876866 pytest_fluent-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.884866 pytest_fluent-0.3.0/src/pytest_fluent/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/additional_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/content_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.884866 pytest_fluent-0.3.0/src/pytest_fluent/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/data/default.stage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/data/schema.stage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/importlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/setting_file_loader_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/complex.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_additional_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_addoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_content_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_importlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_ini_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_logging_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_reporting_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tox.ini
```

### Comparing `pytest-fluent-0.2.0/.github/dependabot.yml` & `pytest_fluent-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/.github/workflows/linting.yml` & `pytest_fluent-0.3.0/.github/workflows/linting.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
   linting:
     strategy:
       fail-fast: true
       matrix:
         python: ["3.8", "3.9", "3.10", "3.11"]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - uses: psf/black@stable
```

### Comparing `pytest-fluent-0.2.0/.github/workflows/python-publish.yml` & `pytest_fluent-0.3.0/.github/workflows/python-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Build
```

### Comparing `pytest-fluent-0.2.0/.github/workflows/tests.yml` & `pytest_fluent-0.3.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python: ["3.8", "3.9", "3.10", "3.11"]
     runs-on: ${{ matrix.os }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run pytest with coverage
         continue-on-error: true
         run: |
           tox -e test -- --junitxml=results.xml tests/
       - name: Test report
-        uses: mikepenz/action-junit-report@v3
+        uses: mikepenz/action-junit-report@v4
         if: always()
         with:
           check_name: Test Report (${{ matrix.os }}, ${{ matrix.python }})
           report_paths: "**/results.xml"
           detailed_summary: true
       - name: Convert coverage
         run: |
```

### Comparing `pytest-fluent-0.2.0/.gitignore` & `pytest_fluent-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/.readthedocs.yaml` & `pytest_fluent-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/LICENSE` & `pytest_fluent-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Rohde & Schwarz GmbH & Co. KG
+Copyright (c) 2022-present Rohde & Schwarz GmbH & Co. KG
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest-fluent-0.2.0/PKG-INFO` & `pytest_fluent-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluent
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pytest plugin in order to provide logs via fluentd
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <carsten.sauerbrey@rohde-schwarz.com>, Nicola Lambiase <nicola.lambiase@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/pytest-fluent
 Keywords: pytest,logging,fluent
 Platform: Unix
@@ -23,17 +23,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pytest>=7.0.0
+Requires-Dist: msgpack
+Requires-Dist: six
+Requires-Dist: fluent-logger
+Requires-Dist: jsonschema
+Requires-Dist: ruamel.yaml
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist[psutil]; extra == "test"
+Requires-Dist: six; extra == "test"
+Requires-Dist: importlib-resources; python_version <= "3.8" and extra == "test"
 
 # pytest-fluent
 
 [![Documentation](https://readthedocs.org/projects/pytest-fluent/badge/?version=latest)](https://pytest-fluent.readthedocs.io/) [![Build Status](https://github.com/Rohde-Schwarz/pytest-fluent/actions/workflows/tests.yml/badge.svg)](https://github.com/Rohde-Schwarz/pytest-fluent/actions/) [![PyPI Versions](https://img.shields.io/pypi/pyversions/pytest-fluent.svg)](https://pypi.python.org/pypi/pytest-fluent) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-fluent)  [![PyPI Status](https://img.shields.io/pypi/status/pytest-fluent.svg)](https://pypi.python.org/pypi/pytest-fluent) [![PyPI License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
 
 _pytest-fluent_ is a Python package in order to extend _pytest_ using _Fluentd_ for logging test results.
```

### Comparing `pytest-fluent-0.2.0/README.md` & `pytest_fluent-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/docs/conf.py` & `pytest_fluent-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/docs/usage/stage_settings.md` & `pytest_fluent-0.3.0/docs/usage/stage_settings.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ### Custom stage settings
 
 Sometimes, the default settings are not enough in order to forward the test information as needed. Therefore, you can set custom stage settings
 in order to fit your needs.
 
-You can set specific values for `all` stages or specific values for any used stage. In order to do so, call your test run with the `--stage-settings=YourFileName.json` parameter. The following example stage settings JSON file content:
+You can set specific values for `all` stages or specific values for any used stage. In order to do so, call your test run with the `--stage-settings=YourFileName.json` parameter. It is also possible to provide a `JSON` or `YAML` string by setting the format
+with a separator e.g. `--stage-settings=json:{"json": "content}` or `--stage-settings=yaml:yaml: content`
+
+The following example stage settings JSON file content:
 
 ```json
 {
     "all": {
         "tag": "run",
         "label": "pytest",
         "replace": {"keys": {"status": "state", "sessionId": "id"}},
@@ -120,14 +123,15 @@
     assert True
 ```
 
 #### Stage setting file
 
 Custom settings for each supported stage can be easily setup. You have to create a file with
 a `.json` or `.yaml` extension and call pytest with this additional parameter `--stage-settings`.
+It's also possible to inject a serialized string with the following prefix `--stage-settings json;{...}`.
 
 The file will be validated against a schema of supported values and in case of an error, a `jsonschema.ValidationError`
 will be thrown.
 
 #### Stage settings
 
 ##### Number of supported stage
@@ -209,14 +213,71 @@
 * `skipped`
 * `error`
 * `start`
 * `finish`
 * `session`
 * `testcase`
 
+##### Use custom RecordFormatter class
+
+If you want to use you own custom record formatter class, you can load you own file by setting in the `logging`
+the `recordFormatter` key with the following object:
+
+```json
+{
+	...
+    "logging": {
+      "recordFormatter": {
+        "className": "RecordFormatter",
+          "filePath": "path/to/my/record/formatter.py"
+      }
+    }
+}
+```
+
+which loads the following `RecordFormatter`
+
+```python
+# path/to/my/record/formatter.py
+import logging
+from pytest_fluent import get_session_uid, get_test_uid
+
+class RecordFormatter(logging.Formatter):
+
+    def format(self, record) -> typing.Any:
+        """Format the specified record as text."""
+        return {
+            "date": datetime.datetime.utcfromtimestamp(record.created).isoformat(),
+            "session_id": get_session_uid(),
+            "test_id": get_test_uid(),
+            "level": record.levelno,
+            "msg": record.msg,
+            "class": record.module,
+            "method": record.funcName,
+            "src": record.filename,
+            "line": record.lineno,
+            "pid": record.process,
+            "tid": record.thread,
+        }
+```
+
+You can also load it as a module from e.g. the site-packages
+
+```json
+{
+	...
+    "logging": {
+      "recordFormatter": {
+        "className": "RecordFormatter",
+          "module": "path.to.my.record.formatter"
+      }
+    }
+}
+```
+
 ##### Use values from ARGV and ENV
 
 If you want to use data provided by the command line arguments or directly from environment variables,
 use the following syntax for value strings.
 
 | Type | Syntax                         |
 | ---- | ------------------------------ |
```

### Comparing `pytest-fluent-0.2.0/pyproject.toml` & `pytest_fluent-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 [project]
+dependencies = [
+    "pytest>=7.0.0",
+    "msgpack",
+    "six",
+    "fluent-logger",
+    "jsonschema",
+    "ruamel.yaml",
+]
 name = "pytest-fluent"
 authors = [
-    {name = "Rohde & Schwarz GmbH & Co. KG", email = "info@rohde-schwarz.com"},
+    { name = "Rohde & Schwarz GmbH & Co. KG", email = "info@rohde-schwarz.com" },
 ]
 maintainers = [
-    {name = "Carsten Sauerbrey", email = "carsten.sauerbrey@rohde-schwarz.com"},
-    {name = "Nicola Lambiase", email = "nicola.lambiase@rohde-schwarz.com"}
+    { name = "Carsten Sauerbrey", email = "carsten.sauerbrey@rohde-schwarz.com" },
+    { name = "Nicola Lambiase", email = "nicola.lambiase@rohde-schwarz.com" },
 ]
 description = "A pytest plugin in order to provide logs via fluentd"
 readme = "README.md"
 keywords = ["pytest", "logging", "fluent"]
-license = {text = "MIT"}
+license = { text = "MIT" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
@@ -22,42 +30,31 @@
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Framework :: Pytest"
+    "Framework :: Pytest",
 ]
 requires-python = ">=3.8"
-dependencies = [
-    "pytest>=7.0.0",
-    "msgpack",
-    "six",
-    "fluent-logger",
-    "jsonschema",
-    "ruamel.yaml",
-]
 dynamic = ["version"]
 
 [project.urls]
 project = "https://github.com/Rohde-Schwarz/pytest-fluent"
 
 [project.optional-dependencies]
-docs = [
-    "sphinx",
-    "sphinx-rtd-theme",
-    "myst-parser"
-]
+docs = ["sphinx", "sphinx-rtd-theme", "myst-parser"]
 test = [
     "pytest",
     "coverage[toml]",
     "pytest-cov",
     "pytest-xdist[psutil]",
-    "six"
+    "six",
+    "importlib-resources; python_version<='3.8'",
 ]
 
 [build-system]
 requires = ["setuptools>=45.2", "wheel", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/__init__.py` & `pytest_fluent-0.3.0/src/pytest_fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/additional_information.py` & `pytest_fluent-0.3.0/src/pytest_fluent/additional_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Set additional information function handler."""
+
 import inspect
 import typing
 
 INFORMATION_CALLBACKS: typing.Dict[str, typing.List[typing.Callable]] = {}
 SESSION_STAGE = "pytest_sessionstart"
 TEST_STAGE = "pytest_runtest_logstart"
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/content_patcher.py` & `pytest_fluent-0.3.0/src/pytest_fluent/content_patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Patch content according to settings."""
+
 import argparse
 import enum
 import inspect
 import os
 import re
 import typing
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/data/schema.stage.json` & `pytest_fluent-0.3.0/src/pytest_fluent/data/schema.stage.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9107142857142857%*

 * *Differences: {"'anyOf'": "{2: {'patternProperties': {replace: "*

 * *            "OrderedDict([('pytest_sessionfinish|pytest_sessionstart|pytest_runtest_logstart|pytest_runtest_logreport|pytest_runtest_logfinish', "*

 * *            "OrderedDict([('$ref', '#/definitions/AdditionalProperties')]))])}}, insert: [(1, "*

 * *            "OrderedDict([('type', 'object'), ('patternProperties', OrderedDict([('logging', "*

 * *            "OrderedDict([('anyOf', [OrderedDict([('$ref', "*

 * *            "'#/definitions/AdditionalProperties')]), OrderedD […]*

```diff
@@ -12,15 +12,30 @@
                     ]
                 }
             },
             "type": "object"
         },
         {
             "patternProperties": {
-                "pytest_sessionfinish|pytest_sessionstart|pytest_runtest_logstart|pytest_runtest_logreport|pytest_runtest_logfinish|logging": {
+                "logging": {
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/AdditionalProperties"
+                        },
+                        {
+                            "$ref": "#/definitions/LogFormatter"
+                        }
+                    ]
+                }
+            },
+            "type": "object"
+        },
+        {
+            "patternProperties": {
+                "pytest_sessionfinish|pytest_sessionstart|pytest_runtest_logstart|pytest_runtest_logreport|pytest_runtest_logfinish": {
                     "$ref": "#/definitions/AdditionalProperties"
                 }
             },
             "type": "object"
         }
     ],
     "definitions": {
@@ -61,22 +76,78 @@
                 "tag": {
                     "$ref": "#/definitions/RegexString",
                     "default": "<fluentd-tag>"
                 }
             },
             "type": "object"
         },
+        "LogFormatter": {
+            "additionalProperties": false,
+            "properties": {
+                "recordFormatter": {
+                    "additionalProperties": false,
+                    "oneOf": [
+                        {
+                            "module": {
+                                "regex": "^([a-z_][a-z0-9_]*)+(\\.[a-z_][a-z0-9_]*)*$",
+                                "type": "string"
+                            },
+                            "required": [
+                                "module",
+                                "className"
+                            ]
+                        },
+                        {
+                            "filePath": {
+                                "type": "string"
+                            },
+                            "required": [
+                                "filePath",
+                                "className"
+                            ]
+                        }
+                    ],
+                    "properties": {
+                        "className": {
+                            "type": "string"
+                        },
+                        "filePath": {
+                            "type": "string"
+                        },
+                        "module": {
+                            "regex": "^([a-z_][a-z0-9_]*)+(\\.[a-z_][a-z0-9_]*)*$",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "className"
+                    ],
+                    "type": "object"
+                }
+            },
+            "required": [
+                "recordFormatter"
+            ],
+            "type": "object"
+        },
         "RegexString": {
             "regex": "(\\$)?([<\\{])?[\\w_.-]+([>\\}])?",
             "type": "string"
         }
     },
     "patternProperties": {
         "all|pytest_sessionfinish|pytest_sessionstart|pytest_runtest_logstart|pytest_runtest_logreport|pytest_runtest_logfinish|logging": {
-            "$ref": "#/definitions/AdditionalProperties"
+            "anyOf": [
+                {
+                    "$ref": "#/definitions/AdditionalProperties"
+                },
+                {
+                    "$ref": "#/definitions/LogFormatter"
+                }
+            ]
         }
     },
     "required": [
         "all"
     ],
     "type": "object"
 }
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/event.py` & `pytest_fluent-0.3.0/src/pytest_fluent/event.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,8 +45,18 @@
             return
         sender_ = self.senders.get(tag)
         if sender_ is None or not isinstance(sender_, FluentSender):
             LOGGER.warning("Could not retrieve fluent instance for tag %s", tag)
             return
         timestamp = kwargs.get("time", int(time.time()))
         if not sender_.emit_with_time(label, timestamp, data):
-            LOGGER.warning("Could not send data via fluent for tag %s: %s", tag, data)
+            if sender_.last_error:
+                LOGGER.warning(
+                    "Error '%s' while sending data via fluent for tag '%s': '%s'",
+                    sender_.last_error,
+                    tag,
+                    data,
+                )
+            else:
+                LOGGER.warning(
+                    "Could not send data via fluent for tag '%s': '%s'", tag, data
+                )
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/plugin.py` & `pytest_fluent-0.3.0/src/pytest_fluent/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """pytest-fluent-logging plugin definition."""
+
 import datetime
 import logging
 import os
 import textwrap
 import time
 import typing
 import uuid
 from io import BytesIO
 
 import msgpack
 import pytest
 from fluent.handler import FluentHandler, FluentRecordFormatter
 
+from pytest_fluent.importlib_utils import extract_function_from_module_string
+
 from .additional_information import get_additional_information_callback
 from .content_patcher import ContentPatcher
 from .event import Event
 from .setting_file_loader_action import (
     SettingFileLoaderAction,
     load_and_check_settings_file,
 )
@@ -26,15 +29,22 @@
 #####################################################
 
 DOCSTRING_KEY = "docstring"
 DOCSTRING_STASHKEY = pytest.StashKey[str]()
 
 
 class FluentLoggerRuntime(object):
+    """Fluent logger runtime.
+
+    Args:
+        config (_type_): Pytest configuration
+    """
+
     def __init__(self, config):
+        """Initialize fluent-logger runtime."""
         self._session_uuid = None
         self._session_start_time = None
         self._test_uuid = None
         self.config = config
         self._set_session_uid(self.config.getoption("--session-uuid"))
         self._host = config.getoption("--fluentd-host")
         self._port = config.getoption("--fluentd-port")
@@ -71,20 +81,15 @@
             raise ValueError(
                 "Tag for logging was not set. Please set either specific tag value for \
                     key 'logging' or use the 'all' object in stage settings file."
             )
         label = self._content_patcher.user_settings.get("logging", {}).get("label")
         if label:
             tag = f"{tag}.{label}"
-        extend_loggers(
-            self._host,
-            self._port,
-            tag,
-            self._content_patcher,
-        )
+        extend_loggers(self._host, self._port, tag, self._content_patcher)
 
     def _set_session_uid(
         self, id: typing.Optional[typing.Union[str, uuid.UUID]] = None
     ) -> None:
         """Set or create a session ID."""
         if id is None:
             self._session_uuid = create_unique_identifier()
@@ -112,15 +117,15 @@
 
     @property
     def test_uid(self) -> str:
         """Get current test ID."""
         return str(self._test_uuid)
 
     def pytest_sessionstart(self):
-        """Custom hook for session start."""
+        """Customize hook for session start."""
         set_stage("session")
         self._session_start_time = time.time()
         if not self.config.getoption("collectonly"):
             data = {
                 "status": "start",
                 "stage": "session",
                 "sessionId": self.session_uid,
@@ -128,15 +133,15 @@
             data = self._content_patcher.patch(data)
             data.update(get_additional_information_callback())
             self._set_timestamp_information(data=data)
             tag, label = self._content_patcher.get_tag_and_label()
             self._event(tag, label, data)
 
     def pytest_runtest_logstart(self, nodeid: str, location: typing.Tuple[int, str]):
-        """Custom hook for test start."""
+        """Customize hook for test start."""
         set_stage("testcase")
         if not self.config.getoption("collectonly"):
             self._create_test_unique_identifier()
             data = {
                 "status": "start",
                 "stage": "testcase",
                 "sessionId": self.session_uid,
@@ -146,44 +151,44 @@
             data = self._content_patcher.patch(data)
             data.update(get_additional_information_callback())
             self._set_timestamp_information(data=data)
             tag, label = self._content_patcher.get_tag_and_label()
             self._event(tag, label, data)
 
     def pytest_runtest_setup(self, item: pytest.Item):
-        """Custom hook for test setup."""
+        """Customize hook for test setup."""
         set_stage("testcase")
         docstring = get_test_docstring(item)
         item.stash[DOCSTRING_STASHKEY] = docstring
         if not self.config.getoption("collectonly"):
             pass
 
     def pytest_runtest_teardown(self, item: pytest.Item, nextitem: pytest.Item):
-        """Custom hook for test teardown."""
+        """Customize hook for test teardown."""
         set_stage("testcase")
         docstring = get_test_docstring(item)
         item.stash[DOCSTRING_STASHKEY] = docstring
         if not self.config.getoption("collectonly"):
             pass
 
     def pytest_runtest_call(self, item: pytest.Item):
-        """Custom hook for test call."""
+        """Customize hook for test call."""
         set_stage("testcase")
         if not self.config.getoption("collectonly"):
             pass
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(self, item: pytest.Item, call):
-        """Custom hook for make report."""
+        """Customize hook for make report."""
         report = (yield).get_result()
         docstring = item.stash.get(DOCSTRING_STASHKEY, None)
         report.stash = {DOCSTRING_KEY: docstring}
 
     def pytest_runtest_logreport(self, report: pytest.TestReport):
-        """Custom hook for logging results."""
+        """Customize hook for logging results."""
         set_stage("testcase")
         if not self.config.getoption("collectonly"):
             data = self._log_reporter(report)
             if not data:
                 return
             data.update(
                 {
@@ -204,15 +209,15 @@
             self._event(tag, label, data)
 
     def pytest_runtest_logfinish(
         self,
         nodeid: str,
         location: typing.Tuple[str, typing.Optional[int], str],
     ):
-        """Custom hook for test end."""
+        """Customize hook for test end."""
         set_stage("testcase")
         if not self.config.getoption("collectonly"):
             data = {
                 "status": "finish",
                 "stage": "testcase",
                 "sessionId": self.session_uid,
                 "testId": self.test_uid,
@@ -225,15 +230,15 @@
             self._event(tag, label, data)
 
     def pytest_sessionfinish(
         self,
         session: pytest.Session,
         exitstatus: typing.Union[int, pytest.ExitCode],
     ):
-        """Custom hook for session end."""
+        """Customize hook for session end."""
         set_stage("session")
         if not self.config.getoption("collectonly"):
             data = {
                 "status": "finish",
                 "duration": (
                     time.time()
                     - (
@@ -371,18 +376,16 @@
 
 #####################################################
 # functions and classes
 #####################################################
 
 
 # Logging extensions
-
-
 class RecordFormatter(FluentRecordFormatter):
-    """Extension of FluentRecordFormatter in order to add unique ID's"""
+    """Extension of FluentRecordFormatter in order to add unique ID's."""
 
     def __init__(self, patcher: typing.Optional[ContentPatcher], *args, **kwargs):
         """Specific initilization."""
         super(RecordFormatter, self).__init__(*args, **kwargs)
         self.content_patcher = patcher
 
     def format(self, record):
@@ -394,51 +397,108 @@
         data["testId"] = get_test_uid()
         data["stage"] = get_stage()
         if self.content_patcher:
             data = self.content_patcher.patch(data, "logging", ["tag", "label"])
         return data
 
 
-def extend_loggers(host, port, tag, patcher: ContentPatcher) -> None:
+def extend_loggers(
+    host,
+    port,
+    tag,
+    patcher: ContentPatcher,
+) -> None:
     """Extend Python logging with a Fluentd handler."""
     modify_logger(host, port, tag, None, patcher)
     modify_logger(host, port, tag, "fluent", patcher)
 
 
 def modify_logger(
-    host, port, tag, name=None, patcher: typing.Optional[ContentPatcher] = None
+    host,
+    port,
+    tag,
+    name=None,
+    patcher: typing.Optional[ContentPatcher] = None,
 ) -> None:
     """Extend Python logging with a Fluentd handler."""
     logger = logging.getLogger(name)
     add_handler(host, port, tag, logger, patcher)
 
 
 def add_handler(
-    host, port, tag, logger, patcher: typing.Optional[ContentPatcher] = None
+    host,
+    port,
+    tag,
+    logger,
+    patcher: typing.Optional[ContentPatcher] = None,
 ):
     """Add handler to a specific logger."""
     handler = FluentHandler(
         tag, host=host, port=port, buffer_overflow_handler=overflow_handler
     )
-    formatter = RecordFormatter(
-        patcher,
-        {
-            "type": "logging",
-            "host": "%(hostname)s",
-            "where": "%(module)s.%(funcName)s",
-            "level": "%(levelname)s",
-            "stack_trace": "%(exc_text)s",
-        },
-    )
+    formatter = get_formatter(patcher)
     handler.setFormatter(formatter)
     logger.addHandler(handler)
 
 
+def get_formatter(patcher: typing.Optional[ContentPatcher] = None) -> logging.Formatter:
+    """Get a prepared logging formatter.
+
+    Args:
+        patcher (typing.Optional[ContentPatcher], optional): Patcher handler.
+            Defaults to None.
+
+    Returns:
+        logging.Formatter: Formatter instance
+    """
+    if patcher:
+        record_formatter = patcher.user_settings.get("logging", {}).get(
+            "recordFormatter"
+        )
+    else:
+        record_formatter = None
+    if record_formatter:
+        formatter = load_record_formatter_class(record_formatter)
+    else:
+        formatter = RecordFormatter(
+            patcher,
+            {
+                "type": "logging",
+                "host": "%(hostname)s",
+                "where": "%(module)s.%(funcName)s",
+                "level": "%(levelname)s",
+                "stack_trace": "%(exc_text)s",
+            },
+        )
+
+    return formatter
+
+
+def load_record_formatter_class(
+    record_formatter_settings: typing.Dict[str, str]
+) -> logging.Formatter:
+    """Load a custom record formatter.
+
+    Args:
+        record_formatter_settings (typing.Dict[str, str]): Record formatter settings
+
+    Returns:
+        logging.Formatter: Record formatter instance
+    """
+    record_formatter = extract_function_from_module_string(
+        record_formatter_settings["className"],
+        record_formatter_settings.get("module"),
+        record_formatter_settings.get("filePath"),
+    )
+    record_formatter_instance = record_formatter()
+    return record_formatter_instance
+
+
 def overflow_handler(pendings):
-    """Custom overflow handler."""
+    """Customize overflow handler."""
     unpacker = msgpack.Unpacker(BytesIO(pendings))
     for unpacked in unpacker:
         print(unpacked)
 
 
 def set_stage(val: str) -> None:
     """Set the current execution stage."""
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/setting_file_loader_action.py` & `pytest_fluent-0.3.0/src/pytest_fluent/setting_file_loader_action.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 """Load and schema check settings file."""
+
 import argparse
 import json
 import os
+import re
+import typing
+from io import StringIO
 
 import jsonschema
 from ruamel.yaml import YAML
 
 
 class SettingFileLoaderAction(argparse.Action):
     """Custom action for loading JSON/YAML configuration."""
 
     def __call__(self, parser, args, values, option_string=None):
-        """Implementing call."""
+        """Implement call."""
         parameter = load_and_check_settings_file(values)
         setattr(args, self.dest, parameter)
 
 
-def load_and_check_settings_file(file_name: str):
+def load_and_check_settings_file(file_name: str) -> typing.Dict[str, typing.Any]:
     """Load settings file and check content against schema.
 
     Args:
         file_name (str): Path to settings file.
 
     Raises:
         ValueError: File type not supported.
 
     Returns:
-        _type_: User settings dictionary.
+        typing.Dict[str, typing.Any]: User settings dictionary.
     """
-    if file_name.endswith(".json"):
+    splitted = re.split(
+        r";",
+        file_name,
+        maxsplit=1,
+        flags=re.IGNORECASE | re.MULTILINE,
+    )
+    if len(splitted) == 1:
+        file_data = splitted[0]
+        data_format = None
+    if len(splitted) == 2:
+        data_format, file_data = splitted
+    if data_format == "json" or file_data.endswith(".json"):
         pickle = json
-    elif file_name.endswith(".yaml"):
+    elif data_format == "yaml" or file_data.endswith(".yaml"):
         pickle = YAML()
 
         def loads(file_pointer):
-            return pickle.load(file_pointer.read())
+            stream = StringIO(file_pointer)
+            return pickle.load(stream)
 
         setattr(pickle, "loads", loads)
     else:
-        raise ValueError("File type not supported.")
-    if os.path.exists(file_name):
-        with open(file_name, encoding="utf-8") as fid:
+        raise ValueError("Wrong input format or file type not supported.")
+    if os.path.exists(file_data):
+        with open(file_data, encoding="utf-8") as fid:
             content = pickle.load(fid)
     else:
-        content = pickle.loads(file_name)
+        content = pickle.loads(file_data)
     with open(
         os.path.join(os.path.dirname(__file__), "data", "schema.stage.json"),
         encoding="utf-8",
     ) as fid:
         schema = json.load(fid)
     jsonschema.validate(instance=content, schema=schema)
     return content
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent/test_report.py` & `pytest_fluent-0.3.0/src/pytest_fluent/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extract result information."""
+
 # The MIT License (MIT)
 
 # Copyright (c) 2019 Israel Fruchter
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent.egg-info/PKG-INFO` & `pytest_fluent-0.3.0/src/pytest_fluent.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluent
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pytest plugin in order to provide logs via fluentd
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <carsten.sauerbrey@rohde-schwarz.com>, Nicola Lambiase <nicola.lambiase@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/pytest-fluent
 Keywords: pytest,logging,fluent
 Platform: Unix
@@ -23,17 +23,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pytest>=7.0.0
+Requires-Dist: msgpack
+Requires-Dist: six
+Requires-Dist: fluent-logger
+Requires-Dist: jsonschema
+Requires-Dist: ruamel.yaml
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist[psutil]; extra == "test"
+Requires-Dist: six; extra == "test"
+Requires-Dist: importlib-resources; python_version <= "3.8" and extra == "test"
 
 # pytest-fluent
 
 [![Documentation](https://readthedocs.org/projects/pytest-fluent/badge/?version=latest)](https://pytest-fluent.readthedocs.io/) [![Build Status](https://github.com/Rohde-Schwarz/pytest-fluent/actions/workflows/tests.yml/badge.svg)](https://github.com/Rohde-Schwarz/pytest-fluent/actions/) [![PyPI Versions](https://img.shields.io/pypi/pyversions/pytest-fluent.svg)](https://pypi.python.org/pypi/pytest-fluent) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-fluent)  [![PyPI Status](https://img.shields.io/pypi/status/pytest-fluent.svg)](https://pypi.python.org/pypi/pytest-fluent) [![PyPI License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
 
 _pytest-fluent_ is a Python package in order to extend _pytest_ using _Fluentd_ for logging test results.
```

### Comparing `pytest-fluent-0.2.0/src/pytest_fluent.egg-info/SOURCES.txt` & `pytest_fluent-0.3.0/src/pytest_fluent.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/installation.md
 docs/usage.md
 docs/usage/stage_settings.md
 src/pytest_fluent/__init__.py
 src/pytest_fluent/additional_information.py
 src/pytest_fluent/content_patcher.py
 src/pytest_fluent/event.py
+src/pytest_fluent/importlib_utils.py
 src/pytest_fluent/plugin.py
 src/pytest_fluent/setting_file_loader_action.py
 src/pytest_fluent/test_report.py
 src/pytest_fluent.egg-info/PKG-INFO
 src/pytest_fluent.egg-info/SOURCES.txt
 src/pytest_fluent.egg-info/dependency_links.txt
 src/pytest_fluent.egg-info/entry_points.txt
@@ -37,15 +38,17 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_additional_information.py
 tests/test_addoptions.py
 tests/test_content_patcher.py
 tests/test_docstrings.py
 tests/test_fixtures.py
+tests/test_importlib_utils.py
 tests/test_ini_configuration.py
+tests/test_logging_extension.py
 tests/test_parser.py
 tests/test_reporting.py
 tests/test_reporting_patching.py
 tests/test_schema.py
 tests/utility.py
 tests/data/complex.json
 tests/data/default.json
```

### Comparing `pytest-fluent-0.2.0/tests/conftest.py` & `pytest_fluent-0.3.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pathlib
 import uuid
 from unittest.mock import MagicMock, patch
 
 import pytest
 from fluent import handler
 
 import pytest_fluent.event
@@ -77,7 +78,20 @@
 
 
 @pytest.fixture()
 def run_mocked_pytest(runpytest, fluentd_sender):
     """Create a temporary pytest environment with FluentSender mock."""
 
     return runpytest, fluentd_sender
+
+
+@pytest.fixture()
+def record_formatter_file(pytester) -> pathlib.Path:
+    path = pytester.makepyfile(
+        record_formatter="""
+    import logging
+
+    class RecordFormatter(logging.Formatter):
+        pass
+    """
+    )
+    return path
```

### Comparing `pytest-fluent-0.2.0/tests/data/complex.json` & `pytest_fluent-0.3.0/tests/data/complex.json`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_additional_information.py` & `pytest_fluent-0.3.0/tests/test_additional_information.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_addoptions.py` & `pytest_fluent-0.3.0/tests/test_addoptions.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_content_patcher.py` & `pytest_fluent-0.3.0/tests/test_content_patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for ContentPatcher."""
+
 # pylint: disable=W0212, C0116, W0621
 import argparse
 import typing
 import uuid
 
 import pytest
```

### Comparing `pytest-fluent-0.2.0/tests/test_docstrings.py` & `pytest_fluent-0.3.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_fixtures.py` & `pytest_fluent-0.3.0/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_ini_configuration.py` & `pytest_fluent-0.3.0/tests/test_ini_configuration.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_reporting.py` & `pytest_fluent-0.3.0/tests/test_reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,20 +61,21 @@
 
 
 def check_for_verdict(session_uuid, report: dict):
     assert "name" in report
     name = report["name"].split("::")[1]
     assert report.get("outcome") == "passed"
     assert "duration" in report
+    assert report.get("sessionId") == str(session_uuid)
+    assert "testId" in report
     markers = report.get("markers")
+    assert markers is not None
     assert markers.get(name) == 1
     assert markers.get("test_data_reporter_xdist_passed.py") == 1
     assert markers.get("test_data_reporter_xdist_passed0") == 1
-    assert report.get("sessionId") == str(session_uuid)
-    assert "testId" in report
 
 
 def test_data_reporter_base_with_xfail(run_mocked_pytest, session_uuid):
     runpytest, fluent_sender = run_mocked_pytest
     _ = runpytest(
         f"--session-uuid={session_uuid}",
         pyfile="""
```

### Comparing `pytest-fluent-0.2.0/tests/test_reporting_patching.py` & `pytest_fluent-0.3.0/tests/test_reporting_patching.py`

 * *Files identical despite different names*

### Comparing `pytest-fluent-0.2.0/tests/test_schema.py` & `pytest_fluent-0.3.0/tests/test_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import json
+import sys
 
 import jsonschema
 import pytest
 
-try:
+if sys.version_info[:2] > (3, 8):
     from importlib.resources import files
-except ImportError:
+else:
     from importlib_resources import files
 
+
 pytest_fluent_resources = files("pytest_fluent")
 schema_file = pytest_fluent_resources / "data" / "schema.stage.json"
 default_file = pytest_fluent_resources / "data" / "default.stage.json"
 
 
 @pytest.fixture
 def default() -> dict:
-    with open(default_file, "r") as fp:
+    with open(str(default_file), "r") as fp:
         default = json.load(fp)
     return default
 
 
 @pytest.fixture
 def schema() -> dict:
-    with open(schema_file, "r") as fp:
+    with open(str(schema_file), "r") as fp:
         schema = json.load(fp)
     return schema
 
 
 def test_default_compliance(default, schema):
     jsonschema.validate(default, schema)
     default["pytest_runtest_logstart"] = {"replace": {"status": "state"}}
```

### Comparing `pytest-fluent-0.2.0/tox.ini` & `pytest_fluent-0.3.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,25 @@
 description = Autoformat code.
 skip_install = true
 envdir = {toxworkdir}/lint
 deps =
     black
     isort >= 5.0
 commands =
-    isort .
-    black src/ tests/
+    isort {posargs:src/ tests/}
+    black {posargs:src/ tests/}
+
+[testenv:format-check]
+description = Check code style using black.
+skip_install = true
+envdir = {toxworkdir}/lint
+deps =
+    black
+commands =
+    black --check {posargs:src/ tests/}
 
 [testenv:lint]
 description = Check code for stylistic and logical errors.
 envdir = {toxworkdir}/lint
 deps =
     {[testenv:codestyle]deps}
     {[testenv:docstyle]deps}
@@ -36,46 +45,42 @@
 
 [testenv:codestyle]
 description = Check code and tests for PEP 8 compliance and code complexity.
 skip_install = true
 envdir = {toxworkdir}/lint
 deps =
     flake8
-    flake8-colors
     isort >= 5.0
 commands =
-    flake8 --select E,W,C --show-source src/ tests/
-    isort --check --diff .
+    flake8 --select E,W,C --show-source {posargs:src/ tests/}
+    isort --check --diff {posargs:src/ tests/}
 
 [testenv:docstyle]
-description = Check docstrings for PEP 257 compliance (reST style).
+description = Check docstrings for PEP 257 compliance (Google style).
 skip_install = true
 envdir = {toxworkdir}/lint
 deps =
-    flake8
-    flake8-colors
-    flake8-rst-docstrings
-commands = flake8 --select RST src/
+    pydocstyle
+commands = pydocstyle {posargs:src/}
 
 [testenv:flake]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     flake8
-    flake8-colors
 commands =
-    flake8 --select F src/ tests/
+    flake8 --select F {posargs:src/ tests/}
 
 [testenv:pylint]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     pylint
 commands =
-    pylint --output-format=colorized --errors-only src/pytest_fluent
+    pylint --output-format=colorized --errors-only {posargs:src/pytest_fluent}
 
 [testenv:errors]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     {[testenv:flake]deps}
     {[testenv:pylint]deps}
@@ -87,31 +92,34 @@
 description = Run static type checker.
 skip_install = true
 envdir = {toxworkdir}/lint
 deps =
     mypy
     types-six
 commands =
-    mypy --check-untyped-defs --no-implicit-optional src/
+    mypy --check-untyped-defs --no-implicit-optional {posargs:src/ tests/}
 
 [testenv:test]
 description = Run tests with pytest.
 passenv = CI
+setenv =
+   COVERAGE_FILE = .coverage.{env:OS:linux}
 extras = test
 deps =
     pytest
     pytest-cov
 commands =
     pytest --cov --cov-report= {posargs:tests}
 
 [testenv:coverage]
-description = Measure and report coverage.
+description = Measure, combine and report coverage.
 deps =
-    coverage[toml]
+    coverage[toml] >= 6.0
 commands =
+    coverage combine
     coverage report
     coverage xml
     coverage html --fail-under 50
 
 [testenv:test_with_reports]
 description = Run tests with pytest and report coverage.
 envdir = {toxworkdir}/test_cov
```


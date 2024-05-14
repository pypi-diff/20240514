# Comparing `tmp/silverback-0.5.0.tar.gz` & `tmp/silverback-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.5.0.tar", last modified: Sat May 11 01:18:26 2024, max compression
+gzip compressed data, was "silverback-0.5.1.tar", last modified: Tue May 14 17:50:32 2024, max compression
```

## Comparing `silverback-0.5.0.tar` & `silverback-0.5.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-11 01:17:31.000000 silverback-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-11 01:17:31.000000 silverback-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-11 01:17:31.000000 silverback-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-11 01:17:31.000000 silverback-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-11 01:17:31.000000 silverback-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-11 01:18:26.451690 silverback-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-11 01:17:31.000000 silverback-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-11 01:17:31.000000 silverback-0.5.0/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-11 01:17:31.000000 silverback-0.5.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-11 01:17:31.000000 silverback-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 01:18:26.451690 silverback-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-11 01:17:31.000000 silverback-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.743176 silverback-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.743176 silverback-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-14 17:49:08.000000 silverback-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-14 17:49:08.000000 silverback-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 17:49:08.000000 silverback-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-14 17:49:08.000000 silverback-0.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-14 17:49:08.000000 silverback-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-14 17:50:32.751175 silverback-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-14 17:49:08.000000 silverback-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-14 17:49:08.000000 silverback-0.5.1/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-14 17:49:08.000000 silverback-0.5.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 17:49:08.000000 silverback-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 17:50:32.751175 silverback-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-14 17:49:08.000000 silverback-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/test_types.py
```

### Comparing `silverback-0.5.0/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.5.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.5.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.5.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/release-drafter.yml` & `silverback-0.5.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/codeql.yaml` & `silverback-0.5.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/commitlint.yaml` & `silverback-0.5.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/docs.yaml` & `silverback-0.5.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/prtitle.yaml` & `silverback-0.5.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/publish.yaml` & `silverback-0.5.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.github/workflows/test.yaml` & `silverback-0.5.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.gitignore` & `silverback-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/.pre-commit-config.yaml` & `silverback-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/CONTRIBUTING.md` & `silverback-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/Dockerfile` & `silverback-0.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/LICENSE` & `silverback-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/PKG-INFO` & `silverback-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.5.0
+Version: 0.5.1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.5.0/README.md` & `silverback-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/build_docs.py` & `silverback-0.5.1/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/_static/custom.css` & `silverback-0.5.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/_static/custom.js` & `silverback-0.5.1/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/_templates/layout.html` & `silverback-0.5.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/conf.py` & `silverback-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/favicon.ico` & `silverback-0.5.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/logo.gif` & `silverback-0.5.1/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/docs/userguides/development.md` & `silverback-0.5.1/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/example.py` & `silverback-0.5.1/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/pyproject.toml` & `silverback-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/setup.py` & `silverback-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/_cli.py` & `silverback-0.5.1/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/_importer.py` & `silverback-0.5.1/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/application.py` & `silverback-0.5.1/silverback/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,17 @@
         self._get_system_config = self.__register_system_task(
             TaskType.SYSTEM_CONFIG, self.__get_system_config_handler
         )
         # NOTE: Register other system tasks here
         self._get_user_taskdata = self.__register_system_task(
             TaskType.SYSTEM_USER_TASKDATA, self.__get_user_taskdata_handler
         )
+        self._get_user_all_taskdata = self.__register_system_task(
+            TaskType.SYSTEM_USER_ALL_TASKDATA, self.__get_user_all_taskdata_handler
+        )
 
     def __register_system_task(
         self, task_type: TaskType, task_handler: Callable
     ) -> AsyncTaskiqDecoratedTask:
         assert str(task_type).startswith("system:"), "Can only add system tasks"
         # NOTE: This has to be registered with the broker in the worker
         return self.broker.register_task(
@@ -132,14 +135,17 @@
         )
 
     def __get_user_taskdata_handler(self, task_type: TaskType) -> list[TaskData]:
         # NOTE: This is actually executed on the worker side
         assert str(task_type).startswith("user:"), "Can only fetch user task data"
         return self.tasks.get(task_type, [])
 
+    def __get_user_all_taskdata_handler(self) -> list[TaskData]:
+        return [v for k, l in self.tasks.items() if str(k).startswith("user:") for v in l]
+
     def broker_task_decorator(
         self,
         task_type: TaskType,
         container: BlockContainer | ContractEvent | None = None,
     ) -> Callable[[Callable], AsyncTaskiqDecoratedTask]:
         """
         Dynamically create a new broker task that handles tasks of ``task_type``.
```

### Comparing `silverback-0.5.0/silverback/exceptions.py` & `silverback-0.5.1/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/middlewares.py` & `silverback-0.5.1/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/recorder.py` & `silverback-0.5.1/silverback/recorder.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/runner.py` & `silverback-0.5.1/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/settings.py` & `silverback-0.5.1/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/state.py` & `silverback-0.5.1/silverback/state.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/subscriptions.py` & `silverback-0.5.1/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback/types.py` & `silverback-0.5.1/silverback/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 logger = get_logger(__name__)
 
 
 class TaskType(str, Enum):
     # System-only Tasks
     SYSTEM_CONFIG = "system:config"
     SYSTEM_USER_TASKDATA = "system:user-taskdata"
+    SYSTEM_USER_ALL_TASKDATA = "system:user-all-taskdata"
 
     # User-accessible Tasks
     STARTUP = "user:startup"
     NEW_BLOCK = "user:new-block"
     EVENT_LOG = "user:event-log"
     SHUTDOWN = "user:shutdown"
```

### Comparing `silverback-0.5.0/silverback/utils.py` & `silverback-0.5.1/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback.egg-info/PKG-INFO` & `silverback-0.5.1/silverback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.5.0
+Version: 0.5.1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.5.0/silverback.egg-info/SOURCES.txt` & `silverback-0.5.1/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/silverback.egg-info/requires.txt` & `silverback-0.5.1/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.5.0/tests/test_types.py` & `silverback-0.5.1/tests/test_types.py`

 * *Files identical despite different names*


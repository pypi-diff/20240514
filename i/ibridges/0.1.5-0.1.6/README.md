# Comparing `tmp/ibridges-0.1.5.tar.gz` & `tmp/ibridges-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibridges-0.1.5.tar", last modified: Fri May  3 10:03:07 2024, max compression
+gzip compressed data, was "ibridges-0.1.6.tar", last modified: Tue May 14 10:25:29 2024, max compression
```

## Comparing `ibridges-0.1.5.tar` & `ibridges-0.1.6.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:03:00.000000 ibridges-0.1.5/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.907883 ibridges-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/integration-tests-irods.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/integration-tests-yoda.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-03 10:03:00.000000 ibridges-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 10:03:00.000000 ibridges-0.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 10:03:00.000000 ibridges-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-03 10:03:07.931883 ibridges-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-03 10:03:00.000000 ibridges-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog/init-user-db.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_catalog_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/setup-4.3.1.input
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/setup-4.3.2.input
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.907883 ibridges-0.1.5/docker/irods_client/environments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/environments/plain-irods/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/irods_environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/environments/yoda/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/yoda/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/yoda/irods_environment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/beach.rtf
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/bunny.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/example.r
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/testdata/more_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/more_data/polarbear.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/plant.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/sun.rtf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docker/irods_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_data_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/ibridges/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/data_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/export_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/icat_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/tickets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/ibridges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-03 10:03:00.000000 ibridges-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:03:07.931883 ibridges-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/test_irodspath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/testdata/bunny.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/testdata/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/testdata/subfolder/sun.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.927883 ibridges-0.1.5/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/01-Setup-and-connect.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/02-Working-with-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/03-iRODS-Paths.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/04-Metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/05-Data-Sharing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/Data_sync.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/QuickStart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.927883 ibridges-0.1.5/tutorials/example_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/example_rules/example.r
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/iRODS_paths.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject1.png
--rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject2.png
--rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject3.png
--rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject4.png
--rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject5.png
--rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject6.png
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/Save_json.png
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/Yoda_environment.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.904852 ibridges-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:25:24.000000 ibridges-0.1.6/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.880852 ibridges-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/integration-tests-irods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/integration-tests-yoda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-14 10:25:24.000000 ibridges-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 10:25:24.000000 ibridges-0.1.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 10:25:24.000000 ibridges-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-14 10:25:29.904852 ibridges-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-14 10:25:24.000000 ibridges-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog/init-user-db.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_catalog_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/setup-4.3.1.input
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/setup-4.3.2.input
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.880852 ibridges-0.1.6/docker/irods_client/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/environments/plain-irods/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/irods_environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/environments/yoda/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/yoda/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/yoda/irods_environment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/beach.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/bunny.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/testdata/more_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/more_data/polarbear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/plant.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/sun.rtf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_data_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.892852 ibridges-0.1.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.892852 ibridges-0.1.6/ibridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/data_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/export_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/icat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.900852 ibridges-0.1.6/ibridges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 10:25:24.000000 ibridges-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:25:29.904852 ibridges-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/test_irodspath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/testdata/bunny.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/testdata/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/testdata/subfolder/sun.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/01-Setup-and-connect.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/02-Working-with-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/03-iRODS-Paths.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/04-Metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/05-Data-Sharing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/Data_sync.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/QuickStart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tutorials/example_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/example_rules/example.r
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/iRODS_paths.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.900852 ibridges-0.1.6/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/Save_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/Yoda_environment.png
```

### Comparing `ibridges-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `ibridges-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `ibridges-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.github/workflows/integration-tests-irods.yml` & `ibridges-0.1.6/.github/workflows/integration-tests-irods.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.github/workflows/integration-tests-yoda.yml` & `ibridges-0.1.6/.github/workflows/integration-tests-yoda.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.github/workflows/main.yml` & `ibridges-0.1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.github/workflows/pypi_release.yml` & `ibridges-0.1.6/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.gitignore` & `ibridges-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/.readthedocs.yaml` & `ibridges-0.1.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/LICENSE` & `ibridges-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/PKG-INFO` & `ibridges-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ibridges-0.1.5/README.md` & `ibridges-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/.gitattributes` & `ibridges-0.1.6/docker/.gitattributes`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/README.md` & `ibridges-0.1.6/docker/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_catalog_provider/Dockerfile` & `ibridges-0.1.6/docker/irods_catalog_provider/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_catalog_provider/entrypoint.sh` & `ibridges-0.1.6/docker/irods_catalog_provider/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/Dockerfile` & `ibridges-0.1.6/docker/irods_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/entrypoint.sh` & `ibridges-0.1.6/docker/irods_client/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/environments/yoda/config.toml` & `ibridges-0.1.6/docker/irods_client/environments/yoda/config.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/environments/yoda/irods_environment.json` & `ibridges-0.1.6/docker/irods_client/environments/yoda/irods_environment.json`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/testdata/beach.rtf` & `ibridges-0.1.6/docker/irods_client/testdata/beach.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/testdata/bunny.rtf` & `ibridges-0.1.6/docker/irods_client/testdata/bunny.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/testdata/more_data/polarbear.txt` & `ibridges-0.1.6/docker/irods_client/testdata/more_data/polarbear.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/testdata/plant.rtf` & `ibridges-0.1.6/docker/irods_client/testdata/plant.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/testdata/sun.rtf` & `ibridges-0.1.6/docker/irods_client/testdata/sun.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/conftest.py` & `ibridges-0.1.6/docker/irods_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_cli.py` & `ibridges-0.1.6/docker/irods_client/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_data_ops.py` & `ibridges-0.1.6/docker/irods_client/tests/test_data_ops.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_meta.py` & `ibridges-0.1.6/docker/irods_client/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_permissions.py` & `ibridges-0.1.6/docker/irods_client/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_session.py` & `ibridges-0.1.6/docker/irods_client/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_sync.py` & `ibridges-0.1.6/docker/irods_client/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker/irods_client/tests/test_ticket.py` & `ibridges-0.1.6/docker/irods_client/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docker-compose.yml` & `ibridges-0.1.6/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/Makefile` & `ibridges-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/make.bat` & `ibridges-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/api.rst` & `ibridges-0.1.6/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/cli.rst` & `ibridges-0.1.6/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/conf.py` & `ibridges-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/faq.rst` & `ibridges-0.1.6/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/index.rst` & `ibridges-0.1.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/docs/source/quickstart.rst` & `ibridges-0.1.6/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/__init__.py` & `ibridges-0.1.6/ibridges/__init__.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/__main__.py` & `ibridges-0.1.6/ibridges/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,25 +28,30 @@
         Download a data object or collection from the iRODS server.
     upload:
         Upload a file or directory to the iRODS server
         (which converts it to a data object/collection respectively).
     sync:
         Synchronize files/folders and data objects/collections with each other.
         Only updated files will be downloaded/uploaded.
+    list:
+        List the content of a collections, if no path is given, the home collection will be listed.
+    midir:
+        Create the collection and all its parent collections.
 
 The iBridges CLI does not implement the complete iBridges API. For example, there
 are no commands to modify metadata on the irods server.
 
 Example usage:
 
 ibridges download "irods:~/test.txt"
 ibridges upload ~/test.txt "irods:/test"
 ibridges init
-ibridges sync ~/collection "irods:~/collection"
+ibridges sync ~/directory "irods:~/collection"
 ibridges list irods:~/collection
+ibridges mkcoll irods://~/bli/bla/blubb
 
 Program information:
     -v, --version - display CLI version and exit
     -h, --help    - display this help file and exit
 """
 
 IBRIDGES_CONFIG_FP = Path.home() / ".ibridges" / "ibridges_cli.json"
@@ -69,14 +74,16 @@
         ibridges_upload()
     elif subcommand == "sync":
         ibridges_sync()
     elif subcommand == "init":
         ibridges_init()
     elif subcommand == "list":
         ibridges_list()
+    elif subcommand == "mkcoll":
+        ibridges_mkcoll()
     else:
         print(f"Invalid subcommand ({subcommand}). For help see ibridges --help")
         sys.exit(1)
 
 def _set_ienv_path(ienv_path: Union[None, str, Path]):
     try:
         with open(IBRIDGES_CONFIG_FP, "r", encoding="utf-8") as handle:
@@ -151,14 +158,35 @@
         nargs="?",
     )
 
     args, _ = parser.parse_known_args()
     with interactive_auth(irods_env_path=_get_ienv_path()) as session:
         _list_coll(session, _parse_remote(args.remote_path, session))
 
+def _create_coll(session: Session, remote_path: IrodsPath):
+    if remote_path.exists():
+        raise ValueError(f'New collection path {remote_path} already exists.')
+    remote_path.create_collection(session, remote_path)
+
+def ibridges_mkcoll():
+    """Create a collection with all its parents given the new path"""
+    parser = argparse.ArgumentParser(
+        prog="ibridges mkcoll",
+        description="Create a new collecion with all its parent collections."
+    )
+    parser.add_argument(
+        "remote_path",
+        help="Path to a new collection, should start with 'irods:'.",
+        type=str,
+    )
+
+    args, _ = parser.parse_known_args()
+    with interactive_auth(irods_env_path=_get_ienv_path()) as session:
+        _create_coll(session, _parse_remote(args.remote_path, session))
+
 def _parse_local(local_path: Union[None, str, Path]) -> Path:
     if local_path is None:
         return Path.cwd()
     if isinstance(local_path, str):
         if local_path.startswith("irods:"):
             raise ValueError("Please provide a local path (not starting with 'irods:')")
         local_path = Path(local_path)
```

### Comparing `ibridges-0.1.5/ibridges/data_operations.py` & `ibridges-0.1.6/ibridges/data_operations.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/export_metadata.py` & `ibridges-0.1.6/ibridges/export_metadata.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/icat_columns.py` & `ibridges-0.1.6/ibridges/icat_columns.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/interactive.py` & `ibridges-0.1.6/ibridges/interactive.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/meta.py` & `ibridges-0.1.6/ibridges/meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/path.py` & `ibridges-0.1.6/ibridges/path.py`

 * *Files 22% similar despite different names*

```diff
@@ -132,17 +132,52 @@
         """
         try:
             return session.irods_session.collections.create(str(coll_path))
         except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
             raise PermissionError(
                 "While creating collection '{coll_path}': iRODS server forbids action.") from exc
 
-    def rename(self):
-        """Rename the collection or data object."""
-        raise NotImplementedError("Rename not implemented yet.")
+    def rename(self, new_name: Union[str, IrodsPath]) -> IrodsPath:
+        """Change the name or the path of a data object or collection.
+        New collections on the path will be created.
+        
+        Parameters
+        ----------
+        new_name: str or IrodsPath
+            new name or a new full path
+        """
+
+        if not self.exists():
+            raise ValueError(f'str{self} does not exist.')
+
+        # Build new path
+        if str(new_name).startswith('/'+self.session.zone):
+            new_path = IrodsPath(self.session, new_name)
+        else:
+            new_path = self.parent.joinpath(new_name)
+
+        try:
+            # Make sure new path exists on iRODS server
+            if not new_path.parent.exists():
+                self.create_collection(self.session, new_path.parent)
+
+            if self.dataobject_exists():
+                self.session.irods_session.data_objects.move(str(self), str(new_path))
+            else:
+                self.session.irods_session.collections.move(str(self), str(new_path))
+            return new_path
+
+        except irods.exception.SAME_SRC_DEST_PATHS_ERR as err:
+            raise ValueError(f'Path {new_path} already exists.') from err
+        except irods.exception.SYS_CROSS_ZONE_MV_NOT_SUPPORTED as err:
+            raise ValueError(
+                    f'Path {new_path} needs to start with /{self.session.zone}/home') from err
+        except irods.exception.CAT_NO_ACCESS_PERMISSION as err:
+            raise PermissionError(f'Not allowed to move data to {new_path}') from err
+
 
     def collection_exists(self) -> bool:
         """Check if the path points to an iRODS collection."""
         return self.session.irods_session.collections.exists(str(self))
 
     def dataobject_exists(self) -> bool:
         """Check if the path points to an iRODS data object."""
```

### Comparing `ibridges-0.1.5/ibridges/permissions.py` & `ibridges-0.1.6/ibridges/permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/resources.py` & `ibridges-0.1.6/ibridges/resources.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/rules.py` & `ibridges-0.1.6/ibridges/rules.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/search.py` & `ibridges-0.1.6/ibridges/search.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/session.py` & `ibridges-0.1.6/ibridges/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """session operations."""
 from __future__ import annotations
 
 import json
-import warnings
 import socket
+import warnings
 from pathlib import Path
 from typing import Optional, Union
 
 import irods.session
 from irods.exception import (
     CAT_INVALID_AUTHENTICATION,
     CAT_INVALID_USER,
@@ -108,42 +108,47 @@
         -------
         bool
             Is the session valid?
 
         """
         return self.irods_session is not None and self.server_version != ()
 
-    def _network_check(self, hostname: str, port: int) -> bool:
+    @classmethod
+    def network_check(cls, hostname: str, port: int) -> bool:
         """Check connectivity to an iRODS server.
 
         Parameters
         ----------
         hostname : str
             FQDN/IP of an iRODS server.
+        port : int
+            Port to which to connect to the server
 
         Returns
         -------
         bool
             Connection to `hostname` possible.
 
         """
+        if hostname is None or port is None:
+            raise LoginError("No host or port set in environment file.")
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             try:
                 sock.settimeout(10.0)
-                sock.connect((hostname, port))
+                sock.connect((hostname, int(port)))
                 return True
             except socket.error:
                 return False
 
 
     def connect(self) -> iRODSSession:
         """Establish an iRODS session."""
-        irods_host = self._irods_env.get('irods_host', '')
-        irods_port = int(self._irods_env.get('irods_port', ''))
-        network = self._network_check(irods_host, irods_port)
+        irods_host = self._irods_env.get('irods_host', None)
+        irods_port = self._irods_env.get('irods_port', None)
+        network = self.network_check(irods_host, irods_port)
         if network is False:
             raise ConnectionError(f'No internet connection to {irods_host} and port {irods_port}')
         user = self._irods_env.get('irods_user_name', '')
         if user == 'anonymous':
             # TODOx: implement and test for SSL enabled iRODS
             # self.irods_session = iRODSSession(user='anonymous',
             #                        password='',
@@ -249,27 +254,25 @@
 
         """
         try:
             return self.irods_session.server_version
         except Exception as e:
             raise _translate_irods_error(e) from e
 
-
     def get_user_info(self) -> tuple[list, list]:
         """Query for user type and groups.
 
         Returns
         -------
         list
             iRODS user type names
         list
             iRODS group names
 
         """
-
         query = self.irods_session.query(icat.USER_TYPE).filter(icat.LIKE(
             icat.USER_NAME, self.username))
         user_type = [
             list(result.values())[0] for result in query.get_results()
         ][0]
         query = self.irods_session.query(icat.USER_GROUP_NAME).filter(icat.LIKE(
             icat.USER_NAME, self.username))
@@ -279,24 +282,26 @@
         return user_type, user_groups
 
 
 class LoginError(AttributeError):
     """Error indicating a failure to log into the iRODS server due to the configuration."""
 
 class PasswordError(ValueError):
-    """Error indicating failure to log into the iRODS server due to wrong or outdated password"""
+    """Error indicating failure to log into the iRODS server due to wrong or outdated password."""
 
 
 
 def _translate_irods_error(exc) -> Exception:  # pylint: disable=too-many-return-statements
     if isinstance(exc, NetworkException):
         if any((a.startswith('Client-Server negotiation failure') for a in exc.args)):
             return LoginError("Host, port, irods_client_server_policy or "
                               "irods_client_server_negotiation not set correctly in "
                               "irods_environment.json")
+    if isinstance(exc, TypeError):
+        return LoginError(f"Add info to irods_environment.json: {exc.args}")
     if isinstance(exc, CAT_INVALID_USER):
         return PasswordError("User credentials are not accepted")
     if isinstance(exc, PAM_AUTH_PASSWORD_FAILED):
         return PasswordError("Wrong password")
     if isinstance(exc, CAT_PASSWORD_EXPIRED):
         return PasswordError("Cached password is expired")
     if isinstance(exc, CAT_INVALID_AUTHENTICATION):
```

### Comparing `ibridges-0.1.5/ibridges/sync.py` & `ibridges-0.1.6/ibridges/sync.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges/tickets.py` & `ibridges-0.1.6/ibridges/tickets.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/ibridges.egg-info/PKG-INFO` & `ibridges-0.1.6/ibridges.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ibridges-0.1.5/ibridges.egg-info/SOURCES.txt` & `ibridges-0.1.6/ibridges.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .dockerignore
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 docker-compose.yml
 pyproject.toml
+.github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/integration-tests-irods.yml
 .github/workflows/integration-tests-yoda.yml
 .github/workflows/main.yml
 .github/workflows/pypi_release.yml
 docker/.gitattributes
@@ -32,14 +33,15 @@
 docker/irods_client/testdata/plant.rtf
 docker/irods_client/testdata/sun.rtf
 docker/irods_client/testdata/more_data/polarbear.txt
 docker/irods_client/tests/conftest.py
 docker/irods_client/tests/test_cli.py
 docker/irods_client/tests/test_data_ops.py
 docker/irods_client/tests/test_meta.py
+docker/irods_client/tests/test_move.py
 docker/irods_client/tests/test_permissions.py
 docker/irods_client/tests/test_resources.py
 docker/irods_client/tests/test_rules.py
 docker/irods_client/tests/test_session.py
 docker/irods_client/tests/test_sync.py
 docker/irods_client/tests/test_ticket.py
 docs/Makefile
```

### Comparing `ibridges-0.1.5/pyproject.toml` & `ibridges-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tests/test_irodspath.py` & `ibridges-0.1.6/tests/test_irodspath.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tests/testdata/bunny.txt` & `ibridges-0.1.6/tests/testdata/bunny.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tests/testdata/subfolder/sun.csv` & `ibridges-0.1.6/tests/testdata/subfolder/sun.csv`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/01-Setup-and-connect.ipynb` & `ibridges-0.1.6/tutorials/01-Setup-and-connect.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/02-Working-with-data.ipynb` & `ibridges-0.1.6/tutorials/02-Working-with-data.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/03-iRODS-Paths.ipynb` & `ibridges-0.1.6/tutorials/03-iRODS-Paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/04-Metadata.ipynb` & `ibridges-0.1.6/tutorials/04-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/05-Data-Sharing.ipynb` & `ibridges-0.1.6/tutorials/05-Data-Sharing.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/Data_sync.ipynb` & `ibridges-0.1.6/tutorials/Data_sync.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/QuickStart.ipynb` & `ibridges-0.1.6/tutorials/QuickStart.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/iRODS_paths.ipynb` & `ibridges-0.1.6/tutorials/iRODS_paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject1.png` & `ibridges-0.1.6/tutorials/img/DataObject1.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject2.png` & `ibridges-0.1.6/tutorials/img/DataObject2.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject3.png` & `ibridges-0.1.6/tutorials/img/DataObject3.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject4.png` & `ibridges-0.1.6/tutorials/img/DataObject4.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject5.png` & `ibridges-0.1.6/tutorials/img/DataObject5.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/DataObject6.png` & `ibridges-0.1.6/tutorials/img/DataObject6.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/Save_json.png` & `ibridges-0.1.6/tutorials/img/Save_json.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.5/tutorials/img/Yoda_environment.png` & `ibridges-0.1.6/tutorials/img/Yoda_environment.png`

 * *Files identical despite different names*


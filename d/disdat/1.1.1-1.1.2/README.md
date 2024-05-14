# Comparing `tmp/disdat-1.1.1.tar.gz` & `tmp/disdat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disdat-1.1.1.tar", last modified: Tue Apr 23 18:31:45 2024, max compression
+gzip compressed data, was "disdat-1.1.2.tar", last modified: Tue May 14 20:47:40 2024, max compression
```

## Comparing `disdat-1.1.1.tar` & `disdat-1.1.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.289847 disdat-1.1.1/
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.240858 disdat-1.1.1/.github/
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.251837 disdat-1.1.1/.github/workflows/
--rwxrwxrwx   0 kyocum     (503) staff       (20)     1538 2021-06-18 01:03:37.000000 disdat-1.1.1/.github/workflows/python-publish.yml
--rwxrwxrwx   0 kyocum     (503) staff       (20)      106 2021-06-18 01:03:37.000000 disdat-1.1.1/.gitignore
--rwxrwxrwx   0 kyocum     (503) staff       (20)    11388 2018-01-16 21:55:45.000000 disdat-1.1.1/LICENSE.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)      164 2022-01-20 01:37:06.000000 disdat-1.1.1/MANIFEST.in
--rwxrwxrwx   0 kyocum     (503) staff       (20)      661 2022-01-20 01:37:06.000000 disdat-1.1.1/NOTICE.txt
--rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-04-23 18:31:45.289367 disdat-1.1.1/PKG-INFO
--rwxrwxrwx   0 kyocum     (503) staff       (20)     2230 2022-04-18 17:07:06.000000 disdat-1.1.1/README.rst
--rwxr-xr-x   0 kyocum     (503) staff       (20)      575 2024-03-09 23:18:32.000000 disdat-1.1.1/build-dist.sh
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.258745 disdat-1.1.1/disdat/
--rwxrwxrwx   0 kyocum     (503) staff       (20)       18 2022-01-07 19:22:09.000000 disdat-1.1.1/disdat/.gitignore
--rw-r--r--   0 kyocum     (503) staff       (20)      739 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2027 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/add.py
--rw-r--r--   0 kyocum     (503) staff       (20)    50251 2024-04-23 18:30:53.000000 disdat-1.1.1/disdat/api.py
--rw-r--r--   0 kyocum     (503) staff       (20)     8241 2024-04-23 00:27:52.000000 disdat-1.1.1/disdat/common.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.262500 disdat-1.1.1/disdat/config/
--rwxrwxrwx   0 kyocum     (503) staff       (20)       85 2022-01-07 19:22:09.000000 disdat-1.1.1/disdat/config/README.md
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.1/disdat/config/__init__.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.263206 disdat-1.1.1/disdat/config/disdat/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.1/disdat/config/disdat/.exclude-from-modeler-docker-image
--rwxrwxrwx   0 kyocum     (503) staff       (20)       70 2022-01-20 01:37:06.000000 disdat-1.1.1/disdat/config/disdat/disdat.cfg
--rw-r--r--   0 kyocum     (503) staff       (20)      702 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/constants.py
--rw-r--r--   0 kyocum     (503) staff       (20)    55557 2024-04-23 00:27:52.000000 disdat-1.1.1/disdat/data_context.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.263699 disdat-1.1.1/disdat/entrypoints/
--rw-r--r--   0 kyocum     (503) staff       (20)     4015 2024-04-18 00:02:53.000000 disdat-1.1.1/disdat/entrypoints/cli_ep.py
--rw-r--r--   0 kyocum     (503) staff       (20)      589 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/exceptions.py
--rw-r--r--   0 kyocum     (503) staff       (20)    67416 2024-04-23 00:27:52.000000 disdat-1.1.1/disdat/fs.py
--rw-r--r--   0 kyocum     (503) staff       (20)    73618 2024-04-23 00:27:52.000000 disdat-1.1.1/disdat/hyperframe.py
--rw-r--r--   0 kyocum     (503) staff       (20)    56763 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/hyperframe_pb2.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4480 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/lineage.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2129 2024-04-17 22:38:16.000000 disdat-1.1.1/disdat/log.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1899 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/resource.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.264815 disdat-1.1.1/disdat/utility/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-20 01:37:06.000000 disdat-1.1.1/disdat/utility/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)    17841 2024-04-23 00:38:16.000000 disdat-1.1.1/disdat/utility/asyncio_aws_s3.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1623 2024-04-17 16:18:22.000000 disdat-1.1.1/disdat/utility/bundle_helpers.py
--rwxrwxrwx   0 kyocum     (503) staff       (20)       21 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat/version.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.288183 disdat-1.1.1/disdat.egg-info/
--rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/PKG-INFO
--rwxrwxrwx   0 kyocum     (503) staff       (20)     2004 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/SOURCES.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)        1 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/dependency_links.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)       56 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/entry_points.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)      234 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/requires.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)        7 2024-04-23 18:31:45.000000 disdat-1.1.1/disdat.egg-info/top_level.txt
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.265589 disdat-1.1.1/docs/
--rwxrwxrwx   0 kyocum     (503) staff       (20)     5120 2021-06-18 01:03:37.000000 disdat-1.1.1/docs/DisdatTitleFig.jpg
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.266065 disdat-1.1.1/infrastructure/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      754 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/.gitignore
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.266507 disdat-1.1.1/infrastructure/Dockerfiles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      292 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/Makefile
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.269167 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      285 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/Dockerfile
--rwxrwxrwx   0 kyocum     (503) staff       (20)      270 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/Makefile
--rwxrwxrwx   0 kyocum     (503) staff       (20)      264 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/README.md
--rwxrwxrwx   0 kyocum     (503) staff       (20)     2327 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/bundle.proto
--rwxrwxrwx   0 kyocum     (503) staff       (20)     6190 2022-01-20 01:37:06.000000 disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto
--rw-r--r--   0 kyocum     (503) staff       (20)       38 2024-04-23 18:31:45.289931 disdat-1.1.1/setup.cfg
--rw-r--r--   0 kyocum     (503) staff       (20)     3804 2024-04-17 16:18:22.000000 disdat-1.1.1/setup.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.269922 disdat-1.1.1/tests/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.1/tests/__init__.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.271627 disdat-1.1.1/tests/bundles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2020-05-15 07:06:53.000000 disdat-1.1.1/tests/bundles/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1332 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/bundles/test_arg_capture.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4752 2024-04-23 00:27:52.000000 disdat-1.1.1/tests/bundles/test_file_bundle_api.py
--rw-r--r--   0 kyocum     (503) staff       (20)    11110 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/bundles/test_hframe.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.277164 disdat-1.1.1/tests/data/
--rwxrwxrwx   0 kyocum     (503) staff       (20)  8918348 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/US_chronic_disease_indicators_CDI_2012.csv
--rwxrwxrwx   0 kyocum     (503) staff       (20)      485 2019-05-18 00:15:09.000000 disdat-1.1.1/tests/data/test_bundle_file.csv
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.282430 disdat-1.1.1/tests/data/testfiles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/A
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/B
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/C
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/D
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/E
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/F
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/G
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/H
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/I
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.1/tests/data/testfiles/J
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 18:31:45.287635 disdat-1.1.1/tests/functional/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.1/tests/functional/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)     3201 2024-04-23 00:27:52.000000 disdat-1.1.1/tests/functional/common.py
--rw-r--r--   0 kyocum     (503) staff       (20)     7255 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_add.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2695 2024-04-23 00:27:52.000000 disdat-1.1.1/tests/functional/test_add_remote.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2159 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_cat.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1742 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_context.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1067 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_hyperframe.py
--rw-r--r--   0 kyocum     (503) staff       (20)     8801 2024-04-23 00:27:52.000000 disdat-1.1.1/tests/functional/test_link_localization.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4157 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_output_types.py
--rw-r--r--   0 kyocum     (503) staff       (20)     3109 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/functional/test_remote.py
--rw-r--r--   0 kyocum     (503) staff       (20)      217 2024-04-17 16:18:22.000000 disdat-1.1.1/tests/setup.py
--rw-r--r--   0 kyocum     (503) staff       (20)      736 2024-04-17 16:18:22.000000 disdat-1.1.1/tox.ini
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.476458 disdat-1.1.2/
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.419381 disdat-1.1.2/.github/
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.431316 disdat-1.1.2/.github/workflows/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     1538 2021-06-18 01:03:37.000000 disdat-1.1.2/.github/workflows/python-publish.yml
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      106 2021-06-18 01:03:37.000000 disdat-1.1.2/.gitignore
+-rwxrwxrwx   0 kyocum     (503) staff       (20)    11388 2018-01-16 21:55:45.000000 disdat-1.1.2/LICENSE.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      164 2022-01-20 01:37:06.000000 disdat-1.1.2/MANIFEST.in
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      661 2022-01-20 01:37:06.000000 disdat-1.1.2/NOTICE.txt
+-rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-05-14 20:47:40.475868 disdat-1.1.2/PKG-INFO
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     2230 2022-04-18 17:07:06.000000 disdat-1.1.2/README.rst
+-rwxr-xr-x   0 kyocum     (503) staff       (20)      575 2024-03-09 23:18:32.000000 disdat-1.1.2/build-dist.sh
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.441357 disdat-1.1.2/disdat/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       18 2022-01-07 19:22:09.000000 disdat-1.1.2/disdat/.gitignore
+-rw-r--r--   0 kyocum     (503) staff       (20)      739 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2027 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/add.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    50243 2024-05-14 20:46:01.000000 disdat-1.1.2/disdat/api.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     8241 2024-04-23 00:27:52.000000 disdat-1.1.2/disdat/common.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.446954 disdat-1.1.2/disdat/config/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       85 2022-01-07 19:22:09.000000 disdat-1.1.2/disdat/config/README.md
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.2/disdat/config/__init__.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.447643 disdat-1.1.2/disdat/config/disdat/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.2/disdat/config/disdat/.exclude-from-modeler-docker-image
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       70 2022-01-20 01:37:06.000000 disdat-1.1.2/disdat/config/disdat/disdat.cfg
+-rw-r--r--   0 kyocum     (503) staff       (20)      702 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/constants.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    55549 2024-05-14 20:46:01.000000 disdat-1.1.2/disdat/data_context.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.448077 disdat-1.1.2/disdat/entrypoints/
+-rw-r--r--   0 kyocum     (503) staff       (20)     4015 2024-04-18 00:02:53.000000 disdat-1.1.2/disdat/entrypoints/cli_ep.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      589 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/exceptions.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    67408 2024-05-14 20:46:01.000000 disdat-1.1.2/disdat/fs.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    73610 2024-05-14 20:46:01.000000 disdat-1.1.2/disdat/hyperframe.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    56763 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/hyperframe_pb2.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4480 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/lineage.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2129 2024-04-17 22:38:16.000000 disdat-1.1.2/disdat/log.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1899 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/resource.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.449829 disdat-1.1.2/disdat/utility/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-20 01:37:06.000000 disdat-1.1.2/disdat/utility/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    17841 2024-05-14 20:46:01.000000 disdat-1.1.2/disdat/utility/aws_s3.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1623 2024-04-17 16:18:22.000000 disdat-1.1.2/disdat/utility/bundle_helpers.py
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       21 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat/version.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.474407 disdat-1.1.2/disdat.egg-info/
+-rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/PKG-INFO
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     1996 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        1 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       56 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/entry_points.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      234 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/requires.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        7 2024-05-14 20:47:40.000000 disdat-1.1.2/disdat.egg-info/top_level.txt
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.450394 disdat-1.1.2/docs/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     5120 2021-06-18 01:03:37.000000 disdat-1.1.2/docs/DisdatTitleFig.jpg
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.450860 disdat-1.1.2/infrastructure/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      754 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/.gitignore
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.451354 disdat-1.1.2/infrastructure/Dockerfiles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      292 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/Makefile
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.454107 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      285 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/Dockerfile
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      270 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/Makefile
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      264 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/README.md
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     2327 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/bundle.proto
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     6190 2022-01-20 01:37:06.000000 disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto
+-rw-r--r--   0 kyocum     (503) staff       (20)       38 2024-05-14 20:47:40.476546 disdat-1.1.2/setup.cfg
+-rw-r--r--   0 kyocum     (503) staff       (20)     3804 2024-04-17 16:18:22.000000 disdat-1.1.2/setup.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.455117 disdat-1.1.2/tests/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.2/tests/__init__.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.457370 disdat-1.1.2/tests/bundles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2020-05-15 07:06:53.000000 disdat-1.1.2/tests/bundles/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1332 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/bundles/test_arg_capture.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4744 2024-05-14 20:46:01.000000 disdat-1.1.2/tests/bundles/test_file_bundle_api.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    11110 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/bundles/test_hframe.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.463524 disdat-1.1.2/tests/data/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)  8918348 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/US_chronic_disease_indicators_CDI_2012.csv
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      485 2019-05-18 00:15:09.000000 disdat-1.1.2/tests/data/test_bundle_file.csv
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.468346 disdat-1.1.2/tests/data/testfiles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/A
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/B
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/C
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/D
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/E
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/F
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/G
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/H
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/I
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.2/tests/data/testfiles/J
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-05-14 20:47:40.473617 disdat-1.1.2/tests/functional/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.2/tests/functional/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     3201 2024-04-23 00:27:52.000000 disdat-1.1.2/tests/functional/common.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     7255 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_add.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2695 2024-04-23 00:27:52.000000 disdat-1.1.2/tests/functional/test_add_remote.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2159 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_cat.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1742 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_context.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1067 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_hyperframe.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     8793 2024-05-14 20:46:01.000000 disdat-1.1.2/tests/functional/test_link_localization.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4157 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_output_types.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     3109 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/functional/test_remote.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      217 2024-04-17 16:18:22.000000 disdat-1.1.2/tests/setup.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      736 2024-04-17 16:18:22.000000 disdat-1.1.2/tox.ini
```

### Comparing `disdat-1.1.1/.github/workflows/python-publish.yml` & `disdat-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/LICENSE.txt` & `disdat-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/NOTICE.txt` & `disdat-1.1.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/PKG-INFO` & `disdat-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Disdat: data versioning
 Home-page: https://github.com/kyocum/disdat
 Author: Ken Yocum
 Author-email: kyocum@gmail.com
 License: Apache License, version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disdat-1.1.1/README.rst` & `disdat-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/build-dist.sh` & `disdat-1.1.2/build-dist.sh`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/__init__.py` & `disdat-1.1.2/disdat/__init__.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/add.py` & `disdat-1.1.2/disdat/add.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/api.py` & `disdat-1.1.2/disdat/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import urllib
 
 import disdat.common as common
 import disdat.fs
 from disdat import logger as _logger
 from disdat.data_context import DataContext
 from disdat.hyperframe import HyperFrameRecord, LineageRecord, parse_return_val
-from disdat.utility.asyncio_aws_s3 import s3_path_exists
+from disdat.utility.aws_s3 import s3_path_exists
 
 PROC_ID_TRUNCATE_HASH = 10  # 10 ls hex digits
 
 
 def _get_fs():
     """Initializing FS, which needs a config.
     These are both singletons.
```

### Comparing `disdat-1.1.1/disdat/common.py` & `disdat-1.1.2/disdat/common.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/constants.py` & `disdat-1.1.2/disdat/constants.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/data_context.py` & `disdat-1.1.2/disdat/data_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pandas as pd
 from sqlalchemy import create_engine
 
 import disdat.common as common
 import disdat.constants as constants
 import disdat.hyperframe as hyperframe
 import disdat.hyperframe_pb2 as hyperframe_pb2
-import disdat.utility.asyncio_aws_s3 as aws_s3
+import disdat.utility.aws_s3 as aws_s3
 from disdat import logger as _logger
 from disdat.common import DisdatConfig
 
 META_CTXT_FILE = "ctxt.json"
 DB_FILE = "ctxt.db"
 DEFAULT_LEN_UNCOMMITTED_HISTORY = 1
```

### Comparing `disdat-1.1.1/disdat/entrypoints/cli_ep.py` & `disdat-1.1.2/disdat/entrypoints/cli_ep.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/exceptions.py` & `disdat-1.1.2/disdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/fs.py` & `disdat-1.1.2/disdat/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from datetime import datetime
 from enum import Enum
 
 import pandas as pd
 
 import disdat.common as common
 import disdat.hyperframe as hyperframe
-import disdat.utility.asyncio_aws_s3 as aws_s3
+import disdat.utility.aws_s3 as aws_s3
 from disdat import logger as _logger
 from disdat.common import CatNoBundleError, DisdatConfig
 from disdat.data_context import DataContext
 
 CodeVersion = collections.namedtuple(
     "CodeVersion", "semver hash tstamp branch url dirty"
 )
```

### Comparing `disdat-1.1.1/disdat/hyperframe.py` & `disdat-1.1.2/disdat/hyperframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 )
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.sql import text
 
 import disdat.common as common
 from disdat import hyperframe_pb2
 from disdat import logger as _logger
-from disdat.utility.asyncio_aws_s3 import s3_path_exists
+from disdat.utility.aws_s3 import s3_path_exists
 
 HyperFrameTuple = namedtuple("HyperFrameTuple", "columns, links, uuid, tags")
 
 # UPSERT policy for inserts that violate constraints (explicit or primary key uniqueness)
 # We can ROLLBACK, ABORT, FAIL, IGNORE, and REPLACE
 # Most cases we want to REPLACE (UPSERT)
 UPSERT_POLICY = "FAIL"
```

### Comparing `disdat-1.1.1/disdat/hyperframe_pb2.py` & `disdat-1.1.2/disdat/hyperframe_pb2.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/lineage.py` & `disdat-1.1.2/disdat/lineage.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/log.py` & `disdat-1.1.2/disdat/log.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/resource.py` & `disdat-1.1.2/disdat/resource.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/utility/asyncio_aws_s3.py` & `disdat-1.1.2/disdat/utility/aws_s3.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat/utility/bundle_helpers.py` & `disdat-1.1.2/disdat/utility/bundle_helpers.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/disdat.egg-info/PKG-INFO` & `disdat-1.1.2/disdat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Disdat: data versioning
 Home-page: https://github.com/kyocum/disdat
 Author: Ken Yocum
 Author-email: kyocum@gmail.com
 License: Apache License, version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disdat-1.1.1/disdat.egg-info/SOURCES.txt` & `disdat-1.1.2/disdat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 disdat.egg-info/top_level.txt
 disdat/config/README.md
 disdat/config/__init__.py
 disdat/config/disdat/.exclude-from-modeler-docker-image
 disdat/config/disdat/disdat.cfg
 disdat/entrypoints/cli_ep.py
 disdat/utility/__init__.py
-disdat/utility/asyncio_aws_s3.py
+disdat/utility/aws_s3.py
 disdat/utility/bundle_helpers.py
 docs/DisdatTitleFig.jpg
 infrastructure/.gitignore
 infrastructure/Dockerfiles/Makefile
 infrastructure/Dockerfiles/hyperframe_def/Dockerfile
 infrastructure/Dockerfiles/hyperframe_def/Makefile
 infrastructure/Dockerfiles/hyperframe_def/README.md
```

### Comparing `disdat-1.1.1/docs/DisdatTitleFig.jpg` & `disdat-1.1.2/docs/DisdatTitleFig.jpg`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/infrastructure/.gitignore` & `disdat-1.1.2/infrastructure/.gitignore`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/bundle.proto` & `disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/bundle.proto`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto` & `disdat-1.1.2/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/setup.py` & `disdat-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/bundles/test_arg_capture.py` & `disdat-1.1.2/tests/bundles/test_arg_capture.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/bundles/test_file_bundle_api.py` & `disdat-1.1.2/tests/bundles/test_file_bundle_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 
 import boto3
 import moto
 import pytest
 
 import disdat.api as api
-import disdat.utility.asyncio_aws_s3 as aws_s3
+import disdat.utility.aws_s3 as aws_s3
 from tests.functional.common import TEST_CONTEXT, run_test
 
 #
 # Copyright 2017 Human Longevity, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `disdat-1.1.1/tests/bundles/test_hframe.py` & `disdat-1.1.2/tests/bundles/test_hframe.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/data/US_chronic_disease_indicators_CDI_2012.csv` & `disdat-1.1.2/tests/data/US_chronic_disease_indicators_CDI_2012.csv`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/common.py` & `disdat-1.1.2/tests/functional/common.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_add.py` & `disdat-1.1.2/tests/functional/test_add.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_add_remote.py` & `disdat-1.1.2/tests/functional/test_add_remote.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_cat.py` & `disdat-1.1.2/tests/functional/test_cat.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_context.py` & `disdat-1.1.2/tests/functional/test_context.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_hyperframe.py` & `disdat-1.1.2/tests/functional/test_hyperframe.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_link_localization.py` & `disdat-1.1.2/tests/functional/test_link_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import tempfile
 
 import boto3
 import moto
 import pytest
 
 import disdat.api as api
-import disdat.utility.asyncio_aws_s3 as aws_s3
+import disdat.utility.aws_s3 as aws_s3
 from tests.functional.common import TEST_CONTEXT
 
 TEST_REMOTE = "__test_remote_context__"
 TEST_BUCKET = "test-bucket"
 TEST_BUCKET_URL = "s3://{}".format(TEST_BUCKET)
```

### Comparing `disdat-1.1.1/tests/functional/test_output_types.py` & `disdat-1.1.2/tests/functional/test_output_types.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tests/functional/test_remote.py` & `disdat-1.1.2/tests/functional/test_remote.py`

 * *Files identical despite different names*

### Comparing `disdat-1.1.1/tox.ini` & `disdat-1.1.2/tox.ini`

 * *Files identical despite different names*


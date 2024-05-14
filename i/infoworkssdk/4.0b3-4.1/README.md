# Comparing `tmp/infoworkssdk-4.0b3.tar.gz` & `tmp/infoworkssdk-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoworkssdk-4.0b3.tar", last modified: Fri Oct  6 13:26:04 2023, max compression
+gzip compressed data, was "infoworkssdk-4.1.tar", last modified: Tue May 14 15:25:29 2024, max compression
```

## Comparing `infoworkssdk-4.0b3.tar` & `infoworkssdk-4.1.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.508104 infoworkssdk-4.0b3/
--rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-4.0b3/LICENSE
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-06 13:26:04.507946 infoworkssdk-4.0b3/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-4.0b3/README.md
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.476524 infoworkssdk-4.0b3/infoworks/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/__init__.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.477156 infoworkssdk-4.0b3/infoworks/core/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/core/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-4.0b3/infoworks/core/iw_authentication.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1234 2023-06-01 10:05:48.000000 infoworkssdk-4.0b3/infoworks/error.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.494209 infoworkssdk-4.0b3/infoworks/sdk/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)   113698 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/admin_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-4.0b3/infoworks/sdk/base_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.494753 infoworkssdk-4.0b3/infoworks/sdk/cicd/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-19 09:22:58.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/cicd_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.498949 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3791 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2368 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)    37501 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/utils.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.506388 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14064 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/cdata_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    21776 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/csv_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13654 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/domains.py
--rw-r--r--   0 infoworks   (501) staff       (20)      185 2023-05-15 06:02:14.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-18 15:08:53.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/misc.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7857 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
--rw-r--r--   0 infoworks   (501) staff       (20)    24801 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipelines.py
--rw-r--r--   0 infoworks   (501) staff       (20)    28163 2023-10-06 13:25:32.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13060 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2445 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/update_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14896 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/workflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)    23700 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
--rw-r--r--   0 infoworks   (501) staff       (20)    30204 2023-10-03 13:33:30.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrappersource.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12333 2023-08-08 15:52:16.000000 infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-08-08 16:16:36.000000 infoworkssdk-4.0b3/infoworks/sdk/client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    34243 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/domain_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.506720 infoworkssdk-4.0b3/infoworks/sdk/ejson/
--rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-4.0b3/infoworks/sdk/ejson/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-4.0b3/infoworks/sdk/generic_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-4.0b3/infoworks/sdk/jobmetrics.py
--rw-r--r--   0 infoworks   (501) staff       (20)    32292 2023-06-20 05:05:38.000000 infoworkssdk-4.0b3/infoworks/sdk/jobs_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-4.0b3/infoworks/sdk/jobs_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-4.0b3/infoworks/sdk/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    66566 2023-10-06 13:25:32.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    47632 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_group_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/pipeline_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    72307 2023-07-18 06:17:15.000000 infoworkssdk-4.0b3/infoworks/sdk/replicator_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)   193543 2023-08-25 14:58:31.000000 infoworkssdk-4.0b3/infoworks/sdk/source_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/source_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    83469 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/url_builder.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/utils.py
--rw-r--r--   0 infoworks   (501) staff       (20)    67499 2023-08-18 09:17:19.000000 infoworkssdk-4.0b3/infoworks/sdk/workflow_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-4.0b3/infoworks/sdk/workflow_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-10-06 13:26:04.507675 infoworkssdk-4.0b3/infoworkssdk.egg-info/
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     2425 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/SOURCES.txt
--rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/dependency_links.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       45 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/requires.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-10-06 13:26:04.000000 infoworkssdk-4.0b3/infoworkssdk.egg-info/top_level.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-10-06 13:26:04.508195 infoworkssdk-4.0b3/setup.cfg
--rw-r--r--   0 infoworks   (501) staff       (20)      907 2023-10-06 13:25:24.000000 infoworkssdk-4.0b3/setup.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.661300 infoworkssdk-4.1/
+-rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-4.1/LICENSE
+-rw-r--r--   0 infoworks   (501) staff       (20)     2568 2024-05-14 15:25:29.661136 infoworkssdk-4.1/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     1936 2024-04-12 07:54:29.000000 infoworkssdk-4.1/README.md
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.630361 infoworkssdk-4.1/infoworks/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/__init__.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.631120 infoworkssdk-4.1/infoworks/core/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/core/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-4.1/infoworks/core/iw_authentication.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1234 2023-06-01 10:05:48.000000 infoworkssdk-4.1/infoworks/error.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.644706 infoworkssdk-4.1/infoworks/sdk/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/sdk/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   133343 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/admin_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11446 2023-11-16 04:12:15.000000 infoworkssdk-4.1/infoworks/sdk/base_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.645222 infoworkssdk-4.1/infoworks/sdk/cicd/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.1/infoworks/sdk/cicd/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-19 09:22:58.000000 infoworkssdk-4.1/infoworks/sdk/cicd/cicd_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.648344 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-08-08 15:52:16.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-08-08 15:52:16.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3791 2023-10-30 10:02:13.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2457 2024-05-11 13:35:12.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-08-08 15:52:16.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-18 15:08:53.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    39723 2024-05-14 15:09:37.000000 infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/utils.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.659075 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-18 15:08:53.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    40388 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/cdata_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    26025 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/csv_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13654 2023-08-08 16:16:36.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/domains.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    23005 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/file_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    41844 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/generic_jdbc_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      185 2023-05-15 06:02:14.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-18 15:08:53.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/misc.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11030 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    23421 2023-12-14 11:01:12.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/pipelines.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    44754 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    16924 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    17754 2024-05-10 14:15:07.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/streaming_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2445 2023-10-26 03:10:09.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/update_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    14896 2023-08-08 15:52:16.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/workflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    23026 2023-12-14 11:01:12.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    86280 2024-05-14 13:05:01.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/wrappersource.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12333 2023-08-08 15:52:16.000000 infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-08-08 16:16:36.000000 infoworkssdk-4.1/infoworks/sdk/client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    39237 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/domain_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.659544 infoworkssdk-4.1/infoworks/sdk/ejson/
+-rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-4.1/infoworks/sdk/ejson/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-4.1/infoworks/sdk/generic_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    73131 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/jobmetrics.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    34266 2024-04-12 08:04:03.000000 infoworkssdk-4.1/infoworks/sdk/jobs_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-4.1/infoworks/sdk/jobs_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-4.1/infoworks/sdk/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    68864 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/pipeline_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    51048 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/pipeline_group_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/sdk/pipeline_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    72307 2023-07-18 06:17:15.000000 infoworkssdk-4.1/infoworks/sdk/replicator_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   217193 2024-05-10 14:15:07.000000 infoworkssdk-4.1/infoworks/sdk/source_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/sdk/source_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    91638 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/url_builder.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/sdk/utils.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    68273 2024-05-03 06:45:12.000000 infoworkssdk-4.1/infoworks/sdk/workflow_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-4.1/infoworks/sdk/workflow_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2024-05-14 15:25:29.660838 infoworkssdk-4.1/infoworkssdk.egg-info/
+-rw-r--r--   0 infoworks   (501) staff       (20)     2568 2024-05-14 15:25:29.000000 infoworkssdk-4.1/infoworkssdk.egg-info/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     2606 2024-05-14 15:25:29.000000 infoworkssdk-4.1/infoworkssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)        1 2024-05-14 15:25:29.000000 infoworkssdk-4.1/infoworkssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       54 2024-05-14 15:25:29.000000 infoworkssdk-4.1/infoworkssdk.egg-info/requires.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       10 2024-05-14 15:25:29.000000 infoworkssdk-4.1/infoworkssdk.egg-info/top_level.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2024-05-14 15:25:29.661381 infoworkssdk-4.1/setup.cfg
+-rw-r--r--   0 infoworks   (501) staff       (20)      912 2024-05-14 15:10:41.000000 infoworkssdk-4.1/setup.py
```

### Comparing `infoworkssdk-4.0b3/LICENSE` & `infoworkssdk-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/PKG-INFO` & `infoworkssdk-4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 4.0b3
-Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
+Version: 4.1
+Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.x onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,23 +46,30 @@
 ```
 ## Requirements
 
 Python 3.4+ (PyPy supported)
 
 ## Usage
 
-The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value:
+The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value.
+
+### Steps to get refresh token:
+
+https://docs.infoworks.io/infoworks-5.5.0/developer-resources/rest-api#using-refresh-token
 
 ```python
 from infoworks.sdk.client import InfoworksClientSDK
 # Your refresh token here
-refresh_token = "zThziQ7MoJJPYAha+U/+PBSTZG944F+SHBDs+m/z2qn8+m/ax8Prpzla1MHzQ5EBLzB2Bw8a+Qs9r6En5BEN2DsmUVJ6sKFb2yI2"
+protocol="https"
+host="<your infoworks hostname>"
+port="443"
+refresh_token = "<your_refresh_token>"
 # Initialise the client
 iwx_client = InfoworksClientSDK()
-iwx_client.initialize_client_with_defaults("http", "10.18.1.28", "3001", refresh_token)
+iwx_client.initialize_client_with_defaults(protocol=protocol, ip=host, port=port, refresh_token=refresh_token)
 ```
 ## Example
 
 Create Oracle Source
 ```
 src_create_response = iwx_client.create_source(source_config={
             "name": "iwx_sdk_srcname",
@@ -76,7 +83,8 @@
 ```
 
 ## Authors
 
 Nitin B.S (nitin.bs@infoworks.io)
 Abhishek Raviprasad (abhishek.raviprasad@infoworks.io)
 
+
```

### Comparing `infoworkssdk-4.0b3/README.md` & `infoworkssdk-4.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -31,23 +31,30 @@
 ```
 ## Requirements
 
 Python 3.4+ (PyPy supported)
 
 ## Usage
 
-The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value:
+The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value.
+
+### Steps to get refresh token:
+
+https://docs.infoworks.io/infoworks-5.5.0/developer-resources/rest-api#using-refresh-token
 
 ```python
 from infoworks.sdk.client import InfoworksClientSDK
 # Your refresh token here
-refresh_token = "zThziQ7MoJJPYAha+U/+PBSTZG944F+SHBDs+m/z2qn8+m/ax8Prpzla1MHzQ5EBLzB2Bw8a+Qs9r6En5BEN2DsmUVJ6sKFb2yI2"
+protocol="https"
+host="<your infoworks hostname>"
+port="443"
+refresh_token = "<your_refresh_token>"
 # Initialise the client
 iwx_client = InfoworksClientSDK()
-iwx_client.initialize_client_with_defaults("http", "10.18.1.28", "3001", refresh_token)
+iwx_client.initialize_client_with_defaults(protocol=protocol, ip=host, port=port, refresh_token=refresh_token)
 ```
 ## Example
 
 Create Oracle Source
 ```
 src_create_response = iwx_client.create_source(source_config={
             "name": "iwx_sdk_srcname",
@@ -59,8 +66,8 @@
             "is_source_ingested": True
         })
 ```
 
 ## Authors
 
 Nitin B.S (nitin.bs@infoworks.io)
-Abhishek Raviprasad (abhishek.raviprasad@infoworks.io)
+Abhishek Raviprasad (abhishek.raviprasad@infoworks.io)
```

### Comparing `infoworkssdk-4.0b3/infoworks/core/iw_authentication.py` & `infoworkssdk-4.1/infoworks/core/iw_authentication.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/error.py` & `infoworkssdk-4.1/infoworks/error.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/admin_client.py` & `infoworkssdk-4.1/infoworks/sdk/admin_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 class AdminClient(BaseClient):
     def __init__(self):
         super(AdminClient, self).__init__()
         self._datalineage = {"path": [], "dataflow_objects": [], "master_pipeline_ids": [],
                              "master_sourcetable_ids": []}
 
-    def list_users(self, params=None):
+    def list_users(self, params=None, pagination=True):
         """
         Function to list the users
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_users = url_builder.list_users_url(self.client_config) + IWUtils.get_query_params_string_from_dict(
             params=params)
 
@@ -29,14 +31,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_users,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     users_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -170,21 +174,23 @@
                                                     error_desc=parsed_response.get("details",
                                                                                    "Error in deleting user ")
                                                     )
         except Exception as e:
             self.logger.error("Error in deleting user " + str(e))
             raise AdminError("Error in deleting user " + str(e))
 
-    def get_user_details(self, user_id=None, params=None):
+    def get_user_details(self, user_id=None, params=None, pagination=True):
         """
         Function to get the user details
         :param user_id: Entity identifier of the user
         :type user_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         if user_id is not None:
             url_to_list_user_details = url_builder.list_users_url(self.client_config) + f"/{user_id}"
         else:
@@ -199,14 +205,16 @@
                 initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 if user_id is not None:
                     users_list.extend([result])
                 else:
                     while len(result) > 0:
                         users_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -455,21 +463,23 @@
         if sourcetable_ids is not None:
             self._datalineage["master_sourcetable_ids"].extend(sourcetable_ids.split(","))
         while len(self._datalineage["master_sourcetable_ids"]) > 0:
             src_table_id = self._datalineage["master_sourcetable_ids"].pop()
             src_id, table_id = src_table_id.split(":")
             self.alation_compatible_lineage_for_source(src_id, table_id)
 
-    def get_environment_details(self, environment_id=None, params=None):
+    def get_environment_details(self, environment_id=None, params=None, pagination=True):
         """
         Function to get environment details
         :param environment_id: Entity identifier of the environment
         :type environment_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type params: Dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by limit under params
+        :type pagination: Boolean
         :return: Response Dict
         """
         if params is None and environment_id is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_environments = url_builder.get_environment_details(
             self.client_config, environment_id) + IWUtils.get_query_params_string_from_dict(params=params)
         env_details = []
@@ -488,14 +498,16 @@
                                                         )
                 initial_msg = response.get("message", "")
                 if environment_id is not None:
                     env_details.extend([result])
                 else:
                     while len(result) > 0:
                         env_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -571,23 +583,25 @@
                                                     error_desc=parsed_response.get("details",
                                                                                    "Error in updating environment ")
                                                     )
         except Exception as e:
             self.logger.error("Error in updating environment" + str(e))
             raise AdminError("Error in updating environment" + str(e))
 
-    def get_storage_details(self, environment_id, storage_id=None, params=None):
+    def get_storage_details(self, environment_id, storage_id=None, params=None, pagination=True):
         """
         Function to get storage details
         :param environment_id: Entity identifier of the environment
         :type environment_id: String
         :param storage_id: Entity identifier of the storage
         :type storage_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type params: Dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: Response Dict
         """
         if params is None and storage_id is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_storages = url_builder.get_environment_storage_details(
             self.client_config, environment_id, storage_id) + IWUtils.get_query_params_string_from_dict(params=params)
         storage_details = []
@@ -606,14 +620,16 @@
                                                         )
                 initial_msg = response.get("message", "")
                 if storage_id is not None:
                     storage_details.extend([result])
                 else:
                     while len(result) > 0:
                         storage_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -628,25 +644,27 @@
                                                     error_code=ErrorCode.USER_ERROR,
                                                     response="Failed to get storage details"
                                                     )
         except Exception as e:
             self.logger.error("Error in getting storage details " + str(e))
             raise AdminError("Error in getting storage details" + str(e))
 
-    def get_compute_template_details(self, environment_id, compute_id=None, is_interactive=False, params=None):
+    def get_compute_template_details(self, environment_id, compute_id=None, is_interactive=False, params=None, pagination=True):
         """
          Function to get compute template details
          :param environment_id: Entity identifier of the environment
          :type environment_id: String
          :param compute_id: Entity identifier of compute cluster
          :type compute_id: String
          :param is_interactive: True/False. If True only the details of interactive clusters is fetched
          :type is_interactive: Boolean
          :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
          :type params: Dict
+         :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+         :type pagination: Boolean
          :return: Response Dict
          """
         if params is None and compute_id is None:
             params = {"limit": 20, "offset": 0}
         if is_interactive:
             url_to_list_computes = url_builder.get_environment_interactive_compute_details(
                 self.client_config, environment_id, compute_id) + IWUtils.get_query_params_string_from_dict(
@@ -671,14 +689,16 @@
                                                         )
                 initial_msg = response.get("message", "")
                 if compute_id is not None:
                     compute_details.extend([result])
                 else:
                     while len(result) > 0:
                         compute_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -828,14 +848,61 @@
                                                     )
         else:
             return GenericResponse.parse_result(status=Response.Status.FAILED,
                                                 error_code=ErrorCode.USER_ERROR,
                                                 response=response.get("result", {}).get("response", {})
                                                 )
 
+    def list_source_extensions(self, params=None, pagination=True):
+        """
+        Function to list the source extensions
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        url_to_list_source_extensions = url_builder.create_source_extension_url(self.client_config) \
+                                    + IWUtils.get_query_params_string_from_dict(params=params)
+        source_extensions_list = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_list_source_extensions,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    source_extensions_list.extend(result)
+                    if not pagination:
+                        break
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", None)
+                    if result is None:
+                        return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                            error_code=ErrorCode.GENERIC_ERROR,
+                                                            error_desc="Error in listing secret store",
+                                                            response=response
+                                                            )
+
+                response["result"] = source_extensions_list
+
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing secret stores")
+            raise AdminError("Error in listing secret store" + str(e))
+
     def get_source_extension(self, extension_id):
         """
         Function to get a source extension details
         :param extension_id: ID of the source extension
         :type extension_id: String
         :return: Response Dict
         """
@@ -1040,21 +1107,23 @@
                                                     error_code=ErrorCode.GENERIC_ERROR,
                                                     error_desc=parsed_response.get("details",
                                                                                    "Failed to update data connection"),
                                                     job_id=None, response=parsed_response)
         except Exception as e:
             raise AdminError(f"Failed to update the data connection" + str(e))
 
-    def get_data_connection(self, data_connection_id=None, params=None):
+    def get_data_connection(self, data_connection_id=None, params=None, pagination=True):
         """
         Function to create data connection in the domain
         :param data_connection_id: id of dataconnection for which config has to be fetched
         :type data_connection_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
 
         if data_connection_id is None:
             url_to_get_data_connection = url_builder.create_data_connection(
@@ -1071,14 +1140,16 @@
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 if data_connection_id is not None:
                     dataconnection_list.append(result)
                 else:
                     while len(result) > 0:
                         dataconnection_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1121,19 +1192,21 @@
                                                     error_code=ErrorCode.GENERIC_ERROR,
                                                     error_desc=parsed_response.get("details",
                                                                                    "Failed to delete data connection"),
                                                     response=parsed_response)
         except Exception as e:
             raise AdminError(f"Failed in delete data connection" + str(e))
 
-    def list_secret_stores(self, params=None):
+    def list_secret_stores(self, params=None, pagination=True):
         """
         Function to list the secret stores
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_secret_stores = url_builder.list_secret_stores_url(self.client_config) \
                                     + IWUtils.get_query_params_string_from_dict(params=params)
 
@@ -1142,14 +1215,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_secret_stores,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     secret_stores_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1297,19 +1372,21 @@
                                                     error_desc=parsed_response.get("details",
                                                                                    "Error in deleting secret store ")
                                                     )
         except Exception as e:
             self.logger.error("Error in deleting secret store " + str(e))
             raise AdminError("Error in deleting secret store " + str(e))
 
-    def list_service_authentication(self, params=None):
+    def list_service_authentication(self, params=None, pagination=True):
         """
         Function to list the service authentication mechanisms in Infoworks
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_service_authentication = url_builder.list_service_authentication_url(self.client_config) \
                                              + IWUtils.get_query_params_string_from_dict(params=params)
 
@@ -1318,14 +1395,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_service_authentication,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     secret_stores_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1489,19 +1568,21 @@
                                                     error_desc=parsed_response.get("details",
                                                                                    "Error in deleting service auth ")
                                                     )
         except Exception as e:
             self.logger.error("Error in deleting service auth " + str(e))
             raise AdminError("Error in deleting service auth " + str(e))
 
-    def list_secrets(self, params=None):
+    def list_secrets(self, params=None, pagination=True):
         """
         Function to list the secrets in Infoworks
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_secrets = url_builder.list_secrets_url(self.client_config) \
                               + IWUtils.get_query_params_string_from_dict(params=params)
 
@@ -1510,14 +1591,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_secrets,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     secret_stores_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1657,19 +1740,21 @@
                                                     error_desc=parsed_response.get("details",
                                                                                    "Error in deleting secret ")
                                                     )
         except Exception as e:
             self.logger.error("Error in deleting secret " + str(e))
             raise AdminError("Error in deleting secret " + str(e))
 
-    def list_domains_as_admin(self, params=None):
+    def list_domains_as_admin(self, params=None, pagination=True):
         """
         Function to list the domains as admin user
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_domains = url_builder.list_domains_admin_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(
             params=params)
@@ -1679,14 +1764,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_domains,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     users_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1822,20 +1909,22 @@
                                                                                    f"Error stop the cluster")
                                                     )
         except Exception as e:
             self.logger.error(f"Error stop the cluster. Please do it by yourself from UI.")
             raise AdminError(
                 f"Error stop the cluster. Please do it by yourself from UI." + str(e))
 
-    def list_accessible_sources_under_domain_as_admin(self, domain_id, params=None):
+    def list_accessible_sources_under_domain_as_admin(self, domain_id, params=None, pagination=True):
         """
         Function to list the accessible sources under domain
         :param domain_id: Entity identifier for domain
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         accessible_sources_url = url_builder.url_to_list_accessible_sources(self.client_config,
                                                                             domain_id) + IWUtils.get_query_params_string_from_dict(
             params=params)
@@ -1845,14 +1934,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", accessible_sources_url,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     output_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1920,19 +2011,21 @@
                                                         error_desc=parsed_response.get("details",
                                                                                        "Error in deleting schedules ")
                                                         )
             except Exception as e:
                 self.logger.error("Error in deleting schedules " + str(e))
                 raise AdminError("Error in deleting schedules " + str(e))
 
-    def list_schedules_as_admin(self, params=None):
+    def list_schedules_as_admin(self, params=None, pagination=True):
         """
         Function to list all the schedules as an admin
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         schedules_url = url_builder.list_all_schedules_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(
             params=params)
@@ -1942,14 +2035,16 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", schedules_url,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     output_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1963,7 +2058,243 @@
                                                             )
 
                 response["result"] = output_list
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in listing schedules")
             raise AdminError("Error in listing schedules" + str(e))
+
+    def list_job_hooks(self, params=None, pagination=True):
+        """
+        Function to list all the job-hooks as an admin
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        job_hooks_url = url_builder.list_job_hooks(
+            self.client_config) + IWUtils.get_query_params_string_from_dict(
+            params=params)
+
+        output_list = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", job_hooks_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    output_list.extend(result)
+                    if not pagination:
+                        break
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", None)
+                    if result is None:
+                        return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                            error_code=ErrorCode.GENERIC_ERROR,
+                                                            error_desc="Error in listing job_hooks",
+                                                            response=response
+                                                            )
+
+                response["result"] = output_list
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing job_hooks")
+            raise AdminError("Error in listing job_hooks" + str(e))
+
+    def get_list_of_job_hook_dependencies(self, job_hook_id=None,params=None):
+        """
+        Function to list all the dependencies of job hook
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param job_hook_id: Identifier of Job hook
+        :type: String
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        if job_hook_id is None:
+            self.logger.error("job_hook_id cannot be None")
+            raise Exception("job_hook_id cannot be None")
+        job_hook_dependencies_url = url_builder.get_list_of_job_hook_dependencies(
+            self.client_config,job_hook_id) + IWUtils.get_query_params_string_from_dict(
+            params=params)
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", job_hook_dependencies_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                if result is None:
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                            error_code=ErrorCode.GENERIC_ERROR,
+                                                            error_desc="Error in listing job_hook dependencies",
+                                                            response=response
+                                                            )
+
+                response["result"] = result
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing job_hook dependencies")
+            raise AdminError("Error in listing job_hook dependencies" + str(e))
+
+    def get_list_of_source_extension_dependencies(self, source_extension_id=None,params=None):
+        """
+        Function to list all the dependencies of source extension
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param source_extension_id : Identifier of source extension
+        :type: String
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        if source_extension_id is None:
+            self.logger.error("source_extension_id cannot be None")
+            raise Exception("source_extension_id cannot be None")
+        source_extension_dependencies_url = url_builder.get_list_of_source_extension_dependencies(
+            self.client_config,source_extension_id) + IWUtils.get_query_params_string_from_dict(
+            params=params)
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", source_extension_dependencies_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                if result is None:
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                            error_code=ErrorCode.GENERIC_ERROR,
+                                                            error_desc="Error in listing source_extension dependencies",
+                                                            response=response
+                                                            )
+
+                response["result"] = result
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing source_extension dependencies")
+            raise AdminError("Error in listing source_extension dependencies" + str(e))
+
+    def list_generic_source_types(self, params=None, pagination=True):
+        """
+        Function to list the generic source types registered in infoworks
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        url_to_list_generic_source_types = url_builder.list_generic_source_types(self.client_config) + IWUtils.get_query_params_string_from_dict(
+            params=params)
+
+        generic_source_types_list = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_list_generic_source_types,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    generic_source_types_list.extend(result)
+                    if not pagination:
+                        break
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", None)
+                    if result is None:
+                        return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                            error_code=ErrorCode.GENERIC_ERROR,
+                                                            error_desc="Error in listing generic source types",
+                                                            response=response
+                                                            )
+
+                response["result"] = generic_source_types_list
+
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing generic source types")
+            raise AdminError("Error in listing generic source types" + str(e))
+
+    def get_generic_source_type_by_id(self, generic_source_type_id=None):
+        """
+        Function to get generic source type by id
+        :param generic_source_type_id: Entity identifier of the generic source type
+        :type generic_source_type_id: String
+        :return: response dict
+        """
+
+        if generic_source_type_id is None:
+            self.logger.error("generic_source_type_id cannot be None")
+            raise Exception("generic_source_type_id cannot be None")
+        get_generic_source_type_by_id_url = url_builder.list_generic_source_types(
+            self.client_config, generic_source_type_id)
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", get_generic_source_type_by_id_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                if result is None:
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                        error_code=ErrorCode.GENERIC_ERROR,
+                                                        error_desc="Error in getting generic source id details",
+                                                        response=response
+                                                        )
+
+                response["result"] = result
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in getting generic source id details")
+            raise AdminError("Error in getting generic source id details" + str(e))
+
+    def get_list_of_generic_source_type_dependencies(self, generic_source_type_id=None,params=None):
+        """
+        Function to list all the dependencies of generic source type
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param generic_source_type_id: Identifier of generic source type
+        :type: String
+        :return: response dict
+        """
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        if generic_source_type_id is None:
+            self.logger.error("generic_source_type_id cannot be None")
+            raise Exception("generic_source_type_id cannot be None")
+        source_extension_dependencies_url = url_builder.list_generic_source_types(
+            self.client_config, generic_source_type_id) + "/dependencies" + IWUtils.get_query_params_string_from_dict(
+            params=params)
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", source_extension_dependencies_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                if result is None:
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                        error_code=ErrorCode.GENERIC_ERROR,
+                                                        error_desc="Error in listing generic source type dependencies",
+                                                        response=response
+                                                        )
+
+                response["result"] = result
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing generic source type dependencies")
+            raise AdminError("Error in listing generic source type dependencies" + str(e))
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/base_client.py` & `infoworkssdk-4.1/infoworks/sdk/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,59 +121,63 @@
                                                                   port=self.client_config["port"],
                                                                   refresh_token=self.client_config["refresh_token"])
             headers = IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
         return headers
 
     def call_api(self, method, url, headers=None, data=None):
         # headers = self.regenerate_bearer_token_if_needed(headers)
+        # adding the below code to encode the # in the url so it doesn't fragment the url
+        import urllib.parse
+        encoded_url = url.replace("#","%23")
+        url = encoded_url
         if method.upper() == "GET":
             self.logger.info(f"Calling {url}")
             response = self.http.get(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
                                      verify=False, data=data)
-            if response.status_code == 406:
+            if response.status_code in [401, 406]:
                 headers = self.regenerate_bearer_token_if_needed(headers)
                 return self.http.get(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
                                      verify=False, data=data)
             else:
                 return response
         elif method.upper() == "POST":
             self.logger.info(f"Calling {url}")
             response = self.http.post(url, headers=headers, json=data,
                                       timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
+            if response.status_code in [401, 406]:
                 headers = self.regenerate_bearer_token_if_needed(headers)
                 return self.http.post(url, headers=headers, json=data,
                                       timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
             else:
                 return response
         elif method.upper() == "PUT":
             self.logger.info(f"Calling {url}")
             response = self.http.put(url, headers=headers, json=data,
                                      timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
+            if response.status_code in [401, 406]:
                 headers = self.regenerate_bearer_token_if_needed(headers)
                 return self.http.put(url, headers=headers, json=data,
                                      timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
             else:
                 return response
         elif method.upper() == "PATCH":
             self.logger.info(f"Calling {url}")
             response = self.http.patch(url, headers=headers, json=data,
                                        timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
+            if response.status_code in [401, 406]:
                 headers = self.regenerate_bearer_token_if_needed(headers)
                 return self.http.put(url, headers=headers, json=data,
                                      timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
             else:
                 return response
         elif method.upper() == "DELETE":
             self.logger.info(f"Calling {url}")
             response = self.http.delete(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
                                         verify=False)
-            if response.status_code == 406:
+            if response.status_code in [401, 406]:
                 headers = self.regenerate_bearer_token_if_needed(headers)
                 return self.http.delete(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
                                         verify=False)
             else:
                 return response
 
     def get_mappings_from_config_file(self, ini_config_file_path):
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/cicd_response.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/cicd_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             os.makedirs(os.path.join(config_file_dump_path, "pipeline_group"))
         utils_obj = Utils(serviceaccountemail)
         target_file_path = os.path.join(os.path.join(config_file_dump_path, "modified_files"), "pipeline.csv")
         target_file_path_pipeline_groups = os.path.join(os.path.join(config_file_dump_path, "modified_files"),
                                                         "pipeline_group.csv")
         if files_overwrite:
             open(target_file_path, 'w').close()
-            open(target_file_path_pipeline_groups, 'w').close()
+            open(target_file_path_pipeline_groups, 'a').close()
             mode = "a"
         else:
             mode = "a"
         f = open(target_file_path, mode)
         f_pipeline_group = open(target_file_path_pipeline_groups, mode)
         for pipeline_id in pipeline_ids:
             try:
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_source_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 
 class DownloadSource(BaseClient):
     def __init__(self):
         super(DownloadSource, self).__init__()
 
     def cicd_get_sourceconfig_export(self, source_ids, config_file_export_path, files_overwrite=True,
-                                    serviceaccountemail="admin@infoworks.io",
-                                    replace_words=""):
+                                     serviceaccountemail="admin@infoworks.io",
+                                     replace_words="", dump_watermarks=True):
         self.cicd_get_sourceconfig_dumps(source_ids, config_file_export_path, files_overwrite,
-                                    serviceaccountemail,
-                                    replace_words)
+                                         serviceaccountemail,
+                                         replace_words,dump_watermarks)
 
     def cicd_get_sourceconfig_dumps(self, source_ids, config_file_dump_path, files_overwrite=True,
                                     serviceaccountemail="admin@infoworks.io",
-                                    replace_words=""):
+                                    replace_words="", dump_watermarks=True):
         # replace_words = "DEV->PROD;dev->prod"
         utils_obj = Utils(serviceaccountemail)
         if not os.path.exists(os.path.join(config_file_dump_path, "modified_files")):
             os.makedirs(os.path.join(config_file_dump_path, "modified_files"))
         if not os.path.exists(os.path.join(config_file_dump_path, "source")):
             os.makedirs(os.path.join(config_file_dump_path, "source"))
         target_file_path = os.path.join(os.path.join(config_file_dump_path, "modified_files"), "source.csv")
@@ -32,15 +32,15 @@
         else:
             mode = "a"
         f = open(target_file_path, mode)
         for source_id in source_ids:
             try:
                 filename, configuration_obj = utils_obj.dump_to_file(self, "source", None,
                                                                      source_id, replace_words,
-                                                                     config_file_dump_path)
+                                                                     config_file_dump_path, dump_watermarks)
                 if filename is not None:
                     f.write(filename)
                     f.write("\n")
             except Exception as e:
                 self.logger.error(f"Unable to export configurations for source {source_id} due to {str(e)}")
                 print(f"Unable to export configurations for source {source_id} due to {str(e)}")
                 print(traceback.format_exc())
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/lineage.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/download_configurations/utils.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/download_configurations/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import copy
 import os
 import traceback
-
-import jwt
-
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import get_parent_entity_url, list_domains_url, configure_pipeline_url, \
     configure_workflow_url, \
     configure_source_url, get_environment_details, get_environment_storage_details, get_environment_compute_details, \
     get_environment_interactive_compute_details, get_source_configurations_url, get_pipeline_url, \
     get_data_connection, source_info, list_users_url, list_secrets_url, get_pipeline_group_base_url, list_pipelines_url, \
-    create_domain_url
+    create_domain_url, get_table_configuration
 from infoworks.sdk.cicd.cicd_response import CICDResponse
 import json
 
 
 class Utils:
     def __init__(self, serviceaccountemail):
         self.serviceaccountemail = serviceaccountemail
@@ -195,16 +192,16 @@
             "pipeline",
             domain_id)
         env_name, storage_name, compute_name = self.get_env_entities_names(
             cicd_client, environment_id,
             environment_compute_template_id,
             environment_storage_id)
 
-        decoded_jwt = jwt.decode(cicd_client.client_config['bearer_token'], options={"verify_signature": False})
-        user_email = json.loads(decoded_jwt.get("sub")).get("email")
+        # decoded_jwt = jwt.decode(cicd_client.client_config['bearer_token'], options={"verify_signature": False})
+        # user_email = json.loads(decoded_jwt.get("sub")).get("email")
         config_obj = {
             "configuration": {
                 "entity": {
                     "entity_type": "pipeline",
                     "entity_id": pipeline_id,
                     "entity_name": pipeline_details.get("name"),
                     "subEntityName": f"V{version_id}",
@@ -218,29 +215,92 @@
                     "query_tag": query_tag,
                     "description": description
                 },
                 "pipeline_advance_configs": pipeline_advance_config_details
             },
             "environment_configurations": {"environment_name": env_name,
                                            "environment_compute_template_name": compute_name,
-                                           "environment_storage_name": storage_name},
-            "user_email": user_email
+                                           "environment_storage_name": storage_name}
         }
         target_file_path = os.path.join(target_file_path, "pipeline", filename)
         if filename is not None and target_file_path is not None:
             cicd_client.logger.info("{} {}".format(filename, target_file_path))
             print(f"Exporting configurations file to {target_file_path}")
             with open(target_file_path, 'w') as file_ptr:
-                #contents_to_write = IWUtils.ejson_serialize(config_obj)
-                json.dump(config_obj,file_ptr,indent=4)
+                # contents_to_write = IWUtils.ejson_serialize(config_obj)
+                json.dump(config_obj, file_ptr, indent=4)
             cicd_client.logger.info("Configurations exported successfully")
             print("Configurations exported successfully")
         return filename, config_obj
 
-    def dump_to_file(self, cicd_client, entity_type, domain_id, entity_id, replace_words, target_file_path):
+    def list_pipelines(self, cicd_client, domain_id=None, params=None):
+        """
+        Function to list the pipelines
+        :param domain_id: Entity identified for domain
+        :type domain_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response list
+        """
+
+        if None in {domain_id}:
+            cicd_client.logger.error("Domain ID cannot be None")
+            raise Exception("Domain ID cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        url_to_list_pipelines = list_pipelines_url(cicd_client.client_config, domain_id) \
+                                + IWUtils.get_query_params_string_from_dict(params=params)
+
+        pipelines_list = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                cicd_client.call_api("GET", url_to_list_pipelines,
+                                     IWUtils.get_default_header_for_v3(
+                                         cicd_client.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    pipelines_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=cicd_client.client_config['ip'],
+                                                                      port=cicd_client.client_config['port'],
+                                                                      protocol=cicd_client.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        cicd_client.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            cicd_client.client_config['bearer_token'])).content)
+                    result = response.get("result", None)
+                    if result is None:
+                        return response
+                response["result"] = pipelines_list
+                response["message"] = initial_msg
+            return response
+        except Exception as e:
+            cicd_client.logger.error("Error in listing pipelines")
+            raise Exception("Error in listing pipelines" + str(e))
+
+    def add_secret_name_to_id(self, data, cicd_client):
+        for key, value in data.items():
+            if isinstance(value, dict):
+                # If the value is a dictionary, recurse into it
+                secret_name = self.add_secret_name_to_id(value, cicd_client)
+                if secret_name:
+                    return secret_name
+            elif key == "secret_id":
+                # print(f"Found secret_name: {value}")
+                # resolve secret name to ID
+                secret_name = self.get_secret_name_from_id(cicd_client=cicd_client, secret_id=value)
+                if secret_name:
+                    data["secret_name"] = secret_name
+                # Add your logic here to do something with the secret_name
+                return value
+
+    def dump_to_file(self, cicd_client, entity_type, domain_id, entity_id, replace_words, target_file_path,
+                     dump_watermarks=True):
         response_to_return = {}
         filename = None
         environment_id, environment_compute_template_id, environment_storage_id = None, None, None
         if entity_type == "pipeline":
             url_to_config = configure_pipeline_url(cicd_client.client_config, domain_id, entity_id)
         elif entity_type == "workflow":
             url_to_config = configure_workflow_url(cicd_client.client_config, domain_id, entity_id)
@@ -256,16 +316,17 @@
             cicd_client.client_config[
                 'bearer_token']))
 
         parsed_response = IWUtils.ejson_deserialize(response.content)
 
         if response.status_code == 200:
             status = "SUCCESS"
-        elif response.status_code == 406:
-            return self.get_sql_pipeline_config(cicd_client, domain_id, entity_id, target_file_path)
+        # removing below elif because sql pipeline migration is supported with config-migration api from 5.5
+        # elif response.status_code == 406:
+        #    return self.get_sql_pipeline_config(cicd_client, domain_id, entity_id, target_file_path)
         else:
             status = "FAILED"
             print(parsed_response)
 
         response_to_return["get_configuration_entity_response"] = CICDResponse.parse_result(status=status,
                                                                                             entity_id=entity_id,
                                                                                             response=parsed_response)
@@ -288,55 +349,15 @@
                 if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
                     result = parsed_response.get("result", [])
                     if len(result) > 0:
                         data_lake_path = result["data_lake_path"]
                         configuration_obj["configuration"]["source_configs"]["data_lake_path"] = data_lake_path
                         configuration_obj["filter_tables_properties"] = result.get("filter_tables_properties", {})
                         source_connection_objects = configuration_obj["configuration"]["source_configs"]["connection"]
-                        if source_connection_objects.get("storage", None) is not None:
-                            # for File based sources
-                            if source_connection_objects.get("storage", {}).get("password", {}).get("password_type",
-                                                                                                    "") == "secret_store":
-                                # for SFTP password auth
-                                secret_id = source_connection_objects["storage"]["password"]["secret_id"]
-                                secret_name = self.get_secret_name_from_id(cicd_client, secret_id)
-                                if secret_name:
-                                    source_connection_objects["storage"]["password"]["secret_name"] = secret_name
-                            elif source_connection_objects.get("storage", {}).get("access_key_name", {}).get(
-                                    "password_type", "") == "secret_store":
-                                # for adls gen2 storage account access key auth
-                                secret_id = source_connection_objects["storage"]["access_key_name"]["secret_id"]
-                                secret_name = self.get_secret_name_from_id(cicd_client, secret_id)
-                                if secret_name:
-                                    source_connection_objects["storage"]["access_key_name"]["secret_name"] = secret_name
-                            elif source_connection_objects.get("storage", {}).get("service_credential", {}).get(
-                                    "password_type", "") == "secret_store":
-                                # for adls gen2 service credential auth
-                                secret_id = source_connection_objects["storage"]["service_credential"]["secret_id"]
-                                secret_name = self.get_secret_name_from_id(cicd_client, secret_id)
-                                if secret_name:
-                                    source_connection_objects["storage"]["service_credential"][
-                                        "secret_name"] = secret_name
-                            elif source_connection_objects.get("storage", {}).get("account_key", {}).get(
-                                    "password_type", "") == "secret_store":
-                                # for blob storage account key auth
-                                secret_id = source_connection_objects["storage"]["account_key"]["secret_id"]
-                                secret_name = self.get_secret_name_from_id(cicd_client, secret_id)
-                                if secret_name:
-                                    source_connection_objects["storage"]["account_key"]["secret_name"] = secret_name
-                            else:
-                                pass
-                        else:
-                            # for RDBMS sources
-                            if source_connection_objects.get("password", {}).get("password_type", "") == "secret_store":
-                                # for SFTP password auth
-                                secret_id = source_connection_objects["password"]["secret_id"]
-                                secret_name = self.get_secret_name_from_id(cicd_client, secret_id)
-                                if secret_name:
-                                    source_connection_objects["password"]["secret_name"] = secret_name
+                        self.add_secret_name_to_id(data=source_connection_objects, cicd_client=cicd_client)
                         # handle associated domains
                         if configuration_obj.get("configuration", {}).get("source_configs", {}).get(
                                 "associated_domains", None) is None:
                             associated_domains = result.get("associated_domains", [])
                             if associated_domains:
                                 configuration_obj["configuration"]["source_configs"][
                                     "associated_domains"] = associated_domains
@@ -347,14 +368,48 @@
                         if table_config["configuration"]["export_configuration"].get("target_type", "") in ["SNOWFLAKE",
                                                                                                             "POSTGRES",
                                                                                                             "AZURE_SQL_DW"]:
                             table_config["configuration"]["export_configuration"]["connection"]["password"] = None
                         else:
                             pass  # TO_DO
 
+                # Dump table watermarks
+                table_watermark_mappings = {}
+                if dump_watermarks:
+                    for table_config in configuration_obj["configuration"]["table_configs"]:
+                        # table_name = table_config.get("configuration", {}).get("name", "")
+                        table_id = table_config.get("entity_id", None)
+                        source_id = entity_id
+                        if source_id is not None and table_id is not None:
+                            get_tbl_details_url = get_table_configuration(cicd_client.client_config, source_id,
+                                                                          table_id)
+                            response = cicd_client.call_api("GET", get_tbl_details_url,
+                                                            IWUtils.get_default_header_for_v3(
+                                                                cicd_client.client_config['bearer_token']))
+                            parsed_response = IWUtils.ejson_deserialize(response.content)
+                            if response.status_code == 200:
+                                last_ingested_cdc_value = parsed_response.get("result").get("last_ingested_cdc_value",
+                                                                                            None)
+                                last_merged_watermark = parsed_response.get("result").get("last_merged_watermark",
+                                                                                          None)
+                                max_modified_timestamp = parsed_response.get("result").get("max_modified_timestamp",
+                                                                                           None)
+                                row_count = parsed_response.get("result").get("row_count", None)
+                                full_load_performed = parsed_response.get("result").get("full_load_performed", None)
+                                table_watermark_mappings[table_id] = {
+                                    "last_ingested_cdc_value": last_ingested_cdc_value,
+                                    "last_merged_watermark": last_merged_watermark,
+                                    "row_count": row_count,
+                                    "full_load_performed": full_load_performed}
+                                if max_modified_timestamp:
+                                    table_watermark_mappings[table_id]["max_modified_timestamp"] = max_modified_timestamp
+                                configuration_obj["table_watermark_mappings"] = table_watermark_mappings
+                            else:
+                                print("Get Table Config Failed " + json.dumps(response))
+
                 # add domain names to mapped domain ids
                 accessible_domain_ids = configuration_obj["configuration"]["source_configs"].get("associated_domains",
                                                                                                  [])
                 accessible_domain_names = []
                 for domain_id in accessible_domain_ids:
                     domain_id_response = cicd_client.call_api("GET",
                                                               create_domain_url(
@@ -447,23 +502,16 @@
                                     result["properties"] = self.get_dataconnection_properties(result["sub_type"],
                                                                                               result["properties"])
                                 for key in ['name', 'type', 'sub_type', 'properties']:
                                     dataconnection_obj[key] = result[key]
                                 configuration_obj["dataconnection_configurations"].append(
                                     copy.deepcopy(dataconnection_obj))
                 elif entity_type == "pipeline_group":
-                    list_pipelines_under_domain_url = list_pipelines_url(cicd_client.client_config, domain_id=domain_id)
-                    cicd_client.logger.info(f"Calling the api: {list_pipelines_under_domain_url}")
+                    pipelines_under_domain_parsed_response = self.list_pipelines(cicd_client, domain_id=domain_id)
                     pipeline_name_lookup = {}
-                    pipelines_under_domain_response = cicd_client.call_api("GET", list_pipelines_under_domain_url,
-                                                                           IWUtils.get_default_header_for_v3(
-                                                                               cicd_client.client_config[
-                                                                                   'bearer_token']))
-                    pipelines_under_domain_parsed_response = IWUtils.ejson_deserialize(
-                        pipelines_under_domain_response.content)
                     if pipelines_under_domain_parsed_response.get("result", "") == "":
                         cicd_client.logger.error(f"Failed to list the pipelines under domain {domain_id}")
                         cicd_client.logger.error(pipelines_under_domain_parsed_response)
                         print(f"Failed to list the pipelines under domain {domain_id}")
                         print(pipelines_under_domain_parsed_response)
                         raise Exception(f"Failed to list the pipelines under domain {domain_id}")
                     for pipeline in pipelines_under_domain_parsed_response["result"]:
@@ -539,24 +587,24 @@
                     result = parsed_response.get("result", [])
                     configuration_obj["user_email"] = result[0]["profile"].get("email", "admin@infoworks.io")
             try:
                 if filename is not None and target_file_path is not None:
                     cicd_client.logger.info("{} {}".format(filename, target_file_path))
                     print(f"Exporting configurations file to {target_file_path}")
                     with open(target_file_path, 'w') as file_ptr:
-                        #contents_to_write = IWUtils.ejson_serialize(configuration_obj)
-                        #if replace_words != "":
+                        # contents_to_write = IWUtils.ejson_serialize(configuration_obj)
+                        # if replace_words != "":
                         #    for key, value in [item.split("->") for item in replace_words.split(";")]:
                         #        contents_to_write = contents_to_write.replace(key, value)
-                        #file_ptr.write(contents_to_write)
-                        json.dump(configuration_obj,file_ptr,indent=4)
+                        # file_ptr.write(contents_to_write)
+                        json.dump(configuration_obj, file_ptr, indent=4)
                     cicd_client.logger.info("Configurations exported successfully")
                     print("Configurations exported successfully")
             except Exception as e:
                 cicd_client.logger.error(str(e))
                 print(str(e))
         else:
             cicd_client.logger.info("Unable to export the configurations")
             print("Unable to export the configurations")
         # for item in response_to_return:
         #    print(item, json.dumps(response_to_return[item]))
-        return filename, configuration_obj
+        return filename, configuration_obj
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/cdata_source.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/salesforce_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import copy
 import json
 
 import requests
 import yaml
-import configparser
+
 from infoworks.sdk.url_builder import get_source_details_url
 from infoworks.sdk.utils import IWUtils
-from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+import configparser
 from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+from infoworks.sdk.source_response import SourceResponse
 
-class CdataSource:
+class SalesforceSource:
     def __init__(self):
         self.configuration_obj = None
         self.source_config_path = None
         self.environment_id = None
         self.storage_id = None
         self.secrets = None
 
@@ -25,14 +26,32 @@
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
         self.secrets = secrets
 
+    def update_table_schema_and_database(self,type,mappings):
+        data=self.configuration_obj
+        for table in data.get("configuration",{}).get("table_configs",[]):
+            if type=="target_schema":
+                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
+                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
+            elif type=="stage_schema":
+                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("staging_schema_name","")
+                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["staging_schema_name"]=mappings.get(schema_from_config.lower())
+            elif type=="database":
+                database_from_config=table.get("configuration",{}).get("configuration",{}).get("target_database_name","")
+                if database_from_config!="" and database_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["target_database_name"]=mappings.get(database_from_config.lower())
+            else:
+                pass
+
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
             if section in PRE_DEFINED_MAPPINGS:
                 continue
@@ -45,22 +64,27 @@
         if "configuration$source_configs$data_lake_schema" in config.sections():
             self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
         if "configuration$source_configs$staging_schema_name" in config.sections():
             self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
         if "configuration$source_configs$target_database_name" in config.sections():
             self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
 
-    def create_cdata_source(self, src_client_obj):
+    def create_salesforce_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
-        create_cdata_source_payload = data.copy()
-        create_cdata_source_payload["data_lake_schema"]= data["data_lake_schema"] if "data_lake_schema" in data else ""
-        create_cdata_source_payload["environment_id"] = self.environment_id
-        create_cdata_source_payload["storage_id"] = self.storage_id
-        create_cdata_source_payload["is_source_ingested"]= True
-        src_create_response = src_client_obj.create_source(source_config=create_cdata_source_payload)
+        create_salesforce_source_payload = {
+            "name": data["name"],
+            "type": "crm",
+            "sub_type": data["sub_type"],
+            "data_lake_path": data["data_lake_path"],
+            "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
+            "environment_id": self.environment_id,
+            "storage_id": self.storage_id,
+            "is_source_ingested": True
+        }
+        src_create_response = src_client_obj.create_source(source_config=create_salesforce_source_payload)
         if src_create_response["result"]["status"].upper() == "SUCCESS":
             source_id_created = src_create_response["result"]["source_id"]
             return source_id_created
         else:
             src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
             src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
             filter_condition = IWUtils.ejson_serialize({"name": data['name']})
@@ -80,20 +104,20 @@
                 src_client_obj.logger.error("Failed to make an api call to get source details")
                 src_client_obj.logger.info(response)
             else:
                 src_client_obj.logger.info(
                     f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 return response['result'][0]['id']
 
-    def configure_cdata_source_connection(self, src_client_obj, source_id, override_config_file=None,
+    def configure_salesforce_source_connection(self, src_client_obj, source_id, override_config_file=None,
                                           read_passwords_from_secrets=False, env_tag="", secret_type=""):
         source_configs = self.configuration_obj["configuration"]["source_configs"]
         src_name = str(source_configs["name"])
         connection_object = source_configs["connection"]
-        connection_object["connection_mode"]="jdbc"
+        connection_object["fetch_mechanism"]=connection_object["fetch_mechanism"].lower()
         if override_config_file is not None:
             with open(override_config_file) as file:
                 information = yaml.load(file, Loader=yaml.FullLoader)
             if information["source_details"].get(src_name, None) is not None:
                 override_keys = information["source_details"].get(src_name).keys()
                 for key in override_keys:
                     connection_object[key] = information["source_details"][src_name][key]
@@ -107,51 +131,17 @@
             return "SUCCESS"
 
     def test_source_connection(self, src_client_obj, source_id):
         response = src_client_obj.source_test_connection_job_poll(source_id, poll_timeout=300,
                                                                   polling_frequency=15, retries=1)
         return response["result"]["status"].upper()
 
-    def browse_source_tables(self, src_client_obj, source_id):
-        filter_tables_properties = self.configuration_obj["filter_tables_properties"]
-        response = src_client_obj.browse_source_tables(source_id, filter_tables_properties=filter_tables_properties,
-                                                       poll_timeout=300, polling_frequency=15, retries=1)
-        return response["result"]["status"].upper()
-
-    def add_tables_to_source(self, src_client_obj, source_id):
-        tables_already_added_in_source = src_client_obj.list_tables_in_source(source_id)["result"]["response"]
-        tables_list = []
-        tables = self.configuration_obj["configuration"]["table_configs"]
-        if len(tables_already_added_in_source) > 0:
-            for table in tables:
-                if table["configuration"]["schema_name_at_source"] + "." + table["configuration"][
-                    "name"] not in tables_already_added_in_source:
-                    temp = {"table_name": table["configuration"]["name"],
-                            "schema_name": table["configuration"]["schema_name_at_source"],
-                            "table_type": table["entity_type"].upper(),
-                            "target_table_name": table["configuration"]["configuration"]["target_table_name"],
-                            "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
-                    if table["configuration"].get("catalog_name","")!="":
-                        temp["catalog_name"]=table["configuration"]["catalog_name"]
-                    tables_list.append(copy.deepcopy(temp))
-                    src_client_obj.logger.info(
-                        f"Adding table {temp['table_name']} to source {source_id} config payload")
-        else:
-            for table in tables:
-                temp = {"table_name": table["configuration"]["name"],
-                        "schema_name": table["configuration"]["schema_name_at_source"],
-                        "table_type": table["entity_type"].upper(),
-                        "target_table_name": table["configuration"]["configuration"]["target_table_name"],
-                        "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
-                if table["configuration"].get("catalog_name", "") != "":
-                    temp["catalog_name"] = table["configuration"]["catalog_name"]
-                tables_list.append(copy.deepcopy(temp))
-                src_client_obj.logger.info(f"Adding table {temp['table_name']} to source {source_id} config payload")
-        response = src_client_obj.add_tables_to_source(source_id, tables_list)
-        print(tables_list)
+    def metacrawl_source(self,src_client_obj,source_id):
+        response = src_client_obj.source_metacrawl_job_poll(source_id, poll_timeout=300,
+                                                                  polling_frequency=15, retries=1)
         return response["result"]["status"].upper()
 
     def configure_tables_and_tablegroups(self, src_client_obj, source_id, export_configuration_file=None,
                                          export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
                                          env_tag="", secret_type=""):
         if mappings is None:
             mappings = {}
@@ -212,7 +202,59 @@
                                         .format(source_id, self.source_config_path))
             src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
                                         .format(self.source_config_path))
             return "FAILED"
         else:
             src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
             return "SUCCESS"
+    def update_table_state_as_ready(self,src_client_obj, source_id):
+        tables = self.configuration_obj["configuration"]["table_configs"]
+        table_state_update_dict = {}
+        tables_watermark_mappings = self.configuration_obj.get("table_watermark_mappings", {})
+        for table in tables:
+            table_name = table["configuration"]["name"]
+            src_client_obj.logger.info(f"Updating the table state information for table {table_name}")
+            table_update_payload = {"name": table_name, "source": source_id, "state": "ready"}
+            print("table_update_payload:",table_update_payload)
+            if table["configuration"].get("schema_name_at_source", "") != "":
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "schemaNameAtSource": table["configuration"]["schema_name_at_source"]}}).get("result",
+                                                                                                            {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"].get("catalog_name", ""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "catalog_name": table["configuration"]["catalog_name"]}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"]["configuration"].get("query",""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"table": table_name}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            else:
+                print(f"Skipping updating state for table {table_name} as it did not match any existing table.")
+            table_id = None
+            if len(table_document) > 0:
+                table_document = table_document[0]
+                table_id = table_document["id"]
+            if table_id is not None:
+                response = src_client_obj.update_table_configuration(source_id=source_id, table_id=table_id,
+                                                                     config_body=table_update_payload)
+                if response["result"]["status"].upper() != "SUCCESS":
+                    src_client_obj.logger.error(
+                        "Failed to update state for table {table_name}".format(table_name=table_name))
+                    src_client_obj.logger.error(response.get("result", {}).get("response", {}).get("message", ""))
+                    table_state_update_dict[table_name] = (
+                    "FAILED", response.get("result", {}).get("response", {}).get("message", ""))
+                else:
+                    src_client_obj.logger.info(
+                        "Successfully updated state for table {table_name}".format(table_name=table_name))
+                    table_state_update_dict[table_name] = ("SUCCESS", "")
+        failed_state_update_tables = [(table_name, status[1]) for table_name, status in
+                                       table_state_update_dict.items() if status[0].upper() == "FAILED"]
+        overall_update_status = "FAILED" if len(failed_state_update_tables) > 0 else "SUCCESS"
+        if overall_update_status == "FAILED":
+            response = {f"Tables state update failed for tables:{failed_state_update_tables}"}
+        else:
+            response = {f"Tables state updated successfully"}
+        return SourceResponse.parse_result(status=overall_update_status, source_id=source_id,
+                                           response=response)
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/csv_source.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/file_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,43 @@
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.local_configurations import Response
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
 from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 import configparser
 
-class CSVSource:
+class FileSource:
     def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
         self.storage_id = storage_id
         self.environment_id = environment_id
         self.source_config_path = source_config_path
         self.secrets = secrets
         with open(self.source_config_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
 
+    def replace_secret_name_with_mapping(self,data,src_client_obj):
+        for key, value in data.items():
+            if isinstance(value, dict):
+                # If the value is a dictionary, recurse into it
+                secret_name = self.replace_secret_name_with_mapping(value,src_client_obj)
+                if secret_name:
+                    return secret_name
+            elif key == "secret_name":
+                #print(f"Found secret_name: {value}")
+                # resolve secret name to ID
+                secret_id = self.get_secret_id_from_name(src_client_obj, value)
+                if secret_id:
+                    data["secret_id"] = secret_id
+                    data.pop('secret_name', None)
+                return value
+
     def update_table_schema_and_database(self,type,mappings):
         data=self.configuration_obj
         for table in data.get("configuration",{}).get("table_configs",[]):
             if type=="target_schema":
                 schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
                 if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
                     table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
@@ -73,30 +89,30 @@
                 secret_id = result[0]["id"]
                 cicd_client.logger.info("Found secret id {} ".format(secret_id))
                 return secret_id
             else:
                 cicd_client.logger.info("Secret id is {} ".format(None))
                 return None
 
-    def create_csv_source(self, src_client_obj):
+    def create_file_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
-        create_csv_source_payload = {
+        create_file_source_payload = {
             "name": data["name"],
             "type": data["type"],
             "sub_type": data["sub_type"],
             "data_lake_path": data["data_lake_path"],
             "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
             "environment_id": self.environment_id,
             "storage_id": self.storage_id,
             "is_source_ingested": True
         }
         if data.get("target_database_name",""):
-            create_csv_source_payload["target_database_name"] = data.get("target_database_name","")
+            create_file_source_payload["target_database_name"] = data.get("target_database_name","")
         if data.get("staging_schema_name",""):
-            create_csv_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
+            create_file_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
         # adding associated domains if any
         accessible_domain_names = data.get("associated_domain_names",[])
         accessible_domain_ids = []
         for domain_name in accessible_domain_names:
             domain_response = src_client_obj.call_api("GET",
                                                          create_domain_url(
                                                              src_client_obj.client_config) + "?filter={\"name\":\""+domain_name+"\"}",
@@ -106,27 +122,30 @@
             if domain_response.status_code == 200 and len(domain_parsed_response.get("result", [])) > 0:
                 result = domain_parsed_response.get("result", [])
                 if len(result) > 0:
                     result = result[0]
                     domain_id = result.get("id", None)
                     if domain_id is not None:
                         accessible_domain_ids.append(domain_id)
-            if "associated_domain_names" in create_csv_source_payload.keys():
-                create_csv_source_payload.pop("associated_domain_names",[])
+            if "associated_domain_names" in create_file_source_payload.keys():
+                create_file_source_payload.pop("associated_domain_names",[])
                 self.configuration_obj["configuration"]["source_configs"].pop("associated_domain_names", [])
             if len(accessible_domain_ids) > 0:
-                create_csv_source_payload["associated_domains"] = accessible_domain_ids
+                create_file_source_payload["associated_domains"] = accessible_domain_ids
                 self.configuration_obj["configuration"]["associated_domains"] = accessible_domain_ids
-        src_create_response = src_client_obj.create_source(source_config=create_csv_source_payload)
+        print("create_file_source_payload:", create_file_source_payload)
+        src_create_response = src_client_obj.create_source(source_config=create_file_source_payload)
         if src_create_response["result"]["status"].upper() == "SUCCESS":
             source_id_created = src_create_response["result"]["source_id"]
             print("Source created successfully")
             return src_create_response
         else:
             src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
+            print('Cant create source {} '.format(data["name"]))
+            print(src_create_response)
             src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
             filter_condition = IWUtils.ejson_serialize({"name": data['name']})
             source_detail_url = get_source_details_url(
                 src_client_obj.client_config) + f"?filter={{filter_condition}}".format(
                 filter_condition=filter_condition)
             response = requests.get(source_detail_url,
                                     headers={'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
@@ -146,44 +165,23 @@
                                                    source_id=None,response=response)
             else:
                 src_client_obj.logger.info(
                     f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 print(f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=response['result'][0]['id'],response=response)
 
-    def configure_csv_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
+    def configure_file_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
                              secret_type="",config_ini_path=None,dont_skip_step=True):
         if not dont_skip_step:
             return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
         data = self.configuration_obj["configuration"]["source_configs"]["connection"]
         src_name = str(self.configuration_obj["configuration"]["source_configs"]["name"])
         storage_type = data["storage"]["storage_type"]
         cloud_type = data["storage"].get("cloud_type", None)
-        if storage_type == "cloud" and cloud_type == "s3":
-            access_id = data["storage"].get("access_id", "")
-            secret_key = data["storage"].get("secret_key", "")
-            if "source_secrets" in mappings:
-                access_id = mappings.get("source_secrets").get("access_id", access_id)
-                secret_key = mappings.get("source_secrets").get("secret_key", secret_key)
-            source_configure_payload = {
-                "source_base_path_relative": data.get("source_base_path_relative",""),
-                "source_base_path": data.get("source_base_path",""),
-                "storage": {
-                    "storage_type": data["storage"]["storage_type"],
-                    "cloud_type": data["storage"]["cloud_type"],
-                    "access_id": access_id,
-                    "secret_key": secret_key,
-                    "account_type": data["storage"]["account_type"],
-                    "access_type": data["storage"]["access_type"]
-                }
-            }
-        elif storage_type == "cloud" and cloud_type == "wasb":
-            source_configure_payload = {}
-            pass
-        elif storage_type == "cloud" and "project_id" in data["storage"]:
+        if storage_type == "cloud" and "project_id" in data["storage"]:
             project_id = data["storage"]["project_id"]
             server_path = data["storage"]["server_path"]
             if "gcp_details" in mappings:
                 project_id = mappings["gcp_details"].get("project_id", project_id)
                 server_path = mappings["gcp_details"].get("service_json_path", server_path)
             if "gcp_project_id_mappings" in mappings:
                 project_id = mappings["gcp_project_id_mappings"].get(data["storage"]["project_id"], project_id)
@@ -200,52 +198,17 @@
                     "project_id": project_id,
                     "access_type": data["storage"]["access_type"],
                     "server_path": server_path,
                     "upload_option": data["storage"]["upload_option"],
                     "file_details": []
                 }
             }
-        elif storage_type == "remote":
-            # SFTP Source
-            data = self.configuration_obj["configuration"]["source_configs"]["connection"]
-            source_configure_payload = data
-            source_configure_payload["source_base_path"]=""
-            if data.get("storage", {}).get("password", {}).get("password_type","") == "secret_store":
-                # for SFTP password auth
-                secret_name = data["storage"]["password"]["secret_name"]
-                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
-                if secret_name:
-                    data["storage"]["password"]["secret_id"] = secret_id
-                    data["storage"]["password"].pop('secret_name', None)
-            elif data.get("storage", {}).get("access_key_name", {}).get("password_type","") == "secret_store":
-                # for adls gen2 storage account access key auth
-                secret_name = data["storage"]["access_key_name"]["secret_name"]
-                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
-                if secret_name:
-                    data["storage"]["access_key_name"]["secret_id"] = secret_id
-                    data["storage"]["access_key_name"].pop('secret_name', None)
-            elif data.get("storage", {}).get("service_credential", {}).get("password_type","") == "secret_store":
-                # for adls gen2 service credential auth
-                secret_name = data["storage"]["service_credential"]["secret_name"]
-                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
-                if secret_name:
-                    data["storage"]["service_credential"]["secret_id"] = secret_id
-                    data["storage"]["service_credential"].pop('secret_name', None)
-            elif data.get("storage", {}).get("account_key", {}).get("password_type","") == "secret_store":
-                #for blob storage account key auth
-                secret_name = data["storage"]["account_key"]["secret_name"]
-                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
-                if secret_name:
-                    data["storage"]["account_key"]["secret_id"] = secret_id
-                    data["storage"]["account_key"].pop('secret_name', None)
-            else:
-                pass
         else:
-            source_configure_payload = {}
-
+            source_configure_payload = data
+            self.replace_secret_name_with_mapping(data,src_client_obj)
         response = src_client_obj.configure_source_connection(source_id, connection_object=source_configure_payload)
         return response
 
     def import_source_configuration(self, src_client_obj, source_id,
                                     mappings, export_configuration_file=None, export_config_lookup=True,
                                     read_passwords_from_secrets=False,dont_skip_step=True):
         if not dont_skip_step:
@@ -318,16 +281,68 @@
                     except Exception as e:
                         src_client_obj.logger.error(
                             f"Failed to lookup the export configuration password from secrets due to {str(e)}")
         response = src_client_obj.configure_tables_and_tablegroups(source_id,
                                                                    configuration_obj=source_import_payload.get(
                                                                        "configuration"))
         return response
-        # if response["result"]["status"].upper() != "SUCCESS":
-        #     src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
-        #                                 .format(source_id, self.source_config_path))
-        #     src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
-        #                                 .format(self.source_config_path))
-        #     return "FAILED"
-        # else:
-        #     src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
-        #     return "SUCCESS"
+
+    def update_table_watermarks_and_state_as_ready(self,src_client_obj, source_id):
+        tables = self.configuration_obj["configuration"]["table_configs"]
+        table_state_update_dict = {}
+        tables_watermark_mappings = self.configuration_obj.get("table_watermark_mappings", {})
+        for table in tables:
+            table_name = table["configuration"]["name"]
+            src_client_obj.logger.info(f"Updating the table state information for table {table_name}")
+            table_update_payload = {"name": table_name, "source": source_id, "state": "ready"}
+            if tables_watermark_mappings:
+                current_table_id = table["entity_id"]
+                current_table_watermark_mappings = tables_watermark_mappings.get(current_table_id,{})
+                for key,value in current_table_watermark_mappings.items():
+                    if key in ["last_ingested_cdc_value","last_merged_watermark"]:
+                        table_update_payload[key] = f'"{value}"'
+                    else:
+                        table_update_payload[key] = value
+            print("table_update_payload:",table_update_payload)
+            if table["configuration"].get("schema_name_at_source", "") != "":
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "schemaNameAtSource": table["configuration"]["schema_name_at_source"]}}).get("result",
+                                                                                                            {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"].get("catalog_name", ""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "catalog_name": table["configuration"]["catalog_name"]}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"]["configuration"].get("query",""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"table": table_name}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            else:
+                print(f"Skipping updating state for table {table_name} as it did not match any existing table.")
+            table_id = None
+            if len(table_document) > 0:
+                table_document = table_document[0]
+                table_id = table_document["id"]
+            if table_id is not None:
+                response = src_client_obj.update_table_configuration(source_id=source_id, table_id=table_id,
+                                                                     config_body=table_update_payload)
+                if response["result"]["status"].upper() != "SUCCESS":
+                    src_client_obj.logger.error(
+                        "Failed to update state for table {table_name}".format(table_name=table_name))
+                    src_client_obj.logger.error(response.get("result", {}).get("response", {}).get("message", ""))
+                    table_state_update_dict[table_name] = (
+                    "FAILED", response.get("result", {}).get("response", {}).get("message", ""))
+                else:
+                    src_client_obj.logger.info(
+                        "Successfully updated state for table {table_name}".format(table_name=table_name))
+                    table_state_update_dict[table_name] = ("SUCCESS", "")
+        failed_state_update_tables = [(table_name, status[1]) for table_name, status in
+                                       table_state_update_dict.items() if status[0].upper() == "FAILED"]
+        overall_update_status = "FAILED" if len(failed_state_update_tables) > 0 else "SUCCESS"
+        if overall_update_status == "FAILED":
+            response = {f"Tables state update failed for tables:{failed_state_update_tables}"}
+        else:
+            response = {f"Tables state updated successfully"}
+        return SourceResponse.parse_result(status=overall_update_status, source_id=source_id,
+                                           response=response)
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/domains.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/domains.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/misc.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/misc.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/pipeline_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,72 @@
             try:
                 final = d.setval(section.split("$"), dict(config.items(section)))
                 print(f"section replacement:{d.getval(section.split('$'))}")
             except KeyError as e:
                 pass
         self.configuration_obj = d.data
 
+
+    def list_pipelines(self, pipeline_group_obj,domain_id=None, params=None):
+        """
+        Function to list the pipelines
+        :param domain_id: Entity identified for domain
+        :type domain_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response list
+        """
+
+        if None in {domain_id}:
+            pipeline_group_obj.logger.error("Domain ID cannot be None")
+            raise Exception("Domain ID cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        url_to_list_pipelines = list_pipelines_url(pipeline_group_obj.client_config, domain_id) \
+                                + IWUtils.get_query_params_string_from_dict(params=params)
+
+        pipelines_list = []
+        headers={'Authorization': 'Bearer ' + pipeline_group_obj.client_config["bearer_token"],
+                'Content-Type': 'application/json'}
+        try:
+            response = requests.request("GET", url_to_list_pipelines,
+                                 headers=headers, verify=False)
+            if response.status_code == 406:
+                headers = pipeline_group_obj.regenerate_bearer_token_if_needed(
+                    {'Authorization': 'Bearer ' + pipeline_group_obj.client_config["bearer_token"],
+                     'Content-Type': 'application/json'})
+                response = requests.request("GET", url_to_list_pipelines, headers=headers, verify=False)
+            if response.status_code==200:
+                response = response.json()
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    pipelines_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=pipeline_group_obj.client_config['ip'],
+                                                                      port=pipeline_group_obj.client_config['port'],
+                                                                      protocol=pipeline_group_obj.client_config['protocol'],
+                                                                      )
+                    response = requests.request("GET", nextUrl, headers=headers,verify=False)
+                    if response.status_code == 406:
+                        headers = pipeline_group_obj.regenerate_bearer_token_if_needed(
+                            {'Authorization': 'Bearer ' + pipeline_group_obj.client_config["bearer_token"],
+                             'Content-Type': 'application/json'})
+                        response = requests.request("GET", nextUrl, headers=headers, verify=False)
+                    response = response.json()
+                    result = response.get("result", None)
+                    if result is None:
+                        return response
+                response["result"] = pipelines_list
+                response["message"] = initial_msg
+            return response
+        except Exception as e:
+            pipeline_group_obj.logger.error("Error in listing pipelines")
+            raise Exception("Error in listing pipelines" + str(e))
+
     def create(self, pipeline_group_obj, domain_id, domain_name):
 
         pipeline_group_name = self.configuration_obj["name"]
         pipeline_group_id = None
         final_domain_id=domain_id
         if self.environment_id is not None:
             self.configuration_obj["environment_id"]=self.environment_id
@@ -67,31 +125,28 @@
         headers = pipeline_group_obj.regenerate_bearer_token_if_needed(
             {'Authorization': 'Bearer ' + pipeline_group_obj.client_config["bearer_token"],
              'Content-Type': 'application/json'})
         pipeline_group_details_response = requests.request("GET", pipeline_group_details_url, headers=headers, verify=False)
         pipeline_group_details_parsed_response = IWUtils.ejson_deserialize(
             pipeline_group_details_response.content)
         pipeline_name_lookup={}
-        list_pipelines_under_domain_url = list_pipelines_url(pipeline_group_obj.client_config,final_domain_id)
-        list_pipelines_response = requests.request("GET", list_pipelines_under_domain_url, headers=headers, verify=False)
-        list_pipelinesparsed_response = IWUtils.ejson_deserialize(
-            list_pipelines_response.content)
+        list_pipelinesparsed_response = self.list_pipelines(pipeline_group_obj=pipeline_group_obj,domain_id=final_domain_id)
         for item in list_pipelinesparsed_response["result"]:
             pipeline_name_lookup[item["name"]]=item["id"]
         for pipeline in self.configuration_obj["pipelines"]:
             pipeline["pipeline_id"]=pipeline_name_lookup[pipeline["name"]]
         if len(pipeline_group_details_parsed_response["result"])>0:
             pipeline_group_obj.logger.info(
                 'Pipeline group already exists. {} {}')
             pipeline_group_obj.logger.info('Getting the existing pipeline group Id with given name.')
             pipeline_group_id = pipeline_group_details_parsed_response["result"][0]["pipeline_group_details"]["id"]
             del self.configuration_obj["id"]
             configuration_obj = copy.deepcopy(self.configuration_obj)
             for item in self.configuration_obj:
-                if item in ["createdAt","createdBy","modifiedAt","modifiedBy","environment_configurations"]:
+                if item in ["createdAt","createdBy","modifiedAt","modifiedBy","environment_configurations","state","state_modified_by"]:
                     del configuration_obj[item]
             self.configuration_obj = configuration_obj
             for pipeline in self.configuration_obj["pipelines"]:
                 if pipeline.get("name",None) is not None:
                     del pipeline["name"]
 
             pipeline_group_create_url = get_pipeline_group_base_url(pipeline_group_obj.client_config, final_domain_id)+pipeline_group_id
@@ -105,15 +160,15 @@
                 pipeline_group_obj.logger.info("Successfully updated the pipeline group")
                 print("Successfully updated the pipeline group")
                 pipeline_group_id = parsed_response["result"]["id"]
         else:
             del self.configuration_obj["id"]
             configuration_obj = copy.deepcopy(self.configuration_obj)
             for item in self.configuration_obj:
-                if item in ["createdAt", "createdBy", "modifiedAt", "modifiedBy", "environment_configurations"]:
+                if item in ["createdAt", "createdBy", "modifiedAt", "modifiedBy", "environment_configurations","state","state_modified_by"]:
                     del configuration_obj[item]
             self.configuration_obj = configuration_obj
             for pipeline in self.configuration_obj["pipelines"]:
                 if pipeline.get("name", None) is not None:
                     del pipeline["name"]
 
             pipeline_group_create_url = get_pipeline_group_base_url(pipeline_group_obj.client_config,final_domain_id)
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/pipelines.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/pipelines.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,24 @@
 import json
 import traceback
 import configparser
 import requests
 import yaml
+import re
 import time
+import base64
 from infoworks.core.iw_authentication import get_bearer_token
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import list_sources_url, list_domains_url, create_pipeline_url, create_data_connection, \
     configure_pipeline_url, get_pipeline_jobs_url, pipeline_version_base_url
 from infoworks.sdk.cicd.upload_configurations.domains import Domain
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
 from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 from infoworks.sdk.local_configurations import POLLING_FREQUENCY_IN_SEC
 
-
-def create_sql_pipeline_version(pipeline_client_obj, pipeline_id=None, domain_id=None, sql_query="",
-                                pipeline_parameters=None):
-    pipeline_version_id = None
-    if pipeline_parameters is None:
-        pipeline_parameters = []
-    try:
-        pipeline_id = str(pipeline_id)
-        pipeline_client_obj.logger.info(
-            'Pipeline {id} has been created/found under domain {domain_id}.'.format(id=pipeline_id,
-                                                                                    domain_id=domain_id))
-        create_pipeline_version_url = pipeline_version_base_url(pipeline_client_obj.client_config,
-                                                                domain_id, pipeline_id)
-        pv_response = pipeline_client_obj.call_api("POST", create_pipeline_version_url, {
-            'Authorization': 'Bearer ' + pipeline_client_obj.client_config["bearer_token"],
-            'Content-Type': 'application/json'}, data={
-            "pipeline_id": pipeline_id,
-            "type": "sql",
-            "query": sql_query,
-            "pipeline_parameters": pipeline_parameters
-        })
-        parsed_response = IWUtils.ejson_deserialize(pv_response.content)
-        if parsed_response.status_code == 406:
-            pv_response = pipeline_client_obj.call_api("POST", create_pipeline_version_url, {
-                'Authorization': 'Bearer ' + pipeline_client_obj.client_config["bearer_token"],
-                'Content-Type': 'application/json'}, data={
-                "pipeline_id": pipeline_id,
-                "type": "sql",
-                "query": sql_query,
-                "pipeline_parameters": pipeline_parameters
-            })
-            parsed_response = IWUtils.ejson_deserialize(pv_response.content)
-
-        if parsed_response["result"].get("status", "") == "success":
-            pipeline_version_id = pv_response["result"]["entity_id"]
-            pipeline_client_obj.logger.info(f"Pipeline version {pipeline_version_id} created")
-            # Make the new created version as active
-            pv_active_response = IWUtils.ejson_deserialize(pipeline_client_obj.call_api("POST",
-                                                                                        create_pipeline_version_url + f"/{pipeline_version_id}/set-active",
-                                                                                        IWUtils.get_default_header_for_v3(
-                                                                                            pipeline_client_obj.client_config[
-                                                                                                'bearer_token'])).content)
-
-            if pv_active_response["result"].get("status", "") != "success":
-                pipeline_client_obj.logger.error(
-                    f"Unable to set the pipeline version {pipeline_version_id} as active")
-                pipeline_client_obj.logger.error(str(pv_active_response))
-            else:
-                pipeline_client_obj.logger.info(f"Pipeline version {pipeline_version_id} set as active")
-        else:
-            pipeline_client_obj.logger.error(f"Unable to create the new pipeline version")
-            pipeline_client_obj.logger.error(str(pv_response))
-
-    except Exception as e:
-        pipeline_client_obj.logger.error('Response from server: ' + str(e))
-        pipeline_client_obj.logger.exception('Error occurred while trying to create a new sql pipeline.')
-
-    return pipeline_version_id
-
-
 class Pipeline:
     def __init__(self, pipeline_config_path, environment_id, storage_id, interactive_id,
                  replace_words="", secrets=None):
         self.storage_id = storage_id
         self.interactive_id = interactive_id
         self.environment_id = environment_id
         self.secrets = secrets
@@ -107,14 +49,30 @@
                 if domain_mappings != {}:
                     for mapping in iw_mappings:
                         domain_name = mapping.get("recommendation", {}).get("domain_name", "")
                         if domain_name != "" and domain_mappings != {}:
                             mapping["recommendation"]["domain_name"] = domain_mappings.get(domain_name.lower(),
                                                                                            domain_name)
                     self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
+            if self.configuration_obj["configuration"].get("pipeline_configs",{}).get("type","")=="sql":
+                query = self.configuration_obj["configuration"].get("pipeline_configs",{}).get("query","")
+                decode_query_binary = base64.b64decode(query)
+                decoded_query = decode_query_binary.decode("ascii")
+                if "sql_pipeline_text_replace" in config.sections():
+                    text_mappings = dict(config.items("sql_pipeline_text_replace"))
+                    if text_mappings != {}:
+                        for k,v in text_mappings.items():
+                            decoded_query = re.sub(k, v, decoded_query, flags=re.IGNORECASE)
+                            print(f"Replacing '{k}' with '{v}' in sql_query")
+                        encoded_query_binary = base64.b64encode(decoded_query.encode('utf-8'))
+                        encoded_query = encoded_query_binary.decode('utf-8')
+                        self.configuration_obj["configuration"]["pipeline_configs"]["query"]=encoded_query
+                        for item in iw_mappings:
+                            if item.get("entity_type","")=="query":
+                                item["recommendation"]["query"] = encoded_query
         except Exception as e:
             print("Failed while doing the domain mappings")
             print(str(e))
             print(traceback.format_exc())
         # handle any other generic name mappings like iw_mappings$recommendation$source_name
         try:
             generic_mappings = [i for i in config.sections() if i.lower().startswith("iw_mappings$")]
@@ -198,28 +156,31 @@
             "name": pipeline_name,
             "environment_id": self.environment_id,
             "domain_id": domain_id
         }
         # 5.2.x versions need storage id and compute id
         batch_engine = self.configuration_obj["configuration"].get("pipeline_configs", {}).get("batch_engine", "")
         storage_id = self.storage_id
-        if storage_id:
+        if storage_id and batch_engine not in ["SNOWFLAKE"]:
             pipeline_json_object["storage_id"] = storage_id
         if batch_engine != "":
             pipeline_json_object["batch_engine"] = batch_engine
-
-        # 5.3.x onwards CDW support
-        if self.interactive_id is None:
-            pipeline_json_object["run_job_on_data_plane"] = False
-        else:
-            pipeline_json_object["compute_id"] = self.interactive_id
-
+        run_job_on_data_plane = False
+        compute_name = self.configuration_obj["configuration"].get("entity", {}).get("computeName", "")
+        if compute_name != "" and self.interactive_id:
+            pipeline_json_object["compute_template_id"] = self.interactive_id
+            run_job_on_data_plane=True
+        pipeline_json_object["run_job_on_data_plane"] = run_job_on_data_plane
+        snowflake_profile = self.configuration_obj["configuration"].get("pipeline_configs", {}).get("snowflake_profile", "")
+        if snowflake_profile!="":
+            pipeline_json_object["snowflake_profile"] = snowflake_profile
         warehouse = self.configuration_obj["configuration"].get("entity", {}).get("warehouse", "")
         if warehouse:
             pipeline_json_object["snowflake_warehouse"] = warehouse
+
         if domain_id is None and domain_name is None:
             pipeline_client_obj.logger.error('Either domainId or domain Name is required to create pipeline.')
             print('Either domainId or domain Name is required to create pipeline.')
             traceback.print_stack()
             raise Exception("Either domainId or domain Name is required to create pipeline.")
         if domain_name is not None and domain_id is None:
             domains_url_base = list_domains_url(pipeline_client_obj.client_config)
@@ -266,14 +227,16 @@
         pipeline_client_obj.logger.info(json_string)
         print(json_string)
         if json_string is not None:
             try:
                 response = requests.post(url_for_creating_pipeline, data=json_string, headers={
                     'Authorization': 'Bearer ' + pipeline_client_obj.client_config["bearer_token"],
                     'Content-Type': 'application/json'}, verify=False)
+                new_pipeline_creation_response = response.content
+                print("Pipeline creation response:",new_pipeline_creation_response)
                 if response.status_code == 406:
                     headers = pipeline_client_obj.regenerate_bearer_token_if_needed(
                         {'Authorization': 'Bearer ' + pipeline_client_obj.client_config["bearer_token"],
                          'Content-Type': 'application/json'})
                     response = requests.post(url_for_creating_pipeline, data=json_string, headers=headers, verify=False)
 
                 response = IWUtils.ejson_deserialize(response.content)
@@ -300,14 +263,17 @@
                         existing_pipeline_id = response.json().get("result", [])[0]["id"]
                     if existing_pipeline_id:
                         new_pipeline_id = str(existing_pipeline_id)
                 else:
                     new_pipeline_id = result.get('id')
                 pipeline_client_obj.logger.info(f'Pipeline ID: {new_pipeline_id}')
                 print(f'Pipeline ID: {new_pipeline_id}')
+                if new_pipeline_id is None:
+                    pipeline_client_obj.logger.exception('Pipeline creation response: {}'.format(str(new_pipeline_creation_response)))
+                    print('Pipeline creation response: {}'.format(str(new_pipeline_creation_response)))
             except Exception as ex:
                 pipeline_client_obj.logger.exception('Response from server: {}'.format(str(ex)))
                 print(f'Response from server: {str(ex)}')
 
         return new_pipeline_id, pipeline_json_object["domain_id"]
 
     def configure(self, pipeline_client_obj, pipeline_id, domain_id, override_dataconnection_config_file=None,
@@ -372,15 +338,14 @@
         url_for_importing_pipeline = configure_pipeline_url(pipeline_client_obj.client_config, domain_id, pipeline_id)
         pipeline_client_obj.logger.info(f"URL to configure pipeline: {url_for_importing_pipeline}")
         print(f"URL to configure pipeline: {url_for_importing_pipeline}")
         del self.configuration_obj["environment_configurations"]
         del self.configuration_obj["user_email"]
         json_string = IWUtils.ejson_serialize(
             {"configuration": self.configuration_obj["configuration"], "import_configs": import_configs})
-
         response = requests.post(url_for_importing_pipeline, data=json_string,
                                  headers={
                                      'Authorization': 'Bearer ' + pipeline_client_obj.client_config["bearer_token"],
                                      'Content-Type': 'application/json'}, verify=False)
         if response.status_code == 406:
             pipeline_client_obj.client_config['bearer_token'] = get_bearer_token(
                 pipeline_client_obj.client_config["protocol"],
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/csv_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,62 @@
-import copy
 import json
-
 import requests
 import yaml
-
 from infoworks.sdk.url_builder import get_source_details_url, list_secrets_url, create_domain_url
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.local_configurations import Response
-import configparser
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
 from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+import configparser
 
-
-class RDBMSSource:
-    def __init__(self):
-        self.configuration_obj = None
-        self.source_config_path = None
-        self.environment_id = None
-        self.storage_id = None
-        self.secrets = None
-
-    def set_variables(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
+class CSVSource:
+    def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
         self.storage_id = storage_id
         self.environment_id = environment_id
         self.source_config_path = source_config_path
+        self.secrets = secrets
         with open(self.source_config_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
-        self.secrets = secrets
-
-    def get_secret_id_from_name(self, cicd_client, secret_name):
-        secret_id = None
-        get_secret_details_url = list_secrets_url(cicd_client.client_config) + '?filter={"name":"' + secret_name + '"}'
-        response = cicd_client.call_api("GET", get_secret_details_url,
-                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
-        parsed_response = IWUtils.ejson_deserialize(response.content)
-        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
-            result = parsed_response.get("result", [])
-
-            if len(result) > 0:
-                secret_id = result[0]["id"]
-                cicd_client.logger.info("Found secret id {} ".format(secret_id))
-                return secret_id
-            else:
-                cicd_client.logger.info("Secret id is {} ".format(None))
-                return None
 
-    def update_table_schema_and_database(self, type, mappings):
-        data = self.configuration_obj
-        for table in data.get("configuration", {}).get("table_configs", []):
-            if type == "target_schema":
-                schema_from_config = table.get("configuration", {}).get("configuration", {}).get("target_schema_name",
-                                                                                                 "")
-                if schema_from_config != "" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_schema_name"] = mappings.get(
-                        schema_from_config.lower())
-            elif type == "stage_schema":
-                schema_from_config = table.get("configuration", {}).get("configuration", {}).get("staging_schema_name",
-                                                                                                 "")
-                if schema_from_config != "" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["staging_schema_name"] = mappings.get(
-                        schema_from_config.lower())
-            elif type == "database":
-                database_from_config = table.get("configuration", {}).get("configuration", {}).get(
-                    "target_database_name", "")
-                if database_from_config != "" and database_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_database_name"] = mappings.get(
-                        database_from_config.lower())
+    def replace_secret_name_with_mapping(self,data,src_client_obj):
+        for key, value in data.items():
+            if isinstance(value, dict):
+                # If the value is a dictionary, recurse into it
+                secret_name = self.replace_secret_name_with_mapping(value,src_client_obj)
+                if secret_name:
+                    return secret_name
+            elif key == "secret_name":
+                #print(f"Found secret_name: {value}")
+                # resolve secret name to ID
+                secret_id = self.get_secret_id_from_name(src_client_obj, value)
+                if secret_id:
+                    data["secret_id"] = secret_id
+                    data.pop('secret_name', None)
+                return value
+
+    def update_table_schema_and_database(self,type,mappings):
+        data=self.configuration_obj
+        for table in data.get("configuration",{}).get("table_configs",[]):
+            if type=="target_schema":
+                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
+                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
+            elif type=="stage_schema":
+                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("staging_schema_name","")
+                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["staging_schema_name"]=mappings.get(schema_from_config.lower())
+            elif type=="database":
+                database_from_config=table.get("configuration",{}).get("configuration",{}).get("target_database_name","")
+                if database_from_config!="" and database_from_config.lower() in mappings.keys():
+                    table["configuration"]["configuration"]["target_database_name"]=mappings.get(database_from_config.lower())
             else:
                 pass
 
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
@@ -84,43 +66,53 @@
             print("section:", section)
             try:
                 final = d.setval(section.split("$"), dict(config.items(section)))
             except KeyError as e:
                 pass
         self.configuration_obj = d.data
         if "configuration$source_configs$data_lake_schema" in config.sections():
-            self.update_table_schema_and_database("target_schema",
-                                                  dict(config.items("configuration$source_configs$data_lake_schema")))
+            self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
         if "configuration$source_configs$staging_schema_name" in config.sections():
-            self.update_table_schema_and_database("stage_schema", dict(
-                config.items("configuration$source_configs$staging_schema_name")))
+            self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
         if "configuration$source_configs$target_database_name" in config.sections():
-            self.update_table_schema_and_database("database", dict(
-                config.items("configuration$source_configs$target_database_name")))
+            self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
+
+    def get_secret_id_from_name(self,cicd_client,secret_name):
+        secret_id = None
+        get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"name":"'+secret_name+'"}'
+        response = cicd_client.call_api("GET", get_secret_details_url,
+                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
+        parsed_response = IWUtils.ejson_deserialize(response.content)
+        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+            result = parsed_response.get("result", [])
+
+            if len(result) > 0:
+                secret_id = result[0]["id"]
+                cicd_client.logger.info("Found secret id {} ".format(secret_id))
+                return secret_id
+            else:
+                cicd_client.logger.info("Secret id is {} ".format(None))
+                return None
 
-    def create_rdbms_source(self, src_client_obj):
+    def create_csv_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
-        create_rdbms_source_payload = {
+        create_csv_source_payload = {
             "name": data["name"],
-            "type": "rdbms",
+            "type": data["type"],
             "sub_type": data["sub_type"],
             "data_lake_path": data["data_lake_path"],
             "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
             "environment_id": self.environment_id,
             "storage_id": self.storage_id,
             "is_source_ingested": True
         }
-        if data.get("target_database_name", ""):
-            create_rdbms_source_payload["target_database_name"] = data.get("target_database_name", "")
-        if data.get("staging_schema_name", ""):
-            create_rdbms_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
-        additional_keys_in_source_config = data.keys()
-        for key in additional_keys_in_source_config:
-            if key not in ["connection"] and key not in create_rdbms_source_payload.keys():
-                create_rdbms_source_payload[key]=data[key]
+        if data.get("target_database_name",""):
+            create_csv_source_payload["target_database_name"] = data.get("target_database_name","")
+        if data.get("staging_schema_name",""):
+            create_csv_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
         # adding associated domains if any
         accessible_domain_names = data.get("associated_domain_names",[])
         accessible_domain_ids = []
         for domain_name in accessible_domain_names:
             domain_response = src_client_obj.call_api("GET",
                                                          create_domain_url(
                                                              src_client_obj.client_config) + "?filter={\"name\":\""+domain_name+"\"}",
@@ -130,36 +122,31 @@
             if domain_response.status_code == 200 and len(domain_parsed_response.get("result", [])) > 0:
                 result = domain_parsed_response.get("result", [])
                 if len(result) > 0:
                     result = result[0]
                     domain_id = result.get("id", None)
                     if domain_id is not None:
                         accessible_domain_ids.append(domain_id)
-            if "associated_domain_names" in create_rdbms_source_payload.keys():
-                create_rdbms_source_payload.pop("associated_domain_names",[])
-                self.configuration_obj["configuration"]["source_configs"].pop("associated_domain_names",[])
+            if "associated_domain_names" in create_csv_source_payload.keys():
+                create_csv_source_payload.pop("associated_domain_names",[])
+                self.configuration_obj["configuration"]["source_configs"].pop("associated_domain_names", [])
             if len(accessible_domain_ids) > 0:
-                create_rdbms_source_payload["associated_domains"] = accessible_domain_ids
-                self.configuration_obj["configuration"]["associated_domains"]=accessible_domain_ids
-        print("create_rdbms_source_payload:",create_rdbms_source_payload)
-        src_create_response = src_client_obj.create_source(source_config=create_rdbms_source_payload)
+                create_csv_source_payload["associated_domains"] = accessible_domain_ids
+                self.configuration_obj["configuration"]["associated_domains"] = accessible_domain_ids
+        print("create_csv_source_payload:", create_csv_source_payload)
+        src_create_response = src_client_obj.create_source(source_config=create_csv_source_payload)
         if src_create_response["result"]["status"].upper() == "SUCCESS":
-            source_id = src_create_response["result"]["response"]["result"]["id"]
-            #added below code to update the source due to IPD-23733
-            associated_domains = create_rdbms_source_payload.get("associated_domains", [])
-            if associated_domains:
-                src_client_obj.update_source(source_id=source_id,
-                                             update_body={"associated_domains": associated_domains})
+            source_id_created = src_create_response["result"]["source_id"]
+            print("Source created successfully")
             return src_create_response
         else:
             src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
             print('Cant create source {} '.format(data["name"]))
             print(src_create_response)
             src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
-            print(f"Getting the existing SourceId with name {data['name']} if exists")
             filter_condition = IWUtils.ejson_serialize({"name": data['name']})
             source_detail_url = get_source_details_url(
                 src_client_obj.client_config) + f"?filter={{filter_condition}}".format(
                 filter_condition=filter_condition)
             response = requests.get(source_detail_url,
                                     headers={'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
                                              'Content-Type': 'application/json'}, verify=False)
@@ -167,248 +154,239 @@
                 headers = src_client_obj.regenerate_bearer_token_if_needed(
                     {'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
                      'Content-Type': 'application/json'})
                 response = requests.get(source_detail_url, headers=headers, verify=False)
             response = IWUtils.ejson_deserialize(response.content)
             if not response.get('result', None):
                 src_client_obj.logger.error("Failed to make an api call to get source details")
-                src_client_obj.logger.info(response)
                 print("Failed to make an api call to get source details")
+                src_client_obj.logger.info(response)
                 print(response)
-                return SourceResponse.parse_result(status=Response.Status.FAILED, source_id=None, response=response)
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   source_id=None,response=response)
             else:
-                existing_source_id =response['result'][0]['id']
                 src_client_obj.logger.info(
                     f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 print(f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
-                # added below code to update the source due to IPD-23733
-                associated_domains=create_rdbms_source_payload.get("associated_domains",[])
-                if associated_domains:
-                    src_client_obj.update_source(source_id=existing_source_id, update_body={"associated_domains":associated_domains})
-                return SourceResponse.parse_result(status=Response.Status.SUCCESS,
-                                                   source_id=response['result'][0]['id'], response=response)
-
-    def configure_rdbms_source_connection(self, src_client_obj, source_id, override_config_file=None,
-                                          read_passwords_from_secrets=False, env_tag="", secret_type="",
-                                          config_ini_path=None, dont_skip_step=True):
-        if not dont_skip_step:
-            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        source_configs = self.configuration_obj["configuration"]["source_configs"]
-        src_name = str(source_configs["name"])
-        connection_object = source_configs["connection"]
-        if connection_object.get('connection_mode', '') != '':
-            connection_object['connection_mode'] = connection_object['connection_mode'].lower()
-        else:
-            connection_object['connection_mode'] = 'jdbc'
-        if override_config_file is not None:
-            with open(override_config_file) as file:
-                information = yaml.load(file, Loader=yaml.FullLoader)
-            if information["source_details"].get(src_name, None) is not None:
-                override_keys = information["source_details"].get(src_name).keys()
-                for key in override_keys:
-                    connection_object[key] = information["source_details"][src_name][key]
-        if connection_object.get("password", {}).get("password_type", "") == "secret_store":
-            # for RDBMS passwords in keyvault
-            secret_name = connection_object["password"]["secret_name"]
-            secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
-            if secret_name:
-                connection_object["password"]["secret_id"] = secret_id
-                connection_object["password"].pop('secret_name', None)
-        # if read_passwords_from_secrets and self.secrets["custom_secrets_read"] is True:
-        #     encrypted_key_name = f"{env_tag}-" + src_name
-        #     decrypt_value = self.secrets.get(encrypted_key_name, "")
-        #     if IWUtils.is_json(decrypt_value):
-        #         decrypt_value_dict = json.loads(decrypt_value)
-        #         for key in decrypt_value_dict.keys():
-        #             connection_object[key] = decrypt_value_dict[key]
-        # elif read_passwords_from_secrets and self.secrets["custom_secrets_read"] is False:
-        #     encrypted_key_name = f"{env_tag}-" + src_name
-        #     decrypt_value = src_client_obj.get_all_secrets(secret_type,keys=encrypted_key_name,ini_config_file_path=config_ini_path)
-        #     if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-        #         decrypt_value_dict = json.loads(decrypt_value[0])
-        #         for key in decrypt_value_dict.keys():
-        #             connection_object[key] = decrypt_value_dict[key]
-        response = src_client_obj.configure_source_connection(source_id, connection_object=connection_object)
-        if response["result"]["status"].upper() != "SUCCESS":
-            src_client_obj.logger.info(f"Failed to configure the source {source_id} connection")
-            print(f"Failed to configure the source {source_id} connection")
-            src_client_obj.logger.info(response)
-            print(response)
-            return SourceResponse.parse_result(status=Response.Status.FAILED, source_id=source_id, response=response)
-        else:
-            src_client_obj.logger.info(response)
-            print(response)
-            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id, response=response)
-
-    def test_source_connection(self, src_client_obj, source_id, dont_skip_step=True):
-        if not dont_skip_step:
-            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        response = src_client_obj.source_test_connection_job_poll(source_id, poll_timeout=300,
-                                                                  polling_frequency=15, retries=1)
-        return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id, response=response)
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=response['result'][0]['id'],response=response)
 
-    def browse_source_tables(self, src_client_obj, source_id, dont_skip_step=True):
+    def configure_csv_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
+                             secret_type="",config_ini_path=None,dont_skip_step=True):
         if not dont_skip_step:
             return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        filter_tables_properties = self.configuration_obj["filter_tables_properties"]
-        response = src_client_obj.browse_source_tables(source_id, filter_tables_properties=filter_tables_properties,
-                                                       poll_timeout=300, polling_frequency=15, retries=1)
-        return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
-                                           response=response)
-
-    def add_tables_to_source(self, src_client_obj, source_id, dont_skip_step=True):
-        if not dont_skip_step:
-            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        tables_already_added_in_source = src_client_obj.list_tables_in_source(source_id).get("result", {}).get(
-            "response", {}).get("result", [])
-        tables_already_added_in_source = [table.get("schema_name_at_source",
-                                                                     table.get("catalog_name",
-                                                                                                "")) + "." + table[
-                                              "name"] for table in tables_already_added_in_source]
-        tables_list = []
-        tables = self.configuration_obj["configuration"]["table_configs"]
-        if len(tables_already_added_in_source) > 0:
-            for table in tables:
-                if table["configuration"].get("schema_name_at_source",
-                                              table["configuration"].get("catalog_name", "")) + "." + \
-                        table["configuration"][
-                            "name"] not in tables_already_added_in_source:
-                    temp = {"table_name": table["configuration"]["name"],
-                            "table_type": table.get("table_type","TABLE").upper(),
-                            "target_table_name": table["configuration"]["configuration"]["target_table_name"],
-                            "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
-                    if table["configuration"].get("catalog_name", "") != "":
-                        temp["catalog_name"] = table["configuration"]["catalog_name"]
-                    if table["configuration"].get("schema_name_at_source", "") != "":
-                        temp["schema_name"] = table["configuration"]["schema_name_at_source"]
-                    if table["configuration"].get("configuration", {}).get("configuration", {}).get("target_database_name","") != "":
-                        temp["target_database_name"] = table["configuration"]["configuration"]["target_database_name"]
-                    tables_list.append(copy.deepcopy(temp))
-                    src_client_obj.logger.info(
-                        f"Adding table {temp['table_name']} to source {source_id} config payload")
-        else:
-            for table in tables:
-                temp = {"table_name": table["configuration"]["name"],
-                        "table_type": table.get("table_type","TABLE").upper(),
-                        "target_table_name": table["configuration"]["configuration"]["target_table_name"],
-                        "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
-                if table["configuration"].get("catalog_name", "") != "":
-                    temp["catalog_name"] = table["configuration"]["catalog_name"]
-                if table["configuration"].get("schema_name_at_source", "") != "":
-                    temp["schema_name"] = table["configuration"]["schema_name_at_source"]
-                if table["configuration"].get("configuration", {}).get("configuration", {}).get("target_database_name",
-                                                                                                "") != "":
-                    temp["target_database_name"] = table["configuration"]["configuration"]["target_database_name"]
-                tables_list.append(copy.deepcopy(temp))
-                src_client_obj.logger.info(f"Adding table {temp['table_name']} to source {source_id} config payload")
-        if len(tables_list) > 0:
-            response = src_client_obj.add_tables_to_source(source_id, tables_list)
-            return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
-                                               response=response)
+        data = self.configuration_obj["configuration"]["source_configs"]["connection"]
+        src_name = str(self.configuration_obj["configuration"]["source_configs"]["name"])
+        storage_type = data["storage"]["storage_type"]
+        cloud_type = data["storage"].get("cloud_type", None)
+        if storage_type == "cloud" and "project_id" in data["storage"]:
+            project_id = data["storage"]["project_id"]
+            server_path = data["storage"]["server_path"]
+            if "gcp_details" in mappings:
+                project_id = mappings["gcp_details"].get("project_id", project_id)
+                server_path = mappings["gcp_details"].get("service_json_path", server_path)
+            if "gcp_project_id_mappings" in mappings:
+                project_id = mappings["gcp_project_id_mappings"].get(data["storage"]["project_id"], project_id)
+            if "service_json_mappings" in mappings:
+                server_path = mappings["service_json_mappings"].get(data["storage"]["server_path"].split("/")[-1],
+                                                                    server_path)
+
+            source_configure_payload = {
+                "source_base_path_relative": data.get("source_base_path_relative",""),
+                "source_base_path": data.get("source_base_path",""),
+                "storage": {
+                    "cloud_type": "gs",
+                    "storage_type": data["storage"]["storage_type"],
+                    "project_id": project_id,
+                    "access_type": data["storage"]["access_type"],
+                    "server_path": server_path,
+                    "upload_option": data["storage"]["upload_option"],
+                    "file_details": []
+                }
+            }
+        # elif storage_type == "remote":
+        #     # SFTP Source
+        #     data = self.configuration_obj["configuration"]["source_configs"]["connection"]
+        #     source_configure_payload = data
+        #     source_configure_payload["source_base_path"]=""
+        #     if data.get("storage", {}).get("password", {}).get("password_type","") == "secret_store":
+        #         # for SFTP password auth
+        #         secret_name = data["storage"]["password"]["secret_name"]
+        #         secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+        #         if secret_name:
+        #             data["storage"]["password"]["secret_id"] = secret_id
+        #             data["storage"]["password"].pop('secret_name', None)
+        #     elif data.get("storage", {}).get("access_key_name", {}).get("password_type","") == "secret_store":
+        #         # for adls gen2 storage account access key auth
+        #         secret_name = data["storage"]["access_key_name"]["secret_name"]
+        #         secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+        #         if secret_name:
+        #             data["storage"]["access_key_name"]["secret_id"] = secret_id
+        #             data["storage"]["access_key_name"].pop('secret_name', None)
+        #     elif data.get("storage", {}).get("service_credential", {}).get("password_type","") == "secret_store":
+        #         # for adls gen2 service credential auth
+        #         secret_name = data["storage"]["service_credential"]["secret_name"]
+        #         secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+        #         if secret_name:
+        #             data["storage"]["service_credential"]["secret_id"] = secret_id
+        #             data["storage"]["service_credential"].pop('secret_name', None)
+        #     elif data.get("storage", {}).get("account_key", {}).get("password_type","") == "secret_store":
+        #         #for blob storage account key auth
+        #         secret_name = data["storage"]["account_key"]["secret_name"]
+        #         secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+        #         if secret_name:
+        #             data["storage"]["account_key"]["secret_id"] = secret_id
+        #             data["storage"]["account_key"].pop('secret_name', None)
+        #     else:
+        #         pass
         else:
-            src_client_obj.logger.info(f"No new tables found to add.")
-            print(f"No new tables found to add.")
-            return SourceResponse.parse_result(status="SUCCESS", source_id=source_id,
-                                               response={})
-
-    def update_schema_for_tables(self,src_client_obj, source_id, export_configuration_file=None,
-                                         export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
-                                         env_tag="", secret_type="", dont_skip_step=True):
+            source_configure_payload = data
+            self.replace_secret_name_with_mapping(data,src_client_obj)
+        response = src_client_obj.configure_source_connection(source_id, connection_object=source_configure_payload)
+        return response
+
+    def import_source_configuration(self, src_client_obj, source_id,
+                                    mappings, export_configuration_file=None, export_config_lookup=True,
+                                    read_passwords_from_secrets=False,dont_skip_step=True):
         if not dont_skip_step:
             return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        tables = self.configuration_obj["configuration"]["table_configs"]
-        table_schema_update_dict={}
-        for table in tables:
-            table_name = table["configuration"]["name"]
-            src_client_obj.logger.info(f"Updating the schema information for table {table_name}")
-            columns = table["configuration"]["columns"]
-            table_update_payload = {"name": table_name,"source":source_id,"columns":columns}
-            table_document=[]
-            if table["configuration"].get("schema_name_at_source","")!="":
-                table_document = src_client_obj.list_tables_in_source(source_id,params={"filter":{"origTableName":table["configuration"]["name"],"schemaNameAtSource":table["configuration"]["schema_name_at_source"]}}).get("result",{}).get("response",{}).get("result",[])
+        src_name = self.configuration_obj["configuration"]["source_configs"]["name"]
+        source_import_payload = {"configuration": self.configuration_obj["configuration"]}
+        modified_table_configs = self.configuration_obj["configuration"]["table_configs"]
+        index = 0
+        for table_config in self.configuration_obj["configuration"]["table_configs"]:
+            modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+            if not table_config["configuration"].get("meta_crawl_performed", False):
+                modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
             else:
-                table_document = src_client_obj.list_tables_in_source(source_id,params={"filter":{"origTableName":table["configuration"]["name"],"catalog_name":table["configuration"]["catalog_name"]}}).get("result",{}).get("response",{}).get("result",[])
-            if len(table_document)>0:
-                table_document=table_document[0]
-            table_id = table_document["id"]
-            response = src_client_obj.update_table_configuration(source_id=source_id,table_id=table_id,config_body=table_update_payload)
-            if response["result"]["status"].upper() != "SUCCESS":
-                src_client_obj.logger.error("Failed to update schema for table {table_name}".format(table_name=table_name))
-                src_client_obj.logger.error(response.get("result", {}).get("response",{}).get("message", ""))
-                table_schema_update_dict[table_name] = ("FAILED",response.get("result", {}).get("response",{}).get("message", ""))
-            else:
-                src_client_obj.logger.info("Successfully updated schema for table {table_name}".format(table_name=table_name))
-                table_schema_update_dict[table_name] = ("SUCCESS","")
-        failed_schema_update_tables = [(table_name,status[1]) for table_name,status in table_schema_update_dict.items() if status[0].upper() == "FAILED"]
-        overall_update_status = "FAILED" if len(failed_schema_update_tables)>0 else "SUCCESS"
-        if overall_update_status =="FAILED":
-            response = {f"Tables schema update failed for tables:{failed_schema_update_tables}"}
-        else:
-            response = {f"Tables schema updated successfully"}
-        return SourceResponse.parse_result(status=overall_update_status, source_id=source_id,
-                                                   response=response)
-
-    def configure_tables_and_tablegroups(self, src_client_obj, source_id, export_configuration_file=None,
-                                         export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
-                                         env_tag="", secret_type="", dont_skip_step=True):
-        if not dont_skip_step:
-            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
-        if mappings is None:
-            mappings = {}
-        source_configs = self.configuration_obj["configuration"]["source_configs"]
-        src_name = str(source_configs["name"])
-        # Update the service account json file mappings if any
+                if not table_config["configuration"]["meta_crawl_performed"]:
+                    modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
+        source_import_payload["configuration"]["table_configs"] = modified_table_configs
         if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
-            for table in self.configuration_obj["configuration"]["table_configs"]:
+            for table in source_import_payload.get("configuration")["table_configs"]:
                 # Check if there are any export configurations and passwords to replace
                 if table.get("configuration", {}).get("export_configuration", None) is not None:
                     export_configs = table.get("configuration", {}).get("export_configuration")
                     target_type = export_configs.get("target_type", "").upper()
                     table_name = table["configuration"]["name"].upper()
                     override_keys = []
-                    if export_configuration_file is not None:
-                        with open(export_configuration_file) as file:
-                            information = yaml.load(file, Loader=yaml.FullLoader)
-                        if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
-                            info_key = src_name + "_" + table_name
-                            override_keys = information["src_export_details"].get(src_name + "_" + table_name,
-                                                                                  {}).keys()
-                        else:
-                            info_key = src_name
-                            override_keys = information["src_export_details"].get(src_name, {}).keys()
-                        for key in override_keys:
-                            table["configuration"]["export_configuration"]["connection"][key] = \
-                                information["src_export_details"][info_key][key]
-                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"]:
-                        pass
-
-                    elif target_type.upper() == "BIGQUERY":
-                        if "server_path" not in override_keys:
-                            server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
-                                "server_path", "")
-                            if "gcp_details" in mappings:
-                                server_path = mappings["gcp_details"].get("service_json_path")
-                            if "service_json_mappings" in mappings:
-                                server_path = mappings["service_json_mappings"].get(
-                                    server_path.split("/")[-1],
-                                    server_path)
+                    try:
+                        if export_configuration_file is not None:
+                            with open(export_configuration_file) as file:
+                                information = yaml.load(file, Loader=yaml.FullLoader)
+                            if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
+                                info_key = src_name + "_" + table_name
+                                override_keys = information["src_export_details"].get(src_name + "_" + table_name,
+                                                                                      {}).keys()
+                            else:
+                                info_key = src_name
+                                override_keys = information["src_export_details"].get(src_name, {}).keys()
+                            for key in override_keys:
+                                table["configuration"]["export_configuration"]["connection"][key] = \
+                                    information["src_export_details"][info_key][key]
+                    except Exception as e:
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration file {export_configuration_file} due to {str(e)}")
+
+                    try:
+                        if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
+                            # Read the password from KMS
+                            encrypted_key_name1 = f"export-configuration-{src_name}-{table['configuration']['name']}"
+                            encrypted_key_name2 = f"export-configuration-{src_name}"
+                            passwd = self.secrets.get(encrypted_key_name1, "")
+                            if passwd == "":
+                                passwd = self.secrets.get(encrypted_key_name2, "")
+                            table["configuration"]["export_configuration"]["connection"]["password"] = passwd
+                        elif target_type.upper() == "BIGQUERY":
+                            if "server_path" not in override_keys:
+                                server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
+                                if "gcp_details" in mappings:
+                                    server_path = mappings["gcp_details"].get("service_json_path")
+                                if "service_json_mappings" in mappings:
+                                    server_path = mappings["service_json_mappings"].get(
+                                        server_path.split("/")[-1],
+                                        server_path)
+                                table["configuration"]["export_configuration"]["connection"][
+                                    "server_path"] = server_path if server_path != "" else table["configuration"][
+                                    "export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
                             table["configuration"]["export_configuration"]["connection"][
-                                "server_path"] = server_path if server_path != "" else table["configuration"][
-                                "export_configuration"].get("connection", {}).get(
-                                "server_path", "")
-                        table["configuration"]["export_configuration"]["connection"][
-                            "upload_option"] = "serverLocation"
-
-        response = src_client_obj.configure_tables_and_tablegroups(source_id, configuration_obj=self.configuration_obj[
-            "configuration"])
-        if response["result"]["status"].upper() != "SUCCESS":
-            src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
-                                        .format(source_id, self.source_config_path))
-            src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
-                                        .format(self.source_config_path))
-            return SourceResponse.parse_result(status="FAILED", source_id=source_id,
-                                               response=response)
+                                "upload_option"] = "serverLocation"
+                    except Exception as e:
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration password from secrets due to {str(e)}")
+        response = src_client_obj.configure_tables_and_tablegroups(source_id,
+                                                                   configuration_obj=source_import_payload.get(
+                                                                       "configuration"))
+        return response
+        # if response["result"]["status"].upper() != "SUCCESS":
+        #     src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
+        #                                 .format(source_id, self.source_config_path))
+        #     src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
+        #                                 .format(self.source_config_path))
+        #     return "FAILED"
+        # else:
+        #     src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
+        #     return "SUCCESS"
 
+    def update_table_watermarks_and_state_as_ready(self,src_client_obj, source_id):
+        tables = self.configuration_obj["configuration"]["table_configs"]
+        table_state_update_dict = {}
+        tables_watermark_mappings = self.configuration_obj.get("table_watermark_mappings", {})
+        for table in tables:
+            table_name = table["configuration"]["name"]
+            src_client_obj.logger.info(f"Updating the table state information for table {table_name}")
+            table_update_payload = {"name": table_name, "source": source_id, "state": "ready"}
+            if tables_watermark_mappings:
+                current_table_id = table["entity_id"]
+                current_table_watermark_mappings = tables_watermark_mappings.get(current_table_id,{})
+                for key,value in current_table_watermark_mappings.items():
+                    if key in ["last_ingested_cdc_value","last_merged_watermark"]:
+                        table_update_payload[key] = f'"{value}"'
+                    else:
+                        table_update_payload[key] = value
+            print("table_update_payload:",table_update_payload)
+            if table["configuration"].get("schema_name_at_source", "") != "":
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "schemaNameAtSource": table["configuration"]["schema_name_at_source"]}}).get("result",
+                                                                                                            {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"].get("catalog_name", ""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"origTableName": table["configuration"]["name"],
+                               "catalog_name": table["configuration"]["catalog_name"]}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            elif table["configuration"]["configuration"].get("query",""):
+                table_document = src_client_obj.list_tables_in_source(source_id, params={
+                    "filter": {"table": table_name}}).get("result", {}).get(
+                    "response", {}).get("result", [])
+            else:
+                print(f"Skipping updating state for table {table_name} as it did not match any existing table.")
+            table_id = None
+            if len(table_document) > 0:
+                table_document = table_document[0]
+                table_id = table_document["id"]
+            if table_id is not None:
+                response = src_client_obj.update_table_configuration(source_id=source_id, table_id=table_id,
+                                                                     config_body=table_update_payload)
+                if response["result"]["status"].upper() != "SUCCESS":
+                    src_client_obj.logger.error(
+                        "Failed to update state for table {table_name}".format(table_name=table_name))
+                    src_client_obj.logger.error(response.get("result", {}).get("response", {}).get("message", ""))
+                    table_state_update_dict[table_name] = (
+                    "FAILED", response.get("result", {}).get("response", {}).get("message", ""))
+                else:
+                    src_client_obj.logger.info(
+                        "Successfully updated state for table {table_name}".format(table_name=table_name))
+                    table_state_update_dict[table_name] = ("SUCCESS", "")
+        failed_state_update_tables = [(table_name, status[1]) for table_name, status in
+                                       table_state_update_dict.items() if status[0].upper() == "FAILED"]
+        overall_update_status = "FAILED" if len(failed_state_update_tables) > 0 else "SUCCESS"
+        if overall_update_status == "FAILED":
+            response = {f"Tables state update failed for tables:{failed_state_update_tables}"}
         else:
-            src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
-            return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
-                                               response=response)
+            response = {f"Tables state updated successfully"}
+        return SourceResponse.parse_result(status=overall_update_status, source_id=source_id,
+                                           response=response)
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/streaming_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import json
-
 import requests
 import yaml
-
-from infoworks.sdk.url_builder import get_source_details_url
+from infoworks.sdk.url_builder import get_source_details_url, list_secrets_url, create_domain_url
 from infoworks.sdk.utils import IWUtils
-import configparser
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+from infoworks.sdk.source_response import SourceResponse
+from infoworks.sdk.local_configurations import Response
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+import configparser
 
-class SalesforceSource:
-    def __init__(self):
-        self.configuration_obj = None
-        self.source_config_path = None
-        self.environment_id = None
-        self.storage_id = None
-        self.secrets = None
-
-    def set_variables(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
+class StreamingSource:
+    def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
         self.storage_id = storage_id
         self.environment_id = environment_id
         self.source_config_path = source_config_path
+        self.secrets = secrets
         with open(self.source_config_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
-        self.secrets = secrets
+
+    def replace_secret_name_with_mapping(self,data,src_client_obj):
+        for key, value in data.items():
+            if isinstance(value, dict):
+                # If the value is a dictionary, recurse into it
+                secret_name = self.replace_secret_name_with_mapping(value,src_client_obj)
+                if secret_name:
+                    return secret_name
+            elif key == "secret_name":
+                #print(f"Found secret_name: {value}")
+                # resolve secret name to ID
+                secret_id = self.get_secret_id_from_name(src_client_obj, value)
+                if secret_id:
+                    data["secret_id"] = secret_id
+                    data.pop('secret_name', None)
+                return value
 
     def update_table_schema_and_database(self,type,mappings):
         data=self.configuration_obj
         for table in data.get("configuration",{}).get("table_configs",[]):
             if type=="target_schema":
                 schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
                 if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
@@ -63,32 +72,80 @@
         if "configuration$source_configs$data_lake_schema" in config.sections():
             self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
         if "configuration$source_configs$staging_schema_name" in config.sections():
             self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
         if "configuration$source_configs$target_database_name" in config.sections():
             self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
 
-    def create_salesforce_source(self, src_client_obj):
+    def get_secret_id_from_name(self,cicd_client,secret_name):
+        secret_id = None
+        get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"name":"'+secret_name+'"}'
+        response = cicd_client.call_api("GET", get_secret_details_url,
+                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
+        parsed_response = IWUtils.ejson_deserialize(response.content)
+        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+            result = parsed_response.get("result", [])
+
+            if len(result) > 0:
+                secret_id = result[0]["id"]
+                cicd_client.logger.info("Found secret id {} ".format(secret_id))
+                return secret_id
+            else:
+                cicd_client.logger.info("Secret id is {} ".format(None))
+                return None
+
+    def create_streaming_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
-        create_salesforce_source_payload = {
+        create_streaming_source_payload = {
             "name": data["name"],
-            "type": "crm",
+            "type": data["type"],
             "sub_type": data["sub_type"],
             "data_lake_path": data["data_lake_path"],
             "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
             "environment_id": self.environment_id,
             "storage_id": self.storage_id,
             "is_source_ingested": True
         }
-        src_create_response = src_client_obj.create_source(source_config=create_salesforce_source_payload)
+        if data.get("target_database_name",""):
+            create_streaming_source_payload["target_database_name"] = data.get("target_database_name","")
+        if data.get("staging_schema_name",""):
+            create_streaming_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
+        # adding associated domains if any
+        accessible_domain_names = data.get("associated_domain_names",[])
+        accessible_domain_ids = []
+        for domain_name in accessible_domain_names:
+            domain_response = src_client_obj.call_api("GET",
+                                                         create_domain_url(
+                                                             src_client_obj.client_config) + "?filter={\"name\":\""+domain_name+"\"}",
+                                                         IWUtils.get_default_header_for_v3(
+                                                             src_client_obj.client_config['bearer_token']))
+            domain_parsed_response = IWUtils.ejson_deserialize(domain_response.content)
+            if domain_response.status_code == 200 and len(domain_parsed_response.get("result", [])) > 0:
+                result = domain_parsed_response.get("result", [])
+                if len(result) > 0:
+                    result = result[0]
+                    domain_id = result.get("id", None)
+                    if domain_id is not None:
+                        accessible_domain_ids.append(domain_id)
+            if "associated_domain_names" in create_streaming_source_payload.keys():
+                create_streaming_source_payload.pop("associated_domain_names",[])
+                self.configuration_obj["configuration"]["source_configs"].pop("associated_domain_names", [])
+            if len(accessible_domain_ids) > 0:
+                create_streaming_source_payload["associated_domains"] = accessible_domain_ids
+                self.configuration_obj["configuration"]["associated_domains"] = accessible_domain_ids
+        print("create_streaming_source_payload:", create_streaming_source_payload)
+        src_create_response = src_client_obj.create_source(source_config=create_streaming_source_payload)
         if src_create_response["result"]["status"].upper() == "SUCCESS":
             source_id_created = src_create_response["result"]["source_id"]
-            return source_id_created
+            print("Source created successfully")
+            return src_create_response
         else:
             src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
+            print('Cant create source {} '.format(data["name"]))
+            print(src_create_response)
             src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
             filter_condition = IWUtils.ejson_serialize({"name": data['name']})
             source_detail_url = get_source_details_url(
                 src_client_obj.client_config) + f"?filter={{filter_condition}}".format(
                 filter_condition=filter_condition)
             response = requests.get(source_detail_url,
                                     headers={'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
@@ -97,111 +154,115 @@
                 headers = src_client_obj.regenerate_bearer_token_if_needed(
                     {'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
                      'Content-Type': 'application/json'})
                 response = requests.get(source_detail_url, headers=headers, verify=False)
             response = IWUtils.ejson_deserialize(response.content)
             if not response.get('result', None):
                 src_client_obj.logger.error("Failed to make an api call to get source details")
+                print("Failed to make an api call to get source details")
                 src_client_obj.logger.info(response)
+                print(response)
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   source_id=None,response=response)
             else:
                 src_client_obj.logger.info(
                     f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
-                return response['result'][0]['id']
+                print(f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=response['result'][0]['id'],response=response)
 
-    def configure_salesforce_source_connection(self, src_client_obj, source_id, override_config_file=None,
-                                          read_passwords_from_secrets=False, env_tag="", secret_type=""):
-        source_configs = self.configuration_obj["configuration"]["source_configs"]
-        src_name = str(source_configs["name"])
-        connection_object = source_configs["connection"]
-        connection_object["fetch_mechanism"]=connection_object["fetch_mechanism"].lower()
-        if override_config_file is not None:
-            with open(override_config_file) as file:
-                information = yaml.load(file, Loader=yaml.FullLoader)
-            if information["source_details"].get(src_name, None) is not None:
-                override_keys = information["source_details"].get(src_name).keys()
-                for key in override_keys:
-                    connection_object[key] = information["source_details"][src_name][key]
-        response = src_client_obj.configure_source_connection(source_id, connection_object=connection_object)
-        if response["result"]["status"].upper() != "SUCCESS":
-            src_client_obj.logger.info(f"Failed to configure the source {source_id} connection")
-            src_client_obj.logger.info(response["result"])
-            return "FAILED"
-        else:
-            src_client_obj.logger.info(response["result"])
-            return "SUCCESS"
-
-    def test_source_connection(self, src_client_obj, source_id):
-        response = src_client_obj.source_test_connection_job_poll(source_id, poll_timeout=300,
-                                                                  polling_frequency=15, retries=1)
-        return response["result"]["status"].upper()
-
-    def metacrawl_source(self,src_client_obj,source_id):
-        response = src_client_obj.source_metacrawl_job_poll(source_id, poll_timeout=300,
-                                                                  polling_frequency=15, retries=1)
-        return response["result"]["status"].upper()
-
-    def configure_tables_and_tablegroups(self, src_client_obj, source_id, export_configuration_file=None,
-                                         export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
-                                         env_tag="", secret_type=""):
-        if mappings is None:
-            mappings = {}
-        iw_mappings = self.configuration_obj["configuration"]["iw_mappings"]
-        table_group_compute_mappings = mappings.get("table_group_compute_mappings", {})
-        source_configs = self.configuration_obj["configuration"]["source_configs"]
-        src_name = str(source_configs["name"])
-        for item in iw_mappings:
-            if item.get("entity_type", "") == "environment_compute_template":
-                item["recommendation"]["compute_name"] = table_group_compute_mappings.get(
-                    item["recommendation"]["compute_name"], item["recommendation"]["compute_name"])
-        self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
-        # Update the service account json file mappings if any
+    def configure_streaming_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
+                             secret_type="",config_ini_path=None,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        data = self.configuration_obj["configuration"]["source_configs"]["connection"]
+        src_name = str(self.configuration_obj["configuration"]["source_configs"]["name"])
+        source_configure_payload = data
+        self.replace_secret_name_with_mapping(data,src_client_obj)
+        response = src_client_obj.configure_source_connection(source_id, connection_object=source_configure_payload)
+        return response
+
+    def import_source_configuration(self, src_client_obj, source_id,
+                                    mappings, export_configuration_file=None, export_config_lookup=True,
+                                    read_passwords_from_secrets=False,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        src_name = self.configuration_obj["configuration"]["source_configs"]["name"]
+        source_import_payload = {"configuration": self.configuration_obj["configuration"]}
+        modified_table_configs = self.configuration_obj["configuration"]["table_configs"]
+        index = 0
+        for table_config in self.configuration_obj["configuration"]["table_configs"]:
+            modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+            if not table_config["configuration"].get("meta_crawl_performed", False):
+                modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
+            else:
+                if not table_config["configuration"]["meta_crawl_performed"]:
+                    modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
+        source_import_payload["configuration"]["table_configs"] = modified_table_configs
         if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
-            for table in self.configuration_obj["configuration"]["table_configs"]:
+            for table in source_import_payload.get("configuration")["table_configs"]:
                 # Check if there are any export configurations and passwords to replace
                 if table.get("configuration", {}).get("export_configuration", None) is not None:
                     export_configs = table.get("configuration", {}).get("export_configuration")
                     target_type = export_configs.get("target_type", "").upper()
                     table_name = table["configuration"]["name"].upper()
                     override_keys = []
-                    if export_configuration_file is not None:
-                        with open(export_configuration_file) as file:
-                            information = yaml.load(file, Loader=yaml.FullLoader)
-                        if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
-                            info_key = src_name + "_" + table_name
-                            override_keys = information["src_export_details"].get(src_name + "_" + table_name,
-                                                                                  {}).keys()
-                        else:
-                            info_key = src_name
-                            override_keys = information["src_export_details"].get(src_name, {}).keys()
-                        for key in override_keys:
-                            table["configuration"]["export_configuration"]["connection"][key] = \
-                                information["src_export_details"][info_key][key]
-                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"]:
-                        pass
-                    elif target_type.upper() == "BIGQUERY":
-                        if "server_path" not in override_keys:
-                            server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
-                                "server_path", "")
-                            if "gcp_details" in mappings:
-                                server_path = mappings["gcp_details"].get("service_json_path")
-                            if "service_json_mappings" in mappings:
-                                server_path = mappings["service_json_mappings"].get(
-                                    server_path.split("/")[-1],
-                                    server_path)
+                    try:
+                        if export_configuration_file is not None:
+                            with open(export_configuration_file) as file:
+                                information = yaml.load(file, Loader=yaml.FullLoader)
+                            if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
+                                info_key = src_name + "_" + table_name
+                                override_keys = information["src_export_details"].get(src_name + "_" + table_name,
+                                                                                      {}).keys()
+                            else:
+                                info_key = src_name
+                                override_keys = information["src_export_details"].get(src_name, {}).keys()
+                            for key in override_keys:
+                                table["configuration"]["export_configuration"]["connection"][key] = \
+                                    information["src_export_details"][info_key][key]
+                    except Exception as e:
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration file {export_configuration_file} due to {str(e)}")
+
+                    try:
+                        if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
+                            # Read the password from KMS
+                            encrypted_key_name1 = f"export-configuration-{src_name}-{table['configuration']['name']}"
+                            encrypted_key_name2 = f"export-configuration-{src_name}"
+                            passwd = self.secrets.get(encrypted_key_name1, "")
+                            if passwd == "":
+                                passwd = self.secrets.get(encrypted_key_name2, "")
+                            table["configuration"]["export_configuration"]["connection"]["password"] = passwd
+                        elif target_type.upper() == "BIGQUERY":
+                            if "server_path" not in override_keys:
+                                server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
+                                if "gcp_details" in mappings:
+                                    server_path = mappings["gcp_details"].get("service_json_path")
+                                if "service_json_mappings" in mappings:
+                                    server_path = mappings["service_json_mappings"].get(
+                                        server_path.split("/")[-1],
+                                        server_path)
+                                table["configuration"]["export_configuration"]["connection"][
+                                    "server_path"] = server_path if server_path != "" else table["configuration"][
+                                    "export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
                             table["configuration"]["export_configuration"]["connection"][
-                                "server_path"] = server_path if server_path != "" else table["configuration"][
-                                "export_configuration"].get("connection", {}).get(
-                                "server_path", "")
-                        table["configuration"]["export_configuration"]["connection"][
-                            "upload_option"] = "serverLocation"
-
-        response = src_client_obj.configure_tables_and_tablegroups(source_id, configuration_obj=self.configuration_obj[
-            "configuration"])
-        if response["result"]["status"].upper() != "SUCCESS":
-            src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
-                                        .format(source_id, self.source_config_path))
-            src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
-                                        .format(self.source_config_path))
-            return "FAILED"
-        else:
-            src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
-            return "SUCCESS"
+                                "upload_option"] = "serverLocation"
+                    except Exception as e:
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration password from secrets due to {str(e)}")
+        response = src_client_obj.configure_tables_and_tablegroups(source_id,
+                                                                   configuration_obj=source_import_payload.get(
+                                                                       "configuration"))
+        return response
+        # if response["result"]["status"].upper() != "SUCCESS":
+        #     src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
+        #                                 .format(source_id, self.source_config_path))
+        #     src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
+        #                                 .format(self.source_config_path))
+        #     return "FAILED"
+        # else:
+        #     src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
+        #     return "SUCCESS"
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/update_configurations.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/update_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/workflow.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/workflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import traceback
 
 from infoworks.sdk import url_builder
 from infoworks.sdk.base_client import BaseClient
-from infoworks.sdk.cicd.upload_configurations.pipelines import Pipeline, create_sql_pipeline_version
+from infoworks.sdk.cicd.upload_configurations.pipelines import Pipeline
 from infoworks.sdk.cicd.upload_configurations.pipeline_group import PipelineGroup
 from pathlib import Path
 from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.local_configurations import Response
 import os.path
 import queue
@@ -110,15 +110,14 @@
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
                                 self.client_config['bearer_token'])).content)
                         result = response.get("result", [])
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=compute_details)
         except Exception as e:
             self.logger.error("Error in getting compute template details")
-
     def cicd_create_configure_pipeline(self, configuration_file_path, domain_id=None, domain_name=None,
                                        override_configuration_file=None,
                                        replace_words="", read_passwords_from_secrets=False, env_tag="", secret_type=""):
         """
         Function to create and configure pipeline using the pipeline configuration JSON file
         Pass either domain_id or domain_name.If both are not passed the name of the domain should be first part of the file name
         :param configuration_file_path: Path of the file with pipeline configurations to be imported
@@ -177,23 +176,15 @@
             pl_obj = Pipeline(configuration_file_path, env_id, storage_id, compute_id, replace_words,
                               self.secrets_config)
             pl_obj.configuration_obj = configuration_obj
             pl_obj.update_mappings_for_configurations(self.mappings)
             pipeline_id, domain_id = pl_obj.create(self, domain_id, domain_name)
 
             if pipeline_id is not None:
-                pl_type = configuration_obj.get("pipeline_configs", {}).get("type", "")
-                if pl_type == "sql":
-                    sql_query = configuration_obj.get("pipeline_configs", {}).get("query", "")
-                    pl_params = configuration_obj.get("pipeline_configs", {}).get("pipeline_parameters", "")
-                    pl_version = create_sql_pipeline_version(pl_obj, pipeline_id=pipeline_id, domain_id=domain_id,
-                                                             sql_query=sql_query,
-                                                             pipeline_parameters=pl_params)
-                else:
-                    status = pl_obj.configure(self, pipeline_id, domain_id, override_configuration_file, self.mappings,
+                status = pl_obj.configure(self, pipeline_id, domain_id, override_configuration_file, self.mappings,
                                               read_passwords_from_secrets, env_tag=env_tag, secret_type=secret_type)
         except Exception as e:
             self.logger.error(str(e))
             print(str(e))
             self.logger.error(traceback.format_exc())
             print(traceback.format_exc())
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py` & `infoworkssdk-4.1/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/client.py` & `infoworkssdk-4.1/infoworks/sdk/client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/domain_client.py` & `infoworkssdk-4.1/infoworks/sdk/domain_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,21 @@
                 return GenericResponse.parse_result(status=Response.Status.FAILED,
                                                     error_code=ErrorCode.GENERIC_ERROR,
                                                     error_desc=parsed_response, job_id=None)
         except Exception as e:
             self.logger.error(f"Failed to create domain" + str(e))
             raise DomainError(f"Failed to create domain" + str(e))
 
-    def list_domains(self, params=None):
+    def list_domains(self, params=None, pagination=True):
         """
         Function to list domains
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_domains = url_builder.create_domain_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
         domains_list = []
@@ -60,14 +63,16 @@
                 self.call_api("GET", url_to_list_domains,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     domains_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -168,21 +173,23 @@
                                                                                    "Error in deleting domain"),
                                                     response=parsed_response
                                                     )
         except Exception as e:
             self.logger.error(f"Error in deleting the domain {domain_id}")
             raise DomainError(f"Error in deleting the domain {domain_id} " + str(e))
 
-    def get_sources_associated_with_domain(self, domain_id, params=None):
+    def get_sources_associated_with_domain(self, domain_id, params=None, pagination=True):
         """
         Function to get sources associated with the domain
         :param domain_id: Entity identifier for the domain
         :type domain_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_sources_under_domain = url_builder.add_sources_to_domain_url(self.client_config,
                                                                                  domain_id) + IWUtils.get_query_params_string_from_dict(
             params=params)
@@ -194,14 +201,16 @@
                 self.call_api("GET", url_to_list_sources_under_domain,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     src_under_domain_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -344,21 +353,23 @@
                 self.logger.error("Failed to get domain id")
                 return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.GENERIC_ERROR,
                                                     response={"domain_id": None})
         except Exception as e:
             self.logger.error("Error in finding domain id")
             raise DomainError("Error in finding domain id" + str(e))
 
-    def get_pipeline_extensions_associated_with_domain(self, domain_id, params=None):
+    def get_pipeline_extensions_associated_with_domain(self, domain_id, params=None, pagination=True):
         """
         Function to get pipeline extensions associated with the domain
         :param domain_id: Entity identifier for the domain
         :type domain_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_pl_extns_under_domain = url_builder.accessible_pipeline_extensions_url(self.client_config,
                                                                                            domain_id) + IWUtils.get_query_params_string_from_dict(
             params=params)
@@ -370,14 +381,16 @@
                 self.call_api("GET", url_to_list_pl_extns_under_domain,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pl_extn_under_domain_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -572,58 +585,111 @@
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to get/delete adv config details.')
             raise DomainError('Error occurred while trying to get/delete adv config details.')
 
-    def get_accessible_pipelines_under_domain(self, domain_id):
+    def get_accessible_pipelines_under_domain(self, domain_id,params=None,pagination=True):
         """
         Function to get the pipelines accessible under a domain
         :param domain_id: Entity identifier for domain
         :type domain_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: Response Dict
         """
         if domain_id is None:
             self.logger.error("domain_id cannot be None")
             raise Exception("domain_id cannot be None")
 
         response = None
-
+        if params is None:
+            params = {"limit": 20, "offset": 0}
         try:
+            accessible_pipelines_under_domain=[]
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.url_to_get_accessible_pipelines(
-                self.client_config, domain_id), IWUtils.get_default_header_for_v3(
+                self.client_config, domain_id) + IWUtils.get_query_params_string_from_dict(params=params), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
-
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=domain_id,
-                                                response=response)
-
+            if response is not None:
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    accessible_pipelines_under_domain.extend(result)
+                    if not pagination:
+                        break
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+                response["result"] = accessible_pipelines_under_domain
+                response["message"] = initial_msg
+                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=domain_id, response=response)
+            else:
+                return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                    error_code=ErrorCode.USER_ERROR,
+                                                    response="Failed to get accessible pipelines under domain"
+                                                    )
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to get accessible pipelines')
             raise DomainError('Error occurred while trying to get accessible pipelines')
 
-    def get_accessible_workflows_under_domain(self, domain_id):
+    def get_accessible_workflows_under_domain(self, domain_id,params=None,pagination=True):
         """
         Function to get the workflows accessible under a domain
         :param domain_id: Entity identifier for domain
         :type domain_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type params: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: Response Dict
         """
         if domain_id is None:
             self.logger.error("domain_id cannot be None")
             raise Exception("domain_id cannot be None")
-
+        if params is None:
+            params = {"limit": 20, "offset": 0}
         response = None
-
         try:
+            accessible_workflows_under_domain = []
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.url_to_get_accessible_workflows(
-                self.client_config, domain_id), IWUtils.get_default_header_for_v3(
+                self.client_config, domain_id) + IWUtils.get_query_params_string_from_dict(params=params), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
-
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=domain_id,
-                                                response=response)
+            if response is not None:
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    accessible_workflows_under_domain.extend(result)
+                    if not pagination:
+                        break
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+                response["result"] = accessible_workflows_under_domain
+                response["message"] = initial_msg
+                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=domain_id,
+                                                    response=response)
+            else:
+                return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                    error_code=ErrorCode.USER_ERROR,
+                                                    response="Failed to get accessible workflows under domain"
+                                                    )
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to get accessible workflows')
             raise DomainError('Error occurred while trying to get accessible workflows')
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/ejson/__init__.py` & `infoworkssdk-4.1/infoworks/sdk/ejson/__init__.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/generic_response.py` & `infoworkssdk-4.1/infoworks/sdk/generic_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/jobmetrics.py` & `infoworkssdk-4.1/infoworks/sdk/jobmetrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import datetime
+import json
 import math
 import traceback
 from collections import OrderedDict
 from infoworks.sdk import url_builder
 from infoworks.sdk.utils import IWUtils
 from infoworks.error import AdminError
 from infoworks.sdk.base_client import BaseClient
@@ -41,15 +42,16 @@
                               ).content)
             if response is not None and "result" in response:
                 result = response.get("result")
                 table_group_id = result.get("sub_entity_id", "")
                 processedAt = result.get("processed_at", "")
                 job_end_time = result.get("last_updated", "")
                 status = result.get("status", "")
-                entity_type = result.get("entity_type", "")
+                # entity_type = result.get("entity_type", "")
+                entity_type = "table"
                 return table_group_id, processedAt, job_end_time, status, entity_type
         except Exception as e:
             raise AdminError("Unable to get table group details from the Job Id")
 
     def get_table_group_name(self, table_group_id, source_id):
         try:
             url_to_get_tginfo = url_builder.create_table_group_url(self.client_config, source_id) + f"/{table_group_id}"
@@ -309,14 +311,38 @@
                                                                       )
                     response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
                     result = response.get("result", [])
                 return combinedJobs
         except Exception as e:
             raise AdminError("Unable to get ingestion jobs list of source")
 
+    def get_cluster_runs_of_job(self, job_id):
+        try:
+            cluster_runs = []
+            url_to_get_cluster_jobs = url_builder.get_cluster_jobs_status_url(self.client_config, job_id)
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_cluster_jobs,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
+                              ).content)
+            if response is not None and "result" in response:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    cluster_runs.extend(result)
+                    next_url = response.get('links')['next']
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=next_url,
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
+                    result = response.get("result", [])
+                return cluster_runs
+        except Exception as e:
+            raise AdminError("Unable to get cluster jobs list of source")
+
     def get_pipeline_jobs(self, date_string):
         try:
             combinedJobs = []
             filter_condition = "{\"$and\": [{\"last_upd\": {\"$gte\": {\"$date\": \"" + date_string + "\"}}},{\"jobType\": {\"$in\": [\"pipeline_build\"]}}, {\"status\":{\"$in\":[\"failed\",\"completed\",\"running\",\"pending\",\"aborted\",\"canceled\"]}}]}"
             url_to_get_jobs = url_builder.get_job_status_url(
                 self.client_config) + f"?filter={filter_condition}&limit=50&offset=0"
             response = IWUtils.ejson_deserialize(
@@ -413,14 +439,230 @@
                               ).content)
             if response is not None and "result" in response:
                 result = response.get("result", None)
                 return result.get('name')
         except:
             raise AdminError("Unable to get pipeline NAME")
 
+    def get_source_jobs_metrics_results_table_level(self, date_string, source, workflow_id=None, workflow_run_id=None):
+        src_name = source["name"]
+        source_id = source["id"]
+        list_of_jobs_obj = self.get_jobs_of_single_source(source_id, date_string)
+        try:
+            for job in list_of_jobs_obj:
+                # self.logger.info(f"Job Data: {json.dumps(job)}")
+                job_id = job["id"]
+                job_type = job["type"]
+                job_status = job["status"]
+                job_createdAt = job["created_at"]
+                job_start_time = job_createdAt.split('.')[0].replace('T', ' ')
+                job_created_by = job.get('created_by')
+                workflow_id = job.get('triggered_by', {}).get('parent_id', '')
+                workflow_run_id = job.get('triggered_by', {}).get('run_id', '')
+
+                # Fetches Cluster Run Info (i.e. Table Data in a Job)
+                cluster_data = self.get_cluster_runs_of_job(job_id)
+
+                # Fetches Table Group Info
+                try:
+                    tg_id, processedAt, job_end_time, job_status, entity_type = self.get_tablegroup_id_from_job(
+                        job_id, source["id"])
+                    table_group_name, all_tables_list = self.get_table_group_name(tg_id, source["id"])
+                except Exception as error:
+                    # This means the job is non-table group job
+                    table_group_name = ""
+                    entity_type = "table"
+                    all_tables_list = []
+
+                # Fetches Ingestion Metrics
+                ing_metrics = self.get_ingestion_metrics(str(job_id), source["id"])
+                ing_metrics_df = pd.DataFrame(ing_metrics)
+                if ing_metrics is not None:
+                    ing_metrics_tables_list = list(set([i['table_id'] for i in ing_metrics]))
+                else:
+                    ing_metrics_tables_list = []
+
+                # Fetches Export Metrics
+                export_metrics = self.get_export_metrics(str(job_id), source_id)
+                df_export = pd.DataFrame(export_metrics)
+                if export_metrics is not None:
+                    export_metrics_tables_list = list([i['table_id'] for i in export_metrics])
+                else:
+                    export_metrics_tables_list = []
+
+                # Job Level Properties
+                source_job_row_template = {
+                    'workflow_id': workflow_id, 'workflow_run_id': workflow_run_id,
+                    'job_id': job_id, 'job_type': self.job_type_mappings[job_type.upper()],
+                    'job_start_time': job_start_time, 'job_end_time': "",
+                    'job_created_by': job_created_by, 'cluster_id': "",
+                    'job_status': job_status.upper(), 'job_table_status': '',
+                    'entity_type': entity_type, "source_name": src_name, "source_schema_name": "",
+                    "source_database_name": "", "source_file_names": [], "table_group_name": table_group_name,
+                    "iwx_table_name": "", 'starting_watermark_value': '', 'ending_watermark_value': '',
+                    "target_schema_name": "", "target_table_name": "", "pre_target_count": "", "fetch_records_count": 0,
+                    "target_records_count": "", "job_link": ""}
+
+                if cluster_data:
+                    # Table Level in a Job
+                    for row in cluster_data:
+                        cluster_id = row.get('cluster_id', '')
+                        table_job_start_time = row.get('started_at', '').split('.')[0].replace('T', ' ')
+                        table_job_end_time = row.get('ended_at', '').split('.')[0].replace('T', ' ')
+                        iwx_table_name = row.get('entity_name', '')
+                        table_id = row.get('sub_entity_id', '')
+                        job_table_status = row.get('entity_run_details', {}).get('entity_run_status', '')
+
+                        table_info = self.get_table_info(source_id, table_id)
+                        table_name = table_info.get('name')
+                        target_table_name = table_info.get("configuration", {}).get('target_table_name', '')
+                        target_schema_name = table_info.get("configuration", {}).get('target_schema_name', '')
+                        table_row_count = table_info.get('row_count', 0)
+
+                        source_job_row_template["job_start_time"] = table_job_start_time
+                        source_job_row_template["job_end_time"] = table_job_end_time
+                        source_job_row_template['cluster_id'] = cluster_id
+                        source_job_row_template['job_table_status'] = job_table_status
+                        source_job_row_template['iwx_table_name'] = table_name
+                        source_job_row_template['target_schema_name'] = target_schema_name
+                        source_job_row_template['target_table_name'] = target_table_name
+
+                        if ing_metrics != [] and job_type != "export_data" and job_table_status.upper() == "SUCCESS":
+                            if table_id in ing_metrics_tables_list:
+                                filter1 = ing_metrics_df["table_id"] == table_id
+                                table = {}
+                                if len(ing_metrics_df.loc[filter1]) > 1:
+                                    # Incremental Job
+                                    filter2 = ing_metrics_df["job_type"] == "CDC"
+                                    filter3 = ing_metrics_df["job_type"] == "MERGE"
+                                    cdc_output = ing_metrics_df.loc[filter1 & filter2].to_dict('records')[0]
+                                    merge_output = ing_metrics_df.loc[filter1 & filter3].to_dict('records')[0]
+                                    for item in ['source_id', 'fetch_records_count', 'job_id',
+                                                 'source_schema_name', 'source_database_name']:
+                                        table[item] = cdc_output.get(item, "")
+                                        table['job_type'] = "INCREMENTAL"
+                                    for item in ['workflow_id', 'workflow_run_id', 'job_status',
+                                                 'target_records_count', 'first_merged_watermark',
+                                                 'last_merged_watermark']:
+                                        table[item] = merge_output.get(item, "")
+                                        table['job_type'] = "INCREMENTAL"
+                                else:
+                                    table = ing_metrics_df.loc[filter1].to_dict('records')[0]
+                                table["source_schema_name"] = table.get("source_schema_name", "")
+                                table["source_database_name"] = table.get("source_database_name", "")
+                                table["source_file_names"] = self.get_source_file_paths(
+                                    source['id'], table_id, job_id) if table["source_schema_name"] == "" else []
+                                table["workflow_id"] = table.get("workflow_id", "")
+                                table["workflow_run_id"] = table.get('workflow_run_id', "")
+                                if workflow_id is not None and workflow_run_id is not None:
+                                    if not (table["workflow_id"] == workflow_id and
+                                            table["workflow_run_id"] == workflow_run_id):
+                                        continue
+                                table["entity_type"] = entity_type
+                                table["starting_watermark_value"] = table.pop('first_merged_watermark', '')
+                                table["ending_watermark_value"] = table.pop('last_merged_watermark', '')
+                                if math.isnan(table.get('target_records_count')):
+                                    table['pre_target_count'] = None
+                                    table['target_records_count'] = None
+                                else:
+                                    if table["job_status"] == "FAILED":
+                                        table['pre_target_count'] = table.get('target_records_count')
+                                        table['target_records_count'] = int(table.get('target_records_count'))
+                                    else:
+                                        table['pre_target_count'] = int(
+                                            table.get('target_records_count') - int(table.get('fetch_records_count')))
+                                        table['target_records_count'] = int(table.get('target_records_count'))
+                                if table.get('job_type') == "CDC":
+                                    table['job_type'] = "INCREMENTAL"
+                                # table['job_start_time'] = table['job_start_time'].split('.')[0].replace('T', ' ')
+                                # table['job_end_time'] = table['job_end_time'].split('.')[0].replace('T', ' ')
+                                table['fetch_records_count'] = int(table['fetch_records_count'])
+
+                                # self.logger.info(f"Ingestion Table Data: {json.dumps(table)}")
+                                # Metrics in Consideration from Ingestion Data
+                                for key in ["job_type", "source_schema_name", "source_database_name",
+                                            "source_file_names", "entity_type", "starting_watermark_value",
+                                            "ending_watermark_value",
+                                            "target_records_count", "pre_target_count", "fetch_records_count"]:
+                                    source_job_row_template[key] = table.get(key, '')
+
+                            # Table not in Ingestion Metrics
+                            else:
+                                sync_type = table_info.get('configuration', {}).get('sync_type', '')
+                                source_job_row_template['job_type'] = sync_type.upper()
+                                source_job_row_template["pre_target_count"] = table_row_count
+                                source_job_row_template["target_records_count"] = table_row_count
+
+                        if job_type == "export_data":
+                            if export_metrics is not None:
+                                if table_id in export_metrics_tables_list:
+                                    filter1 = df_export["table_id"] == table_id
+                                    table = df_export.loc[filter1].to_dict('records')[0]
+                                    table["job_type"] = "EXPORT"
+                                    table_export_config = self.get_table_export_info(table.get('source_id'), table_id)
+                                    if table_export_config.get("target_type", "") == "BIGQUERY":
+                                        table["target_schema_name"] = ".".join(
+                                            [table_export_config.get("connection", {}).get("project_id", ""),
+                                             table_export_config.get("target_configuration", {}).get("dataset_name",
+                                                                                                     "")])
+                                    else:
+                                        table["target_schema_name"] = ".".join(
+                                            [table_export_config.get("target_configuration", {}).get("schema_name", ""),
+                                             table_export_config.get("target_configuration", {}).get("database_name",
+                                                                                                     "")])
+                                    table["target_table_name"] = table_export_config.get("target_configuration",
+                                                                                         {}).get(
+                                        "table_name", "")
+                                    table["workflow_id"] = table.get("workflow_id", "")
+                                    table["workflow_run_id"] = table.get("workflow_run_id", "")
+                                    table["entity_type"] = entity_type
+                                    table["starting_watermark_value"] = table.pop('first_merged_watermark', '')
+                                    table["ending_watermark_value"] = table.pop('last_merged_watermark', '')
+                                    if math.isnan(table.get('target_records_count')):
+                                        table['pre_target_count'] = None
+                                        table['target_records_count'] = None
+                                    else:
+                                        if table["job_status"] == "FAILED":
+                                            table['pre_target_count'] = table.get('target_records_count')
+                                            table['target_records_count'] = int(table.get('target_records_count'))
+                                        else:
+                                            table['pre_target_count'] = int(
+                                                table.get('target_records_count') - int(
+                                                    table.get('number_of_records_written')))
+                                            table['target_records_count'] = int(table.get('target_records_count'))
+                                    od = OrderedDict()
+                                    # table['job_start_time'] = table['job_start_time'].split('.')[0].replace('T', ' ')
+                                    # table['job_end_time'] = table['job_end_time'].split('.')[0].replace('T', ' ')
+                                    table['fetch_records_count'] = int(table['number_of_records_written'])
+
+                                    for key in ["job_type", "target_schema_name",
+                                                "target_table_name", "entity_type", "starting_watermark_value",
+                                                "ending_watermark_value", "target_records_count", "pre_target_count",
+                                                "fetch_records_count"]:
+                                        source_job_row_template[key] = table.get(key, "")
+                                else:
+                                    source_job_row_template['job_type'] = "EXPORT"
+                                    source_job_row_template['pre_target_count'] = table_row_count
+                                    source_job_row_template['target_records_count'] = table_row_count
+                                    source_job_row_template['entity_type'] = entity_type
+
+                        # self.logger.info(f"Source Row Template: {json.dumps(source_job_row_template)}")
+                        job_od = OrderedDict()
+                        for key in source_job_row_template.keys():
+                            job_od[key] = source_job_row_template.get(key, "")
+                        self.job_metrics_final.append(job_od)
+                else:
+                    job_od = OrderedDict()
+                    for key in source_job_row_template.keys():
+                        job_od[key] = source_job_row_template.get(key, "")
+                    self.job_metrics_final.append(job_od)
+        except Exception as e:
+            print(str(e))
+            traceback.print_exc()
+
     def get_source_jobs_metrics_results(self, date_string, source, workflow_id=None, workflow_run_id=None):
         """
         Gets the Infoworks source job metrics
         :param date_string: date string to fetch the data till that date
         :type date_string: String
         :param workflow_id: Workflow id to get the jobs
         :type workflow_id: String
@@ -432,33 +674,37 @@
         list_of_jobs_obj = self.get_jobs_of_single_source(source["id"], date_string)
         try:
             for job in list_of_jobs_obj:
                 job_id = job["id"]
                 job_type = job["type"]
                 job_status = job["status"]
                 job_createdAt = job["created_at"]
+                job_cluster_id = job.get('cluster_id')
+                job_created_by = job.get('created_by')
                 running_job_template = {
                     'workflow_id': job.get('triggered_by', {}).get('parent_id', ''),
                     'workflow_run_id': job.get('triggered_by', {}).get('run_id', ''),
                     'job_id': job_id,
                     'job_type': self.job_type_mappings[job_type.upper()],
                     'job_start_time': job_createdAt.split('.')[0].replace('T', ' '),
                     'job_end_time': "",
+                    'job_created_by': job_created_by,
+                    'cluster_id': job_cluster_id,
                     "source_file_names": [],
                     'job_status': job_status.upper(),
                     'entity_type': "source",
                     "source_name": src_name, "source_schema_name": job.get("source_schema_name", ""),
                     "source_database_name": job.get("source_database_name", ""), "table_group_name": "",
                     "iwx_table_name": "", 'starting_watermark_value': '', 'ending_watermark_value': '',
                     "pre_target_count": "", "fetch_records_count": 0,
                     "target_records_count": ""}
                 running_od = OrderedDict()
                 if job_status.upper() in ["RUNNING", "PENDING", "CANCELED", "ABORTED", "FAILED"]:
                     for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
-                                'job_end_time', 'job_status',
+                                'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                 'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
                                 'table_group_name',
                                 'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                 'target_schema_name', 'target_table_name', 'pre_target_count', 'fetch_records_count',
                                 'target_records_count']:
                         running_od[key] = running_job_template.get(key, "")
                     self.job_metrics_final.append(running_od)
@@ -534,17 +780,19 @@
                                 table['target_records_count'] = int(table.get('target_records_count'))
                         if table.get('job_type') == "CDC":
                             table['job_type'] = "INCREMENTAL"
                         od = OrderedDict()
                         table['job_start_time'] = table['job_start_time'].split('.')[0].replace('T', ' ')
                         table['job_end_time'] = table['job_end_time'].split('.')[0].replace('T', ' ')
                         table['fetch_records_count'] = int(table['fetch_records_count'])
+                        table['cluster_id'] = job_cluster_id
+                        table['job_created_by'] = job_created_by
                         for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type',
                                     'job_start_time',
-                                    'job_end_time', 'job_status',
+                                    'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                     'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
                                     'table_group_name',
                                     'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                     'target_schema_name', 'target_table_name', 'pre_target_count',
                                     'fetch_records_count',
                                     'target_records_count']:
                             od[key] = table.get(key, '')
@@ -560,28 +808,30 @@
                         temp = {
                             'workflow_id': job.get('triggered_by', {}).get('parent_id', ''),
                             'workflow_run_id': job.get('triggered_by', {}).get('run_id', ''),
                             'job_id': job_id,
                             'job_type': synctype.upper(),
                             'job_start_time': processedAt.split('.')[0].replace('T', ' '),
                             'job_end_time': job_end_time.split('.')[0].replace('T', ' '),
+                            'job_created_by': job_created_by,
+                            'cluster_id': job_cluster_id,
                             'job_status': job_status.upper(),
                             'entity_type': entity_type,
                             "source_file_names": [],
                             "target_table_name": tableInfo.get("target_table_name", ""),
                             "target_schema_name": tableInfo.get("target_schema_name", ""),
                             "source_name": src_name, "source_schema_name": job.get("source_schema_name", ""),
                             "source_database_name": job.get("source_database_name", ""),
                             "table_group_name": table_group_name, "iwx_table_name": table_name,
                             'starting_watermark_value': '', 'ending_watermark_value': '',
                             "pre_target_count": row_count, "fetch_records_count": 0,
                             "target_records_count": row_count}
                         for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type',
                                     'job_start_time',
-                                    'job_end_time', 'job_status',
+                                    'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                     'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
                                     'table_group_name',
                                     'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                     'target_schema_name', 'target_table_name', 'pre_target_count',
                                     'fetch_records_count',
                                     'target_records_count']:
                             temp_failed[key] = temp.get(key, "")
@@ -632,16 +882,18 @@
                                     table['pre_target_count'] = int(
                                         table.get('target_records_count') - int(table.get('number_of_records_written')))
                                     table['target_records_count'] = int(table.get('target_records_count'))
                             od = OrderedDict()
                             table['job_start_time'] = table['job_start_time'].split('.')[0].replace('T', ' ')
                             table['job_end_time'] = table['job_end_time'].split('.')[0].replace('T', ' ')
                             table['fetch_records_count'] = int(table['number_of_records_written'])
+                            table['cluster_id'] = job_cluster_id
+                            table['job_created_by'] = job_created_by
                             for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type',
-                                        'job_start_time', 'job_end_time', 'job_status',
+                                        'job_start_time', 'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                         'source_name', 'source_file_names', 'source_schema_name',
                                         'source_database_name',
                                         'table_group_name',
                                         'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                         'target_schema_name', 'target_table_name', 'pre_target_count',
                                         'fetch_records_count',
                                         'target_records_count']:
@@ -657,24 +909,26 @@
                             temp = {
                                 'workflow_id': job.get('triggered_by', {}).get('parent_id', ''),
                                 'workflow_run_id': job.get('triggered_by', {}).get('run_id', ''),
                                 'job_id': job_id,
                                 'job_type': "EXPORT",
                                 'job_start_time': processedAt.split('.')[0].replace('T', ' '),
                                 'job_end_time': job_end_time.split('.')[0].replace('T', ' '),
+                                'job_created_by': job_created_by,
+                                'cluster_id': job_cluster_id,
                                 'job_status': job_status.upper(),
                                 'entity_type': entity_type,
                                 "source_file_names": [],
                                 "source_name": src_name, "table_group_name": table_group_name,
                                 "iwx_table_name": table_name,
                                 'starting_watermark_value': '', 'ending_watermark_value': '',
                                 "pre_target_count": row_count, "fetch_records_count": 0,
                                 "target_records_count": row_count}
                             for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type',
-                                        'job_start_time', 'job_end_time', 'job_status',
+                                        'job_start_time', 'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                         'source_name', 'source_file_names', 'source_schema_name',
                                         'source_database_name',
                                         'table_group_name',
                                         'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                         'target_schema_name', 'target_table_name', 'pre_target_count',
                                         'fetch_records_count',
                                         'target_records_count']:
@@ -698,44 +952,69 @@
         if job is None:
             self.logger.error("job is a mandatory parameter")
             raise Exception("job is a mandatory parameter")
         temp = []
         job_id = job['id']
         job_type = job['type']
         job_status = job['status']
+        job_cluster_id = job.get('cluster_id')
         job_createdAt = job['created_at']
         entity_type = job['entity_type']
+        job_created_by = job.get('created_by')
         running_job_template = {
             'workflow_id': job.get('triggered_by', {}).get('parent_id', ''),
             'workflow_run_id': job.get('triggered_by', {}).get('run_id', ''),
             'job_id': job_id,
             'job_type': job_type.upper(),
             'job_start_time': job_createdAt.split('.')[0].replace('T', ' '),
             'job_end_time': "",
+            'job_created_by': job_created_by,
+            'cluster_id': job_cluster_id,
             "source_file_names": [],
             'job_status': job_status.upper(),
             'entity_type': entity_type,
             "source_name": "", "source_schema_name": job.get("source_schema_name", ""),
             "source_database_name": job.get("source_database_name", ""), "table_group_name": "", "iwx_table_name": "",
             'starting_watermark_value': '', 'ending_watermark_value': '',
             "pre_target_count": "", "fetch_records_count": 0,
             "target_records_count": ""}
+        # Fetches Cluster Run Info (i.e. Table Data in a Job)
+        cluster_data = self.get_cluster_runs_of_job(job_id)
+        if cluster_data:
+            # Job Start Time and End Time for no Pipeline Metrics
+            running_job_template['job_start_time'] = cluster_data[0]['started_at']
+            running_job_template['job_end_time'] = cluster_data[0]['ended_at']
+            running_job_template['cluster_id'] = cluster_data[0]['cluster_id']
+            job_cluster_id = cluster_data[0]['cluster_id']
+
         running_od = OrderedDict()
         if job_status.upper() in ["RUNNING", "PENDING", "CANCELED", "ABORTED", "FAILED"]:
             for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
-                        'job_end_time', 'job_status',
+                        'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                         'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
                         'table_group_name',
                         'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value', 'target_schema_name',
                         'target_table_name', 'pre_target_count', 'fetch_records_count',
                         'target_records_count']:
                 running_od[key] = running_job_template.get(key, "")
             self.job_metrics_final.append(running_od)
             return
         pipeline_metrics = self.get_pipeline_build_metrics(str(job_id))
+        # For SQL Pipeline successful jobs (No Pipeline Metrics)
+        if job_status.upper() == "COMPLETED" and len(pipeline_metrics) == 0:
+            for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
+                        'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
+                        'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
+                        'table_group_name',
+                        'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value', 'target_schema_name',
+                        'target_table_name', 'pre_target_count', 'fetch_records_count',
+                        'target_records_count']:
+                running_od[key] = running_job_template.get(key, "")
+            self.job_metrics_final.append(running_od)
+            return
         pipeline_successful_tables = []
         if pipeline_metrics is not None:
             tables_list = list(set([i['target_table_name'] for i in pipeline_metrics]))
             df_pipeline = pd.DataFrame(pipeline_metrics)
             for target_table_name in tables_list:
                 schema_name, table_name = target_table_name.split(".")
                 pipeline_successful_tables.append(table_name)
@@ -757,14 +1036,16 @@
                         "workflow_run_id"] == workflow_run_id):
                         continue
                 table["entity_type"] = job.get("entity_type", "pipeline")
                 table["starting_watermark_value"] = table.pop('first_merged_watermark', '')
                 table["ending_watermark_value"] = table.pop('last_merged_watermark', '')
                 table["target_records_count"] = table.get("target_records_count", None)
                 table["job_status"] = table.get("job_status", "")
+                table["cluster_id"] = job_cluster_id
+                table['job_created_by'] = job_created_by
                 if math.isnan(table.get('target_records_count')):
                     table['pre_target_count'] = None
                     table['target_records_count'] = None
                 else:
                     if table["job_status"] == "FAILED":
                         table['pre_target_count'] = table.get('target_records_count')
                         table['target_records_count'] = int(table.get('target_records_count'))
@@ -773,15 +1054,15 @@
                             table.get('target_records_count') - int(table.get('number_of_records_written')))
                         table['target_records_count'] = int(table.get('target_records_count'))
                     od = OrderedDict()
                     table['job_start_time'] = table['job_start_time'].split('.')[0].replace('T', ' ')
                     table['job_end_time'] = table['job_end_time'].split('.')[0].replace('T', ' ')
                     table['fetch_records_count'] = int(table['number_of_records_written'])
                     for key in ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
-                                'job_end_time', 'job_status',
+                                'job_end_time', 'job_created_by', 'cluster_id', 'job_status',
                                 'source_name', 'source_file_names', 'source_schema_name', 'source_database_name',
                                 'table_group_name',
                                 'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value',
                                 'target_schema_name', 'target_table_name', 'pre_target_count', 'fetch_records_count',
                                 'target_records_count']:
                         od[key] = table.get(key, "")
                     temp.append(od)
@@ -803,27 +1084,28 @@
             delay = int(time_range_for_jobs_in_mins)
             now = datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(minutes=delay)
             date_string = now.strftime('%Y-%m-%dT%H:%M:%SZ')
             source_jobs = self.get_all_source_jobs(date_string)
             source_jobs_source_ids = list(set([i['entity_id'] for i in source_jobs]))
             sources_info = [i for i in sources_info if i['id'] in source_jobs_source_ids]
             with ThreadPoolExecutor(max_workers=10) as executor:
-                executor.map(self.get_source_jobs_metrics_results,
+                executor.map(self.get_source_jobs_metrics_results_table_level,
                              [date_string] * len(sources_info), sources_info,
                              [workflow_id, workflow_run_id] * len(sources_info))
                 executor.shutdown(wait=True)
             pipeline_jobs_list = self.get_pipeline_jobs(date_string)
             with ThreadPoolExecutor(max_workers=10) as executor:
                 executor.map(self.get_pipeline_build_metrics_results, pipeline_jobs_list,
                              [workflow_id, workflow_run_id] * len(pipeline_jobs_list))
                 executor.shutdown(wait=True)
 
             result = []
             header = ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
-                      'job_end_time', 'job_status', 'source_name', 'source_file_names', 'source_schema_name',
+                      'job_end_time', 'job_created_by', 'cluster_id', 'job_status', 'job_table_status', 'source_name',
+                      'source_file_names', 'source_schema_name',
                       'source_database_name', 'table_group_name', 'iwx_table_name', 'starting_watermark_value',
                       'ending_watermark_value', 'target_schema_name', 'target_table_name', 'pre_target_count',
                       'fetch_records_count', 'target_records_count', 'job_link']
             ui_port = 443 if self.client_config["port"] == '443' else 3000
             if len(self.job_metrics_final) > 0:
                 for item in self.job_metrics_final:
                     dict_temp = {}
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/jobs_client.py` & `infoworkssdk-4.1/infoworks/sdk/jobs_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 
 class JobsClient(BaseClient):
 
     def __init__(self):
         super(JobsClient, self).__init__()
 
-    def get_job_details(self, job_id=None, params=None):
+    def get_job_details(self, job_id=None, params=None, pagination=True):
         """
         Function to get the job details
         :param job_id: entity identifier for job
         :type: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
 
         url_to_list_jobs = url_builder.get_jobs_url(self.client_config)
         if job_id is not None:
@@ -44,14 +46,16 @@
                                                         error_desc='Failed to get job details',
                                                         response=response)
                 if job_id is not None:
                     job_details.extend([result])
                 else:
                     while len(result) > 0:
                         job_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -144,23 +148,25 @@
                     "response": result}
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response.content))
             self.logger.exception('Error occurred while trying to get logs for job.')
             raise JobsError('Error occurred while trying to get logs for job.')
 
-    def get_cluster_job_details(self, job_id=None, run_id=None, params=None):
+    def get_cluster_job_details(self, job_id=None, run_id=None, params=None, pagination=True):
         """
         Function to get cluster job logs for iw_job using job_id
         :param job_id: job_id for the job
         :type job_id: String
         :param run_id: run_id for the job
         :type run_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {job_id}:
             self.logger.error("job_id cannot be None")
             raise Exception("job_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -186,14 +192,16 @@
                                                         error_desc='Failed to get cluster job details',
                                                         response=response)
                 if run_id is not None:
                     job_details.extend([result])
                 else:
                     while len(result) > 0:
                         job_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -202,19 +210,21 @@
             response["result"] = job_details
             response["message"] = initial_msg
             return GenericResponse.parse_result(job_id=job_id, status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting cluster job details")
             raise JobsError("Error in getting cluster job details" + str(e))
 
-    def get_admin_job_details(self, params=None):
+    def get_admin_job_details(self, params=None, pagination=True):
         """
         Function to get the admin job details
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
 
         url_to_list_jobs = url_builder.get_admin_jobs_url(self.client_config)
         url_to_list_jobs = url_to_list_jobs + IWUtils.get_query_params_string_from_dict(params=params)
@@ -231,14 +241,16 @@
                 if len(result) == 0:
                     self.logger.error(f"Failed to get the admin job details.")
                     return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                         error_desc=f"Failed to get the admin job details.",
                                                         response=response)
                 while len(result) > 0:
                     job_details.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -247,21 +259,23 @@
             response["result"] = job_details
             response["message"] = initial_msg
             return GenericResponse.parse_result(job_id=None, status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting job details")
             raise JobsError("Error in getting job details" + str(e))
 
-    def get_all_jobs_for_source(self, source_id=None, params=None):
+    def get_all_jobs_for_source(self, source_id=None, params=None, pagination=True):
         """
         Function to get all jobs for a particular source
         :param source_id: entity identifier for which the jobs are to be fetched
         :type: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by limit under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if None in {source_id}:
             self.logger.error("source_id cannot be None")
             raise Exception("source_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -286,14 +300,16 @@
                     self.logger.error(f"Failed to get the source jobs details.")
                     return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                         error_desc=f"Failed to get the source jobs details.",
                                                         response=response)
 
                 while len(result) > 0:
                     job_details.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -310,14 +326,15 @@
         """
         Function to get job summary for given job_id
         :param source_id: source_id for the job
         :type source_id: String
         :param job_id: job_id for the job
         :type job_id: String
         :param type: can be either summary/logs
+        :param num_of_lines: Number of log lines to capture
         :return: response dict
         """
         if None in {job_id, source_id}:
             self.logger.error("job_id or source_id cannot be None")
             raise Exception("job_id or source_id cannot be None")
         try:
             if type.lower() == "summary":
@@ -337,22 +354,24 @@
                                                     error_desc=f"Failed to get the crawl job summary/log for job_id {job_id}.",
                                                     response=response, job_id=job_id)
             else:
                 return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             raise JobsError(f"Failed to get the crawl job summary/log for job_id {job_id}." + str(e))
 
-    def get_interactive_jobs_list(self, source_id=None, job_id=None, params=None):
+    def get_interactive_jobs_list(self, source_id=None, job_id=None, params=None, pagination=True):
         """
         Function to get all interactive jobs
         :param source_id: source_id for the interactive jobs
         :type source_id: String
         :param job_id: Entity identifier of the job
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by limit under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if None in {source_id}:
             self.logger.error("source_id cannot be None")
             raise Exception("source_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -377,14 +396,16 @@
                                                         error_desc=f"Failed to get the interactive jobs list.",
                                                         response=response)
                 if job_id is not None:
                     job_details.extend([result])
                 else:
                     while len(result) > 0:
                         job_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -393,23 +414,25 @@
             response["result"] = job_details
             response["message"] = initial_msg
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting job details")
             raise JobsError("Error in getting job details" + str(e))
 
-    def get_list_of_pipeline_jobs(self, domain_id=None, pipeline_id=None, params=None):
+    def get_list_of_pipeline_jobs(self, domain_id=None, pipeline_id=None, params=None, pagination=True):
         """
         Function to get all jobs for a particular pipeline
         :param domain_id: entity identifier for domain
         :type domain_id: String
         :param pipeline_id: entity identifier for pipeline
         :type pipeline_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by limit under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if None in {domain_id, pipeline_id}:
             self.logger.error("domain_id or pipeline_id cannot be None")
             raise Exception("domain_id or pipeline_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -424,14 +447,16 @@
                 self.call_api("GET", url_to_list_jobs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 while len(result) > 0:
                     job_details.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -512,21 +537,23 @@
                 self.logger.error(f"Failed to cancel job {job_id}.")
                 return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                     error_desc=f"Failed to cancel job {job_id}.", response=response)
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             raise JobsError(f"Failed to cancel job for job_id {job_id}." + str(e))
 
-    def get_job_details_by_prodops_user(self, job_id=None, params=None):
+    def get_job_details_by_prodops_user(self, job_id=None, params=None, pagination=True):
         """
         Function to get the job details by prodops user
         :param job_id: entity identifier for job
         :type: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by limit under params
+        :type pagination: Boolean
         :return: response list of dict
         """
         if None in {job_id}:
             self.logger.error("job_id cannot be None")
             raise Exception("job_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -552,14 +579,16 @@
                                                         error_desc='Failed to get job details',
                                                         response=response)
                 if job_id is not None:
                     job_details.extend([result])
                 else:
                     while len(result) > 0:
                         job_details.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/local_configurations.py` & `infoworkssdk-4.1/infoworks/sdk/local_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/pipeline_client.py` & `infoworkssdk-4.1/infoworks/sdk/pipeline_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,23 @@
                 if failed_count >= retries - 1:
                     # traceback.print_stack()
                     print(response)
                     raise PipelineError(response.get("message", "Error occurred during job status poll"))
                 failed_count = failed_count + 1
             time.sleep(polling_frequency)
 
-    def list_pipelines(self, domain_id=None, params=None):
+    def list_pipelines(self, domain_id=None, params=None, pagination=True):
         """
         Function to list the pipelines
         :param domain_id: Entity identified for domain
         :type domain_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response list
         """
 
         if None in {domain_id}:
             self.logger.error("Domain ID cannot be None")
             raise Exception("Domain ID cannot be None")
         if params is None:
@@ -102,14 +104,16 @@
                 self.call_api("GET", url_to_list_pipelines,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pipelines_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -390,15 +394,15 @@
         """
         try:
             if None in {pipeline_id, pipeline_version_id, domain_id}:
                 raise Exception(f"pipeline_id, pipeline_version_id, domain_id cannot be None")
             response = IWUtils.ejson_deserialize(self.call_api("DELETE", url_builder.delete_pipeline_version_url(
                 self.client_config, domain_id, pipeline_id, pipeline_version_id), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
-            if response.get("message","")!="Successfully removed Pipeline Version":
+            if response.get("message", "") != "Successfully removed Pipeline Version":
                 self.logger.error('Failed to delete the pipeline version')
                 return PipelineResponse.parse_result(status=Response.Status.FAILED,
                                                      error_code=ErrorCode.USER_ERROR,
                                                      error_desc='Failed to delete the pipeline version',
                                                      response=response)
             pipeline_version_id = str(pipeline_version_id)
             self.logger.info(
@@ -819,22 +823,24 @@
                                                     response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to add/update adv config pipeline.')
             raise PipelineError('Error occurred while trying to add/update adv config pipeline.')
 
-    def list_pipeline_versions(self, domain_id=None, pipeline_id=None, params=None):
+    def list_pipeline_versions(self, domain_id=None, pipeline_id=None, params=None, pagination=True):
         """
         Function to list the pipeline versions
         :param domain_id: Entity identified for domain
         :type domain_id: String
         :param pipeline_id: Entity identified for pipeline
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response list
         """
         if None in {domain_id, pipeline_id}:
             self.logger.error("domain_id and pipeline_id cannot be None")
             raise Exception("omain_id and pipeline_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -848,14 +854,16 @@
                 self.call_api("GET", url_to_list_pipeline_versions,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pipelines_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1166,7 +1174,36 @@
                 return PipelineResponse.parse_result(status=Response.Status.SUCCESS, pipeline_id=pipeline_id,
                                                      response=pv_response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to create a new sql pipeline.')
             raise PipelineError('Error occurred while trying to create a new sql pipeline.')
+
+    def get_pipeline_job_summary(self, domain_id, pipeline_id, job_id):
+        """
+        Function to get pipeline job summary
+        :param domain_id: Entity identifier for domain
+        :param pipeline_id: Entity identifier for pipeline
+        :param job_id: Entity identifier for job
+        :return: response dict
+        """
+        try:
+            if None in {domain_id, pipeline_id, job_id}:
+                self.logger.error("domain id or pipeline id or job_id cannot be None")
+                raise Exception("domain id or pipeline id or job_id cannot be None")
+
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_pipeline_job_summary_url
+            (self.client_config, domain_id, pipeline_id, job_id),
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), ).content)
+            result = response.get('result', None)
+            if not result:
+                self.logger.error(f"Failed to get the pipeline job summary for job {job_id} ")
+                return PipelineResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f"Failed to get pipeline job summary for job {job_id} ",
+                                                     response=response)
+            else:
+                return PipelineResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            raise PipelineError(f"Failed to get pipeline job summary for job {job_id} " + str(e))
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/pipeline_group_client.py` & `infoworkssdk-4.1/infoworks/sdk/pipeline_group_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,22 +71,24 @@
                 if failed_count >= retries - 1:
                     # traceback.print_stack()
                     print(response)
                     raise PipelineError(response.get("message", "Error occurred during job status poll"))
                 failed_count = failed_count + 1
             time.sleep(polling_frequency)
 
-    def list_jobs_under_pipeline_group(self, domain_id, pipeline_group_id, params=None):
+    def list_jobs_under_pipeline_group(self, domain_id, pipeline_group_id, params=None,pagination=True):
         """
             Function to list the jobs under pipeline group
             :param domain_id: Entity identifier for domain
             :type domain_id: String
             :param pipeline_group_id: Entity identifier of the pipeline group
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if None in {domain_id, pipeline_group_id}:
             self.logger.error("domain_id or pipeline_group_id cannot be None")
             raise Exception("domain_id or pipeline_group_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -99,14 +101,16 @@
                 self.call_api("GET", url_to_list_pipeline_grp_jobs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pipeline_groups_jobs_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -196,23 +200,25 @@
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to get pipeline group details.')
             raise PipelineError('Error occurred while trying to get pipeline group details.')
 
-    def list_pipeline_job_details_in_pipeline_group_job(self, domain_id, pipeline_group_id, job_id, params=None):
+    def list_pipeline_job_details_in_pipeline_group_job(self, domain_id, pipeline_group_id, job_id, params=None,pagination=True):
         """
             Function to list the pipeline jobs in a pipeline group job
             :param domain_id: Entity identifier for domain
             :type domain_id: String
             :param pipeline_group_id: Entity identifier of the pipeline group
             :param job_id: Entity identifier of the pipeline group job
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if None in {pipeline_group_id, domain_id, job_id}:
             raise Exception(f"pipeline_group_id, domain_id, job_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_pipeline_grp_jobs = url_builder.get_pipeline_group_jobs_base_url(self.client_config, domain_id,
@@ -224,14 +230,16 @@
                 self.call_api("GET", url_to_list_pipeline_grp_jobs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pipelines_in_pipeline_groups_jobs_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -247,23 +255,25 @@
                 response["result"] = pipelines_in_pipeline_groups_jobs_list
                 response["message"] = initial_msg
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in listing pipeline jobs in pipeline group job")
             raise PipelineError("Error in listing pipeline jobs in pipeline group job" + str(e))
 
-    def list_cluster_job_runs_in_pipeline_group_job(self, domain_id, pipeline_group_id, job_id, params=None):
+    def list_cluster_job_runs_in_pipeline_group_job(self, domain_id, pipeline_group_id, job_id, params=None, pagination=True):
         """
             Function to list the cluster jobs in a pipeline group job
             :param domain_id: Entity identifier for domain
             :type domain_id: String
             :param pipeline_group_id: Entity identifier of the pipeline group
             :param job_id: Entity identifier of the pipeline group job
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if None in {pipeline_group_id, domain_id, job_id}:
             raise Exception(f"pipeline_group_id, domain_id, job_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_pipeline_grp_job_runs = url_builder.get_pipeline_group_jobs_base_url(self.client_config, domain_id,
@@ -275,14 +285,16 @@
                 self.call_api("GET", url_to_list_pipeline_grp_job_runs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     cluster_jobs_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -397,21 +409,23 @@
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to create a new pipeline group.')
             raise PipelineError('Error occurred while trying to create a new pipeline group.')
 
-    def list_pipeline_groups_under_domain(self, domain_id, params=None):
+    def list_pipeline_groups_under_domain(self, domain_id, params=None, pagination=True):
         """
         Function to list the pipeline groups under domain
         :param domain_id: Entity identifier for domain
         :type domain_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response list
         """
         if None in {domain_id}:
             raise Exception(f"domain_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_pipeline_grp = url_builder.get_pipeline_group_base_url(self.client_config,
@@ -423,14 +437,16 @@
                 self.call_api("GET", url_to_list_pipeline_grp,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     pipeline_groups_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -580,21 +596,23 @@
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to update the pipeline group.')
             raise PipelineError('Error occurred while trying to update the pipeline group.')
 
-    def get_accessible_pipeline_groups(self, domain_id, params=None):
+    def get_accessible_pipeline_groups(self, domain_id, params=None, pagination=True):
         """
             Function to get the accessible pipeline group
             :param domain_id: Domain id to which the pipeline  group  belongs to
             :type domain_id: String
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if domain_id is None:
             raise Exception(f"domain_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_get_accessible_pl_grp = url_builder.get_accessible_pipeline_groups_url(self.client_config,
@@ -605,17 +623,17 @@
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_get_accessible_pl_grp,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
-                    print(result)
-                    print(response)
                     pipeline_groups_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -631,23 +649,25 @@
                 response["result"] = pipeline_groups_list
                 response["message"] = initial_msg
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in listing accessible pipeline groups")
             raise PipelineError("Error in listing accessible pipeline groups" + str(e))
 
-    def get_list_of_advanced_config_of_pipeline_groups(self, domain_id, pipeline_group_id, params=None):
+    def get_list_of_advanced_config_of_pipeline_groups(self, domain_id, pipeline_group_id, params=None, pagination=True):
         """
             Function to get list of Advance Config pipeline group
             :param domain_id: Domain id to which the pipeline  group belongs to
             :type domain_id: String
             param pipeline_group_id: Entity identifier of pipeline group
             :type pipeline_group_id: String
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if None in {pipeline_group_id, domain_id}:
             raise Exception(f"pipeline_group_id, domain_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_get_adv_config_pl_grp = url_builder.advance_config_under_pipeline_groups_base_url(self.client_config,
@@ -660,14 +680,16 @@
                 self.call_api("GET", url_to_get_adv_config_pl_grp,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     adv_config_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -786,7 +808,36 @@
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=result.get('entity_id', ''),
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to get/delete adv config details.')
             raise PipelineError('Error occurred while trying to get/delete adv config details.')
+
+    def get_pipeline_group_job_summary(self, domain_id, pipeline_group_id, job_id):
+        """
+        Function to get pipeline group job summary
+        :param domain_id: Entity identifier for domain
+        :param pipeline_group_id: Entity identifier for pipeline group
+        :param job_id: Entity identifier for job
+        :return: response dict
+        """
+        try:
+            if None in {domain_id, pipeline_group_id, job_id}:
+                self.logger.error("domain id or pipeline group id or job_id cannot be None")
+                raise Exception("domain id or pipeline group id or job_id cannot be None")
+
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_pipeline_group_job_summary_url
+            (self.client_config, domain_id, pipeline_group_id, job_id),
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), ).content)
+            result = response.get('result', None)
+            if not result:
+                self.logger.error(f"Failed to get the pipeline group job summary for job {job_id} ")
+                return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                    error_code=ErrorCode.USER_ERROR,
+                                                    error_desc=f"Failed to get pipeline group job summary for job {job_id} ",
+                                                    response=response)
+            else:
+                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            raise PipelineError(f"Failed to get pipeline group job summary for job {job_id} " + str(e))
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/pipeline_response.py` & `infoworkssdk-4.1/infoworks/sdk/pipeline_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/replicator_client.py` & `infoworkssdk-4.1/infoworks/sdk/replicator_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/source_client.py` & `infoworkssdk-4.1/infoworks/sdk/source_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import json
 import time
 import traceback
+import urllib
+
 from infoworks.error import SourceError
 from infoworks.sdk import url_builder, local_configurations
 from infoworks.sdk.base_client import BaseClient
 from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.local_configurations import Response, ErrorCode, SourceMappings
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.utils import IWUtils
@@ -308,16 +311,17 @@
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         try:
             url_for_browse_source = url_builder.browse_source_tables_url(self.client_config, source_id)
             if filter_tables_properties is not None:
-                filter_condition = f"?is_filter_enabled=true&tables_filter={filter_tables_properties.get('tables_filter', '')}&catalogs_filter={filter_tables_properties.get('catalogs_filter', '')}&schemas_filter={filter_tables_properties.get('schemas_filter', '')}"
+                filter_condition = f"?is_filter_enabled=true&tables_filter={filter_tables_properties.get('tables_filter', '%')}&catalogs_filter={filter_tables_properties.get('catalogs_filter', '%')}&schemas_filter={filter_tables_properties.get('schemas_filter', '%')}"
                 url_for_browse_source = url_for_browse_source + filter_condition
+                # print("url_for_browse_source: ",url_for_browse_source)
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_for_browse_source,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             result = response.get('result', {})
             if result.get("message", "") == "Interactive Cluster is not running. Please bring up cluster and retry":
                 return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                    error_code=ErrorCode.GENERIC_ERROR,
@@ -401,15 +405,15 @@
                 "table_name": "",
                 "schema_name": "",
                 "table_type": "TABLE",
                 "target_table_name": "",
                 "target_schema_name": ""
         }]
         ```
-        :param poll_timeout: test connection job timeout in seconds
+        :param poll_timeout: metacrawl job timeout in seconds
         :type poll_timeout: integer. Default 300 seconds
         :param polling_frequency: polling frequency for the job in seconds. Default 15 seconds
         :type polling_frequency: integer
         :param retries: Number of retries during job poll. Default is 3
         :type retries: integer
         :param poll: Poll job until its completion
         :type poll: Boolean
@@ -447,14 +451,85 @@
                                                    error_code=ErrorCode.GENERIC_ERROR,
                                                    error_desc=f"Failed to add the tables to the source {source_id}",
                                                    response=response, job_id=None,
                                                    source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to add the tables to the source {source_id} " + str(e))
 
+    def add_query_tables_to_source(self, source_id=None, tables_to_add_config=None, poll_timeout=300,
+                                   polling_frequency=15,
+                                   retries=3, poll=True):
+        """
+        Function to add query tables to source
+        :param source_id: source identifier entity id
+        :type source_id: String
+        :param tables_to_add_config: Array of JSON configuration object
+        :type tables_to_add_config: List
+        ```
+        tables_to_add_config = [{
+                "table_type": "TABLE",
+                "target_table_name": "",
+                "target_schema_name": ""
+                "is_query_table": true,
+                "query": "select * from \"SALESDB\".\"ORDERS\""
+        }]
+        ```
+        :param poll_timeout: metacrawl job timeout in seconds
+        :type poll_timeout: integer. Default 300 seconds
+        :param polling_frequency: polling frequency for the job in seconds. Default 15 seconds
+        :type polling_frequency: integer
+        :param retries: Number of retries during job poll. Default is 3
+        :type retries: integer
+        :param poll: Poll job until its completion
+        :type poll: Boolean
+        :return: response dict
+        """
+        if None in {source_id} or tables_to_add_config is None:
+            self.logger.error("source id or tables_to_add_config cannot be None")
+            raise Exception("source id or tables_to_add_config cannot be None")
+        try:
+            url_for_add_tables_to_source = url_builder.add_query_tables_to_source_url(self.client_config, source_id)
+            add_tables_dict = {"tables_to_add": tables_to_add_config}
+            response = IWUtils.ejson_deserialize(
+                self.call_api("POST", url_for_add_tables_to_source,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                              add_tables_dict).content)
+            result = response.get('result', None)
+            self.logger.debug(response)
+            if result is not None:
+                self.logger.info(f"Added the below table Ids to the source {source_id}")
+                self.logger.info(result["added_tables"])
+                self.logger.info(response["message"])
+                self.logger.info(f"Triggered metacrawl job for tables. Infoworks JobID {result['job_created']}")
+                job_id = result['job_created']
+                if not poll:
+                    self.logger.info(f"Tables added to source {source_id} and metacrawl job was submitted {job_id}")
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+                else:
+                    if job_id:
+                        return self.poll_job(source_id=source_id, job_id=job_id, poll_timeout=poll_timeout,
+                                             polling_frequency=polling_frequency,
+                                             retries=retries)
+                    else:
+                        return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                           error_code=ErrorCode.GENERIC_ERROR,
+                                                           error_desc=f"Failed to add the tables to the source {source_id}",
+                                                           response=response, job_id=None,
+                                                           source_id=source_id)
+            else:
+                self.logger.error(f"Failed to add the tables to the source {source_id}")
+                self.logger.debug(response)
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.GENERIC_ERROR,
+                                                   error_desc=f"Failed to add the tables to the source {source_id}",
+                                                   response=response, job_id=None,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to add the tables to the source {source_id} " + str(e))
+
     def configure_tables_and_tablegroups(self, source_id=None, configuration_obj=None):
         """
         Function to configure tables and table-groups.
         The configuration_obj should be similar to the json object that is the output of GET source configuration API
         :param source_id: source identifier entity id
         :type source_id: String
         :param configuration_obj: Configurations for the tables and tablegroups under given source id
@@ -463,54 +538,66 @@
         """
         try:
             if None in {source_id} or configuration_obj is None:
                 self.logger.error("source id or configuration_obj cannot be None")
                 raise Exception("source id or configuration_obj cannot be None")
             configure_tables_tg_url = url_builder.configure_tables_and_tablegroups_url(self.client_config, source_id)
             errors = {}
-            response = IWUtils.ejson_deserialize(
-                self.call_api("POST", configure_tables_tg_url,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                              {"configuration": configuration_obj}).content)
-            result = response.get('result', {}).get("configuration", {}).get("iw_mappings", [])
+            response = self.call_api("POST", configure_tables_tg_url,
+                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                                     {"configuration": configuration_obj})
+            parsed_response = IWUtils.ejson_deserialize(response.content)
+            result = parsed_response.get('result', {}).get("configuration", {}).get("iw_mappings", [])
             count = 0
-            # print(response)
+            print("Config Migration API Response:", response)
+
             self.logger.debug(response)
             if result is not None:
                 for config_item in result:
                     table_upsert_status = config_item.get('table_upsert_status', None)
                     if table_upsert_status is not None and len(table_upsert_status.get("error", [])) != 0:
-                        self.logger.info(f"{table_upsert_status}")
-                        count = count + 1
-                        errors[count] = table_upsert_status["error"]
-                        self.logger.error("Found errors during table and table group configurations")
-                        self.logger.error(table_upsert_status.get("error", []))
+                        if not table_upsert_status["error"][0].startswith("Truncate the table:") and not \
+                        table_upsert_status["error"][0].startswith("After ingestion you can't change"):
+                            self.logger.info(f"{table_upsert_status}")
+                            count = count + 1
+                            errors[count] = table_upsert_status["error"]
+                            self.logger.error("Found errors during table and table group configurations")
+                            self.logger.error(table_upsert_status.get("error", []))
                     elif table_upsert_status is None:
                         self.logger.info(f"Could not get table insert status from {config_item}")
                     else:
                         pass
                     self.logger.debug(str(config_item))
                 if len(errors) != 0:
                     self.logger.error(f"Failed due to multiple errors\n{errors}")
+                    result = parsed_response.get("result", [])
+                    return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                       error_code=ErrorCode.GENERIC_ERROR,
+                                                       error_desc=f"Failed to configure tables and table groups",
+                                                       job_id=None,
+                                                       response=result,
+                                                       source_id=source_id)
+                elif response.status_code != 200:
+                    self.logger.error(f"Failed during config migration")
                     return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                        error_code=ErrorCode.GENERIC_ERROR,
-                                                       error_desc=f"Failed to configure tables and table groups {response} ",
+                                                       error_desc=f"Failed to configure tables and table groups {parsed_response} ",
                                                        job_id=None,
-                                                       response=response,
+                                                       response=parsed_response,
                                                        source_id=source_id)
                 else:
                     self.logger.info(f"Successfully configured tables and table groups for the source")
-                    return SourceResponse.parse_result(status=Response.Status.SUCCESS)
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
             else:
                 self.logger.error("Failed to configure tables and table groups")
                 return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                   error_desc=f"Failed to configure tables and table groups {response} ",
+                                                   error_desc=f"Failed to configure tables and table groups {parsed_response} ",
                                                    job_id=None,
-                                                   response=response,
+                                                   response=parsed_response,
                                                    source_id=source_id)
         except Exception as e:
             traceback.print_exc()
             raise SourceError(f"Failed to configure tables and table groups" + str(e))
 
     def create_table_group(self, source_id=None, table_group_obj=None):
         """
@@ -594,23 +681,25 @@
                                                    error_code=ErrorCode.GENERIC_ERROR,
                                                    error_desc="Failed to create table groups",
                                                    response=response, job_id=None,
                                                    source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to update table group" + str(e))
 
-    def get_table_group_details(self, source_id=None, params=None, tg_id=None):
+    def get_table_group_details(self, source_id=None, params=None, tg_id=None, pagination=True):
         """
         Function to list the table groups under source
         :param source_id: entity identifier for source
         :type source_id: String
         :param tg_id: id of table group config to fetch
         :type tg_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -635,14 +724,16 @@
                                                        error_desc=f'Failed to list the table groups under source {source_id}',
                                                        response=response)
                 if tg_id is not None:
                     tg_list.extend([result])
                 else:
                     while len(result) > 0:
                         tg_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -730,30 +821,67 @@
                 raise Exception("source id or body cannot be None")
             response = IWUtils.ejson_deserialize(
                 self.call_api("POST", url_builder.submit_source_job(self.client_config, source_id),
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
                               body).content)
             result = response.get('result', {})
             if len(result) != 0:
-                job_id = result["id"]
-                if not poll:
-                    self.logger.info(f"Job successfully submitted for {source_id}. JobID to track is: {job_id}")
-                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, job_id=job_id, response=response)
+                if body.get('job_type') == "streaming_start":
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+                job_id = result.get("id", None)
+                if job_id is not None:
+                    if not poll:
+                        self.logger.info(f"Job successfully submitted for {source_id}. JobID to track is: {job_id}")
+                        return SourceResponse.parse_result(status=Response.Status.SUCCESS, job_id=job_id,
+                                                           response=response)
+                    else:
+                        return self.poll_job(source_id=source_id, job_id=job_id, poll_timeout=poll_timeout,
+                                             polling_frequency=polling_frequency,
+                                             retries=retries)
                 else:
-                    return self.poll_job(source_id=source_id, job_id=job_id, poll_timeout=poll_timeout,
-                                         polling_frequency=polling_frequency,
-                                         retries=retries)
+                    self.logger.error(f"Failed to submit the source job.")
+                    return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                       error_desc=f"Failed to submit the source job.",
+                                                       response=response)
             else:
                 self.logger.error(f"Failed to submit the source job.")
                 return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                    error_desc=f"Failed to submit the source job.",
                                                    response=response)
         except Exception as e:
             raise SourceError(f"Failed to create source job: " + str(e))
 
+    def stop_streaming_job(self, source_id=None, table_ids=None):
+        """
+        Function to stop Streaming Jobs.
+        :param source_id: Identifier for Source
+        :type source_id: String
+        :table_ids: Identifier for Tables
+        :type table_ids: Array
+        """
+        try:
+            if source_id is None or table_ids is None:
+                self.logger.error("source_id or table_ids cannot be None")
+                raise Exception("source_id or table_ids cannot be None")
+
+            request_body = {
+                "table_ids": [table_id.strip() for table_id in table_ids]
+            }
+            response = self.call_api(
+                "POST", url_builder.stop_streaming_job_url(self.client_config, source_id),
+                IWUtils.get_default_header_for_v3(self.client_config['bearer_token']), request_body)
+            parsed_response = IWUtils.ejson_deserialize(response.content)
+            if response.status_code == 200:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc="Failed to stop streaming jobs", response=parsed_response)
+        except Exception as e:
+            raise SourceError(f"Failed to stop streaming job: " + str(e))
+
     def resubmit_source_job(self, job_id=None, poll=False, poll_timeout=300, polling_frequency=15, retries=3):
         """
         Function to resubmit the jobs
         :param job_id: infoworks ob id of the failed job
         :type job_id: String
         :param poll_timeout: test connection job timeout in seconds
         :type poll_timeout: integer. Default 300 seconds
@@ -785,19 +913,21 @@
             else:
                 self.logger.error("Failed to submit the Job")
                 return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                    error_desc="Failed to submit the Job", response=response)
         except Exception as e:
             raise SourceError(f"Failed to create source job: " + str(e))
 
-    def get_list_of_sources(self, params=None):
+    def get_list_of_sources(self, params=None, pagination=True):
         """
         Function to list the sources
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_sources = url_builder.list_sources_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
         source_list = []
@@ -806,14 +936,16 @@
                 self.call_api("GET", url_to_list_sources,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 while len(result) > 0:
                     source_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -956,23 +1088,25 @@
                                                    error_desc="Error in updating source advanced configs",
                                                    response=parsed_response
                                                    )
         except Exception as e:
             self.logger.error("Error in updating the source advanced configs")
             raise SourceError("Error in updating the source advanced config" + str(e))
 
-    def get_advanced_configuration_of_sources(self, source_id=None, params=None, key=None):
+    def get_advanced_configuration_of_sources(self, source_id=None, params=None, key=None, pagination=True):
         """
         Function to get the advanced configuration of source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param key: Name of advanced config to get
         :type key: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -998,14 +1132,16 @@
                                                        response=response
                                                        )
                 if key is not None:
                     adv_config_list.extend([result])
                 else:
                     while len(result) > 0:
                         adv_config_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1106,21 +1242,23 @@
                                                    error_desc="Error in updating source configs",
                                                    response=response
                                                    )
         except Exception as e:
             self.logger.error("Error in updating the source configs")
             raise SourceError("Error in updating the source configs" + str(e))
 
-    def list_tables_in_source(self, source_id=None, params=None):
+    def list_tables_in_source(self, source_id=None, params=None, pagination=True):
         """
         Function to list the tables part of the source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -1133,14 +1271,16 @@
                 self.call_api("GET", url_to_list_tables,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     tables_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1156,21 +1296,23 @@
                 response["result"] = tables_list
                 response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in listing tables under source")
             raise SourceError("Error in listing tables under source" + str(e))
 
-    def get_list_of_table_groups(self, source_id=None, params=None):
+    def get_list_of_table_groups(self, source_id=None, params=None, pagination=True):
         """
         Function to list the tables groups part of the source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -1183,14 +1325,16 @@
                 self.call_api("GET", url_to_list_tablegrps,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     tablegrp_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1510,40 +1654,50 @@
                                                    error_desc="Error in updating export configuration of the table",
                                                    response=response)
 
         except Exception as e:
             self.logger.error("Error in updating the export configuration of the table")
             raise SourceError(f"Error in updating the export configuration of the table for {table_id} " + str(e))
 
-    def get_table_ingestion_metrics(self, source_id=None, table_id=None):
+    def get_table_ingestion_metrics(self, source_id=None, table_id=None, params=None, pagination=True):
         """
         Function to fetch ingestion metrics of source tables
         :param source_id: Entity identifier for source
         :type source_id: String
         :param table_id: table entity id
         :type table_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
         if table_id is None:
-            url_to_get_ing_metrics = url_builder.get_ingestion_metrics_source_url(self.client_config, source_id)
+            url_to_get_ing_metrics = url_builder.get_ingestion_metrics_source_url(self.client_config, source_id) \
+                                     + IWUtils.get_query_params_string_from_dict(params=params)
         else:
             url_to_get_ing_metrics = url_builder.get_ingestion_metrics_table_url(self.client_config, source_id,
-                                                                                 table_id)
+                                                                                 table_id)\
+                                     + IWUtils.get_query_params_string_from_dict(params=params)
         metric_results = []
         try:
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_get_ing_metrics,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     metric_results.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -1982,21 +2136,23 @@
                                                    error_desc=f"Failed to get the table configurations for {source_id} ",
                                                    response=response, job_id=None, source_id=None)
             else:
                 return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             raise SourceError(f"Failed to get the source configurations for {source_id} " + str(e))
 
-    def list_tables_under_source(self, source_id=None, params=None):
+    def list_tables_under_source(self, source_id=None, params=None, pagination=True):
         """
         Function to list tables under source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         tables_list = []
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
@@ -2009,14 +2165,16 @@
                                                                    self.client_config['bearer_token']),
                                                                ).content)
             initial_msg = response.get("message", "")
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     tables_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2282,22 +2440,24 @@
             else:
                 return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
                                                    source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to update the table schema for {table_id} " + str(e))
 
     def get_file_mappings_for_json_source(self, source_id=None, file_mapping_id=None, file_mapping_name=None,
-                                          params=None):
+                                          params=None, pagination=True):
         """
         Function to get file mappings
         :param source_id: Entity identifier for source
         :type source_id: String
         :param file_mapping_id: Entity identifier of the file mapping
         :param file_mapping_name: Name of the file mapping for which details are to be fetched
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
 
         if params is None:
@@ -2315,14 +2475,16 @@
                     self.call_api("GET", file_mappings_url,
                                   IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
                 if response is not None:
                     initial_msg = response.get("message", "")
                     result = response.get("result", [])
                     while len(result) > 0:
                         file_mappings_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2538,23 +2700,25 @@
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id, response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to create a json table.')
             raise SourceError(response.get("message", "Error occurred while trying to create a json table."))
 
-    def get_json_source_table(self, source_id=None, file_mapping_id=None, table_id=None, params=None):
+    def get_json_source_table(self, source_id=None, file_mapping_id=None, table_id=None, params=None, pagination=True):
         """
         Function to get json source table details
         :param file_mapping_id: Entity identifier for file mapping
         :type file_mapping_id: String
         :param source_id: Entity identifier for source
         :type source_id: String
         :param table_id: Entity identifier for table
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id, file_mapping_id}:
             self.logger.error("source id or file_mapping_id cannot be None")
             raise Exception("source id or file_mapping_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
@@ -2568,14 +2732,16 @@
                     self.call_api("GET", get_json_src_tbls_url,
                                   IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
                 if response is not None:
                     initial_msg = response.get("message", "")
                     result = response.get("result", [])
                     while len(result) > 0:
                         tables_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2638,21 +2804,23 @@
                                                    response=response, job_id=None, source_id=source_id)
             else:
                 return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
                                                    source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to delete the json source table {table_id} " + str(e))
 
-    def get_source_audit_logs(self, source_id=None, params=None):
+    def get_source_audit_logs(self, source_id=None, params=None, pagination=True):
         """
         Function to get audit logs of source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         audit_logs = []
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         if params is None:
@@ -2665,14 +2833,16 @@
                                                                    self.client_config['bearer_token']),
                                                                ).content)
             initial_msg = response.get("message", "")
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     audit_logs.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2685,22 +2855,24 @@
             response["result"] = audit_logs
             response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
         except Exception as e:
             self.logger.error(f"Failed to get the audit logs of {source_id} " + str(e))
             raise SourceError(f"Failed to get the audit logs of {source_id} " + str(e))
 
-    def get_table_audit_logs(self, source_id=None, table_id=None, params=None):
+    def get_table_audit_logs(self, source_id=None, table_id=None, params=None, pagination=True):
         """
         Function to get audit logs of source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param table_id: Entity identifier of table
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         audit_logs = []
         if None in {source_id, table_id}:
             self.logger.error("source id or table_id cannot be None")
             raise Exception("source id or table_id cannot be None")
         if params is None:
@@ -2713,14 +2885,16 @@
                                                                    self.client_config['bearer_token']),
                                                                ).content)
             initial_msg = response.get("message", "")
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     audit_logs.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2733,22 +2907,24 @@
             response["result"] = audit_logs
             response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
         except Exception as e:
             self.logger.error(f"Failed to get the audit logs of table {table_id} " + str(e))
             raise SourceError(f"Failed to get the audit logs of table {table_id} " + str(e))
 
-    def get_tablegroup_audit_logs(self, source_id=None, table_group_id=None, params=None):
+    def get_tablegroup_audit_logs(self, source_id=None, table_group_id=None, params=None, pagination=True):
         """
         Function to get audit logs of source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param table_group_id: Entity identifier of table group
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         audit_logs = []
         if None in {source_id, table_group_id}:
             self.logger.error("source id or table_group_id cannot be None")
             raise Exception("source id or table_group_id cannot be None")
         if params is None:
@@ -2762,14 +2938,16 @@
                                                                    self.client_config['bearer_token']),
                                                                ).content)
             initial_msg = response.get("message", "")
             if response is not None:
                 result = response.get("result", [])
                 while len(result) > 0:
                     audit_logs.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2783,21 +2961,23 @@
             response["result"] = audit_logs
             response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
         except Exception as e:
             self.logger.error(f"Failed to get the audit logs of table group {table_group_id} " + str(e))
             raise SourceError(f"Failed to get the audit logs of table group {table_group_id} " + str(e))
 
-    def get_list_of_advanced_config_of_table(self, source_id=None, table_id=None, params=None):
+    def get_list_of_advanced_config_of_table(self, source_id=None, table_id=None, params=None, pagination=True):
         """
             Function to get list of Advance Config of the table
             :param source_id: Entity identifier of the source
             :param table_id: Entity identifier of the table
             :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
             :type: JSON dict
+            :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+            :type pagination: Boolean
             :return: response dict
         """
         if None in {source_id, table_id}:
             raise Exception(f"source_id, table_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_get_table_adv_config = url_builder.table_advanced_base_url(self.client_config, source_id,
@@ -2809,14 +2989,16 @@
                 self.call_api("GET", url_to_get_table_adv_config,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     adv_config_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -2934,22 +3116,24 @@
                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to get/delete adv config details.')
             raise SourceError('Error occurred while trying to get/delete adv config details.')
 
-    def update_table_configurations(self, source_id=None, table_id=None, config_body=None):
+    def update_table_configurations(self, source_id=None, table_id=None, config_body=None,update_type="PUT"):
         """
         Function to update the table configurations including columns and ingestion configurations
         :param table_id: Entity identifier for table
         :type table_id: String
         :param source_id: Entity identifier for source
         :type source_id: String
         :param config_body: JSON body
+        :param update_type: Specify PUT/PATCH
+        :type update_type: String
         ```
         config_body_example: {
             "id": "9376bf97a286e35efe86d321",
             "name": "dim_state",
             "original_table_name": "dim_state",
             "data_lake_path": "/iw/sources/customer_360_sql_server_schema/9376bf97a286e35efe86d321",
             "meta_crawl_performed": true,
@@ -3027,17 +3211,20 @@
         }
         ```
         :return: response dict
         """
         if None in {source_id, table_id} or config_body is None:
             self.logger.error("source id or table_id or config_body cannot be None")
             raise Exception("source id or table_id or config_body cannot be None")
+        if update_type not in ["PUT","PATCH"]:
+            self.logger.error("update_type can only be PUT/PATCH")
+            raise Exception("update_type can only be PUT/PATCH")
         try:
             table_config_url = url_builder.get_table_configuration(self.client_config, source_id, table_id)
-            response = IWUtils.ejson_deserialize(self.call_api("PUT", table_config_url,
+            response = IWUtils.ejson_deserialize(self.call_api(update_type, table_config_url,
                                                                IWUtils.get_default_header_for_v3(
                                                                    self.client_config['bearer_token']), data=config_body
                                                                ).content)
             result = response.get('result', {})
             if "id" not in result:
                 self.logger.error(f"Failed to update the table configurations for {table_id}")
                 return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
@@ -3192,21 +3379,23 @@
                                                    response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(e))
             self.logger.exception('Error occurred while trying to add/update validation spec for table')
             raise SourceError('Error occurred while trying to add/update validation spec for table')
 
-    def list_validation_specs_for_table(self, source_id=None, table_id=None, params=None):
+    def list_validation_specs_for_table(self, source_id=None, table_id=None, params=None, pagination=True):
         """
         Function to list the validation specs for a table
         :param source_id: Entity identifier of the source
         :param table_id: Entity identifier of the table
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {source_id, table_id}:
             raise Exception(f"source_id, table_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
         url_to_list_validation_specs = url_builder.get_table_configuration(self.client_config, source_id,
@@ -3218,14 +3407,16 @@
                 self.call_api("GET", url_to_list_validation_specs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 while len(result) > 0:
                     validations_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -3271,7 +3462,216 @@
                                                    error_desc=f'Failed to delete validation spec of the table {table_id}',
                                                    response=response)
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
 
         except Exception as e:
             self.logger.error("Error in deleting the validation spec of the table")
             raise SourceError("Error in deleting the validation spec of the table" + str(e))
+
+    def configure_table_group_schedule_user(self, source_id, table_group_id, schedule_user_details=None):
+        """
+        Configure Table Group schedule user of a particular Table Group belonging to the Source
+        :param source_id: Source ID of which Table Group belongs
+        :type source_id: String
+        :param table_group_id: Table Group ID to fetch schedule for.
+        :type table_group_id: String
+        :param schedule_user_details: Scheduler User Details
+        :type schedule_user_details: JSON
+        :return: Response Dict
+        """
+        if source_id is None or table_group_id is None:
+            self.logger.error("source_id or table_group_id cannot be None")
+            raise Exception("source_id or table_group_id cannot be None")
+        if schedule_user_details is None:
+            response = None
+            try:
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("PUT", url_builder.configure_table_group_schedule_user_url(
+                        self.client_config, source_id, table_group_id), IWUtils.get_default_header_for_v3(
+                        self.client_config['bearer_token'])).content)
+
+                result = response.get('result', None)
+
+                if result is None:
+                    self.logger.error('Failed to configure table group schedule user')
+                    return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                       error_code=ErrorCode.USER_ERROR,
+                                                       error_desc='Failed to configure table group schedule user',
+                                                       response=response)
+
+                table_group_id = str(table_group_id)
+                self.logger.info(
+                    'Successfully configured table group {id} schedule user.'.format(id=table_group_id))
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
+                                                   response=response)
+
+            except Exception as e:
+                self.logger.error('Response from server: ' + str(response))
+                self.logger.exception('Error occurred while trying to configure table group schedule user.')
+                raise SourceError('Error occurred while trying to configure table group schedule user.')
+        else:
+            # To Validate credentials
+            update_table_group_response = None
+            try:
+                response = self.call_api("PUT", url_builder.verify_refresh_token_url(self.client_config),
+                                         IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                                         schedule_user_details)
+
+                if response.status_code == 200:
+                    self.logger.info("Email and Refresh token validated")
+                else:
+                    raise Exception("Failed to validate email and refresh token")
+
+                table_group_response = self.get_table_group_details(source_id=source_id, tg_id=table_group_id)
+                table_group_response_parsed = table_group_response.get('result', {}).get('response', {}).get('result', {})
+
+                table_group_response_parsed[0]['scheduler_username'] = schedule_user_details["scheduler_username"]
+                table_group_response_parsed[0]['scheduler_auth_token'] = schedule_user_details["scheduler_auth_token"]
+
+                update_table_group_response = self.update_table_group(source_id=source_id, table_group_id=table_group_id,
+                                                                      table_group_obj=table_group_response_parsed[0])
+
+                if update_table_group_response.get('result', {}).get('response', {}) is None:
+                    self.logger.error('Failed to configure table group schedule user')
+                    return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                       error_code=ErrorCode.USER_ERROR,
+                                                       error_desc='Failed to configure table group schedule user',
+                                                       response=update_table_group_response.get('result', {}).get('response', {}))
+                table_group_id = str(table_group_id)
+                self.logger.info(
+                    'Successfully configured table group {id} schedule user.'.format(id=table_group_id))
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
+                                                   response=update_table_group_response.get('result', {}).get('response', {}))
+            except Exception as e:
+                self.logger.error('Response from server: ' + str(update_table_group_response))
+                self.logger.exception('Error occurred while trying to configure table group schedule user.')
+                raise SourceError('Error occurred while trying to configure table group schedule user.')
+
+
+
+    def enable_table_group_schedule(self, source_id, table_group_id, schedule_config):
+        """
+        Enables Schedule of a particular table group belonging to the source
+        :param source_id: Source ID of which table group belongs
+        :type source_id: String
+        :param table_group_id: Table Group ID to fetch schedule for.
+        :type table_group_id: String
+        :param schedule_config: Schedule Configuration JSON of the Table Group
+        :type schedule_config: JSON
+        ```
+        schedule_config_example = {
+              "start_date": "02/22/2020",
+              "end_date": "02/24/2020",
+              "start_hour": 12,
+              "start_min": 25,
+              "end_hour": 17,
+              "end_min": 30,
+              "repeat_interval_measure": 2,
+              "repeat_interval_unit": "{string}",
+              "ends": True,
+              "is_custom_job": True,
+              "custom_job_details": {
+                "starts_daily_at": "14:00",
+                "ends_daily_at": "15:00",
+                "repeat_interval_unit": "{string}",
+                "repeat_interval_measure": 2
+              },
+              "repeat_on_last_day": "{boolean}",
+              "specified_days": 1
+        }
+        ```
+        :return: Response Dict
+        """
+        if source_id is None or table_group_id is None or schedule_config is None:
+            self.logger.error("source_id or table_group_id or schedule_config cannot be None")
+            raise Exception("source_id or table_group_id or schedule_config cannot be None")
+        response = None
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.get_enable_table_group_schedule_url(
+                self.client_config, source_id, table_group_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), schedule_config).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to enable schedule of the table group')
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.USER_ERROR,
+                                                   error_desc='Failed to enable schedule of the table group',
+                                                   response=response)
+
+            table_group_id = str(table_group_id)
+            self.logger.info(
+                'Successfully enabled schedule for the table group {id}.'.format(id=table_group_id))
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
+                                               response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to enable table group schedule.')
+            raise SourceError('Error occurred while trying to enable table group schedule.')
+
+    def disable_table_group_schedule(self, source_id, table_group_id):
+        """
+        Disables Schedule of a particular Table Group belonging to the Source
+        :param source_id: Source ID of which Table Group belongs
+        :type source_id: String
+        :param table_group_id: Table Group ID to fetch schedule for.
+        :type table_group_id: String
+        :return: Response Dict
+        """
+        if source_id is None or table_group_id is None:
+            self.logger.error("source_id or table_group_id cannot be None")
+            raise Exception("source_id or table_group_id cannot be None")
+        response = None
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.get_disable_table_group_schedule_url(
+                self.client_config, source_id, table_group_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to disable schedule of the table group')
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.USER_ERROR,
+                                                   error_desc='Failed to disable schedule of the table group',
+                                                   response=response)
+
+            table_group_id = str(table_group_id)
+            self.logger.info(
+                'Successfully disabled schedule for the table group {id}.'.format(id=table_group_id))
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
+                                               response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to disable table group schedule.')
+            raise SourceError('Error occurred while trying to disable table group schedule.')
+
+    def get_table_group_schedule(self, source_id, table_group_id):
+        """
+        Gets Schedules of particular Table Group belonging to the Source
+        :param source_id: Table Group ID of which Source belongs
+        :type source_id: String
+        :param table_group_id: Table Group ID to fetch schedule for.
+        :type table_group_id: String
+        :return: Response Dict
+        """
+        if source_id is None or table_group_id is None:
+            self.logger.error("source_id or table_group_id cannot be None")
+            raise Exception("source_id or table_group_id cannot be None")
+
+        response = None
+
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_table_group_schedule_url(
+                self.client_config, source_id, table_group_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
+                                               response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get table group schedule.')
+            raise SourceError('Error occurred while trying to get table group schedule.')
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/source_response.py` & `infoworkssdk-4.1/infoworks/sdk/source_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/url_builder.py` & `infoworkssdk-4.1/infoworks/sdk/url_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,28 @@
     """
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/source_tables'.format(ip=config['ip'],
                                                                                             port=config['port'],
                                                                                             protocol=config['protocol'],
                                                                                             source_id=source_id)
     return request
 
+def add_query_tables_to_source_url(config, source_id):
+    """
+    returns URL to add query tables using v3 api
+    :param config: client configurations
+    :type config: dict
+    :param source_id: source entity id
+    :type source_id: string
+    :return: url to browse source tables details
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/query_tables'.format(ip=config['ip'],
+                                                                                           port=config['port'],
+                                                                                           protocol=config['protocol'],
+                                                                                           source_id=source_id)
+    return request
 
 def configure_tables_and_tablegroups_url(config, source_id):
     """
     returns URL to configure source tables using v3 api
     :param config: client configurations
     :type config: dict
     :param source_id: source entity id
@@ -298,14 +312,31 @@
         request = '{protocol}://{ip}:{port}/v3/admin/jobs/{job_id}'.format(ip=config['ip'],
                                                                            port=config['port'],
                                                                            job_id=job_id,
                                                                            protocol=config['protocol'])
     return request
 
 
+def get_cluster_jobs_status_url(config, job_id):
+    """
+    returns URL for checking job progress
+
+    :param config: client configurations
+    :type config: dict
+    :param job_id: Identifier for Job
+    :type job_id: string
+    :return: url for the job status
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/jobs/{job_id}/runs'.format(ip=config['ip'],
+                                                                            port=config['port'],
+                                                                            job_id=job_id,
+                                                                            protocol=config['protocol'])
+    return request
+
+
 def configure_source_url(config, source_id):
     """
     returns URL to configure the source using v3 rest apis
     :param config: client configurations
     :type config: dict
     :param source_id: source entity id
     :type source_id: string
@@ -562,32 +593,40 @@
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'],
         domain_id=domain_id,
         workflow_id=workflow_id)
     return request
 
 
-def get_workflow_status_url(config, workflow_id, workflow_run_id):
+def get_workflow_status_url(config, workflow_id, workflow_run_id,domain_id):
     """
     returns URL to fetch status of workflow using v3 api
     :param config: client configurations
     :type config: dict
     :param workflow_id: Identifier for workflow id
     :type workflow_id: string
     :param workflow_run_id: Identifier for workflow run id
     :type workflow_run_id: string
     :return: url to fetch status of workflow using v3 api
     """
-    request = '{protocol}://{ip}:{port}/v3/admin/workflows/{workflow_id}/runs/{workflow_run_id}'.format(
-        ip=config['ip'], port=config['port'],
-        protocol=config['protocol'],
-        workflow_id=workflow_id,
-        workflow_run_id=workflow_run_id)
-    return request
-
+    if domain_id is None:
+        request = '{protocol}://{ip}:{port}/v3/admin/workflows/{workflow_id}/runs/{workflow_run_id}'.format(
+            ip=config['ip'], port=config['port'],
+            protocol=config['protocol'],
+            workflow_id=workflow_id,
+            workflow_run_id=workflow_run_id)
+        return request
+    else:
+        request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/workflows/{workflow_id}/runs/{workflow_run_id}'.format(
+            ip=config['ip'], port=config['port'],
+            protocol=config['protocol'],
+            workflow_id=workflow_id,
+            workflow_run_id=workflow_run_id,
+            domain_id=domain_id)
+        return request
 
 def get_all_workflows_url(config):
     """
     returns URL to fetch all workflows in Infoworks using v3 api
     :param config: client configurations
     :type config: dict
     :return: url fetch all workflows in Infoworks using v3 api
@@ -1503,27 +1542,27 @@
     return request
 
 
 def get_table_audit_logs_url(config, source_id, table_id):
     """
     returns url to get table audit logs
     """
-    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}//tables/table_id/audit-logs'.format(
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/audit-logs'.format(
         source_id=source_id,
         table_id=table_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
 
 
 def get_table_group_audit_logs_url(config, source_id, table_group_id):
     """
     returns url to get table group audit logs
     """
-    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/table_group_id/audit-logs'.format(
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/{table_group_id}/audit-logs'.format(
         source_id=source_id,
         table_group_id=table_group_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
 
 
@@ -2038,16 +2077,16 @@
 def list_domains_admin_url(config):
     """
     returns Admin URL to list domains using v3 api
     :param config: client configurations
     :type config: dict
     :return: url to list domains
     """
-    request = '{protocol}://{ip}:{port}/v3/admins/domains'.format(ip=config['ip'], port=config['port'],
-                                                                  protocol=config['protocol'])
+    request = '{protocol}://{ip}:{port}/v3/admin/domains'.format(ip=config['ip'], port=config['port'],
+                                                                 protocol=config['protocol'])
     return request
 
 
 def stop_interactive_cluster_url(config):
     request = '{protocol}://{ip}:{port}/v3/admin/environment/cluster/service/stop'.format(ip=config['ip'],
                                                                                           port=config['port'],
                                                                                           protocol=config[
@@ -2129,7 +2168,169 @@
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/jobs/{job_id}/logs'.format(ip=config['ip'],
                                                                                           port=config['port'],
                                                                                           protocol=config['protocol'],
                                                                                           source_id=source_id,
                                                                                           job_id=job_id
                                                                                           )
     return request
+
+
+def get_table_group_schedule_url(config, source_id, table_group_id):
+    """
+    Returns URL to get Table Group Schedule
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/{table_group_id}/schedules'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], source_id=source_id,
+        table_group_id=table_group_id)
+    return request
+
+
+def get_enable_table_group_schedule_url(config, source_id, table_group_id):
+    """
+    Returns URL to Enable Table Group Schedule
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/{table_group_id}/schedules/enable'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], source_id=source_id,
+        table_group_id=table_group_id)
+    return request
+
+
+def get_disable_table_group_schedule_url(config, source_id, table_group_id):
+    """
+    Returns URL to Disable Table Group Schedule
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/{table_group_id}/schedules/disable'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], source_id=source_id,
+        table_group_id=table_group_id)
+    return request
+
+
+def configure_table_group_schedule_user_url(config, source_id, table_group_id):
+    """
+    Return URL to configure Table Group schedule user
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/{table_group_id}/schedules/user'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], source_id=source_id,
+        table_group_id=table_group_id)
+    return request
+
+
+def get_pipeline_job_summary_url(config, domain_id, pipeline_id, job_id):
+    """
+    returns URL to add tables to replicator definition using v3 api
+    :param config: client configurations
+    :type config: dict
+    :param domain_id: Identifier for domain
+    :type domain_id: string
+    :param pipeline_id: Identifier for Pipeline
+    :type pipeline_id: string
+    :param job_id: Identifier of Job
+    :type job_id: string
+    :return: url to submit replication data job
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipelines/{pipeline_id}/jobs/{job_id}/summary' \
+        .format(ip=config['ip'], port=config['port'], protocol=config['protocol'], domain_id=domain_id,
+                pipeline_id=pipeline_id, job_id=job_id)
+    return request
+
+
+def get_pipeline_group_job_summary_url(config, domain_id, pipeline_group_id, job_id):
+    """
+    returns URL to add tables to replicator definition using v3 api
+    :param config: client configurations
+    :type config: dict
+    :param domain_id: Identifier for domain
+    :type domain_id: string
+    :param pipeline_group_id: Identifier for Pipeline Group
+    :type pipeline_group_id: string
+    :param job_id: Identifier of Job
+    :type job_id: string
+    :return: url to submit replication data job
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipeline-groups/{pipeline_group_id}/jobs' \
+              '/{job_id}/summary'.format(ip=config['ip'], port=config['port'], protocol=config['protocol'],
+                                         domain_id=domain_id, pipeline_group_id=pipeline_group_id, job_id=job_id)
+    return request
+
+
+def stop_streaming_job_url(config, source_id):
+    """
+        returns URL to stop streaming job
+        :param config: client configurations
+        :type config: dict
+        :param source_id: Identifier for source
+        :type source_id: string
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/stop-streaming'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'],
+        source_id=source_id)
+    return request
+
+
+def verify_refresh_token_url(config):
+    """
+        returns URL to verify refresh token
+        :param config: client configurations
+        :return: dict
+    """
+    request = '{protocol}://{ip}:{port}/v3/verify-refresh-token'.format(
+        ip=config['ip'], port=config['port'], protocol=config['protocol']
+    )
+    return request
+
+
+def list_job_hooks(config):
+    """
+        returns URL for listing job hooks under admin
+        :param config: client configurations
+        :type config: dict
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/job-hooks'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+def get_list_of_job_hook_dependencies(config,job_hook_id):
+    """
+        returns URL for listing dependencies under given job hook
+        :param config: client configurations
+        :param job_hook_id: Identifier for job hook
+        :type job_hook_id: string
+        :type config: dict
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/job-hooks/{job_hook_id}/dependencies'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'],
+        job_hook_id=job_hook_id)
+    return request
+
+def get_list_of_source_extension_dependencies(config,source_extension_id):
+    """
+        returns URL for listing dependencies under given source_extension
+        :param config: client configurations
+        :param source_extension_id: Identifier for job hook
+        :type source_extension_id: string
+        :type config: dict
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/source-extensions/{source_extension_id}/dependencies'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'],
+        source_extension_id=source_extension_id)
+    return request
+
+def list_generic_source_types(config,generic_source_type_id=None):
+    """
+        returns URL for list generic source types registered in Infoworks
+        :param config: client configurations
+        :type config: dict
+    """
+    if generic_source_type_id is None:
+        request = '{protocol}://{ip}:{port}/v3/admin/generic-source-type'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    else:
+        request = '{protocol}://{ip}:{port}/v3/admin/generic-source-type/{generic_source_type_id}'.format(
+            ip=config['ip'], port=config['port'],
+            protocol=config['protocol'],
+            generic_source_type_id=generic_source_type_id)
+    return request
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/utils.py` & `infoworkssdk-4.1/infoworks/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/workflow_client.py` & `infoworkssdk-4.1/infoworks/sdk/workflow_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                         result = response.get("result", {}).get("items", [])
                 response["result"] = workflows_list
                 response["message"] = initial_msg
                 return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
             else:
                 workflows_list = []
                 response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.create_workflow_url(
-                    self.client_config, domain_id), IWUtils.get_default_header_for_v3(
+                    self.client_config, domain_id)+ IWUtils.get_query_params_string_from_dict(params=params), IWUtils.get_default_header_for_v3(
                     self.client_config['bearer_token'])).content)
 
                 if response is not None:
                     initial_msg = response.get("message", "")
                     result = response.get("result", [])
                     while len(result) > 0:
                         workflows_list.extend(result)
@@ -464,15 +464,15 @@
                                                  response=result)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to fetch status of workflow.')
             raise WorkflowError('Error occurred while trying to fetch status of workflow.')
 
-    def poll_workflow_run_till_completion(self, workflow_run_id=None, workflow_id=None, poll_interval=30):
+    def poll_workflow_run_till_completion(self, workflow_run_id=None, workflow_id=None,domain_id=None, poll_interval=30):
         """
         Polls Infoworks Data workflow for given workflow id and run id
         :param workflow_run_id: run id of the workflow running
         :type workflow_run_id: String
         :param workflow_id: entity id of the workflow running
         :type workflow_id: String
         :param poll_interval:interval in seconds between poll(default 30)
@@ -481,22 +481,22 @@
         """
         response = None
         if None in {workflow_id, workflow_run_id}:
             self.logger.error("workflow_id or workflow_run_id cannot be None")
             raise Exception("workflow_id or workflow_run_id cannot be None")
         try:
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
-                self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                self.client_config,workflow_id, workflow_run_id,domain_id), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
             result = response.get('result', {})
             if result:
                 workflow_status = result['workflow_status']["state"]
                 while workflow_status.lower() not in ['success', 'completed', 'failed', 'aborted', 'canceled']:
                     response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
-                        self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                        self.client_config, workflow_id, workflow_run_id,domain_id), IWUtils.get_default_header_for_v3(
                         self.client_config['bearer_token'])).content)
                     result = response.get('result', {})
                     workflow_status = result['workflow_status']["state"]
                     if workflow_status.lower() in ['success', 'completed', 'failed', 'aborted', 'canceled']:
                         break
                     print(f"workflow_status : {workflow_status}.Sleeping for {poll_interval} seconds")
                     time.sleep(poll_interval)
@@ -675,29 +675,31 @@
                 result = response.get("result", None)
                 if result is not None:
                     return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
                                                          response={"name": result.get("name")})
         except:
             raise WorkflowError("Unable to get workflow name")
 
-    def get_list_of_workflow_runs(self, domain_id=None, workflow_id=None, params=None, api_body_for_filter={}):
+    def get_list_of_workflow_runs(self, domain_id=None, workflow_id=None, params=None, api_body_for_filter={},pagination=True):
         """
         Gets List of Infoworks Data workflow runs details for given domain id and workflow id
         :param domain_id: Domain id to which the workflows belongs to, if None all workflows in all domains will be fetched
         :type domain_id: String
         :param workflow_id: Workflow id,if None all workflow runs in all domains will be fetched
         :type workflow_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :param api_body_for_filter: dict of API body
         :type api_body_for_filter: JSON dict
         ```
         example:
         {'limit': 10000, 'date_range': {'type': 'last', 'unit': 'day', 'value': 1}, 'offset': 0}
         ```
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response List
         """
         response = None
         initial_msg = ""
         try:
             if domain_id is None:
                 url_to_list_workflow_runs = url_builder.get_all_workflows_runs_url(
@@ -720,41 +722,44 @@
                         self.logger.error('Failed to update the configuration json of workflow')
                         return WorkflowResponse.parse_result(status=Response.Status.FAILED,
                                                              error_code=ErrorCode.USER_ERROR,
                                                              error_desc='Failed to get the workflow run id jobs',
                                                              response=response)
                     while len(result) > 0:
                         workflow_runs_list.extend(result)
+                        if not pagination:
+                            break
                         api_body_for_filter["offset"] = api_body_for_filter.get("limit")
                         response = IWUtils.ejson_deserialize(
                             self.call_api("POST", url_to_list_workflow_runs, IWUtils.get_default_header_for_v3(
                                 self.client_config['bearer_token']), data=api_body_for_filter).content)
                         result = response.get("result", [])
                 response["result"] = workflow_runs_list
                 response["message"] = initial_msg
                 return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
             else:
                 workflow_runs_list = []
                 response = IWUtils.ejson_deserialize(
                     self.call_api("GET", url_builder.get_all_workflows_runs_url_with_domain_id(
-                        self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                        self.client_config, domain_id, workflow_id) + IWUtils.get_query_params_string_from_dict(params=params), IWUtils.get_default_header_for_v3(
                         self.client_config['bearer_token'])).content)
-
                 result = response.get('result', None)
                 if result is None:
                     self.logger.error('Failed to get the list of workflow runs')
                     return WorkflowResponse.parse_result(status=Response.Status.FAILED,
                                                          error_code=ErrorCode.USER_ERROR,
                                                          error_desc='Failed to get the workflow run id jobs',
                                                          response=response)
                 if response is not None:
                     result = response.get("result", [])
                     initial_msg = response.get("message", "")
                     while len(result) > 0:
                         workflow_runs_list.extend(result)
+                        if not pagination:
+                            break
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
@@ -765,21 +770,23 @@
                 return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to get workflow details.')
             raise WorkflowError('Error occurred while trying to get workflow details.')
 
-    def get_list_of_workflow_runs_jobs(self, run_id=None, params=None):
+    def get_list_of_workflow_runs_jobs(self, run_id=None, params=None,pagination=True):
         """
          Gets List of Infoworks Data workflow runs jobs details
         :param run_id: Run id to which the workflows belongs to, if None all workflows
         :type run_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
+        :param pagination: Boolean value to determine whether to return entire result set or only a portion of result defined by 'limit' under params
+        :type pagination: Boolean
         :return: response dict
         """
         if None in {run_id}:
             self.logger.error("run_id cannot be None")
             raise Exception("run_id cannot be None")
         response = None
         try:
@@ -805,23 +812,26 @@
                                                      response=response)
 
             if response is not None:
                 result = response.get("result", [])
                 initial_msg = response.get("message", "")
                 while len(result) > 0:
                     workflow_run_jobs_list.extend(result)
+                    if not pagination:
+                        break
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
                             self.client_config['bearer_token'])).content)
                     result = response.get("result", [])
+
             response["result"] = workflow_run_jobs_list
             response["message"] = initial_msg
             return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to get jobs under workflow run.' + str(e))
```

### Comparing `infoworkssdk-4.0b3/infoworks/sdk/workflow_response.py` & `infoworkssdk-4.1/infoworks/sdk/workflow_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-4.0b3/infoworkssdk.egg-info/PKG-INFO` & `infoworkssdk-4.1/infoworkssdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 4.0b3
-Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
+Version: 4.1
+Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.x onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,23 +46,30 @@
 ```
 ## Requirements
 
 Python 3.4+ (PyPy supported)
 
 ## Usage
 
-The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value:
+The library needs to be configured with your user's refresh token key which is available in your Infoworks UI. Set refresh_token to its value.
+
+### Steps to get refresh token:
+
+https://docs.infoworks.io/infoworks-5.5.0/developer-resources/rest-api#using-refresh-token
 
 ```python
 from infoworks.sdk.client import InfoworksClientSDK
 # Your refresh token here
-refresh_token = "zThziQ7MoJJPYAha+U/+PBSTZG944F+SHBDs+m/z2qn8+m/ax8Prpzla1MHzQ5EBLzB2Bw8a+Qs9r6En5BEN2DsmUVJ6sKFb2yI2"
+protocol="https"
+host="<your infoworks hostname>"
+port="443"
+refresh_token = "<your_refresh_token>"
 # Initialise the client
 iwx_client = InfoworksClientSDK()
-iwx_client.initialize_client_with_defaults("http", "10.18.1.28", "3001", refresh_token)
+iwx_client.initialize_client_with_defaults(protocol=protocol, ip=host, port=port, refresh_token=refresh_token)
 ```
 ## Example
 
 Create Oracle Source
 ```
 src_create_response = iwx_client.create_source(source_config={
             "name": "iwx_sdk_srcname",
@@ -76,7 +83,8 @@
 ```
 
 ## Authors
 
 Nitin B.S (nitin.bs@infoworks.io)
 Abhishek Raviprasad (abhishek.raviprasad@infoworks.io)
 
+
```

### Comparing `infoworkssdk-4.0b3/infoworkssdk.egg-info/SOURCES.txt` & `infoworkssdk-4.1/infoworkssdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,23 @@
 infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
 infoworks/sdk/cicd/download_configurations/lineage.py
 infoworks/sdk/cicd/download_configurations/utils.py
 infoworks/sdk/cicd/upload_configurations/__init__.py
 infoworks/sdk/cicd/upload_configurations/cdata_source.py
 infoworks/sdk/cicd/upload_configurations/csv_source.py
 infoworks/sdk/cicd/upload_configurations/domains.py
+infoworks/sdk/cicd/upload_configurations/file_source.py
+infoworks/sdk/cicd/upload_configurations/generic_jdbc_source.py
 infoworks/sdk/cicd/upload_configurations/local_configurations.py
 infoworks/sdk/cicd/upload_configurations/misc.py
 infoworks/sdk/cicd/upload_configurations/pipeline_group.py
 infoworks/sdk/cicd/upload_configurations/pipelines.py
 infoworks/sdk/cicd/upload_configurations/rdbms_source.py
 infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+infoworks/sdk/cicd/upload_configurations/streaming_source.py
 infoworks/sdk/cicd/upload_configurations/update_configurations.py
 infoworks/sdk/cicd/upload_configurations/workflow.py
 infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
 infoworks/sdk/cicd/upload_configurations/wrappersource.py
 infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
 infoworks/sdk/ejson/__init__.py
 infoworkssdk.egg-info/PKG-INFO
```

### Comparing `infoworkssdk-4.0b3/setup.py` & `infoworkssdk-4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="infoworkssdk",
-    version="4.0.beta3",
+    version="4.1",
     author="Infoworks CE Team",
     author_email="abhishek.raviprasad@infoworks.io",
-    description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
+    description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.x onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Infoworks/InfoworksPythonSDK",
     packages=setuptools.find_packages(),
     install_requires=[
-        'requests', 'bson', 'urllib3', 'pandas', 'networkx', 'pyyaml'],
+        'requests', 'bson', 'urllib3', 'pandas', 'networkx', 'pyyaml', 'tabulate'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```


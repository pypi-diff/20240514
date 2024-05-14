# Comparing `tmp/autosubmit_api-4.0.0b6.tar.gz` & `tmp/autosubmit_api-4.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit_api-4.0.0b6.tar", last modified: Fri Apr 19 11:55:56 2024, max compression
+gzip compressed data, was "autosubmit_api-4.0.0b7.tar", last modified: Tue May 14 10:51:10 2024, max compression
```

## Comparing `autosubmit_api-4.0.0b6.tar` & `autosubmit_api-4.0.0b7.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/LICENSE
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4306 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/README.md
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/app.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/auth/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/auth/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/auth/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    43697 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_list.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/bgtask.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/scheduler.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4376 2024-04-04 11:33:45.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/status_updater.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3381 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/builders/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/basic_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/configuration_facade_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-04-09 11:09:40.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3142 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_history_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_helper_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_loader_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/pkl_organizer_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/cli.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/common/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/utils_for_testing.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/configuration_facade.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/pkl_organizer.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_factory.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_support.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3902 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_helper.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_loader.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/edge.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17188 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/test.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/tree.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/config/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/IConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/basicConfig.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/confConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/config_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/ymlConfigStrategy.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/database/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-04-09 11:09:48.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2677 2024-04-12 10:56:16.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20348 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45645 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_jobdata.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-04-11 13:47:25.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3627 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_structure.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2645 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/queries.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3491 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/tables.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3999 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_db_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    52746 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/experiment_run.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/job_data.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/experiment_history.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/internal_logging.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/logger.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/monitor/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/monitor/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/monitor/monitor.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/performance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/performance_metrics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/persistance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/experiment.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3743 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/job_package_reader.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/pkl_reader.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/statistics/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/job_stat.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/statistics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/stats_summary.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/views/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    15492 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/process_graph_drawings.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/populate.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details_db.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_running_experiments.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/test_esarchive.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4968 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/SOURCES.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/dependency_links.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/entry_points.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      729 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/requires.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/top_level.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/setup.cfg
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2188 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/setup.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/tests/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/tests/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/conftest.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/tests/custom_utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_auth.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/tests/test_bg_tasks.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_config.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20138 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/tests/test_endpoints_v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6473 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/tests/test_endpoints_v4.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/tests/test_persistance.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/LICENSE
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/README.md
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/app.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/auth/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/auth/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/auth/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    43697 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_list.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/bgtask.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/scheduler.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5243 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/status_updater.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-05-10 14:13:19.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3381 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/builders/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/basic_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/configuration_facade_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3142 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_history_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_helper_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_loader_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/pkl_organizer_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/cli.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/common/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/utils_for_testing.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/configuration_facade.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/pkl_organizer.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-05-03 14:10:04.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_factory.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_support.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3902 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_helper.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_loader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/edge.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17188 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/test.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/tree.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/config/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/IConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/basicConfig.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/confConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/config_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/ymlConfigStrategy.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/database/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2798 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20480 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45645 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_jobdata.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-04-11 13:47:25.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3627 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_structure.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2645 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/queries.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3491 2024-05-02 14:40:09.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/tables.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4016 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_db_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    52845 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/experiment_run.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/job_data.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/experiment_history.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/internal_logging.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-04-25 14:05:26.000000 autosubmit_api-4.0.0b7/autosubmit_api/logger.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/monitor/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/monitor/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-04-26 14:40:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/monitor/monitor.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/performance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/performance_metrics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/persistance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/experiment.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3743 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/job_package_reader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/pkl_reader.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/statistics/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/job_stat.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/statistics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/stats_summary.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/views/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    15492 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/process_graph_drawings.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-05-06 11:38:15.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/populate.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details_db.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_running_experiments.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/test_esarchive.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4991 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/entry_points.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      665 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/requires.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/top_level.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/setup.cfg
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2142 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/setup.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/tests/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/tests/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/tests/conftest.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/tests/custom_utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-05-10 13:22:59.000000 autosubmit_api-4.0.0b7/tests/test_auth.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/tests/test_bg_tasks.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/tests/test_config.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      773 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/tests/test_database.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20138 2024-05-13 15:01:30.000000 autosubmit_api-4.0.0b7/tests/test_endpoints_v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6473 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/tests/test_endpoints_v4.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/tests/test_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/tests/test_persistance.py
```

### Comparing `autosubmit_api-4.0.0b6/LICENSE` & `autosubmit_api-4.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/PKG-INFO` & `autosubmit_api-4.0.0b7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b6
+Version: 4.0.0b7
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
@@ -21,60 +21,55 @@
 Requires-Dist: flask_cors~=3.0.10
 Requires-Dist: bscearth.utils~=0.5.2
 Requires-Dist: pysqlite-binary
 Requires-Dist: pydotplus~=2.0.2
 Requires-Dist: portalocker~=2.6.0
 Requires-Dist: networkx~=2.6.3
 Requires-Dist: scipy~=1.7.3
-Requires-Dist: paramiko~=2.12.0
 Requires-Dist: python-dotenv
 Requires-Dist: autosubmitconfigparser~=1.0.48
 Requires-Dist: autosubmit>=3.13
 Requires-Dist: Flask-APScheduler
 Requires-Dist: gunicorn
 Requires-Dist: pydantic~=2.5.2
 Requires-Dist: SQLAlchemy~=2.0.23
 Requires-Dist: python-cas>=1.6.0
-Requires-Dist: Authlib>=1.3.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: all
 Requires-Dist: Flask~=2.2.5; extra == "all"
 Requires-Dist: pyjwt~=2.8.0; extra == "all"
 Requires-Dist: requests~=2.28.1; extra == "all"
 Requires-Dist: flask_cors~=3.0.10; extra == "all"
 Requires-Dist: bscearth.utils~=0.5.2; extra == "all"
 Requires-Dist: pysqlite-binary; extra == "all"
 Requires-Dist: pydotplus~=2.0.2; extra == "all"
 Requires-Dist: portalocker~=2.6.0; extra == "all"
 Requires-Dist: networkx~=2.6.3; extra == "all"
 Requires-Dist: scipy~=1.7.3; extra == "all"
-Requires-Dist: paramiko~=2.12.0; extra == "all"
 Requires-Dist: python-dotenv; extra == "all"
 Requires-Dist: autosubmitconfigparser~=1.0.48; extra == "all"
 Requires-Dist: autosubmit>=3.13; extra == "all"
 Requires-Dist: Flask-APScheduler; extra == "all"
 Requires-Dist: gunicorn; extra == "all"
 Requires-Dist: pydantic~=2.5.2; extra == "all"
 Requires-Dist: SQLAlchemy~=2.0.23; extra == "all"
 Requires-Dist: python-cas>=1.6.0; extra == "all"
-Requires-Dist: Authlib>=1.3.0; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 
 # Autosubmit API
 
 # Table of Contents
 
-1. [Overview](#overview) 
+1. [Overview](#overview)
 2. [Installation](#installation)
 3. [Configuration options](#configuration-options)
 4. [How to run tests](#how-to-run-tests)
-5. [Autosubmit Big Picture at BSC](#autosubmit-big-picture-at-bsc)
 
 ## Overview
 
 Autosubmit API is a package that consumes the information generated by Autosubmit and serves it as an API.
 
 Distribution: https://pypi.org/project/autosubmit-api/
 
@@ -97,27 +92,26 @@
 autosubmit_api start
 ```
 
 ## Configuration options
 
 The Autosubmit API have some configuration options that can be modified by setting their specific environment variable before starting the server:
 
-* **`PROTECTION_LEVEL`**: Default `ALL`. Possible values `ALL`, `WRITEONLY`, `NONE`.
-    * If set to `ALL`, all the endpoints will be protected by needing a valid token inside the `Authorization` header of the request.
-    * If set to `WRITEONLY`, only a subset of the endpoints will be protected.
-    * If set to `NONE`, none of the endpoints will be protected.
-* **`SECRET_KEY`**: The secret key to encode the JWT tokens from the Authorization Module. **Important to be set up on production.**
-* **`CAS_SERVER_URL`**: CAS Protocol server base URL to request a ticket and verify it. Used for `/v4` endpoints. `CAS_LOGIN_URL` and `CAS_VERIFY_URL` can be empty if this variable is set (the API will append the protocol URL subpaths).
-* **`CAS_LOGIN_URL`**: CAS Protocol URL to request a ticket. Used for `/v3` endpoints.
-* **`CAS_VERIFY_URL`**: CAS Protocol URL to verify a given ticket. Used for `/v3` endpoints.
-* **`GITHUB_OAUTH_CLIENT_ID`**: Client ID of the Github Oauth app.
-* **`GITHUB_OAUTH_CLIENT_SECRET`**: Secret key of the Github Oauth app.
-* **`GITHUB_OAUTH_WHITELIST_ORGANIZATION`**: Used to use authorization based on the membership of a Github organization.
-* **`GITHUB_OAUTH_WHITELIST_TEAM`**: Used to use authorization based on the membership of a Github team in an organization. `GITHUB_OAUTH_WHITELIST_ORGANIZATION` is required
-
+- **`PROTECTION_LEVEL`**: Default `ALL`. Possible values `ALL`, `WRITEONLY`, `NONE`.
+  - If set to `ALL`, all the endpoints will be protected by needing a valid token inside the `Authorization` header of the request.
+  - If set to `WRITEONLY`, only a subset of the endpoints will be protected.
+  - If set to `NONE`, none of the endpoints will be protected.
+- **`SECRET_KEY`**: The secret key to encode the JWT tokens from the Authorization Module. **Important to be set up on production.**
+- **`CAS_SERVER_URL`**: CAS Protocol server base URL to request a ticket and verify it. Used for `/v4` endpoints. `CAS_LOGIN_URL` and `CAS_VERIFY_URL` can be empty if this variable is set (the API will append the protocol URL subpaths).
+- **`CAS_LOGIN_URL`**: CAS Protocol URL to request a ticket. Used for `/v3` endpoints.
+- **`CAS_VERIFY_URL`**: CAS Protocol URL to verify a given ticket. Used for `/v3` endpoints.
+- **`GITHUB_OAUTH_CLIENT_ID`**: Client ID of the Github Oauth app.
+- **`GITHUB_OAUTH_CLIENT_SECRET`**: Secret key of the Github Oauth app.
+- **`GITHUB_OAUTH_WHITELIST_ORGANIZATION`**: Used to use authorization based on the membership of a Github organization.
+- **`GITHUB_OAUTH_WHITELIST_TEAM`**: Used to use authorization based on the membership of a Github team in an organization. `GITHUB_OAUTH_WHITELIST_ORGANIZATION` is required
 
 ## How to run tests
 
 ### Install pytest
 
 ```bash
 pip install -e .[test]
@@ -132,25 +126,7 @@
 ### Run tests with coverage HTML report:
 
 ```bash
 pytest --cov=autosubmit_api --cov-config=.coveragerc --cov-report=html tests/
 ```
 
 You will find the report in `htmlcov/index.html`
-
-## Autosubmit Big Picture at BSC
-
-![Autosubmit Big Picture](/docs/Total_Autosubmit_Diagram.png)
-
-In this image you can see the flow of information in the **Autosubmit environment**.
-
-* **Autosubmit**: Machines running Autosubmit.
-* **Remote Platforms**: Platforms (HPCs in most cases) to which Autosubmit connects to run jobs. 
-* **Experiment Database**: Starting from Autosubmit `3.13.0`, each experiment generates a set of databases that save important (reusable) information about it. We have the `historical database`, `graph database`, `structures database`.
-* **File System**: The file system where the experiment files are stored.
-* **Data Process Workers**: **Autosubmit API** implements a set of workers that periodically collect information from the experiments or complement that information. In the current **BSC** implementation, these workers are running no `bscesweb04` under `webadmin` user.
-* **Main Database**: **Autosubmit API** uses a centralized database to keep track of important experiment information. The **workers** fill this information. **Autosubmit** also writes into this database.
-* **Autosubmit API**: See [Autosubmit API](https://earth.bsc.es/gitlab/es/autosubmit_api). Currently, under **BSC** implementation, this API is running on `bscesweb04` under `webadmin` user. This API exposes a set of requests that **Autosubmit GUI** consumes and serves to the users through the front end.
-* **Autosubmit GUI**: This project.
-* **Authentication Server**: **BSC Central Authentication Service**.
-* **Users**: Users that access the GUI through their web browsers from any device. The current implementation requires that an user generates a token using the Authentication server once every 5 days.
-
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/__init__.py` & `autosubmit_api-4.0.0b7/autosubmit_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "4.0.0b6"
+__version__ = "4.0.0b7"
 __author__ = "Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi"
 __credits__ = "Barcelona Supercomputing Center"
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/app.py` & `autosubmit_api-4.0.0b7/autosubmit_api/app.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/auth/__init__.py` & `autosubmit_api-4.0.0b7/autosubmit_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_list.py` & `autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/bgtask.py` & `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/bgtask.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/scheduler.py` & `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/scheduler.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/status_updater.py` & `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/status_updater.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 import os
 import time
-from typing import List
+from typing import Dict, List
 
 from sqlalchemy import select
 from autosubmit_api.bgtasks.bgtask import BackgroundTaskTemplate
 from autosubmit_api.database import tables
 from autosubmit_api.database.common import (
     create_autosubmit_db_engine,
     create_as_times_db_engine,
@@ -47,14 +47,23 @@
         Get the experiments list
         """
         with create_autosubmit_db_engine().connect() as conn:
             query_result = conn.execute(tables.experiment_table.select()).all()
         return [ExperimentModel.model_validate(row._mapping) for row in query_result]
 
     @classmethod
+    def _get_current_status(cls) -> Dict[str, str]:
+        """
+        Get the current status of the experiments
+        """
+        with create_as_times_db_engine().connect() as conn:
+            query_result = conn.execute(tables.experiment_status_table.select()).all()
+        return {row.name: row.status for row in query_result}
+
+    @classmethod
     def _check_exp_running(cls, expid: str) -> bool:
         """
         Decide if the experiment is running
         """
         MAX_PKL_AGE = 600  # 10 minutes
         MAX_PKL_AGE_EXHAUSTIVE = 3600  # 1 hour
 
@@ -109,11 +118,24 @@
         Updates STATUS of experiments.
         """
         cls._clear_missing_experiments()
 
         # Read experiments table
         exp_list = cls._get_experiments()
 
+        # Read current status of all experiments
+        current_status = cls._get_current_status()
+
         # Check every experiment status & update
         for experiment in exp_list:
             is_running = cls._check_exp_running(experiment.name)
-            cls._update_experiment_status(experiment, is_running)
+            new_status = (
+                RunningStatus.RUNNING if is_running else RunningStatus.NOT_RUNNING
+            )
+            if (
+                current_status.get(experiment.name, RunningStatus.NOT_RUNNING)
+                != new_status
+            ):
+                cls.logger.info(
+                    f"[{cls.id}] Updating status of {experiment.name} to {new_status}"
+                )
+                cls._update_experiment_status(experiment, is_running)
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v3.py` & `autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v4.py` & `autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/basic_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/basic_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/configuration_facade_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/configuration_facade_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_history_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_history_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_helper_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_helper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_loader_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_loader_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/builders/pkl_organizer_builder.py` & `autosubmit_api-4.0.0b7/autosubmit_api/builders/pkl_organizer_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/cli.py` & `autosubmit_api-4.0.0b7/autosubmit_api/cli.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/common/utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/common/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/common/utils_for_testing.py` & `autosubmit_api-4.0.0b7/autosubmit_api/common/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/configuration_facade.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/configuration_facade.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/pkl_organizer.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/pkl_organizer.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/test.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_factory.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_support.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_support.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_helper.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_loader.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_loader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/edge.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/edge.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/graph.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/test.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/test.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/tree.py` & `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/tree.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/IConfigStrategy.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/IConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/__init__.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/basicConfig.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/basicConfig.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/confConfigStrategy.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/confConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/config_common.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/config_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/config/ymlConfigStrategy.py` & `autosubmit_api-4.0.0b7/autosubmit_api/config/ymlConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/__init__.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/common.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import os
 from typing import Any
-from sqlalchemy import Connection, Engine, Select, create_engine, select, text, func
+from sqlalchemy import (
+    Connection,
+    Engine,
+    NullPool,
+    Select,
+    create_engine,
+    select,
+    text,
+    func,
+)
 from autosubmit_api.builders import BaseBuilder
 from autosubmit_api.logger import logger
 from autosubmit_api.config.basicConfig import APIBasicConfig
 
 
 class AttachedDatabaseConnBuilder(BaseBuilder):
     """
     SQLite utility to build attached databases.
     """
 
     def __init__(self) -> None:
         super().__init__(False)
         APIBasicConfig.read()
-        self.engine = create_engine("sqlite://")
+        self.engine = create_engine("sqlite://", poolclass=NullPool)
         self._product = self.engine.connect()
 
     def attach_db(self, path: str, name: str):
         self._product.execute(text(f"attach database '{path}' as {name};"))
 
     def attach_autosubmit_db(self):
         autosubmit_db_path = os.path.abspath(APIBasicConfig.DB_PATH)
@@ -47,24 +56,26 @@
 
 
 def create_autosubmit_db_engine() -> Engine:
     """
     Create an engine for the autosubmit DDBB. Usually named autosubmit.db
     """
     APIBasicConfig.read()
-    return create_engine(f"sqlite:///{ os.path.abspath(APIBasicConfig.DB_PATH)}")
+    return create_engine(
+        f"sqlite:///{ os.path.abspath(APIBasicConfig.DB_PATH)}", poolclass=NullPool
+    )
 
 
 def create_as_times_db_engine() -> Engine:
     """
     Create an engine for the AS_TIMES DDBB. Usually named as_times.db
     """
     APIBasicConfig.read()
     db_path = os.path.join(APIBasicConfig.DB_DIR, APIBasicConfig.AS_TIMES_DB)
-    return create_engine(f"sqlite:///{ os.path.abspath(db_path)}")
+    return create_engine(f"sqlite:///{ os.path.abspath(db_path)}", poolclass=NullPool)
 
 
 def execute_with_limit_offset(
     statement: Select[Any], conn: Connection, limit: int = None, offset: int = None
 ):
     """
     Execute query statement adding limit and offset.
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/db_common.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/db_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,18 @@
     try:
         (conn, cursor) = open_conn()
     except DbException as e:
         Log.error(
             'Connection to database could not be established: {0}', e.message)
         return False
     if owner:
-        query = "SELECT id,name,user,created,model,branch,hpc,description FROM listexp WHERE user='{0}'".format(owner)
+        query = "SELECT id,name,user,created,model,branch,hpc,description FROM experiment e left join details d on e.id = d.exp_id WHERE user='{0}'".format(owner)
         # print(query)
     else:
-        query = "SELECT id,name,user,created,model,branch,hpc,description FROM listexp WHERE (name LIKE '" + query + \
+        query = "SELECT id,name,user,created,model,branch,hpc,description FROM experiment e left join details d on e.id = d.exp_id WHERE (name LIKE '" + query + \
             "%' OR description LIKE '%" + query + \
                 "%' OR user LIKE '%" + query + "%')"
     if exp_type and len(exp_type) > 0:
         if exp_type == "test":
             query += " AND name LIKE 't%'"
         elif exp_type == "experiment":
             query += " AND name NOT LIKE 't%'"
@@ -298,15 +298,15 @@
         return False
     try:
         (conn, cursor) = open_conn()
     except DbException as e:
         Log.error(
             'Connection to database could not be established: {0}', e.message)
         return False
-    query = "SELECT id,name,user,created,model,branch,hpc,description FROM listexp"
+    query = "SELECT id,name,user,created,model,branch,hpc,description FROM experiment e left join details d on e.id = d.exp_id"
     APIBasicConfig.read()
     # print(query)
     cursor.execute(query)
     table = cursor.fetchall()
     cursor.close()
     conn.close()
     result = list()
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/db_jobdata.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/db_jobdata.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/db_manager.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/db_structure.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/models.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/queries.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/queries.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/database/tables.py` & `autosubmit_api-4.0.0b7/autosubmit_api/database/tables.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_db_requests.py` & `autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_db_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,13 +106,14 @@
     try:
         with create_as_times_db_engine().connect() as conn:
             row = conn.execute(
                 tables.experiment_status_table.select().where(
                     tables.experiment_status_table.c.name == expid
                 )
             ).one_or_none()
+            if row:
+                return (row.name, row.status)
     except Exception as exc:
         logger.error(f"Exception while reading experiment_status for {expid}: {exc}")
         logger.error(traceback.format_exc())
-    if row:
-        return (row.name, row.status)
+
     return (expid, "NOT RUNNING")
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_requests.py` & `autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,25 @@
 from autosubmit_api.components.representations.tree.tree import TreeRepresentation
 from autosubmit_api.components.representations.graph.graph import GraphRepresentation, GroupedBy, Layout
 
 from autosubmit_api.builders.experiment_history_builder import ExperimentHistoryDirector, ExperimentHistoryBuilder
 from autosubmit_api.builders.configuration_facade_builder import ConfigurationFacadeDirector, AutosubmitConfigurationFacadeBuilder
 from autosubmit_api.builders.joblist_loader_builder import JobListLoaderBuilder, JobListLoaderDirector
 from autosubmit_api.components.jobs.job_support import JobSupport
-from typing import Dict, Any, Optional
+from typing import Dict, Any, Optional, Tuple
 import locale
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig as Autosubmit4Config
 
 APIBasicConfig.read()
 
 SAFE_TIME_LIMIT = 300
 SAFE_TIME_LIMIT_STATUS = 180
 
 
-def get_experiment_stats(expid, filter_period, filter_type):
-    # type: (str, int, str) -> Dict[str, Any]
+def get_experiment_stats(expid: str, filter_period: int, filter_type: str) -> Dict[str, Any]:
     """
     Lite version of the stats generator from Autosubmit autosubmit.py
     """
     error = False
     error_message = ""
     period_fi = ""
     period_ini = ""
@@ -147,16 +146,22 @@
             "chunk_size": 0,
             "chunk_unit": "default",
             'total_jobs': 0,
             'completed_jobs': 0,
             'db_historic_version': "NA"}
     try:
         autosubmit_config_facade = ConfigurationFacadeDirector(AutosubmitConfigurationFacadeBuilder(expid)).build_autosubmit_configuration_facade()
-        _, experiment_status = DbRequests.get_specific_experiment_status(expid)
-        result["running"] = (experiment_status == "RUNNING")
+        try:
+            _, experiment_status = DbRequests.get_specific_experiment_status(expid)
+            result["running"] = (experiment_status == "RUNNING")
+        except Exception as exc:
+            logger.warning((traceback.format_exc()))
+            logger.warning((f"Warning: Error in get_experiment_data: {exc}. Trying to get the status exhaustively."))
+            _, _, is_running, _, _ = _is_exp_running(expid)
+            result["running"] = is_running
         result["path"] = autosubmit_config_facade.experiment_path
         result["owner_id"] = autosubmit_config_facade.get_owner_id()
         result["owner"] = autosubmit_config_facade.get_owner_name()
         result["time_last_access"] = autosubmit_config_facade.get_experiment_last_access_time_as_datetime()
         result["time_last_mod"] = autosubmit_config_facade.get_experiment_last_modified_time_as_datetime()
         result["description"] = db_common.get_experiment_by_id(expid)["description"]
         result["version"] = autosubmit_config_facade.get_autosubmit_version()
@@ -177,15 +182,15 @@
             result["total_jobs"] = 0
             result["completed_jobs"] = 0
             result["db_historic_version"] = "NA"
 
     except Exception as exp:
         result["error"] = True
         result["error_message"] = str(exp)
-        print((traceback.format_exc()))
+        logger.error((traceback.format_exc()))
     return result
 
 
 def get_current_status_log_plus(expid):
     """
     Get the current status, name of current log, last time modified, and last 5 lines of the latest log of the experiment.
     Presents _is_exp_running as a JSON object.
@@ -195,21 +200,20 @@
     return {"error": error,
             "error_message": error_message,
             "is_running": is_running,
             "timediff": timediff,
             "log_path": log_path}
 
 
-def _is_exp_running(expid, time_condition=300):
+def _is_exp_running(expid: str, time_condition=300) -> Tuple[bool, str, bool, int, str]:
     """
     Tests if experiment is running
     :param expid: Experiment name
     :param time_condition: Time constraint, 120 by default. Represents max seconds before an experiment is considered as NOT RUNNING
     :return: (error (true if error is found, false otherwise), error_message, is_running (true if running, false otherwise), timediff, path_to_log)
-    :rtype: tuple (bool, string, bool, int)
     """
     is_running = False
     error = False
     error_message = ""
     timediff = 0
     definite_log_path = None
     try:
@@ -221,22 +225,21 @@
         look_old_folder = False
         current_version = None
         try:
             as_conf = AutosubmitConfigResolver(
                 expid, APIBasicConfig, ConfigParserFactory())
             as_conf.reload()
             current_version = as_conf.get_version()
-        except Exception as exp:
-            # print(exp)
-            pass
+        except Exception as exc:
+            logger.warning("Error in getting current_version: " + str(exc))
         look_old_folder = True if current_version is not None and (str(current_version).startswith(
             "3.11") or str(current_version).startswith("3.9") or str(current_version).startswith("3.12")) else False
 
-        pathlog_first = pathlog_aslog if look_old_folder == False else pathlog_tmp
-        pathlog_second = pathlog_aslog if look_old_folder == True else pathlog_tmp
+        pathlog_first = pathlog_aslog if look_old_folder is False else pathlog_tmp
+        pathlog_second = pathlog_aslog if look_old_folder is True else pathlog_tmp
         # print("Experiment {0} version {1} \nLook {2} \nLook {3}".format(
         #     expid, current_version, pathlog_first, pathlog_second))
         # print(pathlog)
         reading = os.popen(
             'ls -t ' + pathlog_first + ' | grep "_run.log"').read() if (os.path.exists(pathlog_first)) else ""
 
         #print("Length {0}".format(len(reading)))
@@ -309,16 +312,16 @@
         APIBasicConfig.read()
         tmp_path = os.path.join(
             APIBasicConfig.LOCAL_ROOT_DIR, expid, APIBasicConfig.LOCAL_TMP_DIR)
         # Try to get packages
         job_package_reader = JobPackageReader(expid)
         try:
             job_package_reader.read()
-        except:
-            logger.warning("Failed to read job_packages")
+        except Exception as exc:
+            logger.warning(f"Failed to read job_packages: {exc}")
         # Basic data
         job_running_to_seconds = dict()
         job_running_to_runtext = dict()
         jobs_in_pkl = dict()
         fakeAllJobs = list()
 
         # Read PKL
@@ -355,15 +358,14 @@
             for job_name in list(jobs_in_pkl.keys()):
                 # print(value)
                 job_info = job_running_to_seconds[job_name] if job_name in list(job_running_to_seconds.keys(
                 )) else None
                 queue_seconds = job_info.queue_time if job_info else 0
                 running_seconds = job_info.run_time if job_info else 0
                 status = job_info.status if job_info else "UNKNOWN"
-                energy = job_info.energy if job_info else 0
                 # Identifying SIM
                 name_components = job_name.split('_')
                 if "SIM" in name_components:
                     # print(name_components)
                     sim_count += 1
                     if status in ["QUEUING"]:
                         sim_q_count += 1
@@ -532,15 +534,14 @@
     # Initializing results:
     found = False
     log_file_lastmodified = ""
     timest = ""
     error = False
     error_message = ""
     logcontent = []
-    reading = ""
     APIBasicConfig.read()
     exp_paths = ExperimentPaths(expid)
     logfilepath = os.path.join(exp_paths.tmp_log_dir, logfile)
     try:
         if os.path.exists(logfilepath):
             current_stat = os.stat(logfilepath)
             timest = int(current_stat.st_mtime)
@@ -748,15 +749,14 @@
     :param expid: Name of experiment
     :type expid: String
     :return: Dictionary [Variable Name] to Value
     :rtype: Dictionary Key: String, Value: Object
     """
 
     try:
-        notransitive = False
         APIBasicConfig.read()
 
         # TODO: Encapsulate this following 2 lines or move to the parent function in app.py
         curr_exp_as_version = db_common.get_autosubmit_version(expid, log)
         main, secondary = common_utils.parse_version_number(curr_exp_as_version)
         if main and main >= 4:
             as_conf = Autosubmit4Config(expid)
@@ -808,26 +808,20 @@
         logger.error(exc)
     return {"error": error, "error_message": error_message, "expid": expid, "total": total, "counters": experiment_counters}
 
 
 # TODO: Update to current representation standards and classes
 def get_quick_view(expid):
     """ Lighter View """
-    pkl_file_name = ""
     error = False
     error_message = ""
     #quick_view = list()
     view_data = []
     quick_tree_view = deque()
-    source = JobList.get_sourcetag()
-    target = JobList.get_targettag()
-    sync = JobList.get_synctag()
-    check_mark = JobList.get_checkmark()
     jobs_in_pkl = {}
-    fakeAllJobs = []
     total_count = completed_count = failed_count = running_count = queuing_count = 0
     try:
         APIBasicConfig.read()
         exp_paths = ExperimentPaths(expid)
         path_to_logs = exp_paths.tmp_log_dir
 
         # Retrieving packages
@@ -836,16 +830,16 @@
         package_to_package_id = {}
 
         job_package_reader = JobPackageReader(expid)
         try:
             job_package_reader.read()
             job_to_package = job_package_reader.job_to_package
             package_to_package_id = job_package_reader.package_to_package_id
-        except:
-            logger.warning("Failed to read job_packages")
+        except Exception as exc:
+            logger.warning(f"Failed to read job_packages: {exc}")
         
         logger.debug(("Retrieving packages {0} seconds.".format(
             str(time.time() - now_))))
         
         # Reading PKL
         try:
             autosubmit_config_facade = ConfigurationFacadeDirector(
@@ -868,29 +862,29 @@
                 id_number = job_item.id
                 out = job_item.out_path_local
                 err = job_item.err_path_local
                 status_color = Monitor.color_status(status_code)
                 status_text = str(common_utils.Status.VALUE_TO_KEY[status_code])
                 jobs_in_pkl[job_name] = (
                     status_code, status_color, status_text, out, err, priority, id_number)
-        except Exception as exp:
+        except Exception as exc:
             raise Exception(
-                "Autosubmit API couldn't open pkl file. If you are sure that your experiment is running correctly, try again.")
+                f"Autosubmit API couldn't open pkl file. If you are sure that your experiment is running correctly, try again: {exc}")
 
         total_count = len(list(jobs_in_pkl.keys()))
 
         if len(list(jobs_in_pkl.keys())) > 0:
             for job_name in list(jobs_in_pkl.keys()):
                 status_code, status_color, status_text, out, err, priority, id_number = jobs_in_pkl[
                     job_name]
                 wrapper_tag = ""
                 wrapper_id = 0
-                wrapper_name = ""
+                # wrapper_name = ""
                 if job_name in list(job_to_package.keys()):
-                    wrapper_name = job_to_package[job_name]
+                    # wrapper_name = job_to_package[job_name]
                     wrapper_id = package_to_package_id[job_to_package[job_name]]
                     wrapper_tag = " <span class='badge' style='background-color:#94b8b8'>Wrapped " + \
                         wrapper_id + "</span>"
 
                 view_data.append({'name': job_name,
                                     'path_log': path_to_logs,
                                     'out': "/" + out,
@@ -905,16 +899,16 @@
                 if status_code in [common_utils.Status.COMPLETED, common_utils.Status.WAITING, common_utils.Status.READY]:
                     quick_tree_view.append(tree_job)
                 else:
                     quick_tree_view.appendleft(tree_job)
             # return {}
             # quick_tree_view = list(quick_tree_view)
                     
-    except Exception as exp:
-        error_message = "Exception: {0}".format(str(exp))
+    except Exception as exc:
+        error_message = "Exception: {0}".format(str(exc))
         error = True
         logger.error(error_message)
         logger.error(traceback.format_exc())
 
     return {"error": error, "error_message": error_message, "view_data": view_data, "tree_view": list(quick_tree_view), "total": total_count, "completed": completed_count, "failed": failed_count, "running": running_count, "queuing": queuing_count}
 
 
@@ -985,15 +979,15 @@
             expid, APIBasicConfig, ConfigParserFactory())
         is_as3 = isinstance(autosubmitConfig._configWrapper, confConfigStrategy)
         
         historicalDatabase = JobData.JobDataStructure(expid, APIBasicConfig)
         experimentRun = historicalDatabase.get_max_id_experiment_run()
         currentMetadata = json.loads(
             experimentRun.metadata) if experimentRun and experimentRun.metadata else None
-        currentRunId = experimentRun.run_id if experimentRun else None
+        # currentRunId = experimentRun.run_id if experimentRun else None
         # Main keys = conf, exp, jobs, platforms, proj
         # Can we ignore proj by now? Including it.
         # TODO: Define which keys should be included in the answer
         if currentMetadata:
             currentRunConfig = {
                 key: currentMetadata[key] 
                 for key in currentMetadata 
@@ -1195,15 +1189,15 @@
         status = result[0]
         abandwith = result[1]
         alatency = result[2]
         cbandwidth = result[3]
         clatency = result[4]
         DbRequests.insert_archive_status(
             status, alatency, abandwith, clatency, cbandwidth, rtime)
-    except Exception as exp:
+    except Exception:
         print((traceback.format_exc()))
         # error_message = str(exp)
 
 
 def get_last_test_archive_status():
     error = False
     error_message = ""
@@ -1221,17 +1215,17 @@
             # 90.0  as a standard
             bandwidth_warning = "Lower bandwidth than usual" if cbandwidth < (
                 abandwidth - abandwidth * 0.1) or cbandwidth < 90.0 else None
             response_warning = "Higher response times than usual" if int(
                 rtime) > 1 else None
         else:
             str_status = "OFFLINE"
-    except Exception as exp:
+    except Exception as exc:
         error = True
-        error_message = ""
+        error_message = exc
 
     return {"status": str_status,
             "error": error,
             "error_message": error_message,
             "avg_latency": alatency,
             "avg_bandwidth": abandwidth,
             "current_latency": clatency,
@@ -1243,18 +1237,18 @@
             "response_warning": response_warning,
             }
 
 def enforceLocal(log):
     try:
         try:
             locale.setlocale(locale.LC_ALL, 'en_GB.UTF-8')
-        except Exception as e:
+        except Exception:
             try:
                 locale.setlocale(locale.LC_ALL, 'C.utf8')
-            except Exception as e:
+            except Exception:
                 try:
                     locale.setlocale(locale.LC_ALL, 'en_GB')
-                except Exception as e:
+                except Exception:
                     locale.setlocale(locale.LC_ALL, 'es_ES')
-    except Exception as e:
+    except Exception:
         log.info("Locale C.utf8 is not found, using '{0}' as fallback".format("C"))
         locale.setlocale(locale.LC_ALL, 'C')
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/experiment/utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/experiment_run.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/job_data.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_manager.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_models.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/experiment_history_db_manager.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/experiment_history.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/internal_logging.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/history/utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/logger.py` & `autosubmit_api-4.0.0b7/autosubmit_api/logger.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/monitor/monitor.py` & `autosubmit_api-4.0.0b7/autosubmit_api/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/performance/performance_metrics.py` & `autosubmit_api-4.0.0b7/autosubmit_api/performance/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/performance/utils.py` & `autosubmit_api-4.0.0b7/autosubmit_api/performance/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/persistance/experiment.py` & `autosubmit_api-4.0.0b7/autosubmit_api/persistance/experiment.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/persistance/job_package_reader.py` & `autosubmit_api-4.0.0b7/autosubmit_api/persistance/job_package_reader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/persistance/pkl_reader.py` & `autosubmit_api-4.0.0b7/autosubmit_api/persistance/pkl_reader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/statistics/job_stat.py` & `autosubmit_api-4.0.0b7/autosubmit_api/statistics/job_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/statistics/statistics.py` & `autosubmit_api-4.0.0b7/autosubmit_api/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/statistics/stats_summary.py` & `autosubmit_api-4.0.0b7/autosubmit_api/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/views/v3.py` & `autosubmit_api-4.0.0b7/autosubmit_api/views/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/views/v4.py` & `autosubmit_api-4.0.0b7/autosubmit_api/views/v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/workers/business/process_graph_drawings.py` & `autosubmit_api-4.0.0b7/autosubmit_api/workers/business/process_graph_drawings.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/populate.py` & `autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/populate.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/PKG-INFO` & `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b6
+Version: 4.0.0b7
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
@@ -21,60 +21,55 @@
 Requires-Dist: flask_cors~=3.0.10
 Requires-Dist: bscearth.utils~=0.5.2
 Requires-Dist: pysqlite-binary
 Requires-Dist: pydotplus~=2.0.2
 Requires-Dist: portalocker~=2.6.0
 Requires-Dist: networkx~=2.6.3
 Requires-Dist: scipy~=1.7.3
-Requires-Dist: paramiko~=2.12.0
 Requires-Dist: python-dotenv
 Requires-Dist: autosubmitconfigparser~=1.0.48
 Requires-Dist: autosubmit>=3.13
 Requires-Dist: Flask-APScheduler
 Requires-Dist: gunicorn
 Requires-Dist: pydantic~=2.5.2
 Requires-Dist: SQLAlchemy~=2.0.23
 Requires-Dist: python-cas>=1.6.0
-Requires-Dist: Authlib>=1.3.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: all
 Requires-Dist: Flask~=2.2.5; extra == "all"
 Requires-Dist: pyjwt~=2.8.0; extra == "all"
 Requires-Dist: requests~=2.28.1; extra == "all"
 Requires-Dist: flask_cors~=3.0.10; extra == "all"
 Requires-Dist: bscearth.utils~=0.5.2; extra == "all"
 Requires-Dist: pysqlite-binary; extra == "all"
 Requires-Dist: pydotplus~=2.0.2; extra == "all"
 Requires-Dist: portalocker~=2.6.0; extra == "all"
 Requires-Dist: networkx~=2.6.3; extra == "all"
 Requires-Dist: scipy~=1.7.3; extra == "all"
-Requires-Dist: paramiko~=2.12.0; extra == "all"
 Requires-Dist: python-dotenv; extra == "all"
 Requires-Dist: autosubmitconfigparser~=1.0.48; extra == "all"
 Requires-Dist: autosubmit>=3.13; extra == "all"
 Requires-Dist: Flask-APScheduler; extra == "all"
 Requires-Dist: gunicorn; extra == "all"
 Requires-Dist: pydantic~=2.5.2; extra == "all"
 Requires-Dist: SQLAlchemy~=2.0.23; extra == "all"
 Requires-Dist: python-cas>=1.6.0; extra == "all"
-Requires-Dist: Authlib>=1.3.0; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 
 # Autosubmit API
 
 # Table of Contents
 
-1. [Overview](#overview) 
+1. [Overview](#overview)
 2. [Installation](#installation)
 3. [Configuration options](#configuration-options)
 4. [How to run tests](#how-to-run-tests)
-5. [Autosubmit Big Picture at BSC](#autosubmit-big-picture-at-bsc)
 
 ## Overview
 
 Autosubmit API is a package that consumes the information generated by Autosubmit and serves it as an API.
 
 Distribution: https://pypi.org/project/autosubmit-api/
 
@@ -97,27 +92,26 @@
 autosubmit_api start
 ```
 
 ## Configuration options
 
 The Autosubmit API have some configuration options that can be modified by setting their specific environment variable before starting the server:
 
-* **`PROTECTION_LEVEL`**: Default `ALL`. Possible values `ALL`, `WRITEONLY`, `NONE`.
-    * If set to `ALL`, all the endpoints will be protected by needing a valid token inside the `Authorization` header of the request.
-    * If set to `WRITEONLY`, only a subset of the endpoints will be protected.
-    * If set to `NONE`, none of the endpoints will be protected.
-* **`SECRET_KEY`**: The secret key to encode the JWT tokens from the Authorization Module. **Important to be set up on production.**
-* **`CAS_SERVER_URL`**: CAS Protocol server base URL to request a ticket and verify it. Used for `/v4` endpoints. `CAS_LOGIN_URL` and `CAS_VERIFY_URL` can be empty if this variable is set (the API will append the protocol URL subpaths).
-* **`CAS_LOGIN_URL`**: CAS Protocol URL to request a ticket. Used for `/v3` endpoints.
-* **`CAS_VERIFY_URL`**: CAS Protocol URL to verify a given ticket. Used for `/v3` endpoints.
-* **`GITHUB_OAUTH_CLIENT_ID`**: Client ID of the Github Oauth app.
-* **`GITHUB_OAUTH_CLIENT_SECRET`**: Secret key of the Github Oauth app.
-* **`GITHUB_OAUTH_WHITELIST_ORGANIZATION`**: Used to use authorization based on the membership of a Github organization.
-* **`GITHUB_OAUTH_WHITELIST_TEAM`**: Used to use authorization based on the membership of a Github team in an organization. `GITHUB_OAUTH_WHITELIST_ORGANIZATION` is required
-
+- **`PROTECTION_LEVEL`**: Default `ALL`. Possible values `ALL`, `WRITEONLY`, `NONE`.
+  - If set to `ALL`, all the endpoints will be protected by needing a valid token inside the `Authorization` header of the request.
+  - If set to `WRITEONLY`, only a subset of the endpoints will be protected.
+  - If set to `NONE`, none of the endpoints will be protected.
+- **`SECRET_KEY`**: The secret key to encode the JWT tokens from the Authorization Module. **Important to be set up on production.**
+- **`CAS_SERVER_URL`**: CAS Protocol server base URL to request a ticket and verify it. Used for `/v4` endpoints. `CAS_LOGIN_URL` and `CAS_VERIFY_URL` can be empty if this variable is set (the API will append the protocol URL subpaths).
+- **`CAS_LOGIN_URL`**: CAS Protocol URL to request a ticket. Used for `/v3` endpoints.
+- **`CAS_VERIFY_URL`**: CAS Protocol URL to verify a given ticket. Used for `/v3` endpoints.
+- **`GITHUB_OAUTH_CLIENT_ID`**: Client ID of the Github Oauth app.
+- **`GITHUB_OAUTH_CLIENT_SECRET`**: Secret key of the Github Oauth app.
+- **`GITHUB_OAUTH_WHITELIST_ORGANIZATION`**: Used to use authorization based on the membership of a Github organization.
+- **`GITHUB_OAUTH_WHITELIST_TEAM`**: Used to use authorization based on the membership of a Github team in an organization. `GITHUB_OAUTH_WHITELIST_ORGANIZATION` is required
 
 ## How to run tests
 
 ### Install pytest
 
 ```bash
 pip install -e .[test]
@@ -132,25 +126,7 @@
 ### Run tests with coverage HTML report:
 
 ```bash
 pytest --cov=autosubmit_api --cov-config=.coveragerc --cov-report=html tests/
 ```
 
 You will find the report in `htmlcov/index.html`
-
-## Autosubmit Big Picture at BSC
-
-![Autosubmit Big Picture](/docs/Total_Autosubmit_Diagram.png)
-
-In this image you can see the flow of information in the **Autosubmit environment**.
-
-* **Autosubmit**: Machines running Autosubmit.
-* **Remote Platforms**: Platforms (HPCs in most cases) to which Autosubmit connects to run jobs. 
-* **Experiment Database**: Starting from Autosubmit `3.13.0`, each experiment generates a set of databases that save important (reusable) information about it. We have the `historical database`, `graph database`, `structures database`.
-* **File System**: The file system where the experiment files are stored.
-* **Data Process Workers**: **Autosubmit API** implements a set of workers that periodically collect information from the experiments or complement that information. In the current **BSC** implementation, these workers are running no `bscesweb04` under `webadmin` user.
-* **Main Database**: **Autosubmit API** uses a centralized database to keep track of important experiment information. The **workers** fill this information. **Autosubmit** also writes into this database.
-* **Autosubmit API**: See [Autosubmit API](https://earth.bsc.es/gitlab/es/autosubmit_api). Currently, under **BSC** implementation, this API is running on `bscesweb04` under `webadmin` user. This API exposes a set of requests that **Autosubmit GUI** consumes and serves to the users through the front end.
-* **Autosubmit GUI**: This project.
-* **Authentication Server**: **BSC Central Authentication Service**.
-* **Users**: Users that access the GUI through their web browsers from any device. The current implementation requires that an user generates a token using the Authentication server once every 5 days.
-
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/SOURCES.txt` & `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,11 +114,12 @@
 autosubmit_api/workers/populate_details/populate.py
 tests/__init__.py
 tests/conftest.py
 tests/custom_utils.py
 tests/test_auth.py
 tests/test_bg_tasks.py
 tests/test_config.py
+tests/test_database.py
 tests/test_endpoints_v3.py
 tests/test_endpoints_v4.py
 tests/test_graph.py
 tests/test_persistance.py
```

### Comparing `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/requires.txt` & `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,45 +4,41 @@
 flask_cors~=3.0.10
 bscearth.utils~=0.5.2
 pysqlite-binary
 pydotplus~=2.0.2
 portalocker~=2.6.0
 networkx~=2.6.3
 scipy~=1.7.3
-paramiko~=2.12.0
 python-dotenv
 autosubmitconfigparser~=1.0.48
 autosubmit>=3.13
 Flask-APScheduler
 gunicorn
 pydantic~=2.5.2
 SQLAlchemy~=2.0.23
 python-cas>=1.6.0
-Authlib>=1.3.0
 
 [all]
 Flask~=2.2.5
 pyjwt~=2.8.0
 requests~=2.28.1
 flask_cors~=3.0.10
 bscearth.utils~=0.5.2
 pysqlite-binary
 pydotplus~=2.0.2
 portalocker~=2.6.0
 networkx~=2.6.3
 scipy~=1.7.3
-paramiko~=2.12.0
 python-dotenv
 autosubmitconfigparser~=1.0.48
 autosubmit>=3.13
 Flask-APScheduler
 gunicorn
 pydantic~=2.5.2
 SQLAlchemy~=2.0.23
 python-cas>=1.6.0
-Authlib>=1.3.0
 pytest
 pytest-cov
 
 [test]
 pytest
 pytest-cov
```

### Comparing `autosubmit_api-4.0.0b6/setup.py` & `autosubmit_api-4.0.0b7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,24 +26,22 @@
     "flask_cors~=3.0.10",
     "bscearth.utils~=0.5.2",
     "pysqlite-binary",
     "pydotplus~=2.0.2",
     "portalocker~=2.6.0",
     "networkx~=2.6.3",
     "scipy~=1.7.3",
-    "paramiko~=2.12.0",
     "python-dotenv",
     "autosubmitconfigparser~=1.0.48",
     "autosubmit>=3.13",
     "Flask-APScheduler",
     "gunicorn",
     "pydantic~=2.5.2",
     "SQLAlchemy~=2.0.23",
-    "python-cas>=1.6.0",
-    "Authlib>=1.3.0"
+    "python-cas>=1.6.0"
 ]
 
 # Test dependencies
 test_requires = [
     "pytest",
     "pytest-cov"
 ]
```

### Comparing `autosubmit_api-4.0.0b6/tests/conftest.py` & `autosubmit_api-4.0.0b7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_auth.py` & `autosubmit_api-4.0.0b7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_bg_tasks.py` & `autosubmit_api-4.0.0b7/tests/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_config.py` & `autosubmit_api-4.0.0b7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_endpoints_v3.py` & `autosubmit_api-4.0.0b7/tests/test_endpoints_v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_endpoints_v4.py` & `autosubmit_api-4.0.0b7/tests/test_endpoints_v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_graph.py` & `autosubmit_api-4.0.0b7/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b6/tests/test_persistance.py` & `autosubmit_api-4.0.0b7/tests/test_persistance.py`

 * *Files identical despite different names*


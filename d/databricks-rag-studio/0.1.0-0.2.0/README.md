# Comparing `tmp/databricks_rag_studio-0.1.0-py3-none-any.whl.zip` & `tmp/databricks_rag_studio-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,97 @@
-Zip file size: 71441 bytes, number of entries: 55
--rw-r--r--  2.0 unx      344 b- defN 24-Apr-12 22:41 databricks/__init__.py
--rw-r--r--  2.0 unx      493 b- defN 24-Apr-17 02:51 databricks/rag/__init__.py
--rw-r--r--  2.0 unx     4294 b- defN 24-Apr-12 22:41 databricks/rag/configs.py
--rw-r--r--  2.0 unx     1529 b- defN 24-Apr-12 22:41 databricks/rag/constants.py
--rw-r--r--  2.0 unx    25475 b- defN 24-Apr-12 22:41 databricks/rag/entities.py
--rw-r--r--  2.0 unx     7071 b- defN 24-Apr-12 22:41 databricks/rag/environments.py
--rw-r--r--  2.0 unx      141 b- defN 24-Apr-12 22:41 databricks/rag/errors.py
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-23 22:19 databricks/rag/version.py
--rw-r--r--  2.0 unx      476 b- defN 24-Apr-13 01:44 databricks/rag/evaluation/__init__.py
--rw-r--r--  2.0 unx     5377 b- defN 24-Apr-13 01:44 databricks/rag/evaluation/offline.py
--rw-r--r--  2.0 unx     4197 b- defN 24-Apr-13 01:44 databricks/rag/evaluation/online.py
--rw-r--r--  2.0 unx      493 b- defN 24-Apr-12 22:41 databricks/rag/scoring/__init__.py
--rw-r--r--  2.0 unx     3691 b- defN 24-Apr-12 22:41 databricks/rag/scoring/feedback.py
--rw-r--r--  2.0 unx    14954 b- defN 24-Apr-18 00:51 databricks/rag/scoring/langchain_tracer.py
--rw-r--r--  2.0 unx    12893 b- defN 24-Apr-23 08:04 databricks/rag/scoring/predictions.py
--rw-r--r--  2.0 unx     2771 b- defN 24-Apr-18 00:51 databricks/rag/scoring/schema_v2.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-12 22:41 databricks/rag/studio/__init__.py
--rw-r--r--  2.0 unx      392 b- defN 24-Apr-12 22:41 databricks/rag/studio/chain_logging.py
--rw-r--r--  2.0 unx     1552 b- defN 24-Apr-12 22:41 databricks/rag/studio/configs.py
--rw-r--r--  2.0 unx      440 b- defN 24-Apr-23 08:04 databricks/rag/unpacking/__init__.py
--rw-r--r--  2.0 unx    10134 b- defN 24-Apr-19 07:04 databricks/rag/unpacking/schemas.py
--rw-r--r--  2.0 unx     9564 b- defN 24-Apr-23 22:19 databricks/rag/unpacking/unpack.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-12 22:41 databricks/rag/utils/__init__.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-12 22:41 databricks/rag/utils/mlflow.py
--rw-r--r--  2.0 unx     1147 b- defN 24-Apr-12 22:41 databricks/rag/utils/tables.py
--rw-r--r--  2.0 unx     4964 b- defN 24-Apr-12 22:41 databricks/rag/utils/uc.py
--rw-r--r--  2.0 unx      789 b- defN 24-Apr-25 16:58 databricks/rag_studio/__init__.py
--rw-r--r--  2.0 unx    11378 b- defN 24-Apr-25 16:58 databricks/rag_studio/chain_logging.py
+Zip file size: 117368 bytes, number of entries: 95
+-rw-r--r--  2.0 unx      344 b- defN 24-Apr-25 04:30 databricks/__init__.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-13 22:51 databricks/version.py
+-rw-r--r--  2.0 unx      493 b- defN 24-Apr-25 04:30 databricks/rag/__init__.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Apr-25 04:30 databricks/rag/configs.py
+-rw-r--r--  2.0 unx     1529 b- defN 24-Apr-25 04:30 databricks/rag/constants.py
+-rw-r--r--  2.0 unx    25475 b- defN 24-Apr-25 04:30 databricks/rag/entities.py
+-rw-r--r--  2.0 unx     7071 b- defN 24-Apr-25 04:30 databricks/rag/environments.py
+-rw-r--r--  2.0 unx      141 b- defN 24-Apr-25 04:30 databricks/rag/errors.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-10 04:19 databricks/rag/version.py
+-rw-r--r--  2.0 unx      476 b- defN 24-Apr-25 04:30 databricks/rag/evaluation/__init__.py
+-rw-r--r--  2.0 unx     5377 b- defN 24-Apr-25 04:30 databricks/rag/evaluation/offline.py
+-rw-r--r--  2.0 unx     4197 b- defN 24-Apr-25 04:30 databricks/rag/evaluation/online.py
+-rw-r--r--  2.0 unx      493 b- defN 24-Apr-25 04:30 databricks/rag/scoring/__init__.py
+-rw-r--r--  2.0 unx     3691 b- defN 24-Apr-25 04:30 databricks/rag/scoring/feedback.py
+-rw-r--r--  2.0 unx    14954 b- defN 24-Apr-25 04:30 databricks/rag/scoring/langchain_tracer.py
+-rw-r--r--  2.0 unx    12893 b- defN 24-Apr-25 04:30 databricks/rag/scoring/predictions.py
+-rw-r--r--  2.0 unx     2771 b- defN 24-Apr-25 04:30 databricks/rag/scoring/schema_v2.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 04:30 databricks/rag/studio/__init__.py
+-rw-r--r--  2.0 unx      493 b- defN 24-May-09 04:48 databricks/rag/studio/chain_logging.py
+-rw-r--r--  2.0 unx      569 b- defN 24-May-09 04:48 databricks/rag/studio/configs.py
+-rw-r--r--  2.0 unx      440 b- defN 24-Apr-25 04:30 databricks/rag/unpacking/__init__.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-09 04:48 databricks/rag/unpacking/entities.py
+-rw-r--r--  2.0 unx     4935 b- defN 24-May-09 04:48 databricks/rag/unpacking/job.py
+-rw-r--r--  2.0 unx    10134 b- defN 24-Apr-25 04:30 databricks/rag/unpacking/schemas.py
+-rw-r--r--  2.0 unx     9571 b- defN 24-May-09 04:48 databricks/rag/unpacking/unpack.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-25 04:30 databricks/rag/utils/__init__.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-25 04:30 databricks/rag/utils/mlflow.py
+-rw-r--r--  2.0 unx     1147 b- defN 24-Apr-25 04:30 databricks/rag/utils/tables.py
+-rw-r--r--  2.0 unx     4964 b- defN 24-Apr-25 04:30 databricks/rag/utils/uc.py
+-rw-r--r--  2.0 unx       98 b- defN 24-May-02 16:35 databricks/rag_eval/__init__.py
+-rw-r--r--  2.0 unx       95 b- defN 24-Apr-25 18:01 databricks/rag_eval/_library_version.py
+-rw-r--r--  2.0 unx      556 b- defN 24-May-13 22:51 databricks/rag_eval/constants.py
+-rw-r--r--  2.0 unx     5335 b- defN 24-May-08 01:33 databricks/rag_eval/context.py
+-rw-r--r--  2.0 unx     1647 b- defN 24-May-13 22:51 databricks/rag_eval/env_vars.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 18:01 databricks/rag_eval/clients/__init__.py
+-rw-r--r--  2.0 unx     3679 b- defN 24-May-07 20:08 databricks/rag_eval/clients/databricks_api_client.py
+-rw-r--r--  2.0 unx      111 b- defN 24-May-07 03:49 databricks/rag_eval/clients/llmjudge/__init__.py
+-rw-r--r--  2.0 unx     2498 b- defN 24-May-13 22:51 databricks/rag_eval/clients/llmjudge/llm_judge_client.py
+-rw-r--r--  2.0 unx    15513 b- defN 24-May-13 22:51 databricks/rag_eval/clients/llmjudge/proto_serde.py
+-rw-r--r--  2.0 unx      726 b- defN 24-Apr-25 18:01 databricks/rag_eval/clients/llmproxy/__init__.py
+-rw-r--r--  2.0 unx     7454 b- defN 24-May-07 20:08 databricks/rag_eval/clients/llmproxy/llm_proxy_client.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 18:01 databricks/rag_eval/config/__init__.py
+-rw-r--r--  2.0 unx     9294 b- defN 24-May-13 22:51 databricks/rag_eval/config/assessment_config.py
+-rw-r--r--  2.0 unx      240 b- defN 24-May-13 22:51 databricks/rag_eval/config/constants.py
+-rw-r--r--  2.0 unx     4858 b- defN 24-May-13 22:51 databricks/rag_eval/config/evaluation_config.py
+-rw-r--r--  2.0 unx     1695 b- defN 24-May-13 22:51 databricks/rag_eval/config/example_config.py
+-rw-r--r--  2.0 unx     5757 b- defN 24-May-13 22:51 databricks/rag_eval/config/judge_config.py
+-rw-r--r--  2.0 unx       83 b- defN 24-Apr-25 18:01 databricks/rag_eval/evaluation/__init__.py
+-rw-r--r--  2.0 unx    21429 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/assessments.py
+-rw-r--r--  2.0 unx    12186 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/entities.py
+-rw-r--r--  2.0 unx     6088 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/harness.py
+-rw-r--r--  2.0 unx      511 b- defN 24-May-07 03:49 databricks/rag_eval/evaluation/metrics.py
+-rw-r--r--  2.0 unx     5149 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/models.py
+-rw-r--r--  2.0 unx     1919 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/schemas.py
+-rw-r--r--  2.0 unx     5695 b- defN 24-May-13 22:51 databricks/rag_eval/evaluation/summary.py
+-rw-r--r--  2.0 unx     7709 b- defN 24-May-08 01:33 databricks/rag_eval/evaluation/traces.py
+-rw-r--r--  2.0 unx      127 b- defN 24-Apr-25 18:01 databricks/rag_eval/judges/__init__.py
+-rw-r--r--  2.0 unx     3674 b- defN 24-May-13 22:51 databricks/rag_eval/judges/builtin_judge.py
+-rw-r--r--  2.0 unx      305 b- defN 24-Apr-25 18:01 databricks/rag_eval/judges/constants.py
+-rw-r--r--  2.0 unx     5935 b- defN 24-Apr-25 18:01 databricks/rag_eval/judges/content_relevance.py
+-rw-r--r--  2.0 unx     8456 b- defN 24-May-13 22:51 databricks/rag_eval/judges/custom_judges.py
+-rw-r--r--  2.0 unx       61 b- defN 24-May-13 22:51 databricks/rag_eval/mlflow/__init__.py
+-rw-r--r--  2.0 unx     4644 b- defN 24-May-13 22:51 databricks/rag_eval/mlflow/databricks_rag_evaluator.py
+-rw-r--r--  2.0 unx     6292 b- defN 24-May-13 22:51 databricks/rag_eval/mlflow/dataframe_wrapper.py
+-rw-r--r--  2.0 unx     1853 b- defN 24-May-13 22:51 databricks/rag_eval/mlflow/datasets.py
+-rw-r--r--  2.0 unx     5242 b- defN 24-May-13 22:51 databricks/rag_eval/mlflow/mlflow_log_metrics.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 18:01 databricks/rag_eval/utils/__init__.py
+-rw-r--r--  2.0 unx      352 b- defN 24-May-13 22:51 databricks/rag_eval/utils/collection_utils.py
+-rw-r--r--  2.0 unx      474 b- defN 24-May-13 22:51 databricks/rag_eval/utils/enum_utils.py
+-rw-r--r--  2.0 unx      355 b- defN 24-Apr-25 18:01 databricks/rag_eval/utils/prompt_utils.py
+-rw-r--r--  2.0 unx     5629 b- defN 24-Apr-25 18:01 databricks/rag_eval/utils/rate_limit.py
+-rw-r--r--  2.0 unx      824 b- defN 24-May-08 01:33 databricks/rag_eval/utils/token_count_utils.py
+-rw-r--r--  2.0 unx      977 b- defN 24-May-13 22:51 databricks/rag_eval/utils/workspace_url_resolver.py
+-rw-r--r--  2.0 unx      778 b- defN 24-Apr-30 21:13 databricks/rag_studio/__init__.py
+-rw-r--r--  2.0 unx     4778 b- defN 24-May-13 22:51 databricks/rag_studio/chain_logging.py
 -rw-r--r--  2.0 unx    11727 b- defN 24-Apr-11 16:58 databricks/rag_studio/deployments.py
--rw-r--r--  2.0 unx     1361 b- defN 24-Apr-11 16:58 databricks/rag_studio/feedback.py
+-rw-r--r--  2.0 unx     1338 b- defN 24-May-13 22:51 databricks/rag_studio/feedback.py
 -rw-r--r--  2.0 unx    19720 b- defN 24-Apr-23 15:23 databricks/rag_studio/permissions.py
--rw-r--r--  2.0 unx     6805 b- defN 24-Apr-22 16:27 databricks/rag_studio/reviews.py
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-25 17:32 databricks/rag_studio/version.py
+-rw-r--r--  2.0 unx     6805 b- defN 24-May-13 22:51 databricks/rag_studio/reviews.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 23:45 databricks/rag_studio/client/__init__.py
 -rw-r--r--  2.0 unx     4610 b- defN 24-Apr-22 16:27 databricks/rag_studio/client/rest_client.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 23:45 databricks/rag_studio/sdk_utils/__init__.py
 -rw-r--r--  2.0 unx      664 b- defN 24-Apr-04 23:45 databricks/rag_studio/sdk_utils/deployments.py
 -rw-r--r--  2.0 unx      600 b- defN 24-Apr-22 16:27 databricks/rag_studio/sdk_utils/entities.py
 -rw-r--r--  2.0 unx     1467 b- defN 24-Apr-04 23:45 databricks/rag_studio/sdk_utils/permissions_checker.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 23:45 databricks/rag_studio/utils/__init__.py
--rw-r--r--  2.0 unx     2461 b- defN 24-Apr-04 23:45 databricks/rag_studio/utils/annotations.py
 -rw-r--r--  2.0 unx      664 b- defN 24-Apr-04 23:45 databricks/rag_studio/utils/mlflow_utils.py
 -rw-r--r--  2.0 unx     1274 b- defN 24-Apr-04 23:45 databricks/rag_studio/utils/rest_utils.py
 -rw-r--r--  2.0 unx      853 b- defN 24-Apr-04 23:45 databricks/rag_studio/utils/uc.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-12 22:41 tests/evaluation/__init__.py
--rw-r--r--  2.0 unx    21379 b- defN 24-Apr-13 01:44 tests/evaluation/test_offline.py
--rw-r--r--  2.0 unx    17337 b- defN 24-Apr-13 01:44 tests/evaluation/test_online.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-13 01:44 tests/unpacking/__init__.py
--rw-r--r--  2.0 unx     1146 b- defN 24-Apr-13 01:44 tests/unpacking/eval_test_utils.py
--rw-r--r--  2.0 unx    18061 b- defN 24-Apr-19 07:04 tests/unpacking/test_unpacking.py
--rw-r--r--  2.0 unx     2413 b- defN 24-Apr-25 17:36 databricks_rag_studio-0.1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      768 b- defN 24-Apr-25 17:36 databricks_rag_studio-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 17:36 databricks_rag_studio-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-25 17:36 databricks_rag_studio-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4997 b- defN 24-Apr-25 17:36 databricks_rag_studio-0.1.0.dist-info/RECORD
-55 files, 248291 bytes uncompressed, 63349 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx     2413 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3640 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      159 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9011 b- defN 24-May-13 22:54 databricks_rag_studio-0.2.0.dist-info/RECORD
+95 files, 363368 bytes uncompressed, 102718 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: databricks/__init__.py
 Comment: 
 
+Filename: databricks/version.py
+Comment: 
+
 Filename: databricks/rag/__init__.py
 Comment: 
 
 Filename: databricks/rag/configs.py
 Comment: 
 
 Filename: databricks/rag/constants.py
@@ -54,14 +57,20 @@
 
 Filename: databricks/rag/studio/configs.py
 Comment: 
 
 Filename: databricks/rag/unpacking/__init__.py
 Comment: 
 
+Filename: databricks/rag/unpacking/entities.py
+Comment: 
+
+Filename: databricks/rag/unpacking/job.py
+Comment: 
+
 Filename: databricks/rag/unpacking/schemas.py
 Comment: 
 
 Filename: databricks/rag/unpacking/unpack.py
 Comment: 
 
 Filename: databricks/rag/utils/__init__.py
@@ -72,14 +81,146 @@
 
 Filename: databricks/rag/utils/tables.py
 Comment: 
 
 Filename: databricks/rag/utils/uc.py
 Comment: 
 
+Filename: databricks/rag_eval/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/_library_version.py
+Comment: 
+
+Filename: databricks/rag_eval/constants.py
+Comment: 
+
+Filename: databricks/rag_eval/context.py
+Comment: 
+
+Filename: databricks/rag_eval/env_vars.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/databricks_api_client.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/llmjudge/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/llmjudge/llm_judge_client.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/llmjudge/proto_serde.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/llmproxy/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/clients/llmproxy/llm_proxy_client.py
+Comment: 
+
+Filename: databricks/rag_eval/config/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/config/assessment_config.py
+Comment: 
+
+Filename: databricks/rag_eval/config/constants.py
+Comment: 
+
+Filename: databricks/rag_eval/config/evaluation_config.py
+Comment: 
+
+Filename: databricks/rag_eval/config/example_config.py
+Comment: 
+
+Filename: databricks/rag_eval/config/judge_config.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/assessments.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/entities.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/harness.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/metrics.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/models.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/schemas.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/summary.py
+Comment: 
+
+Filename: databricks/rag_eval/evaluation/traces.py
+Comment: 
+
+Filename: databricks/rag_eval/judges/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/judges/builtin_judge.py
+Comment: 
+
+Filename: databricks/rag_eval/judges/constants.py
+Comment: 
+
+Filename: databricks/rag_eval/judges/content_relevance.py
+Comment: 
+
+Filename: databricks/rag_eval/judges/custom_judges.py
+Comment: 
+
+Filename: databricks/rag_eval/mlflow/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/mlflow/databricks_rag_evaluator.py
+Comment: 
+
+Filename: databricks/rag_eval/mlflow/dataframe_wrapper.py
+Comment: 
+
+Filename: databricks/rag_eval/mlflow/datasets.py
+Comment: 
+
+Filename: databricks/rag_eval/mlflow/mlflow_log_metrics.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/__init__.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/collection_utils.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/enum_utils.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/prompt_utils.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/rate_limit.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/token_count_utils.py
+Comment: 
+
+Filename: databricks/rag_eval/utils/workspace_url_resolver.py
+Comment: 
+
 Filename: databricks/rag_studio/__init__.py
 Comment: 
 
 Filename: databricks/rag_studio/chain_logging.py
 Comment: 
 
 Filename: databricks/rag_studio/deployments.py
@@ -90,17 +231,14 @@
 
 Filename: databricks/rag_studio/permissions.py
 Comment: 
 
 Filename: databricks/rag_studio/reviews.py
 Comment: 
 
-Filename: databricks/rag_studio/version.py
-Comment: 
-
 Filename: databricks/rag_studio/client/__init__.py
 Comment: 
 
 Filename: databricks/rag_studio/client/rest_client.py
 Comment: 
 
 Filename: databricks/rag_studio/sdk_utils/__init__.py
@@ -114,53 +252,35 @@
 
 Filename: databricks/rag_studio/sdk_utils/permissions_checker.py
 Comment: 
 
 Filename: databricks/rag_studio/utils/__init__.py
 Comment: 
 
-Filename: databricks/rag_studio/utils/annotations.py
-Comment: 
-
 Filename: databricks/rag_studio/utils/mlflow_utils.py
 Comment: 
 
 Filename: databricks/rag_studio/utils/rest_utils.py
 Comment: 
 
 Filename: databricks/rag_studio/utils/uc.py
 Comment: 
 
-Filename: tests/evaluation/__init__.py
-Comment: 
-
-Filename: tests/evaluation/test_offline.py
-Comment: 
-
-Filename: tests/evaluation/test_online.py
-Comment: 
-
-Filename: tests/unpacking/__init__.py
-Comment: 
-
-Filename: tests/unpacking/eval_test_utils.py
-Comment: 
-
-Filename: tests/unpacking/test_unpacking.py
+Filename: databricks_rag_studio-0.2.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: databricks_rag_studio-0.1.0.dist-info/LICENSE.md
+Filename: databricks_rag_studio-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: databricks_rag_studio-0.1.0.dist-info/METADATA
+Filename: databricks_rag_studio-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_rag_studio-0.1.0.dist-info/WHEEL
+Filename: databricks_rag_studio-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: databricks_rag_studio-0.1.0.dist-info/top_level.txt
+Filename: databricks_rag_studio-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks_rag_studio-0.1.0.dist-info/RECORD
+Filename: databricks_rag_studio-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/rag/version.py

```diff
@@ -1,2 +1,2 @@
 # Update this when publishing a new version
-VERSION = "0.1.0"
+VERSION = "0.2.0"
```

## databricks/rag/studio/chain_logging.py

```diff
@@ -1,10 +1,12 @@
 import mlflow
+from mlflow.utils.annotations import deprecated
 
 
+@deprecated("Use `mlflow.models.set_model` instead")
 def set_chain(chain):
     """
     After defining your LangChain in a Python file or notebook, call
     set_chain() so that it can be identified later when logging the
     chain with the log_model() method.
 
     :param chain: The LangChain model instance that is defined in a
```

## databricks/rag/studio/configs.py

```diff
@@ -1,43 +1,20 @@
-import os
-import mlflow
-import yaml
+from mlflow.models import ModelConfig
 from typing import Optional
+from mlflow.utils.annotations import deprecated
 
 
+@deprecated("Use `mlflow.models.ModelConfig` instead")
 class RagConfig:
-    def __init__(self, config_path: Optional[str] = None):
-        _mlflow_rag_config_path = getattr(
-            mlflow.langchain._rag_utils, "__databricks_rag_config_path__", None
+    def __init__(
+        self,
+        config_path: Optional[str] = None,
+        *,
+        development_config: Optional[str] = None
+    ):
+        self.model_config = ModelConfig(
+            development_config=development_config or config_path,
         )
-        self.config_path = _mlflow_rag_config_path or config_path
-
-        if not self.config_path:
-            raise FileNotFoundError("Config file is None. Please provide a valid path.")
-
-        if not os.path.isfile(self.config_path):
-            raise FileNotFoundError(f"Config file '{self.config_path}' not found.")
-
-    def _read_config(self):
-        """Reads the YAML configuration file and returns its contents.
-
-        Raises:
-            FileNotFoundError: If the configuration file does not exist.
-            yaml.YAMLError: If there is an error parsing the YAML content.
-
-        Returns:
-            dict or None: The content of the YAML file as a dictionary, or None if the config path is not set.
-        """
-        with open(self.config_path, "r") as file:
-            try:
-                return yaml.safe_load(file)
-            except yaml.YAMLError as e:
-                raise yaml.YAMLError(f"Error parsing YAML file: {e}")
 
     def get(self, key):
-        """Gets the value of a top-level parameter in the configuration."""
-        config_data = self._read_config()
-
-        if config_data and key in config_data:
-            return config_data[key]
-        else:
-            raise KeyError(f"Key '{key}' not found in configuration: {config_data}.")
+        """Delegates the get method to ModelConfig."""
+        return self.model_config.get(key)
```

## databricks/rag/unpacking/unpack.py

```diff
@@ -211,25 +211,26 @@
             "all_assessments.retrieval_assessment",
         )
     )
     return assessment_logs
 
 
 def _generate_request_logs(
-    payload_df: DataFrame, contains_v2_trace: Optional[bool] = None
+    payload_df: DataFrame, trace_version: Optional[int] = None
 ) -> DataFrame:
     request_payloads = payload_df.filter(F.expr("response:choices IS NOT NULL"))
     request_payloads_v2 = request_payloads.filter(
         F.expr(f"response:databricks_output.trace['{MLFLOW_TRACE_SCHEMA_VERSION}']==2")
     )
 
-    if contains_v2_trace is None:
-        contains_v2_trace = not request_payloads_v2.isEmpty()
-
-    if contains_v2_trace:
+    # when called by streaming job, we cannot call .isEmpty()
+    # only want to call .isEmpty() if trace_version is None (when called via SDK)
+    if trace_version == 2 or (
+        trace_version is None and not request_payloads_v2.isEmpty()
+    ):
         return _generate_request_logs_v2(request_payloads_v2)
 
     return _generate_request_logs_old(request_payloads)
 
 
 def unpack_and_split_payloads(
     payload_df: DataFrame, trace_version: Optional[int] = None
@@ -243,16 +244,12 @@
 
     payloads = payload_df.filter(
         F.col("status_code") == "200"
     ).withColumn(  # Ignore error requests
         "timestamp", (F.col("timestamp_ms") / 1000).cast("timestamp")
     )
 
-    contains_v2_trace = None
-    if trace_version is not None:
-        contains_v2_trace = trace_version == 2
-
     # Split the payloads into requests and assessments based on the payload structure
-    request_logs = _generate_request_logs(payloads, contains_v2_trace)
+    request_logs = _generate_request_logs(payloads, trace_version)
     assessment_logs = _generate_assessment_logs(payloads)
 
     return request_logs, assessment_logs
```

## databricks/rag_studio/__init__.py

```diff
@@ -6,15 +6,15 @@
 )
 from databricks.rag_studio.permissions import set_permissions, get_permissions
 from databricks.rag_studio.reviews import (
     enable_trace_reviews,
     set_review_instructions,
     get_review_instructions,
 )
-from databricks.rag_studio.version import VERSION as __version__
+from databricks.version import VERSION as __version__
 from databricks.rag_studio.sdk_utils.entities import PermissionLevel
 
 __all__ = [
     "log_model",
     "deploy_model",
     "get_deployments",
     "list_deployments",
```

## databricks/rag_studio/chain_logging.py

```diff
@@ -1,125 +1,19 @@
 import mlflow
-import base64
 import os
-import re
-import yaml
-import tempfile
 from typing import Optional, Union, Dict, Any
 from contextlib import contextmanager
+from mlflow.utils.annotations import deprecated
 from mlflow.models import ModelSignature
 from mlflow.models.model import ModelInfo
 from mlflow.types import DataType
 from mlflow.types.schema import Schema, ColSpec, Object, Array, Property
-from databricks.sdk import WorkspaceClient
-from databricks.sdk.service.workspace import ExportFormat
 from databricks.rag.version import VERSION as RAG_SERVING_VERSION
 
 
-def _is_in_comment(line, start):
-    """
-    Check if the code at the index "start" of the line is in a comment.
-
-    Limitations: This function does not handle multi-line comments, and the # symbol could be in a
-    string, or otherwise not indicate a comment.
-    """
-    return "#" in line[:start]
-
-
-def _is_in_string_only(line, search_string):
-    """
-    Check is the search_string
-
-    Limitations: This function does not handle multi-line strings.
-    """
-    # Regex for matching double quotes and everything inside
-    double_quotes_regex = r"\"(\\.|[^\"])*\""
-
-    # Regex for matching single quotes and everything inside
-    single_quotes_regex = r"\'(\\.|[^\'])*\'"
-
-    # Regex for matching search_string exactly
-    search_string_regex = rf"({re.escape(search_string)})"
-
-    # Concatenate the patterns using the OR operator '|'
-    # This will matches left to right - on quotes first, search_string last
-    pattern = (
-        double_quotes_regex + r"|" + single_quotes_regex + r"|" + search_string_regex
-    )
-
-    # Iterate through all matches in the line
-    for match in re.finditer(pattern, line):
-        # If the regex matched on the search_string, we know that it did not match in quotes since
-        # that is the order. So we know that the search_string exists outside of quotes (at least once).
-        if match.group() == search_string:
-            return False
-    return True
-
-
-# TODO (ML-39713): Improve validation of unsupported code
-def _validate_code_content(content_str) -> None:
-    """
-    Validate that there isn't any code that would work in Databricks but not as exported Python file.
-    For now, this only checks for references to 'dbutils'.
-    """
-    error_message = (
-        "The file specified by 'code_path' uses 'dbutils' command which are not supported in a chain model. "
-        "To ensure your code functions correctly, remove or comment out usage of 'dbutils' command."
-    )
-
-    for line in content_str.splitlines():
-        for match in re.finditer(r"\bdbutils\b", line):
-            start = match.start()
-            if not _is_in_comment(line, start) and not _is_in_string_only(
-                line, "dbutils"
-            ):
-                raise ValueError(error_message)
-
-
-def _get_temp_file_with_content(file_name: str, content: str, content_format) -> str:
-    """
-    Write the contents to a temporary file and return the path to that file.
-
-    :param file_name: The name of the file to be created.
-    :param content: The contents to be written to the file.
-
-    :return: The string path to the file where the chain model is build.
-    """
-    # Get the temporary directory path
-    temp_dir = tempfile.gettempdir()
-
-    # Construct the full path where the temporary file will be created
-    temp_file_path = os.path.join(temp_dir, file_name)
-
-    # Create and write to the file
-    with open(temp_file_path, content_format) as tmp_file:
-        tmp_file.write(content)
-
-    return temp_file_path
-
-
-def _get_code(code_path: str) -> str:
-    """
-    Use the chain file notebook path and convert to python file.
-    Here we get the contents using workspace client, write the contents
-    to a temporary chain.py file and return the path to that file.
-
-    :param code_path: The string notebook path to the file where the chain
-                       model is build.
-
-    :return: The string python path to the file where the chain model is build.
-    """
-    w = WorkspaceClient()
-    response = w.workspace.export(path=code_path, format=ExportFormat.SOURCE)
-    decoded_content = base64.b64decode(response.content)
-    _validate_code_content(decoded_content.decode("utf-8"))
-
-    return _get_temp_file_with_content("chain.py", decoded_content, "wb")
-
-
 @contextmanager
 def _start_run_or_reuse_active_run():
     """
     Context manager that:
      - returns the active run ID, if exists
      - otherwise start a new mlflow run, and return the run id.
     """
@@ -127,53 +21,15 @@
     if active_run:
         yield active_run.info.run_id
     else:
         with mlflow.start_run() as run:
             yield run.info.run_id
 
 
-# This function serves as a monkey patch for the `_load_code_model` method
-# in the `mlflow.langchain` module. Its primary goal is to circumvent the issue of
-# Python's module caching mechanism, which by default, prevents the re-importation
-# of previously loaded modules. This is particularly problematic in contexts where
-# it's necessary to reload a module (in this case, the `chain` module) multiple times
-# within the same Python runtime environment.
-# The issue at hand arises from the desire to import the `chain` module multiple times
-# during a single runtime session. Normally, once a module is imported, it's added to
-# `sys.modules`, and subsequent import attempts retrieve the cached module rather than
-# re-importing it.
-# To address this, the function dynamically imports the `chain` module under unique,
-# dynamically generated module names. This is achieved by creating a unique name for
-# each import using a combination of the original module name and a randomly generated
-# UUID. This approach effectively bypasses the caching mechanism, as each import is
-# considered as a separate module by the Python interpreter.
-def _fix_load_code_model(code_path=None):
-    import importlib.util
-    import sys
-    import uuid
-
-    with mlflow.langchain._config_path_context(code_path):
-        module_name = "chain"
-
-        # here we are using the module_path as sys.path[0] and chain.py
-        # to import the chain module since MLflow prepends the module directory
-        # of the chain model to sys.path
-        module_path = os.path.join(sys.path[0], "chain.py")
-        try:
-            new_module_name = f"{module_name}_{uuid.uuid4().hex}"
-            spec = importlib.util.spec_from_file_location(new_module_name, module_path)
-            module = importlib.util.module_from_spec(spec)
-            sys.modules[new_module_name] = module
-            spec.loader.exec_module(module)
-        except ImportError as e:
-            raise mlflow.MlflowException("Failed to import LangChain model.") from e
-
-    return mlflow.langchain._rag_utils.__databricks_rag_chain__
-
-
+@deprecated("Use `mlflow.langchain.log_model` instead")
 def log_model(
     *,
     code_path: str,
     config: Optional[Union[str, Dict[str, Any]]] = None,
     **kwags,
 ) -> ModelInfo:
     """
@@ -221,41 +77,26 @@
         raise ValueError(f"Chain config file {config_path} does not exist")
 
     if config is not None:
         if config_path is not None:
             raise ValueError(
                 "Cannot specify both 'config' and 'config_path' arguments."
             )
-
-        if isinstance(config, str):
-            # This is a file path. Validate that it exists
-            if not os.path.exists(config):
-                raise ValueError(f"Chain config file {config} does not exist")
-            config_path = config
-        elif isinstance(config, Dict):
-            # This is a dictionary. Write it to a temporary YAML file
-            config_path = _get_temp_file_with_content(
-                "config.yml", yaml.dump(config), "w"
-            )
-        else:
-            raise ValueError(
-                f"Invalid argument type for config {config}. Must be a file path or a dictionary"
-            )
+        config_path = config
 
     if not isinstance(code_path, str):
         raise ValueError(f"Chain file {code_path} does not exist.")
 
     chain_path = os.path.abspath(code_path)
     if not os.path.exists(chain_path):
         raise ValueError(
             f"Specified chain file {code_path} resolved to full path {chain_path} does not exist."
         )
 
     with _start_run_or_reuse_active_run():
-        desired_chain_path = _get_code(chain_path)
         input_example = {
             "messages": [
                 {
                     "role": "user",
                     "content": "What is Retrieval-augmented Generation?",
                 }
             ]
@@ -284,24 +125,23 @@
                     ColSpec(name="model", type=DataType.string),
                     ColSpec(name="choices", type=DataType.string),
                     ColSpec(name="usage", type=DataType.string),
                 ]
             ),
         )
 
-        mlflow.langchain._load_code_model = _fix_load_code_model
         return mlflow.langchain.log_model(
-            lc_model=desired_chain_path,
+            lc_model=chain_path,
             artifact_path="chain",
             pip_requirements=[
-                f"mlflow=={mlflow.__version__}",
+                "mlflow>=2.12.2",
                 f"langchain=={langchain.__version__}",
                 f"langchain-core=={langchain_core.__version__}",
                 f"langchain-community=={langchain_community.__version__}",
                 f"databricks-vectorsearch=={databricks.vector_search.__version__}",
                 f"https://ml-team-public-read.s3.us-west-2.amazonaws.com/wheels/rag-serving/uqr082kj-3c87-40b1-b04c-bb1977254aa3/databricks_rag_serving-{RAG_SERVING_VERSION}-py3-none-any.whl",
             ],
             signature=signature,
             input_example=input_example,
             example_no_conversion=True,
-            code_paths=[config_path] if config_path else [],
+            model_config=config_path if config_path else None,
         )
```

## databricks/rag_studio/feedback.py

```diff
@@ -31,12 +31,12 @@
 
     with mlflow.start_run(run_name="feedback-model"):
         return log_model(
             artifact_path=_FEEDBACK_MODEL_NAME,
             signature=input_signature,
             loader_module="feedback",
             pip_requirements=[
-                f"mlflow=={mlflow.__version__}",
+                "mlflow",
             ],
             registered_model_name=feedback_uc_model_name,
             code_path=[__file__],
         )
```

## Comparing `databricks_rag_studio-0.1.0.dist-info/LICENSE.md` & `databricks_rag_studio-0.2.0.dist-info/LICENSE.md`

 * *Files identical despite different names*


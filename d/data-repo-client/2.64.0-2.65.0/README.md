# Comparing `tmp/data-repo-client-2.64.0.tar.gz` & `tmp/data-repo-client-2.65.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-akyptdri/data-repo-client-2.64.0.tar", last modified: Tue May 14 12:51:40 2024, max compression
+gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-em1k1s2i/data-repo-client-2.65.0.tar", last modified: Tue May 14 17:55:46 2024, max compression
```

## Comparing `data-repo-client-2.64.0.tar` & `data-repo-client-2.65.0.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43869 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   225812 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   470937 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   188090 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:51:40.000000 data-repo-client-2.64.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-14 12:51:31.000000 data-repo-client-2.64.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 12:51:33.000000 data-repo-client-2.64.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 12:51:32.000000 data-repo-client-2.64.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43869 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225830 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470955 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188090 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api/upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/models/workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/data_repo_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:46.000000 data-repo-client-2.65.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 17:55:36.000000 data-repo-client-2.65.0/test/test_drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 17:55:37.000000 data-repo-client-2.65.0/test/test_workspace_policy_model.py
```

### Comparing `data-repo-client-2.64.0/PKG-INFO` & `data-repo-client-2.65.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.64.0
+Version: 2.65.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.64.0/README.md` & `data-repo-client-2.65.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 2.64.0
+- Package version: 2.65.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `data-repo-client-2.64.0/data_repo_client/__init__.py` & `data-repo-client-2.65.0/data_repo_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.64.0"
+__version__ = "2.65.0"
 
 # import apis into sdk package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
 from data_repo_client.api.snapshot_access_request_api import SnapshotAccessRequestApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
```

### Comparing `data-repo-client-2.64.0/data_repo_client/api/__init__.py` & `data-repo-client-2.65.0/data_repo_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/admin_api.py` & `data-repo-client-2.65.0/data_repo_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/configs_api.py` & `data-repo-client-2.65.0/data_repo_client/api/configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/data_repository_service_api.py` & `data-repo-client-2.65.0/data_repo_client/api/data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/datasets_api.py` & `data-repo-client-2.65.0/data_repo_client/api/datasets_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,53 +656,53 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def bulk_file_results_delete(self, id, loadtag, **kwargs):  # noqa: E501
+    def bulk_file_results_delete(self, id, load_tag, **kwargs):  # noqa: E501
         """bulk_file_results_delete  # noqa: E501
 
         Delete results from the bulk file load table of the dataset. If jobId is specified, then only the results for the loadTag plus that jobId are deleted. Otherwise, all results associated with the loadTag are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.bulk_file_results_delete(id, loadtag, async_req=True)
+        >>> thread = api.bulk_file_results_delete(id, load_tag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str loadtag: a load tag (required)
+        :param str load_tag: a load tag (required)
         :param str job_id: The job id associated with the load
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.bulk_file_results_delete_with_http_info(id, loadtag, **kwargs)  # noqa: E501
+        return self.bulk_file_results_delete_with_http_info(id, load_tag, **kwargs)  # noqa: E501
 
-    def bulk_file_results_delete_with_http_info(self, id, loadtag, **kwargs):  # noqa: E501
+    def bulk_file_results_delete_with_http_info(self, id, load_tag, **kwargs):  # noqa: E501
         """bulk_file_results_delete  # noqa: E501
 
         Delete results from the bulk file load table of the dataset. If jobId is specified, then only the results for the loadTag plus that jobId are deleted. Otherwise, all results associated with the loadTag are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.bulk_file_results_delete_with_http_info(id, loadtag, async_req=True)
+        >>> thread = api.bulk_file_results_delete_with_http_info(id, load_tag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str loadtag: a load tag (required)
+        :param str load_tag: a load tag (required)
         :param str job_id: The job id associated with the load
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -714,15 +714,15 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'loadtag',
+            'load_tag',
             'job_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -738,26 +738,26 @@
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `id` when calling `bulk_file_results_delete`")  # noqa: E501
-        # verify the required parameter 'loadtag' is set
-        if self.api_client.client_side_validation and ('loadtag' not in local_var_params or  # noqa: E501
-                                                        local_var_params['loadtag'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `loadtag` when calling `bulk_file_results_delete`")  # noqa: E501
+        # verify the required parameter 'load_tag' is set
+        if self.api_client.client_side_validation and ('load_tag' not in local_var_params or  # noqa: E501
+                                                        local_var_params['load_tag'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `load_tag` when calling `bulk_file_results_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'loadtag' in local_var_params:
-            path_params['loadtag'] = local_var_params['loadtag']  # noqa: E501
+        if 'load_tag' in local_var_params:
+            path_params['loadTag'] = local_var_params['load_tag']  # noqa: E501
 
         query_params = []
         if 'job_id' in local_var_params and local_var_params['job_id'] is not None:  # noqa: E501
             query_params.append(('jobId', local_var_params['job_id']))  # noqa: E501
 
         header_params = {}
 
@@ -3477,15 +3477,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.remove_dataset_asset_specifications(id, assetid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str assetid: An asset id (required)
+        :param str assetid: An asset name (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3503,15 +3503,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.remove_dataset_asset_specifications_with_http_info(id, assetid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str assetid: An asset id (required)
+        :param str assetid: An asset name (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `data-repo-client-2.64.0/data_repo_client/api/duos_api.py` & `data-repo-client-2.65.0/data_repo_client/api/duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/jobs_api.py` & `data-repo-client-2.65.0/data_repo_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/journal_api.py` & `data-repo-client-2.65.0/data_repo_client/api/journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/profiles_api.py` & `data-repo-client-2.65.0/data_repo_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/register_api.py` & `data-repo-client-2.65.0/data_repo_client/api/register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/repository_api.py` & `data-repo-client-2.65.0/data_repo_client/api/repository_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,53 +911,53 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def bulk_file_results_delete(self, id, loadtag, **kwargs):  # noqa: E501
+    def bulk_file_results_delete(self, id, load_tag, **kwargs):  # noqa: E501
         """bulk_file_results_delete  # noqa: E501
 
         Delete results from the bulk file load table of the dataset. If jobId is specified, then only the results for the loadTag plus that jobId are deleted. Otherwise, all results associated with the loadTag are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.bulk_file_results_delete(id, loadtag, async_req=True)
+        >>> thread = api.bulk_file_results_delete(id, load_tag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str loadtag: a load tag (required)
+        :param str load_tag: a load tag (required)
         :param str job_id: The job id associated with the load
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.bulk_file_results_delete_with_http_info(id, loadtag, **kwargs)  # noqa: E501
+        return self.bulk_file_results_delete_with_http_info(id, load_tag, **kwargs)  # noqa: E501
 
-    def bulk_file_results_delete_with_http_info(self, id, loadtag, **kwargs):  # noqa: E501
+    def bulk_file_results_delete_with_http_info(self, id, load_tag, **kwargs):  # noqa: E501
         """bulk_file_results_delete  # noqa: E501
 
         Delete results from the bulk file load table of the dataset. If jobId is specified, then only the results for the loadTag plus that jobId are deleted. Otherwise, all results associated with the loadTag are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.bulk_file_results_delete_with_http_info(id, loadtag, async_req=True)
+        >>> thread = api.bulk_file_results_delete_with_http_info(id, load_tag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str loadtag: a load tag (required)
+        :param str load_tag: a load tag (required)
         :param str job_id: The job id associated with the load
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -969,15 +969,15 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'loadtag',
+            'load_tag',
             'job_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -993,26 +993,26 @@
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `id` when calling `bulk_file_results_delete`")  # noqa: E501
-        # verify the required parameter 'loadtag' is set
-        if self.api_client.client_side_validation and ('loadtag' not in local_var_params or  # noqa: E501
-                                                        local_var_params['loadtag'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `loadtag` when calling `bulk_file_results_delete`")  # noqa: E501
+        # verify the required parameter 'load_tag' is set
+        if self.api_client.client_side_validation and ('load_tag' not in local_var_params or  # noqa: E501
+                                                        local_var_params['load_tag'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `load_tag` when calling `bulk_file_results_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'loadtag' in local_var_params:
-            path_params['loadtag'] = local_var_params['loadtag']  # noqa: E501
+        if 'load_tag' in local_var_params:
+            path_params['loadTag'] = local_var_params['load_tag']  # noqa: E501
 
         query_params = []
         if 'job_id' in local_var_params and local_var_params['job_id'] is not None:  # noqa: E501
             query_params.append(('jobId', local_var_params['job_id']))  # noqa: E501
 
         header_params = {}
 
@@ -6529,15 +6529,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.remove_dataset_asset_specifications(id, assetid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str assetid: An asset id (required)
+        :param str assetid: An asset name (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -6555,15 +6555,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.remove_dataset_asset_specifications_with_http_info(id, assetid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str assetid: An asset id (required)
+        :param str assetid: An asset name (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `data-repo-client-2.64.0/data_repo_client/api/resources_api.py` & `data-repo-client-2.65.0/data_repo_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/search_api.py` & `data-repo-client-2.65.0/data_repo_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/snapshot_access_request_api.py` & `data-repo-client-2.65.0/data_repo_client/api/snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/snapshots_api.py` & `data-repo-client-2.65.0/data_repo_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/unauthenticated_api.py` & `data-repo-client-2.65.0/data_repo_client/api/unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-2.65.0/data_repo_client/api/upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/api_client.py` & `data-repo-client-2.65.0/data_repo_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.64.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.65.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-2.64.0/data_repo_client/configuration.py` & `data-repo-client-2.65.0/data_repo_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 2.64.0".\
+               "SDK Package Version: 2.65.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-2.64.0/data_repo_client/exceptions.py` & `data-repo-client-2.65.0/data_repo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/__init__.py` & `data-repo-client-2.65.0/data_repo_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/access_info_big_query_model.py` & `data-repo-client-2.65.0/data_repo_client/models/access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/access_info_big_query_model_table.py` & `data-repo-client-2.65.0/data_repo_client/models/access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/access_info_model.py` & `data-repo-client-2.65.0/data_repo_client/models/access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/access_info_parquet_model.py` & `data-repo-client-2.65.0/data_repo_client/models/access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-2.65.0/data_repo_client/models/access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/add_auth_domain_response_model.py` & `data-repo-client-2.65.0/data_repo_client/models/add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/asset_model.py` & `data-repo-client-2.65.0/data_repo_client/models/asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-2.65.0/data_repo_client/models/asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-2.65.0/data_repo_client/models/billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/billing_profile_update_model.py` & `data-repo-client-2.65.0/data_repo_client/models/billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_array_result_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_file_state.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_history_model_list.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-2.65.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/cloud_platform.py` & `data-repo-client-2.65.0/data_repo_client/models/cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_model.py` & `data-repo-client-2.65.0/data_repo_client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_double_model.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_double_model_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_int_model.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_int_model_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_model.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_model.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_model_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/column_statistics_text_value.py` & `data-repo-client-2.65.0/data_repo_client/models/column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_enable_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_fault_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_group_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_list_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-2.65.0/data_repo_client/models/config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/data_deletion_gcs_file_model.py` & `data-repo-client-2.65.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/data_deletion_json_array_model.py` & `data-repo-client-2.65.0/data_repo_client/models/data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-2.65.0/data_repo_client/models/data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/data_deletion_table_model.py` & `data-repo-client-2.65.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_data_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_patch_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_request_model_policies.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_schema_column_update_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_schema_update_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_schema_update_model_changes.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_specification_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-2.65.0/data_repo_client/models/dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/date_partition_options_model.py` & `data-repo-client-2.65.0/data_repo_client/models/date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/delete_response_model.py` & `data-repo-client-2.65.0/data_repo_client/models/delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/directory_detail_model.py` & `data-repo-client-2.65.0/data_repo_client/models/directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_access_url.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_alias_model.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_error.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_object.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_passport_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_passport_request_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,26 +56,26 @@
             self.expand = expand
         self.passports = passports
 
     @property
     def expand(self):
         """Gets the expand of this DRSPassportRequestModel.  # noqa: E501
 
-        If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains aother bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.  # noqa: E501
+        If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains other bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.  # noqa: E501
 
         :return: The expand of this DRSPassportRequestModel.  # noqa: E501
         :rtype: bool
         """
         return self._expand
 
     @expand.setter
     def expand(self, expand):
         """Sets the expand of this DRSPassportRequestModel.
 
-        If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains aother bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.  # noqa: E501
+        If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains other bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.  # noqa: E501
 
         :param expand: The expand of this DRSPassportRequestModel.  # noqa: E501
         :type: bool
         """
 
         self._expand = expand
```

### Comparing `data-repo-client-2.64.0/data_repo_client/models/drs_service_info.py` & `data-repo-client-2.65.0/data_repo_client/models/drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/duos_firecloud_group_model.py` & `data-repo-client-2.65.0/data_repo_client/models/duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-2.65.0/data_repo_client/models/duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/enumerate_billing_profile_model.py` & `data-repo-client-2.65.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/enumerate_dataset_model.py` & `data-repo-client-2.65.0/data_repo_client/models/enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/enumerate_snapshot_access_request.py` & `data-repo-client-2.65.0/data_repo_client/models/enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/enumerate_snapshot_model.py` & `data-repo-client-2.65.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/enumerate_sort_by_param.py` & `data-repo-client-2.65.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/error_model.py` & `data-repo-client-2.65.0/data_repo_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-2.65.0/data_repo_client/models/file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/file_load_model.py` & `data-repo-client-2.65.0/data_repo_client/models/file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/file_model.py` & `data-repo-client-2.65.0/data_repo_client/models/file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/file_model_type.py` & `data-repo-client-2.65.0/data_repo_client/models/file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/iam_resource_type_enum.py` & `data-repo-client-2.65.0/data_repo_client/models/iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/inaccessible_workspace_policy_model.py` & `data-repo-client-2.65.0/data_repo_client/models/inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/ingest_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-2.65.0/data_repo_client/models/ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-2.65.0/data_repo_client/models/int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/job_model.py` & `data-repo-client-2.65.0/data_repo_client/models/job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/journal_entry_model.py` & `data-repo-client-2.65.0/data_repo_client/models/journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/policy_member_request.py` & `data-repo-client-2.65.0/data_repo_client/models/policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/policy_model.py` & `data-repo-client-2.65.0/data_repo_client/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/policy_response.py` & `data-repo-client-2.65.0/data_repo_client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/query_column_statistics_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/query_data_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/relationship_model.py` & `data-repo-client-2.65.0/data_repo_client/models/relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-2.65.0/data_repo_client/models/relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/repository_configuration_model.py` & `data-repo-client-2.65.0/data_repo_client/models/repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/repository_status_model.py` & `data-repo-client-2.65.0/data_repo_client/models/repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/repository_status_model_systems.py` & `data-repo-client-2.65.0/data_repo_client/models/repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/resource_locks.py` & `data-repo-client-2.65.0/data_repo_client/models/resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/resource_policy_model.py` & `data-repo-client-2.65.0/data_repo_client/models/resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/sam_policy_model.py` & `data-repo-client-2.65.0/data_repo_client/models/sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request_response.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_access_request_status.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_cohort.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_concept.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_concepts_response.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_request.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_response.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_count_response_result.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_criteria.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_criteria_group.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_criteria.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_option.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_feature_value_group.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_option.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_parent_concept.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_item.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_option.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_option.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_option.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_request.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_builder_settings.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_ids_and_roles_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_link_duos_dataset_response.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_patch_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_preview_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_model_policies.py` & `data-repo-client-2.65.0/data_repo_client/models/upgrade_response_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,120 +14,126 @@
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotRequestModelPolicies(object):
+class UpgradeResponseModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'stewards': 'list[str]',
-        'readers': 'list[str]',
-        'discoverers': 'list[str]'
+        'upgrade_name': 'str',
+        'start_time': 'str',
+        'end_time': 'str'
     }
 
     attribute_map = {
-        'stewards': 'stewards',
-        'readers': 'readers',
-        'discoverers': 'discoverers'
+        'upgrade_name': 'upgradeName',
+        'start_time': 'startTime',
+        'end_time': 'endTime'
     }
 
-    def __init__(self, stewards=None, readers=None, discoverers=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotRequestModelPolicies - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, upgrade_name=None, start_time=None, end_time=None, local_vars_configuration=None):  # noqa: E501
+        """UpgradeResponseModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._stewards = None
-        self._readers = None
-        self._discoverers = None
+        self._upgrade_name = None
+        self._start_time = None
+        self._end_time = None
         self.discriminator = None
 
-        if stewards is not None:
-            self.stewards = stewards
-        if readers is not None:
-            self.readers = readers
-        if discoverers is not None:
-            self.discoverers = discoverers
+        if upgrade_name is not None:
+            self.upgrade_name = upgrade_name
+        if start_time is not None:
+            self.start_time = start_time
+        if end_time is not None:
+            self.end_time = end_time
 
     @property
-    def stewards(self):
-        """Gets the stewards of this SnapshotRequestModelPolicies.  # noqa: E501
+    def upgrade_name(self):
+        """Gets the upgrade_name of this UpgradeResponseModel.  # noqa: E501
 
+        Unique name for the upgrade  # noqa: E501
 
-        :return: The stewards of this SnapshotRequestModelPolicies.  # noqa: E501
-        :rtype: list[str]
+        :return: The upgrade_name of this UpgradeResponseModel.  # noqa: E501
+        :rtype: str
         """
-        return self._stewards
+        return self._upgrade_name
 
-    @stewards.setter
-    def stewards(self, stewards):
-        """Sets the stewards of this SnapshotRequestModelPolicies.
+    @upgrade_name.setter
+    def upgrade_name(self, upgrade_name):
+        """Sets the upgrade_name of this UpgradeResponseModel.
 
+        Unique name for the upgrade  # noqa: E501
 
-        :param stewards: The stewards of this SnapshotRequestModelPolicies.  # noqa: E501
-        :type: list[str]
+        :param upgrade_name: The upgrade_name of this UpgradeResponseModel.  # noqa: E501
+        :type: str
         """
 
-        self._stewards = stewards
+        self._upgrade_name = upgrade_name
 
     @property
-    def readers(self):
-        """Gets the readers of this SnapshotRequestModelPolicies.  # noqa: E501
+    def start_time(self):
+        """Gets the start_time of this UpgradeResponseModel.  # noqa: E501
 
+        Timestamp the upgrade was started  # noqa: E501
 
-        :return: The readers of this SnapshotRequestModelPolicies.  # noqa: E501
-        :rtype: list[str]
+        :return: The start_time of this UpgradeResponseModel.  # noqa: E501
+        :rtype: str
         """
-        return self._readers
+        return self._start_time
 
-    @readers.setter
-    def readers(self, readers):
-        """Sets the readers of this SnapshotRequestModelPolicies.
+    @start_time.setter
+    def start_time(self, start_time):
+        """Sets the start_time of this UpgradeResponseModel.
 
+        Timestamp the upgrade was started  # noqa: E501
 
-        :param readers: The readers of this SnapshotRequestModelPolicies.  # noqa: E501
-        :type: list[str]
+        :param start_time: The start_time of this UpgradeResponseModel.  # noqa: E501
+        :type: str
         """
 
-        self._readers = readers
+        self._start_time = start_time
 
     @property
-    def discoverers(self):
-        """Gets the discoverers of this SnapshotRequestModelPolicies.  # noqa: E501
+    def end_time(self):
+        """Gets the end_time of this UpgradeResponseModel.  # noqa: E501
 
+        Timestamp the upgrade completed  # noqa: E501
 
-        :return: The discoverers of this SnapshotRequestModelPolicies.  # noqa: E501
-        :rtype: list[str]
+        :return: The end_time of this UpgradeResponseModel.  # noqa: E501
+        :rtype: str
         """
-        return self._discoverers
+        return self._end_time
 
-    @discoverers.setter
-    def discoverers(self, discoverers):
-        """Sets the discoverers of this SnapshotRequestModelPolicies.
+    @end_time.setter
+    def end_time(self, end_time):
+        """Sets the end_time of this UpgradeResponseModel.
 
+        Timestamp the upgrade completed  # noqa: E501
 
-        :param discoverers: The discoverers of this SnapshotRequestModelPolicies.  # noqa: E501
-        :type: list[str]
+        :param end_time: The end_time of this UpgradeResponseModel.  # noqa: E501
+        :type: str
         """
 
-        self._discoverers = discoverers
+        self._end_time = end_time
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -155,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotRequestModelPolicies):
+        if not isinstance(other, UpgradeResponseModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotRequestModelPolicies):
+        if not isinstance(other, UpgradeResponseModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_row_id_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_retrieve_include_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_source_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/snapshot_summary_model.py` & `data-repo-client-2.65.0/data_repo_client/models/snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/sql_sort_direction_asc_default.py` & `data-repo-client-2.65.0/data_repo_client/models/sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/sql_sort_direction_desc_default.py` & `data-repo-client-2.65.0/data_repo_client/models/sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/storage_resource_model.py` & `data-repo-client-2.65.0/data_repo_client/models/storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/table_data_type.py` & `data-repo-client-2.65.0/data_repo_client/models/table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/table_model.py` & `data-repo-client-2.65.0/data_repo_client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/tag_count.py` & `data-repo-client-2.65.0/data_repo_client/models/tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/tag_count_result_model.py` & `data-repo-client-2.65.0/data_repo_client/models/tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-2.65.0/data_repo_client/models/tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-2.65.0/data_repo_client/models/transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/transaction_create_model.py` & `data-repo-client-2.65.0/data_repo_client/models/transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/transaction_model.py` & `data-repo-client-2.65.0/data_repo_client/models/transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/unlock_resource_request.py` & `data-repo-client-2.65.0/data_repo_client/models/unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-2.65.0/data_repo_client/models/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/user_status_info.py` & `data-repo-client-2.65.0/data_repo_client/models/user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/models/workspace_policy_model.py` & `data-repo-client-2.65.0/data_repo_client/models/workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client/rest.py` & `data-repo-client-2.65.0/data_repo_client/rest.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/data_repo_client.egg-info/PKG-INFO` & `data-repo-client-2.65.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.64.0
+Version: 2.65.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.64.0/data_repo_client.egg-info/SOURCES.txt` & `data-repo-client-2.65.0/data_repo_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/setup.py` & `data-repo-client-2.65.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "data-repo-client"
-VERSION = "2.64.0"
+VERSION = "2.65.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `data-repo-client-2.64.0/test/test_access_info_big_query_model.py` & `data-repo-client-2.65.0/test/test_access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_access_info_big_query_model_table.py` & `data-repo-client-2.65.0/test/test_access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_access_info_model.py` & `data-repo-client-2.65.0/test/test_access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_access_info_parquet_model.py` & `data-repo-client-2.65.0/test/test_access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_access_info_parquet_model_table.py` & `data-repo-client-2.65.0/test/test_access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_add_auth_domain_response_model.py` & `data-repo-client-2.65.0/test/test_add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_admin_api.py` & `data-repo-client-2.65.0/test/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_asset_model.py` & `data-repo-client-2.65.0/test/test_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_asset_table_model.py` & `data-repo-client-2.65.0/test/test_asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_billing_profile_model.py` & `data-repo-client-2.65.0/test/test_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_billing_profile_request_model.py` & `data-repo-client-2.65.0/test/test_billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_billing_profile_update_model.py` & `data-repo-client-2.65.0/test/test_billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_array_request_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_array_result_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_file_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_file_result_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_file_state.py` & `data-repo-client-2.65.0/test/test_bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_history_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_history_model_list.py` & `data-repo-client-2.65.0/test/test_bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_request_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_bulk_load_result_model.py` & `data-repo-client-2.65.0/test/test_bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_cloud_platform.py` & `data-repo-client-2.65.0/test/test_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_model.py` & `data-repo-client-2.65.0/test/test_column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_double_model.py` & `data-repo-client-2.65.0/test/test_column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_double_model_all_of.py` & `data-repo-client-2.65.0/test/test_column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_int_model.py` & `data-repo-client-2.65.0/test/test_column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_int_model_all_of.py` & `data-repo-client-2.65.0/test/test_column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_model.py` & `data-repo-client-2.65.0/test/test_column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_text_model.py` & `data-repo-client-2.65.0/test/test_column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_text_model_all_of.py` & `data-repo-client-2.65.0/test/test_column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_column_statistics_text_value.py` & `data-repo-client-2.65.0/test/test_column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_enable_model.py` & `data-repo-client-2.65.0/test/test_config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_fault_counted_model.py` & `data-repo-client-2.65.0/test/test_config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_fault_model.py` & `data-repo-client-2.65.0/test/test_config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_group_model.py` & `data-repo-client-2.65.0/test/test_config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_list_model.py` & `data-repo-client-2.65.0/test/test_config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_model.py` & `data-repo-client-2.65.0/test/test_config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_config_parameter_model.py` & `data-repo-client-2.65.0/test/test_config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_configs_api.py` & `data-repo-client-2.65.0/test/test_configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_data_deletion_gcs_file_model.py` & `data-repo-client-2.65.0/test/test_data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_data_deletion_json_array_model.py` & `data-repo-client-2.65.0/test/test_data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_data_deletion_request.py` & `data-repo-client-2.65.0/test/test_data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_data_deletion_table_model.py` & `data-repo-client-2.65.0/test/test_data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_data_repository_service_api.py` & `data-repo-client-2.65.0/test/test_data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_data_model.py` & `data-repo-client-2.65.0/test/test_dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_model.py` & `data-repo-client-2.65.0/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_patch_request_model.py` & `data-repo-client-2.65.0/test/test_dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_request_access_include_model.py` & `data-repo-client-2.65.0/test/test_dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_request_model.py` & `data-repo-client-2.65.0/test/test_dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_request_model_policies.py` & `data-repo-client-2.65.0/test/test_dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_schema_column_update_model.py` & `data-repo-client-2.65.0/test/test_dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_schema_update_model.py` & `data-repo-client-2.65.0/test/test_dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_schema_update_model_changes.py` & `data-repo-client-2.65.0/test/test_dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_specification_model.py` & `data-repo-client-2.65.0/test/test_dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_dataset_summary_model.py` & `data-repo-client-2.65.0/test/test_dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_datasets_api.py` & `data-repo-client-2.65.0/test/test_datasets_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_date_partition_options_model.py` & `data-repo-client-2.65.0/test/test_date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_delete_response_model.py` & `data-repo-client-2.65.0/test/test_delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_directory_detail_model.py` & `data-repo-client-2.65.0/test/test_directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_access_method.py` & `data-repo-client-2.65.0/test/test_drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_access_url.py` & `data-repo-client-2.65.0/test/test_drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_alias_model.py` & `data-repo-client-2.65.0/test/test_drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_authorizations.py` & `data-repo-client-2.65.0/test/test_drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_checksum.py` & `data-repo-client-2.65.0/test/test_drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_contents_object.py` & `data-repo-client-2.65.0/test/test_drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_error.py` & `data-repo-client-2.65.0/test/test_drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_object.py` & `data-repo-client-2.65.0/test/test_drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_passport_request_model.py` & `data-repo-client-2.65.0/test/test_drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_drs_service_info.py` & `data-repo-client-2.65.0/test/test_drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_duos_api.py` & `data-repo-client-2.65.0/test/test_duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_duos_firecloud_group_model.py` & `data-repo-client-2.65.0/test/test_duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_duos_firecloud_groups_sync_response.py` & `data-repo-client-2.65.0/test/test_duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_enumerate_billing_profile_model.py` & `data-repo-client-2.65.0/test/test_enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_enumerate_dataset_model.py` & `data-repo-client-2.65.0/test/test_enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_enumerate_snapshot_access_request.py` & `data-repo-client-2.65.0/test/test_enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-2.65.0/test/test_enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_enumerate_sort_by_param.py` & `data-repo-client-2.65.0/test/test_enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_error_model.py` & `data-repo-client-2.65.0/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_file_detail_model.py` & `data-repo-client-2.65.0/test/test_file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_file_load_model.py` & `data-repo-client-2.65.0/test/test_file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_file_model.py` & `data-repo-client-2.65.0/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_file_model_type.py` & `data-repo-client-2.65.0/test/test_file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_iam_resource_type_enum.py` & `data-repo-client-2.65.0/test/test_iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_inaccessible_workspace_policy_model.py` & `data-repo-client-2.65.0/test/test_inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_ingest_request_model.py` & `data-repo-client-2.65.0/test/test_ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_ingest_response_model.py` & `data-repo-client-2.65.0/test/test_ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_int_partition_options_model.py` & `data-repo-client-2.65.0/test/test_int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_job_model.py` & `data-repo-client-2.65.0/test/test_job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_jobs_api.py` & `data-repo-client-2.65.0/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_journal_api.py` & `data-repo-client-2.65.0/test/test_journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_journal_entry_model.py` & `data-repo-client-2.65.0/test/test_journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_policy_member_request.py` & `data-repo-client-2.65.0/test/test_policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_policy_model.py` & `data-repo-client-2.65.0/test/test_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_policy_response.py` & `data-repo-client-2.65.0/test/test_policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_profiles_api.py` & `data-repo-client-2.65.0/test/test_profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_query_column_statistics_request_model.py` & `data-repo-client-2.65.0/test/test_query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_query_data_request_model.py` & `data-repo-client-2.65.0/test/test_query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_register_api.py` & `data-repo-client-2.65.0/test/test_register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_relationship_model.py` & `data-repo-client-2.65.0/test/test_relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_relationship_term_model.py` & `data-repo-client-2.65.0/test/test_relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_repository_api.py` & `data-repo-client-2.65.0/test/test_repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_repository_configuration_model.py` & `data-repo-client-2.65.0/test/test_repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_repository_status_model.py` & `data-repo-client-2.65.0/test/test_repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_repository_status_model_systems.py` & `data-repo-client-2.65.0/test/test_repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_resource_locks.py` & `data-repo-client-2.65.0/test/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_resource_policy_model.py` & `data-repo-client-2.65.0/test/test_resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_resources_api.py` & `data-repo-client-2.65.0/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_sam_policy_model.py` & `data-repo-client-2.65.0/test/test_sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_search_api.py` & `data-repo-client-2.65.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_access_request.py` & `data-repo-client-2.65.0/test/test_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_access_request_api.py` & `data-repo-client-2.65.0/test/test_snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_access_request_response.py` & `data-repo-client-2.65.0/test/test_snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_access_request_status.py` & `data-repo-client-2.65.0/test/test_snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_cohort.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_concept.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_concepts_response.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_count_request.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_count_response.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_count_response_result.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_criteria.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_criteria_group.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_domain_criteria.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_domain_option.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_feature_value_group.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_option.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_parent_concept.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_item.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_option.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_option.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_option.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_request.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_builder_settings.py` & `data-repo-client-2.65.0/test/test_snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model_format.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.65.0/test/test_snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_ids_and_roles_model.py` & `data-repo-client-2.65.0/test/test_snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_link_duos_dataset_response.py` & `data-repo-client-2.65.0/test/test_snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_model.py` & `data-repo-client-2.65.0/test/test_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_patch_request_model.py` & `data-repo-client-2.65.0/test/test_snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_preview_model.py` & `data-repo-client-2.65.0/test/test_snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_asset_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_contents_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                         '0'
                         ], 
                     readers = [
                         '0'
                         ], 
                     discoverers = [
                         '0'
+                        ], 
+                    aggregate_data_readers = [
+                        '0'
                         ], ), 
                 global_file_ids = True, 
                 compact_id_prefix = 'drs.42', 
                 tags = [
                     'a-resource-tag'
                     ]
             )
```

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_model_policies.py` & `data-repo-client-2.65.0/test/test_snapshot_request_model_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
                     '0'
                     ], 
                 readers = [
                     '0'
                     ], 
                 discoverers = [
                     '0'
+                    ], 
+                aggregate_data_readers = [
+                    '0'
                     ]
             )
         else :
             return SnapshotRequestModelPolicies(
         )
 
     def testSnapshotRequestModelPolicies(self):
```

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_query_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_request_row_id_table_model.py` & `data-repo-client-2.65.0/test/test_snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_retrieve_include_model.py` & `data-repo-client-2.65.0/test/test_snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_source_model.py` & `data-repo-client-2.65.0/test/test_snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshot_summary_model.py` & `data-repo-client-2.65.0/test/test_snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_snapshots_api.py` & `data-repo-client-2.65.0/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_sql_sort_direction_asc_default.py` & `data-repo-client-2.65.0/test/test_sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_sql_sort_direction_desc_default.py` & `data-repo-client-2.65.0/test/test_sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_storage_resource_model.py` & `data-repo-client-2.65.0/test/test_storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_table_data_type.py` & `data-repo-client-2.65.0/test/test_table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_table_model.py` & `data-repo-client-2.65.0/test/test_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_tag_count.py` & `data-repo-client-2.65.0/test/test_tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_tag_count_result_model.py` & `data-repo-client-2.65.0/test/test_tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_tag_update_request_model.py` & `data-repo-client-2.65.0/test/test_tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_transaction_close_model.py` & `data-repo-client-2.65.0/test/test_transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_transaction_create_model.py` & `data-repo-client-2.65.0/test/test_transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_transaction_model.py` & `data-repo-client-2.65.0/test/test_transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_unauthenticated_api.py` & `data-repo-client-2.65.0/test/test_unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_unlock_resource_request.py` & `data-repo-client-2.65.0/test/test_unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_upgrade_api.py` & `data-repo-client-2.65.0/test/test_upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_upgrade_model.py` & `data-repo-client-2.65.0/test/test_upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_upgrade_response_model.py` & `data-repo-client-2.65.0/test/test_upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_user_status_info.py` & `data-repo-client-2.65.0/test/test_user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.64.0/test/test_workspace_policy_model.py` & `data-repo-client-2.65.0/test/test_workspace_policy_model.py`

 * *Files identical despite different names*


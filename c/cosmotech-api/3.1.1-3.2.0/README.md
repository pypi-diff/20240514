# Comparing `tmp/cosmotech-api-3.1.1.tar.gz` & `tmp/cosmotech_api-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-api-3.1.1.tar", last modified: Wed Mar 13 15:45:14 2024, max compression
+gzip compressed data, was "cosmotech_api-3.2.0.tar", last modified: Tue May 14 14:37:53 2024, max compression
```

## Comparing `cosmotech-api-3.1.1.tar` & `cosmotech_api-3.2.0.tar`

### file list

```diff
@@ -1,394 +1,402 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.413602 cosmotech-api-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-13 15:45:14.413602 cosmotech-api-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46752 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.345601 cosmotech-api-3.1.1/cosmotech_api/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.353601 cosmotech-api-3.1.1/cosmotech_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24393 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   175241 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    88435 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/organization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30098 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    87664 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/runner_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   130009 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77626 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/scenariorunresult_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   124080 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/solution_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    79596 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46554 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48786 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/validator_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   116644 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api/workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37644 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/api_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.353601 cosmotech-api-3.1.1/cosmotech_api/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.373602 cosmotech-api-3.1.1/cosmotech_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11689 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/file_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/file_upload_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    19619 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/runner_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14594 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/solution_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/solution_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/solution_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/sub_dataset_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/user_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/validator_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    20329 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model/workspace_web_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    82062 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.393602 cosmotech-api-3.1.1/cosmotech_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/file_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/file_upload_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/organization_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_parent_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_root_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/runner_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/solution_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/solution_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/solution_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/sub_dataset_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/validator_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/models/workspace_web_app.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/cosmotech_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.413602 cosmotech-api-3.1.1/cosmotech_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-13 15:45:14.000000 cosmotech-api-3.1.1/cosmotech_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-03-13 15:45:14.000000 cosmotech-api-3.1.1/cosmotech_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:45:14.000000 cosmotech-api-3.1.1/cosmotech_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-13 15:45:14.000000 cosmotech-api-3.1.1/cosmotech_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-13 15:45:14.000000 cosmotech-api-3.1.1/cosmotech_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-13 15:45:14.413602 cosmotech-api-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:45:14.413602 cosmotech-api-3.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_twin_graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_dataset_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_file_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_file_upload_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_graph_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_parent_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_root_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_runner_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_resource_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_scenariorunresult_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_solution_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_solution_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_solution_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_solution_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_sub_dataset_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twin_graph_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twin_graph_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_user_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_validator_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-13 15:45:10.000000 cosmotech-api-3.1.1/test/test_workspace_web_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.347987 cosmotech_api-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 14:37:53.347987 cosmotech_api-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.279987 cosmotech_api-3.2.0/cosmotech_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.283987 cosmotech_api-3.2.0/cosmotech_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51476 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   373272 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189252 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89686 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   185420 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   285588 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170691 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29237 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/scenariorunresult_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   264564 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173284 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46554 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102393 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   248262 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api/workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25763 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/api_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.283987 cosmotech_api-3.2.0/cosmotech_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.303987 cosmotech_api-3.2.0/cosmotech_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11689 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/file_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/file_upload_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19619 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/runner_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14594 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/solution_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/solution_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/solution_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/sub_dataset_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20329 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model/workspace_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82062 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.323987 cosmotech_api-3.2.0/cosmotech_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/file_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/file_upload_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_data_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_parent_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_root_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/runner_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/send_run_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/solution_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/solution_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/solution_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/sub_dataset_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/models/workspace_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/cosmotech_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.343987 cosmotech_api-3.2.0/cosmotech_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 14:37:53.000000 cosmotech_api-3.2.0/cosmotech_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-05-14 14:37:53.000000 cosmotech_api-3.2.0/cosmotech_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:37:53.000000 cosmotech_api-3.2.0/cosmotech_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 14:37:53.000000 cosmotech_api-3.2.0/cosmotech_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 14:37:53.000000 cosmotech_api-3.2.0/cosmotech_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 14:37:53.347987 cosmotech_api-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:37:53.343987 cosmotech_api-3.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_twin_graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_dataset_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_file_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_file_upload_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_data_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_parent_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_root_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_runner_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_resource_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_scenariorunresult_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_send_run_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_solution_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_solution_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_solution_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_sub_dataset_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 14:37:49.000000 cosmotech_api-3.2.0/test/test_workspace_web_app.py
```

### Comparing `cosmotech-api-3.1.1/LICENSE` & `cosmotech_api-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/README.md` & `cosmotech_api-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # cosmotech-api
 Cosmo Tech Platform API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 3.1.1
+- API version: 3.1.1-SNAPSHOT
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://github.com/Cosmo-Tech/cosmotech-api](https://github.com/Cosmo-Tech/cosmotech-api)
 
 ## Requirements.
 
-Python >=3.6
+Python 3.7+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
@@ -37,56 +37,57 @@
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
 import cosmotech_api
 ```
 
+### Tests
+
+Execute `pytest` to run the tests.
+
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import time
 import cosmotech_api
+from cosmotech_api.rest import ApiException
 from pprint import pprint
-from cosmotech_api.api import connector_api
-from cosmotech_api.model.connector import Connector
+
 # Defining the host is optional and defaults to https://dev.api.cosmotech.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = cosmotech_api.Configuration(
     host = "https://dev.api.cosmotech.com"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
-# Configure OAuth2 access token for authorization: oAuth2AuthCode
-configuration = cosmotech_api.Configuration(
-    host = "https://dev.api.cosmotech.com"
-)
-configuration.access_token = 'YOUR_ACCESS_TOKEN'
+configuration.access_token = os.environ["ACCESS_TOKEN"]
 
 
 # Enter a context with an instance of the API client
 with cosmotech_api.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = connector_api.ConnectorApi(api_client)
-    page = 1 # int | page number to query (optional)
-size = 1 # int | amount of result by page (optional)
+    api_instance = cosmotech_api.ConnectorApi(api_client)
+    page = 56 # int | page number to query (optional)
+    size = 56 # int | amount of result by page (optional)
 
     try:
         # List all Connectors
         api_response = api_instance.find_all_connectors(page=page, size=size)
+        print("The response of ConnectorApi->find_all_connectors:\n")
         pprint(api_response)
-    except cosmotech_api.ApiException as e:
+    except ApiException as e:
         print("Exception when calling ConnectorApi->find_all_connectors: %s\n" % e)
+
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://dev.api.cosmotech.com*
 
 Class | Method | HTTP request | Description
@@ -145,14 +146,16 @@
 *OrganizationApi* | [**update_storage_by_organization_id**](docs/OrganizationApi.md#update_storage_by_organization_id) | **PATCH** /organizations/{organization_id}/services/storage | Update storage configuration for the Organization specified
 *OrganizationApi* | [**update_tenant_credentials_by_organization_id**](docs/OrganizationApi.md#update_tenant_credentials_by_organization_id) | **PATCH** /organizations/{organization_id}/services/tenantCredentials | Update tenant credentials for the Organization specified
 *RunApi* | [**delete_run**](docs/RunApi.md#delete_run) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id} | Delete a run
 *RunApi* | [**get_run**](docs/RunApi.md#get_run) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id} | Get the details of a run
 *RunApi* | [**get_run_logs**](docs/RunApi.md#get_run_logs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id}/logs | get the logs for the Run
 *RunApi* | [**get_run_status**](docs/RunApi.md#get_run_status) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id}/status | get the status for the Run
 *RunApi* | [**list_runs**](docs/RunApi.md#list_runs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs | get the list of Runs for the Runner
+*RunApi* | [**query_run_data**](docs/RunApi.md#query_run_data) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id}/data/query | query the run data
+*RunApi* | [**send_run_data**](docs/RunApi.md#send_run_data) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/runs/{run_id}/data/send | Send data associated to a run
 *RunnerApi* | [**add_runner_access_control**](docs/RunnerApi.md#add_runner_access_control) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/security/access | Add a control access to the Runner
 *RunnerApi* | [**create_runner**](docs/RunnerApi.md#create_runner) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/runners | Create a new Runner
 *RunnerApi* | [**delete_runner**](docs/RunnerApi.md#delete_runner) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id} | Delete a runner
 *RunnerApi* | [**get_runner**](docs/RunnerApi.md#get_runner) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id} | Get the details of an runner
 *RunnerApi* | [**get_runner_access_control**](docs/RunnerApi.md#get_runner_access_control) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/security/access/{identity_id} | Get a control access for the Runner
 *RunnerApi* | [**get_runner_permissions**](docs/RunnerApi.md#get_runner_permissions) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/permissions/{role} | Get the Runner permission by given role
 *RunnerApi* | [**get_runner_security**](docs/RunnerApi.md#get_runner_security) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/runners/{runner_id}/security | Get the Runner security information
@@ -196,16 +199,14 @@
 *ScenariorunApi* | [**get_scenario_run_status**](docs/ScenariorunApi.md#get_scenario_run_status) | **GET** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/status | get the status for the ScenarioRun
 *ScenariorunApi* | [**get_scenario_runs**](docs/ScenariorunApi.md#get_scenario_runs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/scenarioruns | get the list of ScenarioRuns for the Scenario
 *ScenariorunApi* | [**get_workspace_scenario_runs**](docs/ScenariorunApi.md#get_workspace_scenario_runs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarioruns | get the list of ScenarioRuns for the Workspace
 *ScenariorunApi* | [**run_scenario**](docs/ScenariorunApi.md#run_scenario) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/run | run a ScenarioRun for the Scenario
 *ScenariorunApi* | [**search_scenario_runs**](docs/ScenariorunApi.md#search_scenario_runs) | **POST** /organizations/{organization_id}/scenarioruns/search | Search ScenarioRuns
 *ScenariorunApi* | [**start_scenario_run_containers**](docs/ScenariorunApi.md#start_scenario_run_containers) | **POST** /organizations/{organization_id}/scenarioruns/startcontainers | Start a new scenariorun with raw containers definition
 *ScenariorunApi* | [**stop_scenario_run**](docs/ScenariorunApi.md#stop_scenario_run) | **POST** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/stop | stop a ScenarioRun for the Scenario
-*ScenariorunresultApi* | [**get_scenario_run_result**](docs/ScenariorunresultApi.md#get_scenario_run_result) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/scenarioruns/{scenariorun_id}/probes/{probe_id} | Get a ScenarioRunResult in the Organization
-*ScenariorunresultApi* | [**send_scenario_run_result**](docs/ScenariorunresultApi.md#send_scenario_run_result) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/scenarioruns/{scenariorun_id}/probes/{probe_id} | Create a new ScenarioRunResult in the Organization
 *SolutionApi* | [**add_or_replace_parameter_groups**](docs/SolutionApi.md#add_or_replace_parameter_groups) | **POST** /organizations/{organization_id}/solutions/{solution_id}/parameterGroups | Add Parameter Groups. Any item with the same ID will be overwritten
 *SolutionApi* | [**add_or_replace_parameters**](docs/SolutionApi.md#add_or_replace_parameters) | **POST** /organizations/{organization_id}/solutions/{solution_id}/parameters | Add Parameters. Any item with the same ID will be overwritten
 *SolutionApi* | [**add_or_replace_run_templates**](docs/SolutionApi.md#add_or_replace_run_templates) | **POST** /organizations/{organization_id}/solutions/{solution_id}/runTemplates | Add Run Templates. Any item with the same ID will be overwritten
 *SolutionApi* | [**add_solution_access_control**](docs/SolutionApi.md#add_solution_access_control) | **POST** /organizations/{organization_id}/solutions/{solution_id}/security/access | Add a control access to the Solution
 *SolutionApi* | [**create_solution**](docs/SolutionApi.md#create_solution) | **POST** /organizations/{organization_id}/solutions | Register a new solution
 *SolutionApi* | [**delete_solution**](docs/SolutionApi.md#delete_solution) | **DELETE** /organizations/{organization_id}/solutions/{solution_id} | Delete a solution
 *SolutionApi* | [**delete_solution_run_template**](docs/SolutionApi.md#delete_solution_run_template) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/runTemplates/{run_template_id} | Remove the specified Solution Run Template
@@ -234,23 +235,14 @@
 *TwingraphApi* | [**find_all_twingraphs**](docs/TwingraphApi.md#find_all_twingraphs) | **GET** /organizations/{organization_id}/twingraphs | Return the list of all graphs stored in the organization
 *TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Get entities in a graph instance
 *TwingraphApi* | [**get_graph_meta_data**](docs/TwingraphApi.md#get_graph_meta_data) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Return the metaData of the specified graph
 *TwingraphApi* | [**job_status**](docs/TwingraphApi.md#job_status) | **GET** /organizations/{organization_id}/job/{job_id}/status | Get the status of a job
 *TwingraphApi* | [**query**](docs/TwingraphApi.md#query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/query | Run a query on a graph instance
 *TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/entity/{type} | Update entities in a graph instance
 *TwingraphApi* | [**update_graph_meta_data**](docs/TwingraphApi.md#update_graph_meta_data) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/metadata | Update the metaData of the specified graph
-*ValidatorApi* | [**create_validator**](docs/ValidatorApi.md#create_validator) | **POST** /organizations/{organization_id}/datasets/validators | Register a new validator
-*ValidatorApi* | [**create_validator_run**](docs/ValidatorApi.md#create_validator_run) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/history | Register a new validator run
-*ValidatorApi* | [**delete_validator**](docs/ValidatorApi.md#delete_validator) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id} | Delete a validator
-*ValidatorApi* | [**delete_validator_run**](docs/ValidatorApi.md#delete_validator_run) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Delete a validator run
-*ValidatorApi* | [**find_all_validator_runs**](docs/ValidatorApi.md#find_all_validator_runs) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history | List all Validator Runs
-*ValidatorApi* | [**find_all_validators**](docs/ValidatorApi.md#find_all_validators) | **GET** /organizations/{organization_id}/datasets/validators | List all Validators
-*ValidatorApi* | [**find_validator_by_id**](docs/ValidatorApi.md#find_validator_by_id) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id} | Get the details of a validator
-*ValidatorApi* | [**find_validator_run_by_id**](docs/ValidatorApi.md#find_validator_run_by_id) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Get the details of a validator run
-*ValidatorApi* | [**run_validator**](docs/ValidatorApi.md#run_validator) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/run | Run a Validator
 *WorkspaceApi* | [**add_workspace_access_control**](docs/WorkspaceApi.md#add_workspace_access_control) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/security/access | Add a control access to the Workspace
 *WorkspaceApi* | [**create_secret**](docs/WorkspaceApi.md#create_secret) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/secret | Create a secret for the Workspace
 *WorkspaceApi* | [**create_workspace**](docs/WorkspaceApi.md#create_workspace) | **POST** /organizations/{organization_id}/workspaces | Create a new workspace
 *WorkspaceApi* | [**delete_all_workspace_files**](docs/WorkspaceApi.md#delete_all_workspace_files) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/files | Delete all Workspace files
 *WorkspaceApi* | [**delete_workspace**](docs/WorkspaceApi.md#delete_workspace) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id} | Delete a workspace
 *WorkspaceApi* | [**delete_workspace_file**](docs/WorkspaceApi.md#delete_workspace_file) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/files/delete | Delete a workspace file
 *WorkspaceApi* | [**download_workspace_file**](docs/WorkspaceApi.md#download_workspace_file) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/files/download | Download the Workspace File specified
@@ -296,19 +288,22 @@
  - [GraphProperties](docs/GraphProperties.md)
  - [Organization](docs/Organization.md)
  - [OrganizationAccessControl](docs/OrganizationAccessControl.md)
  - [OrganizationRole](docs/OrganizationRole.md)
  - [OrganizationSecurity](docs/OrganizationSecurity.md)
  - [OrganizationService](docs/OrganizationService.md)
  - [OrganizationServices](docs/OrganizationServices.md)
+ - [QueryResult](docs/QueryResult.md)
  - [ResourceSizeInfo](docs/ResourceSizeInfo.md)
  - [Run](docs/Run.md)
  - [RunContainer](docs/RunContainer.md)
  - [RunContainerArtifact](docs/RunContainerArtifact.md)
  - [RunContainerLogs](docs/RunContainerLogs.md)
+ - [RunData](docs/RunData.md)
+ - [RunDataQuery](docs/RunDataQuery.md)
  - [RunLogs](docs/RunLogs.md)
  - [RunResourceRequested](docs/RunResourceRequested.md)
  - [RunSearch](docs/RunSearch.md)
  - [RunStartContainers](docs/RunStartContainers.md)
  - [RunState](docs/RunState.md)
  - [RunStatus](docs/RunStatus.md)
  - [RunStatusNode](docs/RunStatusNode.md)
@@ -324,16 +319,18 @@
  - [RunnerAccessControl](docs/RunnerAccessControl.md)
  - [RunnerChangedParameterValue](docs/RunnerChangedParameterValue.md)
  - [RunnerComparisonResult](docs/RunnerComparisonResult.md)
  - [RunnerDataDownloadInfo](docs/RunnerDataDownloadInfo.md)
  - [RunnerDataDownloadJob](docs/RunnerDataDownloadJob.md)
  - [RunnerJobState](docs/RunnerJobState.md)
  - [RunnerLastRun](docs/RunnerLastRun.md)
+ - [RunnerParentLastRun](docs/RunnerParentLastRun.md)
  - [RunnerResourceSizing](docs/RunnerResourceSizing.md)
  - [RunnerRole](docs/RunnerRole.md)
+ - [RunnerRootLastRun](docs/RunnerRootLastRun.md)
  - [RunnerRunTemplateParameterValue](docs/RunnerRunTemplateParameterValue.md)
  - [RunnerSecurity](docs/RunnerSecurity.md)
  - [RunnerValidationStatus](docs/RunnerValidationStatus.md)
  - [Scenario](docs/Scenario.md)
  - [ScenarioAccessControl](docs/ScenarioAccessControl.md)
  - [ScenarioChangedParameterValue](docs/ScenarioChangedParameterValue.md)
  - [ScenarioComparisonResult](docs/ScenarioComparisonResult.md)
@@ -345,30 +342,29 @@
  - [ScenarioRole](docs/ScenarioRole.md)
  - [ScenarioRun](docs/ScenarioRun.md)
  - [ScenarioRunContainer](docs/ScenarioRunContainer.md)
  - [ScenarioRunContainerArtifact](docs/ScenarioRunContainerArtifact.md)
  - [ScenarioRunContainerLogs](docs/ScenarioRunContainerLogs.md)
  - [ScenarioRunLogs](docs/ScenarioRunLogs.md)
  - [ScenarioRunResourceRequested](docs/ScenarioRunResourceRequested.md)
- - [ScenarioRunResult](docs/ScenarioRunResult.md)
  - [ScenarioRunSearch](docs/ScenarioRunSearch.md)
  - [ScenarioRunStartContainers](docs/ScenarioRunStartContainers.md)
  - [ScenarioRunState](docs/ScenarioRunState.md)
  - [ScenarioRunStatus](docs/ScenarioRunStatus.md)
  - [ScenarioRunStatusNode](docs/ScenarioRunStatusNode.md)
  - [ScenarioRunTemplateParameterValue](docs/ScenarioRunTemplateParameterValue.md)
  - [ScenarioSecurity](docs/ScenarioSecurity.md)
  - [ScenarioValidationStatus](docs/ScenarioValidationStatus.md)
+ - [SendRunDataRequest](docs/SendRunDataRequest.md)
  - [Solution](docs/Solution.md)
  - [SolutionAccessControl](docs/SolutionAccessControl.md)
  - [SolutionRole](docs/SolutionRole.md)
  - [SolutionSecurity](docs/SolutionSecurity.md)
  - [SourceInfo](docs/SourceInfo.md)
  - [SubDatasetGraphQuery](docs/SubDatasetGraphQuery.md)
- - [TranslatedLabels](docs/TranslatedLabels.md)
  - [TwinGraphBatchResult](docs/TwinGraphBatchResult.md)
  - [TwinGraphHash](docs/TwinGraphHash.md)
  - [TwinGraphQuery](docs/TwinGraphQuery.md)
  - [Validator](docs/Validator.md)
  - [ValidatorRun](docs/ValidatorRun.md)
  - [Workspace](docs/Workspace.md)
  - [WorkspaceAccessControl](docs/WorkspaceAccessControl.md)
@@ -376,43 +372,27 @@
  - [WorkspaceRole](docs/WorkspaceRole.md)
  - [WorkspaceSecret](docs/WorkspaceSecret.md)
  - [WorkspaceSecurity](docs/WorkspaceSecurity.md)
  - [WorkspaceSolution](docs/WorkspaceSolution.md)
  - [WorkspaceWebApp](docs/WorkspaceWebApp.md)
 
 
+<a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
-## oAuth2AuthCode
+Authentication schemes defined for the API:
+<a id="oAuth2AuthCode"></a>
+### oAuth2AuthCode
 
 - **Type**: OAuth
 - **Flow**: implicit
 - **Authorization URL**: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
 - **Scopes**: 
  - **http://dev.api.cosmotech.com/platform**: Platform scope
 
 
 ## Author
 
 platform@cosmotech.com
 
 
-## Notes for Large OpenAPI documents
-If the OpenAPI document is large, imports in cosmotech_api.apis and cosmotech_api.models may fail with a
-RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-
-Solution 1:
-Use specific imports for apis and models like:
-- `from cosmotech_api.api.default_api import DefaultApi`
-- `from cosmotech_api.model.pet import Pet`
-
-Solution 2:
-Before importing the package, adjust the maximum recursion limit as shown below:
-```
-import sys
-sys.setrecursionlimit(1500)
-import cosmotech_api
-from cosmotech_api.apis import *
-from cosmotech_api.models import *
-```
-
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/api/user_api.py` & `cosmotech_api-3.2.0/cosmotech_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/api_response.py` & `cosmotech_api-3.2.0/cosmotech_api/api_response.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/apis/__init__.py` & `cosmotech_api-3.2.0/cosmotech_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/configuration.py` & `cosmotech_api-3.2.0/cosmotech_api/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,78 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import copy
 import logging
+from logging import FileHandler
 import multiprocessing
 import sys
+from typing import Optional
 import urllib3
 
-from http import client as http_client
-from cosmotech_api.exceptions import ApiValueError
-
+import http.client as httplib
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
-class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
+class Configuration:
+    """This class contains various settings of the API client.
 
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
-
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
+      The validation of enums is performed for variables with defined enum
+      values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
+      in PEM format.
 
     :Example:
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
+                 access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
-                 ):
+                 ) -> None:
         """Constructor
         """
         self._base_path = "https://dev.api.cosmotech.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -105,15 +82,14 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -125,28 +101,29 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("cosmotech_api")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
-        self.logger_file_handler = None
+        self.logger_file_handler: Optional[FileHandler] = None
         """Log file handler
         """
         self.logger_file = None
         """Debug file location
         """
         self.debug = False
         """Debug switch
@@ -165,43 +142,53 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
-        self.proxy = None
+        self.proxy: Optional[str] = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -211,46 +198,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -296,23 +286,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -384,15 +374,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 3.1.1\n"\
+               "Version of the API: 3.1.1-SNAPSHOT\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/exceptions.py` & `cosmotech_api-3.2.0/cosmotech_api/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
+from typing import Any, Optional
+from typing_extensions import Self
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
     def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
+                 key_type=None) -> None:
         """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
@@ -40,15 +45,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiTypeError, self).__init__(full_msg)
 
 
 class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list) the path to the exception in the
                 received_data dict. None if unset
@@ -58,15 +63,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
 class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Raised when an attribute reference or assignment fails.
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -77,15 +82,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiAttributeError, self).__init__(full_msg)
 
 
 class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (None/list) the path to the exception in the
                 received_data dict
@@ -95,62 +100,97 @@
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
 
-    def __init__(self, status=None, reason=None, http_resp=None):
+    def __init__(
+        self, 
+        status=None, 
+        reason=None, 
+        http_resp=None,
+        *,
+        body: Optional[str] = None,
+        data: Optional[Any] = None,
+    ) -> None:
+        self.status = status
+        self.reason = reason
+        self.body = body
+        self.data = data
+        self.headers = None
+
         if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
+            if self.status is None:
+                self.status = http_resp.status
+            if self.reason is None:
+                self.reason = http_resp.reason
+            if self.body is None:
+                try:
+                    self.body = http_resp.data.decode('utf-8')
+                except Exception:
+                    pass
             self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
+
+    @classmethod
+    def from_response(
+        cls, 
+        *, 
+        http_resp, 
+        body: Optional[str], 
+        data: Optional[Any],
+    ) -> Self:
+        if http_resp.status == 400:
+            raise BadRequestException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 401:
+            raise UnauthorizedException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 403:
+            raise ForbiddenException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 404:
+            raise NotFoundException(http_resp=http_resp, body=body, data=data)
+
+        if 500 <= http_resp.status <= 599:
+            raise ServiceException(http_resp=http_resp, body=body, data=data)
+        raise ApiException(http_resp=http_resp, body=body, data=data)
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
+        if self.data or self.body:
+            error_message += "HTTP response body: {0}\n".format(self.data or self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
+class BadRequestException(ApiException):
+    pass
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
 
+class NotFoundException(ApiException):
+    pass
 
-class UnauthorizedException(ApiException):
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+class UnauthorizedException(ApiException):
+    pass
 
 
 class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
+    pass
 
 
 class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
+    pass
 
 
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/component_role_permissions.py` & `cosmotech_api-3.2.0/cosmotech_api/model/component_role_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/connector.py` & `cosmotech_api-3.2.0/cosmotech_api/model/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/connector_parameter.py` & `cosmotech_api-3.2.0/cosmotech_api/model/connector_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/connector_parameter_group.py` & `cosmotech_api-3.2.0/cosmotech_api/model/connector_parameter_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/container_resource_size_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/container_resource_size_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/container_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/model/container_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_compatibility.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_connector.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_copy_parameters.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_copy_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_search.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_source_type.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_hash.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/dataset_twin_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/model/dataset_twin_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/delete_historical_data.py` & `cosmotech_api-3.2.0/cosmotech_api/model/delete_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/file_upload_metadata.py` & `cosmotech_api-3.2.0/cosmotech_api/model/file_upload_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/file_upload_validation.py` & `cosmotech_api-3.2.0/cosmotech_api/model/file_upload_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/graph_properties.py` & `cosmotech_api-3.2.0/cosmotech_api/model/graph_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_service.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_services.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/organization_user.py` & `cosmotech_api-3.2.0/cosmotech_api/model/organization_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/resource_size_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_container.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_container_artifact.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_container_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_container_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_container_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_resource_requested.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_resource_requested.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_search.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_start_containers.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_start_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_state.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_status.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_status_node.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_status_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_handler_id.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_handler_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_orchestrator.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter_group.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/run_template_step_source.py` & `cosmotech_api-3.2.0/cosmotech_api/model/run_template_step_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_changed_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_changed_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_comparison_result.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_comparison_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_data_download_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_data_download_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_data_download_job.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_data_download_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_job_state.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_job_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_last_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/runner_validation_status.py` & `cosmotech_api-3.2.0/cosmotech_api/model/runner_validation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_changed_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_changed_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_comparison_result.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_comparison_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_data_download_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_data_download_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_data_download_job.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_data_download_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_job_state.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_job_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_last_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container_artifact.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_container_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_container_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_resource_requested.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_resource_requested.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_result.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_search.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_start_containers.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_start_containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_state.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_status.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_status_node.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_status_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_run_template_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_user.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/scenario_validation_status.py` & `cosmotech_api-3.2.0/cosmotech_api/model/scenario_validation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/solution.py` & `cosmotech_api-3.2.0/cosmotech_api/model/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/solution_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/solution_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/solution_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/solution_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/solution_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/solution_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/source_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/source_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/sub_dataset_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/model/sub_dataset_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/translated_labels.py` & `cosmotech_api-3.2.0/cosmotech_api/model/translated_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_batch_result.py` & `cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_batch_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_hash.py` & `cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_import.py` & `cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.11
+    The version of the OpenAPI document: 2.4.13
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_import_info.py` & `cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_import_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.4.11
+    The version of the OpenAPI document: 2.4.13
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/twin_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/model/twin_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/user.py` & `cosmotech_api-3.2.0/cosmotech_api/model/user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/user_organization.py` & `cosmotech_api-3.2.0/cosmotech_api/model/user_organization.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/user_workspace.py` & `cosmotech_api-3.2.0/cosmotech_api/model/user_workspace.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/validator.py` & `cosmotech_api-3.2.0/cosmotech_api/model/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/validator_run.py` & `cosmotech_api-3.2.0/cosmotech_api/model/validator_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_file.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_role.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_secret.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_security.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_solution.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_user.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_user.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model/workspace_web_app.py` & `cosmotech_api-3.2.0/cosmotech_api/model/workspace_web_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/model_utils.py` & `cosmotech_api-3.2.0/cosmotech_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/__init__.py` & `cosmotech_api-3.2.0/cosmotech_api/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,127 @@
+# coding: utf-8
+
 # flake8: noqa
+"""
+    Cosmo Tech Platform API
+
+    Cosmo Tech Platform API
+
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
+    Contact: platform@cosmotech.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from from cosmotech_api.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
-
-from cosmotech_api.model.component_role_permissions import ComponentRolePermissions
-from cosmotech_api.model.connector import Connector
-from cosmotech_api.model.connector_parameter import ConnectorParameter
-from cosmotech_api.model.connector_parameter_group import ConnectorParameterGroup
-from cosmotech_api.model.container_resource_size_info import ContainerResourceSizeInfo
-from cosmotech_api.model.container_resource_sizing import ContainerResourceSizing
-from cosmotech_api.model.dataset import Dataset
-from cosmotech_api.model.dataset_access_control import DatasetAccessControl
-from cosmotech_api.model.dataset_compatibility import DatasetCompatibility
-from cosmotech_api.model.dataset_connector import DatasetConnector
-from cosmotech_api.model.dataset_copy_parameters import DatasetCopyParameters
-from cosmotech_api.model.dataset_role import DatasetRole
-from cosmotech_api.model.dataset_search import DatasetSearch
-from cosmotech_api.model.dataset_security import DatasetSecurity
-from cosmotech_api.model.dataset_source_type import DatasetSourceType
-from cosmotech_api.model.dataset_twin_graph_hash import DatasetTwinGraphHash
-from cosmotech_api.model.dataset_twin_graph_info import DatasetTwinGraphInfo
-from cosmotech_api.model.dataset_twin_graph_query import DatasetTwinGraphQuery
-from cosmotech_api.model.delete_historical_data import DeleteHistoricalData
-from cosmotech_api.model.file_upload_metadata import FileUploadMetadata
-from cosmotech_api.model.file_upload_validation import FileUploadValidation
-from cosmotech_api.model.graph_properties import GraphProperties
-from cosmotech_api.model.organization import Organization
-from cosmotech_api.model.organization_access_control import OrganizationAccessControl
-from cosmotech_api.model.organization_role import OrganizationRole
-from cosmotech_api.model.organization_security import OrganizationSecurity
-from cosmotech_api.model.organization_service import OrganizationService
-from cosmotech_api.model.organization_services import OrganizationServices
-from cosmotech_api.model.resource_size_info import ResourceSizeInfo
-from cosmotech_api.model.run import Run
-from cosmotech_api.model.run_container import RunContainer
-from cosmotech_api.model.run_container_artifact import RunContainerArtifact
-from cosmotech_api.model.run_container_logs import RunContainerLogs
-from cosmotech_api.model.run_logs import RunLogs
-from cosmotech_api.model.run_resource_requested import RunResourceRequested
-from cosmotech_api.model.run_search import RunSearch
-from cosmotech_api.model.run_start_containers import RunStartContainers
-from cosmotech_api.model.run_state import RunState
-from cosmotech_api.model.run_status import RunStatus
-from cosmotech_api.model.run_status_node import RunStatusNode
-from cosmotech_api.model.run_template import RunTemplate
-from cosmotech_api.model.run_template_handler_id import RunTemplateHandlerId
-from cosmotech_api.model.run_template_orchestrator import RunTemplateOrchestrator
-from cosmotech_api.model.run_template_parameter import RunTemplateParameter
-from cosmotech_api.model.run_template_parameter_group import RunTemplateParameterGroup
-from cosmotech_api.model.run_template_parameter_value import RunTemplateParameterValue
-from cosmotech_api.model.run_template_resource_sizing import RunTemplateResourceSizing
-from cosmotech_api.model.run_template_step_source import RunTemplateStepSource
-from cosmotech_api.model.runner import Runner
-from cosmotech_api.model.runner_access_control import RunnerAccessControl
-from cosmotech_api.model.runner_changed_parameter_value import RunnerChangedParameterValue
-from cosmotech_api.model.runner_comparison_result import RunnerComparisonResult
-from cosmotech_api.model.runner_data_download_info import RunnerDataDownloadInfo
-from cosmotech_api.model.runner_data_download_job import RunnerDataDownloadJob
-from cosmotech_api.model.runner_job_state import RunnerJobState
-from cosmotech_api.model.runner_last_run import RunnerLastRun
-from cosmotech_api.model.runner_resource_sizing import RunnerResourceSizing
-from cosmotech_api.model.runner_role import RunnerRole
-from cosmotech_api.model.runner_run_template_parameter_value import RunnerRunTemplateParameterValue
-from cosmotech_api.model.runner_security import RunnerSecurity
-from cosmotech_api.model.runner_validation_status import RunnerValidationStatus
-from cosmotech_api.model.scenario import Scenario
-from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
-from cosmotech_api.model.scenario_changed_parameter_value import ScenarioChangedParameterValue
-from cosmotech_api.model.scenario_comparison_result import ScenarioComparisonResult
-from cosmotech_api.model.scenario_data_download_info import ScenarioDataDownloadInfo
-from cosmotech_api.model.scenario_data_download_job import ScenarioDataDownloadJob
-from cosmotech_api.model.scenario_job_state import ScenarioJobState
-from cosmotech_api.model.scenario_last_run import ScenarioLastRun
-from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
-from cosmotech_api.model.scenario_role import ScenarioRole
-from cosmotech_api.model.scenario_run import ScenarioRun
-from cosmotech_api.model.scenario_run_container import ScenarioRunContainer
-from cosmotech_api.model.scenario_run_container_artifact import ScenarioRunContainerArtifact
-from cosmotech_api.model.scenario_run_container_logs import ScenarioRunContainerLogs
-from cosmotech_api.model.scenario_run_logs import ScenarioRunLogs
-from cosmotech_api.model.scenario_run_resource_requested import ScenarioRunResourceRequested
-from cosmotech_api.model.scenario_run_result import ScenarioRunResult
-from cosmotech_api.model.scenario_run_search import ScenarioRunSearch
-from cosmotech_api.model.scenario_run_start_containers import ScenarioRunStartContainers
-from cosmotech_api.model.scenario_run_state import ScenarioRunState
-from cosmotech_api.model.scenario_run_status import ScenarioRunStatus
-from cosmotech_api.model.scenario_run_status_node import ScenarioRunStatusNode
-from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
-from cosmotech_api.model.scenario_security import ScenarioSecurity
-from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
-from cosmotech_api.model.solution import Solution
-from cosmotech_api.model.solution_access_control import SolutionAccessControl
-from cosmotech_api.model.solution_role import SolutionRole
-from cosmotech_api.model.solution_security import SolutionSecurity
-from cosmotech_api.model.source_info import SourceInfo
-from cosmotech_api.model.sub_dataset_graph_query import SubDatasetGraphQuery
-from cosmotech_api.model.translated_labels import TranslatedLabels
-from cosmotech_api.model.twin_graph_batch_result import TwinGraphBatchResult
-from cosmotech_api.model.twin_graph_hash import TwinGraphHash
-from cosmotech_api.model.twin_graph_query import TwinGraphQuery
-from cosmotech_api.model.validator import Validator
-from cosmotech_api.model.validator_run import ValidatorRun
-from cosmotech_api.model.workspace import Workspace
-from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
-from cosmotech_api.model.workspace_file import WorkspaceFile
-from cosmotech_api.model.workspace_role import WorkspaceRole
-from cosmotech_api.model.workspace_secret import WorkspaceSecret
-from cosmotech_api.model.workspace_security import WorkspaceSecurity
-from cosmotech_api.model.workspace_solution import WorkspaceSolution
-from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
+# import models into model package
+from cosmotech_api.models.component_role_permissions import ComponentRolePermissions
+from cosmotech_api.models.connector import Connector
+from cosmotech_api.models.connector_parameter import ConnectorParameter
+from cosmotech_api.models.connector_parameter_group import ConnectorParameterGroup
+from cosmotech_api.models.container_resource_size_info import ContainerResourceSizeInfo
+from cosmotech_api.models.container_resource_sizing import ContainerResourceSizing
+from cosmotech_api.models.dataset import Dataset
+from cosmotech_api.models.dataset_access_control import DatasetAccessControl
+from cosmotech_api.models.dataset_compatibility import DatasetCompatibility
+from cosmotech_api.models.dataset_connector import DatasetConnector
+from cosmotech_api.models.dataset_copy_parameters import DatasetCopyParameters
+from cosmotech_api.models.dataset_role import DatasetRole
+from cosmotech_api.models.dataset_search import DatasetSearch
+from cosmotech_api.models.dataset_security import DatasetSecurity
+from cosmotech_api.models.dataset_source_type import DatasetSourceType
+from cosmotech_api.models.dataset_twin_graph_hash import DatasetTwinGraphHash
+from cosmotech_api.models.dataset_twin_graph_info import DatasetTwinGraphInfo
+from cosmotech_api.models.dataset_twin_graph_query import DatasetTwinGraphQuery
+from cosmotech_api.models.delete_historical_data import DeleteHistoricalData
+from cosmotech_api.models.file_upload_metadata import FileUploadMetadata
+from cosmotech_api.models.file_upload_validation import FileUploadValidation
+from cosmotech_api.models.graph_properties import GraphProperties
+from cosmotech_api.models.organization import Organization
+from cosmotech_api.models.organization_access_control import OrganizationAccessControl
+from cosmotech_api.models.organization_role import OrganizationRole
+from cosmotech_api.models.organization_security import OrganizationSecurity
+from cosmotech_api.models.organization_service import OrganizationService
+from cosmotech_api.models.organization_services import OrganizationServices
+from cosmotech_api.models.query_result import QueryResult
+from cosmotech_api.models.resource_size_info import ResourceSizeInfo
+from cosmotech_api.models.run import Run
+from cosmotech_api.models.run_container import RunContainer
+from cosmotech_api.models.run_container_artifact import RunContainerArtifact
+from cosmotech_api.models.run_container_logs import RunContainerLogs
+from cosmotech_api.models.run_data import RunData
+from cosmotech_api.models.run_data_query import RunDataQuery
+from cosmotech_api.models.run_logs import RunLogs
+from cosmotech_api.models.run_resource_requested import RunResourceRequested
+from cosmotech_api.models.run_search import RunSearch
+from cosmotech_api.models.run_start_containers import RunStartContainers
+from cosmotech_api.models.run_state import RunState
+from cosmotech_api.models.run_status import RunStatus
+from cosmotech_api.models.run_status_node import RunStatusNode
+from cosmotech_api.models.run_template import RunTemplate
+from cosmotech_api.models.run_template_handler_id import RunTemplateHandlerId
+from cosmotech_api.models.run_template_orchestrator import RunTemplateOrchestrator
+from cosmotech_api.models.run_template_parameter import RunTemplateParameter
+from cosmotech_api.models.run_template_parameter_group import RunTemplateParameterGroup
+from cosmotech_api.models.run_template_parameter_value import RunTemplateParameterValue
+from cosmotech_api.models.run_template_resource_sizing import RunTemplateResourceSizing
+from cosmotech_api.models.run_template_step_source import RunTemplateStepSource
+from cosmotech_api.models.runner import Runner
+from cosmotech_api.models.runner_access_control import RunnerAccessControl
+from cosmotech_api.models.runner_changed_parameter_value import RunnerChangedParameterValue
+from cosmotech_api.models.runner_comparison_result import RunnerComparisonResult
+from cosmotech_api.models.runner_data_download_info import RunnerDataDownloadInfo
+from cosmotech_api.models.runner_data_download_job import RunnerDataDownloadJob
+from cosmotech_api.models.runner_job_state import RunnerJobState
+from cosmotech_api.models.runner_last_run import RunnerLastRun
+from cosmotech_api.models.runner_parent_last_run import RunnerParentLastRun
+from cosmotech_api.models.runner_resource_sizing import RunnerResourceSizing
+from cosmotech_api.models.runner_role import RunnerRole
+from cosmotech_api.models.runner_root_last_run import RunnerRootLastRun
+from cosmotech_api.models.runner_run_template_parameter_value import RunnerRunTemplateParameterValue
+from cosmotech_api.models.runner_security import RunnerSecurity
+from cosmotech_api.models.runner_validation_status import RunnerValidationStatus
+from cosmotech_api.models.scenario import Scenario
+from cosmotech_api.models.scenario_access_control import ScenarioAccessControl
+from cosmotech_api.models.scenario_changed_parameter_value import ScenarioChangedParameterValue
+from cosmotech_api.models.scenario_comparison_result import ScenarioComparisonResult
+from cosmotech_api.models.scenario_data_download_info import ScenarioDataDownloadInfo
+from cosmotech_api.models.scenario_data_download_job import ScenarioDataDownloadJob
+from cosmotech_api.models.scenario_job_state import ScenarioJobState
+from cosmotech_api.models.scenario_last_run import ScenarioLastRun
+from cosmotech_api.models.scenario_resource_sizing import ScenarioResourceSizing
+from cosmotech_api.models.scenario_role import ScenarioRole
+from cosmotech_api.models.scenario_run import ScenarioRun
+from cosmotech_api.models.scenario_run_container import ScenarioRunContainer
+from cosmotech_api.models.scenario_run_container_artifact import ScenarioRunContainerArtifact
+from cosmotech_api.models.scenario_run_container_logs import ScenarioRunContainerLogs
+from cosmotech_api.models.scenario_run_logs import ScenarioRunLogs
+from cosmotech_api.models.scenario_run_resource_requested import ScenarioRunResourceRequested
+from cosmotech_api.models.scenario_run_search import ScenarioRunSearch
+from cosmotech_api.models.scenario_run_start_containers import ScenarioRunStartContainers
+from cosmotech_api.models.scenario_run_state import ScenarioRunState
+from cosmotech_api.models.scenario_run_status import ScenarioRunStatus
+from cosmotech_api.models.scenario_run_status_node import ScenarioRunStatusNode
+from cosmotech_api.models.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
+from cosmotech_api.models.scenario_security import ScenarioSecurity
+from cosmotech_api.models.scenario_validation_status import ScenarioValidationStatus
+from cosmotech_api.models.send_run_data_request import SendRunDataRequest
+from cosmotech_api.models.solution import Solution
+from cosmotech_api.models.solution_access_control import SolutionAccessControl
+from cosmotech_api.models.solution_role import SolutionRole
+from cosmotech_api.models.solution_security import SolutionSecurity
+from cosmotech_api.models.source_info import SourceInfo
+from cosmotech_api.models.sub_dataset_graph_query import SubDatasetGraphQuery
+from cosmotech_api.models.twin_graph_batch_result import TwinGraphBatchResult
+from cosmotech_api.models.twin_graph_hash import TwinGraphHash
+from cosmotech_api.models.twin_graph_query import TwinGraphQuery
+from cosmotech_api.models.validator import Validator
+from cosmotech_api.models.validator_run import ValidatorRun
+from cosmotech_api.models.workspace import Workspace
+from cosmotech_api.models.workspace_access_control import WorkspaceAccessControl
+from cosmotech_api.models.workspace_file import WorkspaceFile
+from cosmotech_api.models.workspace_role import WorkspaceRole
+from cosmotech_api.models.workspace_secret import WorkspaceSecret
+from cosmotech_api.models.workspace_security import WorkspaceSecurity
+from cosmotech_api.models.workspace_solution import WorkspaceSolution
+from cosmotech_api.models.workspace_web_app import WorkspaceWebApp
```

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/component_role_permissions.py` & `cosmotech_api-3.2.0/cosmotech_api/models/component_role_permissions.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/connector.py` & `cosmotech_api-3.2.0/cosmotech_api/models/connector.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/connector_parameter.py` & `cosmotech_api-3.2.0/cosmotech_api/models/connector_parameter.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/connector_parameter_group.py` & `cosmotech_api-3.2.0/cosmotech_api/models/connector_parameter_group.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/container_resource_size_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/container_resource_size_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/container_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/models/container_resource_sizing.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_compatibility.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_compatibility.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_connector.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_connector.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_copy_parameters.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_copy_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_search.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_search.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_source_type.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_source_type.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_hash.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_hash.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/dataset_twin_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/models/dataset_twin_graph_query.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/delete_historical_data.py` & `cosmotech_api-3.2.0/cosmotech_api/models/delete_historical_data.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/file_upload_metadata.py` & `cosmotech_api-3.2.0/cosmotech_api/models/file_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/file_upload_validation.py` & `cosmotech_api-3.2.0/cosmotech_api/models/file_upload_validation.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/graph_properties.py` & `cosmotech_api-3.2.0/cosmotech_api/models/graph_properties.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization_service.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization_service.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/organization_services.py` & `cosmotech_api-3.2.0/cosmotech_api/models/organization_services.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/resource_size_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/resource_size_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_container.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_container.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_container_artifact.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_container_artifact.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_container_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_container_logs.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_logs.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_resource_requested.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_resource_requested.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_search.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_search.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_start_containers.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_start_containers.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_state.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_state.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_status.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_status.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_status_node.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_status_node.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_handler_id.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_handler_id.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_orchestrator.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter_group.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter_group.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_parameter_value.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_resource_sizing.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/run_template_step_source.py` & `cosmotech_api-3.2.0/cosmotech_api/models/run_template_step_source.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_changed_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_changed_parameter_value.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_comparison_result.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_comparison_result.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_data_download_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_data_download_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_data_download_job.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_data_download_job.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_job_state.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_job_state.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_parent_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_parent_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_resource_sizing.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_root_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_root_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_run_template_parameter_value.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/runner_validation_status.py` & `cosmotech_api-3.2.0/cosmotech_api/models/runner_validation_status.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_changed_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_changed_parameter_value.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_comparison_result.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_comparison_result.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_data_download_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_data_download_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_data_download_job.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_data_download_job.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_job_state.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_job_state.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_last_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_resource_sizing.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_resource_sizing.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container_artifact.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container_artifact.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_container_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_container_logs.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_logs.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_logs.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_resource_requested.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_resource_requested.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_result.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_result.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_search.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_search.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_start_containers.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_start_containers.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_state.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_state.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_status.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_status.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_status_node.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_status_node.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_run_template_parameter_value.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_run_template_parameter_value.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/scenario_validation_status.py` & `cosmotech_api-3.2.0/cosmotech_api/models/scenario_validation_status.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/solution.py` & `cosmotech_api-3.2.0/cosmotech_api/models/solution.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/solution_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/solution_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/solution_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/solution_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/solution_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/solution_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/source_info.py` & `cosmotech_api-3.2.0/cosmotech_api/models/source_info.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/sub_dataset_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/models/sub_dataset_graph_query.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_batch_result.py` & `cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_batch_result.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_hash.py` & `cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_hash.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/twin_graph_query.py` & `cosmotech_api-3.2.0/cosmotech_api/models/twin_graph_query.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/validator.py` & `cosmotech_api-3.2.0/cosmotech_api/models/validator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/validator_run.py` & `cosmotech_api-3.2.0/cosmotech_api/models/validator_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_access_control.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_access_control.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_file.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_file.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_role.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_role.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_secret.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_secret.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_security.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_security.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_solution.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_solution.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api/models/workspace_web_app.py` & `cosmotech_api-3.2.0/cosmotech_api/models/workspace_web_app.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/cosmotech_api.egg-info/SOURCES.txt` & `cosmotech_api-3.2.0/cosmotech_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -171,19 +171,22 @@
 cosmotech_api/models/graph_properties.py
 cosmotech_api/models/organization.py
 cosmotech_api/models/organization_access_control.py
 cosmotech_api/models/organization_role.py
 cosmotech_api/models/organization_security.py
 cosmotech_api/models/organization_service.py
 cosmotech_api/models/organization_services.py
+cosmotech_api/models/query_result.py
 cosmotech_api/models/resource_size_info.py
 cosmotech_api/models/run.py
 cosmotech_api/models/run_container.py
 cosmotech_api/models/run_container_artifact.py
 cosmotech_api/models/run_container_logs.py
+cosmotech_api/models/run_data.py
+cosmotech_api/models/run_data_query.py
 cosmotech_api/models/run_logs.py
 cosmotech_api/models/run_resource_requested.py
 cosmotech_api/models/run_search.py
 cosmotech_api/models/run_start_containers.py
 cosmotech_api/models/run_state.py
 cosmotech_api/models/run_status.py
 cosmotech_api/models/run_status_node.py
@@ -231,14 +234,15 @@
 cosmotech_api/models/scenario_run_start_containers.py
 cosmotech_api/models/scenario_run_state.py
 cosmotech_api/models/scenario_run_status.py
 cosmotech_api/models/scenario_run_status_node.py
 cosmotech_api/models/scenario_run_template_parameter_value.py
 cosmotech_api/models/scenario_security.py
 cosmotech_api/models/scenario_validation_status.py
+cosmotech_api/models/send_run_data_request.py
 cosmotech_api/models/solution.py
 cosmotech_api/models/solution_access_control.py
 cosmotech_api/models/solution_role.py
 cosmotech_api/models/solution_security.py
 cosmotech_api/models/source_info.py
 cosmotech_api/models/sub_dataset_graph_query.py
 cosmotech_api/models/twin_graph_batch_result.py
@@ -282,20 +286,23 @@
 test/test_organization_access_control.py
 test/test_organization_api.py
 test/test_organization_role.py
 test/test_organization_security.py
 test/test_organization_service.py
 test/test_organization_services.py
 test/test_organization_user.py
+test/test_query_result.py
 test/test_resource_size_info.py
 test/test_run.py
 test/test_run_api.py
 test/test_run_container.py
 test/test_run_container_artifact.py
 test/test_run_container_logs.py
+test/test_run_data.py
+test/test_run_data_query.py
 test/test_run_logs.py
 test/test_run_resource_requested.py
 test/test_run_search.py
 test/test_run_start_containers.py
 test/test_run_state.py
 test/test_run_status.py
 test/test_run_status_node.py
@@ -348,14 +355,15 @@
 test/test_scenario_run_status_node.py
 test/test_scenario_run_template_parameter_value.py
 test/test_scenario_security.py
 test/test_scenario_user.py
 test/test_scenario_validation_status.py
 test/test_scenariorun_api.py
 test/test_scenariorunresult_api.py
+test/test_send_run_data_request.py
 test/test_solution.py
 test/test_solution_access_control.py
 test/test_solution_api.py
 test/test_solution_role.py
 test/test_solution_security.py
 test/test_source_info.py
 test/test_sub_dataset_graph_query.py
```

### Comparing `cosmotech-api-3.1.1/pyproject.toml` & `cosmotech_api-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/setup.py` & `cosmotech_api-3.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,51 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "cosmotech-api"
-VERSION = "3.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-
+NAME = "cosmotech-api"
+VERSION = "3.2.0"
+PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
-  "urllib3 >= 1.25.3",
-  "python-dateutil",
+    "urllib3 >= 1.25.3, < 2.1.0",
+    "python-dateutil",
+    "pydantic >= 2",
+    "typing-extensions >= 4.7.1",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Cosmo Tech Platform API",
     author="Repository",
     author_email="platform@cosmotech.com",
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "Cosmo Tech Platform API"],
-    python_requires=">=3.6",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT License",
+    long_description_content_type='text/markdown',
     long_description="""\
-    Cosmo Tech Platform API  # noqa: E501
-    """
+    Cosmo Tech Platform API
+    """,  # noqa: E501
+    package_data={"cosmotech_api": ["py.typed"]},
 )
```

### Comparing `cosmotech-api-3.1.1/test/test_connector.py` & `cosmotech_api-3.2.0/test/test_connector_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,67 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-import sys
 import unittest
 
-import cosmotech_api
-from cosmotech_api.model.connector_parameter_group import ConnectorParameterGroup
-globals()['ConnectorParameterGroup'] = ConnectorParameterGroup
-from cosmotech_api.model.connector import Connector
+from cosmotech_api.api.connector_api import ConnectorApi
+
+
+class TestConnectorApi(unittest.TestCase):
+    """ConnectorApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = ConnectorApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_find_all_connectors(self) -> None:
+        """Test case for find_all_connectors
+
+        List all Connectors
+        """
+        pass
 
+    def test_find_connector_by_id(self) -> None:
+        """Test case for find_connector_by_id
 
-class TestConnector(unittest.TestCase):
-    """Connector unit test stubs"""
+        Get the details of a connector
+        """
+        pass
+
+    def test_find_connector_by_name(self) -> None:
+        """Test case for find_connector_by_name
 
-    def setUp(self):
+        Get the details of a connector
+        """
         pass
 
-    def tearDown(self):
+    def test_register_connector(self) -> None:
+        """Test case for register_connector
+
+        Register a new connector
+        """
         pass
 
-    def testConnector(self):
-        """Test Connector"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Connector()  # noqa: E501
+    def test_unregister_connector(self) -> None:
+        """Test case for unregister_connector
+
+        Unregister a connector
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_access_control.py` & `cosmotech_api-3.2.0/test/test_twin_graph_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.4.13
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_access_control import DatasetAccessControl
+from cosmotech_api.model.source_info import SourceInfo
+globals()['SourceInfo'] = SourceInfo
+from cosmotech_api.model.twin_graph_import import TwinGraphImport
 
 
-class TestDatasetAccessControl(unittest.TestCase):
-    """DatasetAccessControl unit test stubs"""
+class TestTwinGraphImport(unittest.TestCase):
+    """TwinGraphImport unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetAccessControl(self):
-        """Test DatasetAccessControl"""
+    def testTwinGraphImport(self):
+        """Test TwinGraphImport"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetAccessControl()  # noqa: E501
+        # model = TwinGraphImport()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_compatibility.py` & `cosmotech_api-3.2.0/test/test_workspace_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Platform API
+    Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_compatibility import DatasetCompatibility
+from cosmotech_api.model.workspace_user import WorkspaceUser
 
 
-class TestDatasetCompatibility(unittest.TestCase):
-    """DatasetCompatibility unit test stubs"""
+class TestWorkspaceUser(unittest.TestCase):
+    """WorkspaceUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetCompatibility(self):
-        """Test DatasetCompatibility"""
+    def testWorkspaceUser(self):
+        """Test WorkspaceUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetCompatibility()  # noqa: E501
+        # model = WorkspaceUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_role.py` & `cosmotech_api-3.2.0/test/test_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.3.17
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_role import DatasetRole
+from cosmotech_api.model.user_organization import UserOrganization
+globals()['UserOrganization'] = UserOrganization
+from cosmotech_api.model.user import User
 
 
-class TestDatasetRole(unittest.TestCase):
-    """DatasetRole unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetRole(self):
-        """Test DatasetRole"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetRole()  # noqa: E501
+        # model = User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_search.py` & `cosmotech_api-3.2.0/test/test_scenario_run_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.dataset_search import DatasetSearch
+import unittest
 
+from cosmotech_api.models.scenario_run_state import ScenarioRunState
 
-class TestDatasetSearch(unittest.TestCase):
-    """DatasetSearch unit test stubs"""
+class TestScenarioRunState(unittest.TestCase):
+    """ScenarioRunState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetSearch(self):
-        """Test DatasetSearch"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetSearch()  # noqa: E501
-        pass
-
+    def testScenarioRunState(self):
+        """Test ScenarioRunState"""
+        # inst = ScenarioRunState()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_security.py` & `cosmotech_api-3.2.0/test/test_user_workspace.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.3.17
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_access_control import DatasetAccessControl
-globals()['DatasetAccessControl'] = DatasetAccessControl
-from cosmotech_api.model.dataset_security import DatasetSecurity
+from cosmotech_api.model.user_workspace import UserWorkspace
 
 
-class TestDatasetSecurity(unittest.TestCase):
-    """DatasetSecurity unit test stubs"""
+class TestUserWorkspace(unittest.TestCase):
+    """UserWorkspace unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetSecurity(self):
-        """Test DatasetSecurity"""
+    def testUserWorkspace(self):
+        """Test UserWorkspace"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetSecurity()  # noqa: E501
+        # model = UserWorkspace()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_source_type.py` & `cosmotech_api-3.2.0/test/test_run_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.dataset_source_type import DatasetSourceType
+import unittest
 
+from cosmotech_api.models.run_state import RunState
 
-class TestDatasetSourceType(unittest.TestCase):
-    """DatasetSourceType unit test stubs"""
+class TestRunState(unittest.TestCase):
+    """RunState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetSourceType(self):
-        """Test DatasetSourceType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetSourceType()  # noqa: E501
-        pass
-
+    def testRunState(self):
+        """Test RunState"""
+        # inst = RunState()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_twin_graph_hash.py` & `cosmotech_api-3.2.0/test/test_twin_graph_import_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.4.13
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_twin_graph_hash import DatasetTwinGraphHash
+from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
 
 
-class TestDatasetTwinGraphHash(unittest.TestCase):
-    """DatasetTwinGraphHash unit test stubs"""
+class TestTwinGraphImportInfo(unittest.TestCase):
+    """TwinGraphImportInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetTwinGraphHash(self):
-        """Test DatasetTwinGraphHash"""
+    def testTwinGraphImportInfo(self):
+        """Test TwinGraphImportInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetTwinGraphHash()  # noqa: E501
+        # model = TwinGraphImportInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_dataset_twin_graph_info.py` & `cosmotech_api-3.2.0/test/test_organization_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Platform API
+    Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.dataset_twin_graph_info import DatasetTwinGraphInfo
+from cosmotech_api.model.organization_user import OrganizationUser
 
 
-class TestDatasetTwinGraphInfo(unittest.TestCase):
-    """DatasetTwinGraphInfo unit test stubs"""
+class TestOrganizationUser(unittest.TestCase):
+    """OrganizationUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetTwinGraphInfo(self):
-        """Test DatasetTwinGraphInfo"""
+    def testOrganizationUser(self):
+        """Test OrganizationUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetTwinGraphInfo()  # noqa: E501
+        # model = OrganizationUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_delete_historical_data.py` & `cosmotech_api-3.2.0/test/test_translated_labels.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.5
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.delete_historical_data import DeleteHistoricalData
+from cosmotech_api.model.translated_labels import TranslatedLabels
 
 
-class TestDeleteHistoricalData(unittest.TestCase):
-    """DeleteHistoricalData unit test stubs"""
+class TestTranslatedLabels(unittest.TestCase):
+    """TranslatedLabels unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDeleteHistoricalData(self):
-        """Test DeleteHistoricalData"""
+    def testTranslatedLabels(self):
+        """Test TranslatedLabels"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DeleteHistoricalData()  # noqa: E501
+        # model = TranslatedLabels()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_file_upload_metadata.py` & `cosmotech_api-3.2.0/test/test_dataset_source_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.file_upload_metadata import FileUploadMetadata
+import unittest
 
+from cosmotech_api.models.dataset_source_type import DatasetSourceType
 
-class TestFileUploadMetadata(unittest.TestCase):
-    """FileUploadMetadata unit test stubs"""
+class TestDatasetSourceType(unittest.TestCase):
+    """DatasetSourceType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFileUploadMetadata(self):
-        """Test FileUploadMetadata"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FileUploadMetadata()  # noqa: E501
-        pass
-
+    def testDatasetSourceType(self):
+        """Test DatasetSourceType"""
+        # inst = DatasetSourceType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_file_upload_validation.py` & `cosmotech_api-3.2.0/test/test_file_upload_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,61 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.file_upload_metadata import FileUploadMetadata
-globals()['FileUploadMetadata'] = FileUploadMetadata
-from cosmotech_api.model.file_upload_validation import FileUploadValidation
+import unittest
 
+from cosmotech_api.models.file_upload_validation import FileUploadValidation
 
 class TestFileUploadValidation(unittest.TestCase):
     """FileUploadValidation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> FileUploadValidation:
+        """Test FileUploadValidation
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FileUploadValidation`
+        """
+        model = FileUploadValidation()
+        if include_optional:
+            return FileUploadValidation(
+                nodes = [
+                    cosmotech_api.models.file_upload_metadata.FileUploadMetadata(
+                        name = '', 
+                        size = 56, )
+                    ],
+                edges = [
+                    cosmotech_api.models.file_upload_metadata.FileUploadMetadata(
+                        name = '', 
+                        size = 56, )
+                    ]
+            )
+        else:
+            return FileUploadValidation(
+        )
+        """
+
     def testFileUploadValidation(self):
         """Test FileUploadValidation"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FileUploadValidation()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_access_control.py` & `cosmotech_api-3.2.0/test/test_user_organization.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 2.3.17
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.organization_access_control import OrganizationAccessControl
+from cosmotech_api.model.user_workspace import UserWorkspace
+globals()['UserWorkspace'] = UserWorkspace
+from cosmotech_api.model.user_organization import UserOrganization
 
 
-class TestOrganizationAccessControl(unittest.TestCase):
-    """OrganizationAccessControl unit test stubs"""
+class TestUserOrganization(unittest.TestCase):
+    """UserOrganization unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationAccessControl(self):
-        """Test OrganizationAccessControl"""
+    def testUserOrganization(self):
+        """Test UserOrganization"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = OrganizationAccessControl()  # noqa: E501
+        # model = UserOrganization()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_api.py` & `cosmotech_api-3.2.0/test/test_organization_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,151 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import unittest
 
-import cosmotech_api
-from cosmotech_api.api.organization_api import OrganizationApi  # noqa: E501
+from cosmotech_api.api.organization_api import OrganizationApi
 
 
 class TestOrganizationApi(unittest.TestCase):
     """OrganizationApi unit test stubs"""
 
-    def setUp(self):
-        self.api = OrganizationApi()  # noqa: E501
+    def setUp(self) -> None:
+        self.api = OrganizationApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    def test_add_organization_access_control(self):
+    def test_add_organization_access_control(self) -> None:
         """Test case for add_organization_access_control
 
-        Add a control access to the Organization  # noqa: E501
+        Add a control access to the Organization
         """
         pass
 
-    def test_find_all_organizations(self):
+    def test_find_all_organizations(self) -> None:
         """Test case for find_all_organizations
 
-        List all Organizations  # noqa: E501
+        List all Organizations
         """
         pass
 
-    def test_find_organization_by_id(self):
+    def test_find_organization_by_id(self) -> None:
         """Test case for find_organization_by_id
 
-        Get the details of an Organization  # noqa: E501
+        Get the details of an Organization
         """
         pass
 
-    def test_get_all_permissions(self):
+    def test_get_all_permissions(self) -> None:
         """Test case for get_all_permissions
 
-        Get all permissions per components  # noqa: E501
+        Get all permissions per components
         """
         pass
 
-    def test_get_organization_access_control(self):
+    def test_get_organization_access_control(self) -> None:
         """Test case for get_organization_access_control
 
-        Get a control access for the Organization  # noqa: E501
+        Get a control access for the Organization
         """
         pass
 
-    def test_get_organization_permissions(self):
+    def test_get_organization_permissions(self) -> None:
         """Test case for get_organization_permissions
 
-        Get the Organization permissions by given role  # noqa: E501
+        Get the Organization permissions by given role
         """
         pass
 
-    def test_get_organization_security(self):
+    def test_get_organization_security(self) -> None:
         """Test case for get_organization_security
 
-        Get the Organization security information  # noqa: E501
+        Get the Organization security information
         """
         pass
 
-    def test_get_organization_security_users(self):
+    def test_get_organization_security_users(self) -> None:
         """Test case for get_organization_security_users
 
-        Get the Organization security users list  # noqa: E501
+        Get the Organization security users list
         """
         pass
 
-    def test_register_organization(self):
+    def test_register_organization(self) -> None:
         """Test case for register_organization
 
-        Register a new organization  # noqa: E501
+        Register a new organization
         """
         pass
 
-    def test_remove_organization_access_control(self):
+    def test_remove_organization_access_control(self) -> None:
         """Test case for remove_organization_access_control
 
-        Remove the specified access from the given Organization  # noqa: E501
+        Remove the specified access from the given Organization
         """
         pass
 
-    def test_set_organization_default_security(self):
+    def test_set_organization_default_security(self) -> None:
         """Test case for set_organization_default_security
 
-        Set the Organization default security  # noqa: E501
+        Set the Organization default security
         """
         pass
 
-    def test_unregister_organization(self):
+    def test_unregister_organization(self) -> None:
         """Test case for unregister_organization
 
-        Unregister an organization  # noqa: E501
+        Unregister an organization
         """
         pass
 
-    def test_update_organization(self):
+    def test_update_organization(self) -> None:
         """Test case for update_organization
 
-        Update an Organization  # noqa: E501
+        Update an Organization
         """
         pass
 
-    def test_update_organization_access_control(self):
+    def test_update_organization_access_control(self) -> None:
         """Test case for update_organization_access_control
 
-        Update the specified access to User for an Organization  # noqa: E501
+        Update the specified access to User for an Organization
         """
         pass
 
-    def test_update_solutions_container_registry_by_organization_id(self):
+    def test_update_solutions_container_registry_by_organization_id(self) -> None:
         """Test case for update_solutions_container_registry_by_organization_id
 
-        Update the solutions container registry configuration for the Organization specified  # noqa: E501
+        Update the solutions container registry configuration for the Organization specified
         """
         pass
 
-    def test_update_storage_by_organization_id(self):
+    def test_update_storage_by_organization_id(self) -> None:
         """Test case for update_storage_by_organization_id
 
-        Update storage configuration for the Organization specified  # noqa: E501
+        Update storage configuration for the Organization specified
         """
         pass
 
-    def test_update_tenant_credentials_by_organization_id(self):
+    def test_update_tenant_credentials_by_organization_id(self) -> None:
         """Test case for update_tenant_credentials_by_organization_id
 
-        Update tenant credentials for the Organization specified  # noqa: E501
+        Update tenant credentials for the Organization specified
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_role.py` & `cosmotech_api-3.2.0/test/test_runner_job_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.organization_role import OrganizationRole
+import unittest
 
+from cosmotech_api.models.runner_job_state import RunnerJobState
 
-class TestOrganizationRole(unittest.TestCase):
-    """OrganizationRole unit test stubs"""
+class TestRunnerJobState(unittest.TestCase):
+    """RunnerJobState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationRole(self):
-        """Test OrganizationRole"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = OrganizationRole()  # noqa: E501
-        pass
-
+    def testRunnerJobState(self):
+        """Test RunnerJobState"""
+        # inst = RunnerJobState()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_security.py` & `cosmotech_api-3.2.0/test/test_organization_role.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,53 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.organization_access_control import OrganizationAccessControl
-globals()['OrganizationAccessControl'] = OrganizationAccessControl
-from cosmotech_api.model.organization_security import OrganizationSecurity
+import unittest
 
+from cosmotech_api.models.organization_role import OrganizationRole
 
-class TestOrganizationSecurity(unittest.TestCase):
-    """OrganizationSecurity unit test stubs"""
+class TestOrganizationRole(unittest.TestCase):
+    """OrganizationRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationSecurity(self):
-        """Test OrganizationSecurity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = OrganizationSecurity()  # noqa: E501
-        pass
-
+    def make_instance(self, include_optional) -> OrganizationRole:
+        """Test OrganizationRole
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `OrganizationRole`
+        """
+        model = OrganizationRole()
+        if include_optional:
+            return OrganizationRole(
+                role = ''
+            )
+        else:
+            return OrganizationRole(
+                role = '',
+        )
+        """
+
+    def testOrganizationRole(self):
+        """Test OrganizationRole"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_service.py` & `cosmotech_api-3.2.0/test/test_organization_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,56 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.organization_service import OrganizationService
+import unittest
 
+from cosmotech_api.models.organization_service import OrganizationService
 
 class TestOrganizationService(unittest.TestCase):
     """OrganizationService unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> OrganizationService:
+        """Test OrganizationService
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `OrganizationService`
+        """
+        model = OrganizationService()
+        if include_optional:
+            return OrganizationService(
+                cloud_service = '',
+                base_uri = '',
+                platform_service = '',
+                resource_uri = '',
+                credentials = { }
+            )
+        else:
+            return OrganizationService(
+        )
+        """
+
     def testOrganizationService(self):
         """Test OrganizationService"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = OrganizationService()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_organization_user.py` & `cosmotech_api-3.2.0/test/test_scenario_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.organization_user import OrganizationUser
+from cosmotech_api.model.scenario_user import ScenarioUser
 
 
-class TestOrganizationUser(unittest.TestCase):
-    """OrganizationUser unit test stubs"""
+class TestScenarioUser(unittest.TestCase):
+    """ScenarioUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationUser(self):
-        """Test OrganizationUser"""
+    def testScenarioUser(self):
+        """Test ScenarioUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = OrganizationUser()  # noqa: E501
+        # model = ScenarioUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_container_artifact.py` & `cosmotech_api-3.2.0/test/test_run_container_artifact.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,53 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_container_artifact import RunContainerArtifact
+import unittest
 
+from cosmotech_api.models.run_container_artifact import RunContainerArtifact
 
 class TestRunContainerArtifact(unittest.TestCase):
     """RunContainerArtifact unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunContainerArtifact:
+        """Test RunContainerArtifact
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunContainerArtifact`
+        """
+        model = RunContainerArtifact()
+        if include_optional:
+            return RunContainerArtifact(
+                name = '',
+                path = ''
+            )
+        else:
+            return RunContainerArtifact(
+        )
+        """
+
     def testRunContainerArtifact(self):
         """Test RunContainerArtifact"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunContainerArtifact()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_container_logs.py` & `cosmotech_api-3.2.0/test/test_run_template_step_source.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_container_logs import RunContainerLogs
+import unittest
 
+from cosmotech_api.models.run_template_step_source import RunTemplateStepSource
 
-class TestRunContainerLogs(unittest.TestCase):
-    """RunContainerLogs unit test stubs"""
+class TestRunTemplateStepSource(unittest.TestCase):
+    """RunTemplateStepSource unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRunContainerLogs(self):
-        """Test RunContainerLogs"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunContainerLogs()  # noqa: E501
-        pass
-
+    def testRunTemplateStepSource(self):
+        """Test RunTemplateStepSource"""
+        # inst = RunTemplateStepSource()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_resource_requested.py` & `cosmotech_api-3.2.0/test/test_run_resource_requested.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,53 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_resource_requested import RunResourceRequested
+import unittest
 
+from cosmotech_api.models.run_resource_requested import RunResourceRequested
 
 class TestRunResourceRequested(unittest.TestCase):
     """RunResourceRequested unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunResourceRequested:
+        """Test RunResourceRequested
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunResourceRequested`
+        """
+        model = RunResourceRequested()
+        if include_optional:
+            return RunResourceRequested(
+                cpu = 56,
+                memory = 56
+            )
+        else:
+            return RunResourceRequested(
+        )
+        """
+
     def testRunResourceRequested(self):
         """Test RunResourceRequested"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunResourceRequested()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_search.py` & `cosmotech_api-3.2.0/test/test_run_template_handler_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_search import RunSearch
+import unittest
 
+from cosmotech_api.models.run_template_handler_id import RunTemplateHandlerId
 
-class TestRunSearch(unittest.TestCase):
-    """RunSearch unit test stubs"""
+class TestRunTemplateHandlerId(unittest.TestCase):
+    """RunTemplateHandlerId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRunSearch(self):
-        """Test RunSearch"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunSearch()  # noqa: E501
-        pass
-
+    def testRunTemplateHandlerId(self):
+        """Test RunTemplateHandlerId"""
+        # inst = RunTemplateHandlerId()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_template_parameter.py` & `cosmotech_api-3.2.0/test/test_run_template_parameter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,62 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.translated_labels import TranslatedLabels
-globals()['TranslatedLabels'] = TranslatedLabels
-from cosmotech_api.model.run_template_parameter import RunTemplateParameter
+import unittest
 
+from cosmotech_api.models.run_template_parameter import RunTemplateParameter
 
 class TestRunTemplateParameter(unittest.TestCase):
     """RunTemplateParameter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunTemplateParameter:
+        """Test RunTemplateParameter
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunTemplateParameter`
+        """
+        model = RunTemplateParameter()
+        if include_optional:
+            return RunTemplateParameter(
+                id = '',
+                labels = {
+                    'key' : ''
+                    },
+                var_type = '',
+                default_value = '',
+                min_value = '',
+                max_value = '',
+                regex_validation = '',
+                options = { }
+            )
+        else:
+            return RunTemplateParameter(
+                id = '',
+        )
+        """
+
     def testRunTemplateParameter(self):
         """Test RunTemplateParameter"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunTemplateParameter()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_template_parameter_value.py` & `cosmotech_api-3.2.0/test/test_run_template_parameter_value.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,56 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_template_parameter_value import RunTemplateParameterValue
+import unittest
 
+from cosmotech_api.models.run_template_parameter_value import RunTemplateParameterValue
 
 class TestRunTemplateParameterValue(unittest.TestCase):
     """RunTemplateParameterValue unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunTemplateParameterValue:
+        """Test RunTemplateParameterValue
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunTemplateParameterValue`
+        """
+        model = RunTemplateParameterValue()
+        if include_optional:
+            return RunTemplateParameterValue(
+                parameter_id = '',
+                var_type = '',
+                value = ''
+            )
+        else:
+            return RunTemplateParameterValue(
+                parameter_id = '',
+                value = '',
+        )
+        """
+
     def testRunTemplateParameterValue(self):
         """Test RunTemplateParameterValue"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunTemplateParameterValue()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_run_template_resource_sizing.py` & `cosmotech_api-3.2.0/test/test_run_template_resource_sizing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,63 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.resource_size_info import ResourceSizeInfo
-globals()['ResourceSizeInfo'] = ResourceSizeInfo
-from cosmotech_api.model.run_template_resource_sizing import RunTemplateResourceSizing
+import unittest
 
+from cosmotech_api.models.run_template_resource_sizing import RunTemplateResourceSizing
 
 class TestRunTemplateResourceSizing(unittest.TestCase):
     """RunTemplateResourceSizing unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunTemplateResourceSizing:
+        """Test RunTemplateResourceSizing
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunTemplateResourceSizing`
+        """
+        model = RunTemplateResourceSizing()
+        if include_optional:
+            return RunTemplateResourceSizing(
+                requests = cosmotech_api.models.resource_size_info.ResourceSizeInfo(
+                    cpu = '', 
+                    memory = '', ),
+                limits = cosmotech_api.models.resource_size_info.ResourceSizeInfo(
+                    cpu = '', 
+                    memory = '', )
+            )
+        else:
+            return RunTemplateResourceSizing(
+                requests = cosmotech_api.models.resource_size_info.ResourceSizeInfo(
+                    cpu = '', 
+                    memory = '', ),
+                limits = cosmotech_api.models.resource_size_info.ResourceSizeInfo(
+                    cpu = '', 
+                    memory = '', ),
+        )
+        """
+
     def testRunTemplateResourceSizing(self):
         """Test RunTemplateResourceSizing"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunTemplateResourceSizing()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_runner_access_control.py` & `cosmotech_api-3.2.0/test/test_runner_validation_status.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.runner_access_control import RunnerAccessControl
+import unittest
 
+from cosmotech_api.models.runner_validation_status import RunnerValidationStatus
 
-class TestRunnerAccessControl(unittest.TestCase):
-    """RunnerAccessControl unit test stubs"""
+class TestRunnerValidationStatus(unittest.TestCase):
+    """RunnerValidationStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRunnerAccessControl(self):
-        """Test RunnerAccessControl"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunnerAccessControl()  # noqa: E501
-        pass
-
+    def testRunnerValidationStatus(self):
+        """Test RunnerValidationStatus"""
+        # inst = RunnerValidationStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_runner_api.py` & `cosmotech_api-3.2.0/test/test_runner_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,137 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import unittest
 
-import cosmotech_api
-from cosmotech_api.api.runner_api import RunnerApi  # noqa: E501
+from cosmotech_api.api.runner_api import RunnerApi
 
 
 class TestRunnerApi(unittest.TestCase):
     """RunnerApi unit test stubs"""
 
-    def setUp(self):
-        self.api = RunnerApi()  # noqa: E501
+    def setUp(self) -> None:
+        self.api = RunnerApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    def test_add_runner_access_control(self):
+    def test_add_runner_access_control(self) -> None:
         """Test case for add_runner_access_control
 
-        Add a control access to the Runner  # noqa: E501
+        Add a control access to the Runner
         """
         pass
 
-    def test_create_runner(self):
+    def test_create_runner(self) -> None:
         """Test case for create_runner
 
-        Create a new Runner  # noqa: E501
+        Create a new Runner
         """
         pass
 
-    def test_delete_runner(self):
+    def test_delete_runner(self) -> None:
         """Test case for delete_runner
 
-        Delete a runner  # noqa: E501
+        Delete a runner
         """
         pass
 
-    def test_get_runner(self):
+    def test_get_runner(self) -> None:
         """Test case for get_runner
 
-        Get the details of an runner  # noqa: E501
+        Get the details of an runner
         """
         pass
 
-    def test_get_runner_access_control(self):
+    def test_get_runner_access_control(self) -> None:
         """Test case for get_runner_access_control
 
-        Get a control access for the Runner  # noqa: E501
+        Get a control access for the Runner
         """
         pass
 
-    def test_get_runner_permissions(self):
+    def test_get_runner_permissions(self) -> None:
         """Test case for get_runner_permissions
 
-        Get the Runner permission by given role  # noqa: E501
+        Get the Runner permission by given role
         """
         pass
 
-    def test_get_runner_security(self):
+    def test_get_runner_security(self) -> None:
         """Test case for get_runner_security
 
-        Get the Runner security information  # noqa: E501
+        Get the Runner security information
         """
         pass
 
-    def test_get_runner_security_users(self):
+    def test_get_runner_security_users(self) -> None:
         """Test case for get_runner_security_users
 
-        Get the Runner security users list  # noqa: E501
+        Get the Runner security users list
         """
         pass
 
-    def test_list_runners(self):
+    def test_list_runners(self) -> None:
         """Test case for list_runners
 
-        List all Runners  # noqa: E501
+        List all Runners
         """
         pass
 
-    def test_remove_runner_access_control(self):
+    def test_remove_runner_access_control(self) -> None:
         """Test case for remove_runner_access_control
 
-        Remove the specified access from the given Organization Runner  # noqa: E501
+        Remove the specified access from the given Organization Runner
         """
         pass
 
-    def test_set_runner_default_security(self):
+    def test_set_runner_default_security(self) -> None:
         """Test case for set_runner_default_security
 
-        Set the Runner default security  # noqa: E501
+        Set the Runner default security
         """
         pass
 
-    def test_start_run(self):
+    def test_start_run(self) -> None:
         """Test case for start_run
 
-        Start a run with runner parameters  # noqa: E501
+        Start a run with runner parameters
         """
         pass
 
-    def test_stop_run(self):
+    def test_stop_run(self) -> None:
         """Test case for stop_run
 
-        Stop the last run  # noqa: E501
+        Stop the last run
         """
         pass
 
-    def test_update_runner(self):
+    def test_update_runner(self) -> None:
         """Test case for update_runner
 
-        Update a runner  # noqa: E501
+        Update a runner
         """
         pass
 
-    def test_update_runner_access_control(self):
+    def test_update_runner_access_control(self) -> None:
         """Test case for update_runner_access_control
 
-        Update the specified access to User for a Runner  # noqa: E501
+        Update the specified access to User for a Runner
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_runner_comparison_result.py` & `cosmotech_api-3.2.0/test/test_runner_comparison_result.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,60 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.runner_changed_parameter_value import RunnerChangedParameterValue
-globals()['RunnerChangedParameterValue'] = RunnerChangedParameterValue
-from cosmotech_api.model.runner_comparison_result import RunnerComparisonResult
+import unittest
 
+from cosmotech_api.models.runner_comparison_result import RunnerComparisonResult
 
 class TestRunnerComparisonResult(unittest.TestCase):
     """RunnerComparisonResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> RunnerComparisonResult:
+        """Test RunnerComparisonResult
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RunnerComparisonResult`
+        """
+        model = RunnerComparisonResult()
+        if include_optional:
+            return RunnerComparisonResult(
+                runner_id = '',
+                compared_runner_id = '',
+                changed_values = [
+                    cosmotech_api.models.runner_changed_parameter_value.RunnerChangedParameterValue(
+                        parameter_id = '', 
+                        var_type = '', 
+                        value = '', 
+                        compared_value = '', )
+                    ]
+            )
+        else:
+            return RunnerComparisonResult(
+        )
+        """
+
     def testRunnerComparisonResult(self):
         """Test RunnerComparisonResult"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunnerComparisonResult()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_runner_last_run.py` & `cosmotech_api-3.2.0/test/test_scenario_validation_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.runner_last_run import RunnerLastRun
+import unittest
 
+from cosmotech_api.models.scenario_validation_status import ScenarioValidationStatus
 
-class TestRunnerLastRun(unittest.TestCase):
-    """RunnerLastRun unit test stubs"""
+class TestScenarioValidationStatus(unittest.TestCase):
+    """ScenarioValidationStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRunnerLastRun(self):
-        """Test RunnerLastRun"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunnerLastRun()  # noqa: E501
-        pass
-
+    def testScenarioValidationStatus(self):
+        """Test ScenarioValidationStatus"""
+        # inst = ScenarioValidationStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_runner_parent_last_run.py` & `cosmotech_api-3.2.0/test/test_runner_parent_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/test/test_runner_root_last_run.py` & `cosmotech_api-3.2.0/test/test_runner_root_last_run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/test/test_runner_security.py` & `cosmotech_api-3.2.0/test/test_workspace_secret.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,52 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.runner_access_control import RunnerAccessControl
-globals()['RunnerAccessControl'] = RunnerAccessControl
-from cosmotech_api.model.runner_security import RunnerSecurity
+import unittest
 
+from cosmotech_api.models.workspace_secret import WorkspaceSecret
 
-class TestRunnerSecurity(unittest.TestCase):
-    """RunnerSecurity unit test stubs"""
+class TestWorkspaceSecret(unittest.TestCase):
+    """WorkspaceSecret unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRunnerSecurity(self):
-        """Test RunnerSecurity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = RunnerSecurity()  # noqa: E501
-        pass
-
+    def make_instance(self, include_optional) -> WorkspaceSecret:
+        """Test WorkspaceSecret
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `WorkspaceSecret`
+        """
+        model = WorkspaceSecret()
+        if include_optional:
+            return WorkspaceSecret(
+                dedicated_event_hub_key = ''
+            )
+        else:
+            return WorkspaceSecret(
+        )
+        """
+
+    def testWorkspaceSecret(self):
+        """Test WorkspaceSecret"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario.py` & `cosmotech_api-3.2.0/test/test_scenario_run_logs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,61 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_job_state import ScenarioJobState
-from cosmotech_api.model.scenario_last_run import ScenarioLastRun
-from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
-from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
-from cosmotech_api.model.scenario_security import ScenarioSecurity
-from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
-globals()['ScenarioJobState'] = ScenarioJobState
-globals()['ScenarioLastRun'] = ScenarioLastRun
-globals()['ScenarioResourceSizing'] = ScenarioResourceSizing
-globals()['ScenarioRunTemplateParameterValue'] = ScenarioRunTemplateParameterValue
-globals()['ScenarioSecurity'] = ScenarioSecurity
-globals()['ScenarioValidationStatus'] = ScenarioValidationStatus
-from cosmotech_api.model.scenario import Scenario
+import unittest
 
+from cosmotech_api.models.scenario_run_logs import ScenarioRunLogs
 
-class TestScenario(unittest.TestCase):
-    """Scenario unit test stubs"""
+class TestScenarioRunLogs(unittest.TestCase):
+    """ScenarioRunLogs unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenario(self):
-        """Test Scenario"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Scenario()  # noqa: E501
-        pass
-
+    def make_instance(self, include_optional) -> ScenarioRunLogs:
+        """Test ScenarioRunLogs
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ScenarioRunLogs`
+        """
+        model = ScenarioRunLogs()
+        if include_optional:
+            return ScenarioRunLogs(
+                scenariorun_id = '',
+                containers = {
+                    'key' : cosmotech_api.models.scenario_run_container_logs.ScenarioRunContainerLogs(
+                        node_id = '', 
+                        container_name = '', 
+                        children = [
+                            ''
+                            ], 
+                        logs = '', )
+                    }
+            )
+        else:
+            return ScenarioRunLogs(
+        )
+        """
+
+    def testScenarioRunLogs(self):
+        """Test ScenarioRunLogs"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_api.py` & `cosmotech_api-3.2.0/test/test_scenario_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,186 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import unittest
 
-import cosmotech_api
-from cosmotech_api.api.scenario_api import ScenarioApi  # noqa: E501
+from cosmotech_api.api.scenario_api import ScenarioApi
 
 
 class TestScenarioApi(unittest.TestCase):
     """ScenarioApi unit test stubs"""
 
-    def setUp(self):
-        self.api = ScenarioApi()  # noqa: E501
+    def setUp(self) -> None:
+        self.api = ScenarioApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    def test_add_or_replace_scenario_parameter_values(self):
+    def test_add_or_replace_scenario_parameter_values(self) -> None:
         """Test case for add_or_replace_scenario_parameter_values
 
-        Add (or replace) Parameter Values for the Scenario specified  # noqa: E501
+        Add (or replace) Parameter Values for the Scenario specified
         """
         pass
 
-    def test_add_scenario_access_control(self):
+    def test_add_scenario_access_control(self) -> None:
         """Test case for add_scenario_access_control
 
-        Add a control access to the Scenario  # noqa: E501
+        Add a control access to the Scenario
         """
         pass
 
-    def test_compare_scenarios(self):
+    def test_compare_scenarios(self) -> None:
         """Test case for compare_scenarios
 
-        Compare the Scenario with another one and returns the difference for parameters values  # noqa: E501
+        Compare the Scenario with another one and returns the difference for parameters values
         """
         pass
 
-    def test_create_scenario(self):
+    def test_create_scenario(self) -> None:
         """Test case for create_scenario
 
-        Create a new Scenario  # noqa: E501
+        Create a new Scenario
         """
         pass
 
-    def test_delete_all_scenarios(self):
+    def test_delete_all_scenarios(self) -> None:
         """Test case for delete_all_scenarios
 
-        Delete all Scenarios of the Workspace  # noqa: E501
+        Delete all Scenarios of the Workspace
         """
         pass
 
-    def test_delete_scenario(self):
+    def test_delete_scenario(self) -> None:
         """Test case for delete_scenario
 
-        Delete a scenario  # noqa: E501
+        Delete a scenario
         """
         pass
 
-    def test_download_scenario_data(self):
+    def test_download_scenario_data(self) -> None:
         """Test case for download_scenario_data
 
-        Download Scenario data  # noqa: E501
+        Download Scenario data
         """
         pass
 
-    def test_find_all_scenarios(self):
+    def test_find_all_scenarios(self) -> None:
         """Test case for find_all_scenarios
 
-        List all Scenarios  # noqa: E501
+        List all Scenarios
         """
         pass
 
-    def test_find_all_scenarios_by_validation_status(self):
+    def test_find_all_scenarios_by_validation_status(self) -> None:
         """Test case for find_all_scenarios_by_validation_status
 
-        List all Scenarios by validation status  # noqa: E501
+        List all Scenarios by validation status
         """
         pass
 
-    def test_find_scenario_by_id(self):
+    def test_find_scenario_by_id(self) -> None:
         """Test case for find_scenario_by_id
 
-        Get the details of an scenario  # noqa: E501
+        Get the details of an scenario
         """
         pass
 
-    def test_get_scenario_access_control(self):
+    def test_get_scenario_access_control(self) -> None:
         """Test case for get_scenario_access_control
 
-        Get a control access for the Scenario  # noqa: E501
+        Get a control access for the Scenario
         """
         pass
 
-    def test_get_scenario_data_download_job_info(self):
+    def test_get_scenario_data_download_job_info(self) -> None:
         """Test case for get_scenario_data_download_job_info
 
-        Get Scenario data download URL  # noqa: E501
+        Get Scenario data download URL
         """
         pass
 
-    def test_get_scenario_permissions(self):
+    def test_get_scenario_permissions(self) -> None:
         """Test case for get_scenario_permissions
 
-        Get the Scenario permission by given role  # noqa: E501
+        Get the Scenario permission by given role
         """
         pass
 
-    def test_get_scenario_security(self):
+    def test_get_scenario_security(self) -> None:
         """Test case for get_scenario_security
 
-        Get the Scenario security information  # noqa: E501
+        Get the Scenario security information
         """
         pass
 
-    def test_get_scenario_security_users(self):
+    def test_get_scenario_security_users(self) -> None:
         """Test case for get_scenario_security_users
 
-        Get the Scenario security users list  # noqa: E501
+        Get the Scenario security users list
         """
         pass
 
-    def test_get_scenario_validation_status_by_id(self):
+    def test_get_scenario_validation_status_by_id(self) -> None:
         """Test case for get_scenario_validation_status_by_id
 
-        Get the validation status of an scenario  # noqa: E501
+        Get the validation status of an scenario
         """
         pass
 
-    def test_get_scenarios_tree(self):
+    def test_get_scenarios_tree(self) -> None:
         """Test case for get_scenarios_tree
 
-        Get the Scenarios Tree  # noqa: E501
+        Get the Scenarios Tree
         """
         pass
 
-    def test_remove_all_scenario_parameter_values(self):
+    def test_remove_all_scenario_parameter_values(self) -> None:
         """Test case for remove_all_scenario_parameter_values
 
-        Remove all Parameter Values from the Scenario specified  # noqa: E501
+        Remove all Parameter Values from the Scenario specified
         """
         pass
 
-    def test_remove_scenario_access_control(self):
+    def test_remove_scenario_access_control(self) -> None:
         """Test case for remove_scenario_access_control
 
-        Remove the specified access from the given Organization Scenario  # noqa: E501
+        Remove the specified access from the given Organization Scenario
         """
         pass
 
-    def test_set_scenario_default_security(self):
+    def test_set_scenario_default_security(self) -> None:
         """Test case for set_scenario_default_security
 
-        Set the Scenario default security  # noqa: E501
+        Set the Scenario default security
         """
         pass
 
-    def test_update_scenario(self):
+    def test_update_scenario(self) -> None:
         """Test case for update_scenario
 
-        Update a scenario  # noqa: E501
+        Update a scenario
         """
         pass
 
-    def test_update_scenario_access_control(self):
+    def test_update_scenario_access_control(self) -> None:
         """Test case for update_scenario_access_control
 
-        Update the specified access to User for a Scenario  # noqa: E501
+        Update the specified access to User for a Scenario
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_comparison_result.py` & `cosmotech_api-3.2.0/test/test_scenario_comparison_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,60 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_changed_parameter_value import ScenarioChangedParameterValue
-globals()['ScenarioChangedParameterValue'] = ScenarioChangedParameterValue
-from cosmotech_api.model.scenario_comparison_result import ScenarioComparisonResult
+import unittest
 
+from cosmotech_api.models.scenario_comparison_result import ScenarioComparisonResult
 
 class TestScenarioComparisonResult(unittest.TestCase):
     """ScenarioComparisonResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> ScenarioComparisonResult:
+        """Test ScenarioComparisonResult
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ScenarioComparisonResult`
+        """
+        model = ScenarioComparisonResult()
+        if include_optional:
+            return ScenarioComparisonResult(
+                scenario_id = '',
+                compared_scenario_id = '',
+                changed_values = [
+                    cosmotech_api.models.scenario_changed_parameter_value.ScenarioChangedParameterValue(
+                        parameter_id = '', 
+                        var_type = '', 
+                        value = '', 
+                        compared_value = '', )
+                    ]
+            )
+        else:
+            return ScenarioComparisonResult(
+        )
+        """
+
     def testScenarioComparisonResult(self):
         """Test ScenarioComparisonResult"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioComparisonResult()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_run.py` & `cosmotech_api-3.2.0/test/test_scenario_run_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,57 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.run_template_parameter_value import RunTemplateParameterValue
-from cosmotech_api.model.scenario_run_container import ScenarioRunContainer
-from cosmotech_api.model.scenario_run_state import ScenarioRunState
-globals()['RunTemplateParameterValue'] = RunTemplateParameterValue
-globals()['ScenarioRunContainer'] = ScenarioRunContainer
-globals()['ScenarioRunState'] = ScenarioRunState
-from cosmotech_api.model.scenario_run import ScenarioRun
+import unittest
 
+from cosmotech_api.models.scenario_run_result import ScenarioRunResult
 
-class TestScenarioRun(unittest.TestCase):
-    """ScenarioRun unit test stubs"""
+class TestScenarioRunResult(unittest.TestCase):
+    """ScenarioRunResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRun(self):
-        """Test ScenarioRun"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRun()  # noqa: E501
-        pass
-
+    def make_instance(self, include_optional) -> ScenarioRunResult:
+        """Test ScenarioRunResult
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ScenarioRunResult`
+        """
+        model = ScenarioRunResult()
+        if include_optional:
+            return ScenarioRunResult(
+                id = '',
+                results = [
+                    {
+                        'key' : ''
+                        }
+                    ]
+            )
+        else:
+            return ScenarioRunResult(
+        )
+        """
+
+    def testScenarioRunResult(self):
+        """Test ScenarioRunResult"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_run_logs.py` & `cosmotech_api-3.2.0/test/test_scenario_run_container_logs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,57 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_run_container_logs import ScenarioRunContainerLogs
-globals()['ScenarioRunContainerLogs'] = ScenarioRunContainerLogs
-from cosmotech_api.model.scenario_run_logs import ScenarioRunLogs
+import unittest
 
+from cosmotech_api.models.scenario_run_container_logs import ScenarioRunContainerLogs
 
-class TestScenarioRunLogs(unittest.TestCase):
-    """ScenarioRunLogs unit test stubs"""
+class TestScenarioRunContainerLogs(unittest.TestCase):
+    """ScenarioRunContainerLogs unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunLogs(self):
-        """Test ScenarioRunLogs"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunLogs()  # noqa: E501
-        pass
-
+    def make_instance(self, include_optional) -> ScenarioRunContainerLogs:
+        """Test ScenarioRunContainerLogs
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ScenarioRunContainerLogs`
+        """
+        model = ScenarioRunContainerLogs()
+        if include_optional:
+            return ScenarioRunContainerLogs(
+                node_id = '',
+                container_name = '',
+                children = [
+                    ''
+                    ],
+                logs = ''
+            )
+        else:
+            return ScenarioRunContainerLogs(
+        )
+        """
+
+    def testScenarioRunContainerLogs(self):
+        """Test ScenarioRunContainerLogs"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_run_start_containers.py` & `cosmotech_api-3.2.0/test/test_scenario_job_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,34 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_run_container import ScenarioRunContainer
-globals()['ScenarioRunContainer'] = ScenarioRunContainer
-from cosmotech_api.model.scenario_run_start_containers import ScenarioRunStartContainers
+import unittest
 
+from cosmotech_api.models.scenario_job_state import ScenarioJobState
 
-class TestScenarioRunStartContainers(unittest.TestCase):
-    """ScenarioRunStartContainers unit test stubs"""
+class TestScenarioJobState(unittest.TestCase):
+    """ScenarioJobState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunStartContainers(self):
-        """Test ScenarioRunStartContainers"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunStartContainers()  # noqa: E501
-        pass
-
+    def testScenarioJobState(self):
+        """Test ScenarioJobState"""
+        # inst = ScenarioJobState()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_security.py` & `cosmotech_api-3.2.0/test/test_scenario_security.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,63 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
-globals()['ScenarioAccessControl'] = ScenarioAccessControl
-from cosmotech_api.model.scenario_security import ScenarioSecurity
+import unittest
 
+from cosmotech_api.models.scenario_security import ScenarioSecurity
 
 class TestScenarioSecurity(unittest.TestCase):
     """ScenarioSecurity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> ScenarioSecurity:
+        """Test ScenarioSecurity
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ScenarioSecurity`
+        """
+        model = ScenarioSecurity()
+        if include_optional:
+            return ScenarioSecurity(
+                default = '',
+                access_control_list = [
+                    cosmotech_api.models.scenario_access_control.ScenarioAccessControl(
+                        id = '', 
+                        role = '', )
+                    ]
+            )
+        else:
+            return ScenarioSecurity(
+                default = '',
+                access_control_list = [
+                    cosmotech_api.models.scenario_access_control.ScenarioAccessControl(
+                        id = '', 
+                        role = '', )
+                    ],
+        )
+        """
+
     def testScenarioSecurity(self):
         """Test ScenarioSecurity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioSecurity()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenario_validation_status.py` & `cosmotech_api-3.2.0/test/test_scenariorunresult_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,46 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-import sys
 import unittest
 
-import cosmotech_api
-from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
+from cosmotech_api.api.scenariorunresult_api import ScenariorunresultApi
 
 
-class TestScenarioValidationStatus(unittest.TestCase):
-    """ScenarioValidationStatus unit test stubs"""
+class TestScenariorunresultApi(unittest.TestCase):
+    """ScenariorunresultApi unit test stubs"""
 
-    def setUp(self):
+    def setUp(self) -> None:
+        self.api = ScenariorunresultApi()
+
+    def tearDown(self) -> None:
         pass
 
-    def tearDown(self):
+    def test_get_scenario_run_result(self) -> None:
+        """Test case for get_scenario_run_result
+
+        Get a ScenarioRunResult in the Organization
+        """
         pass
 
-    def testScenarioValidationStatus(self):
-        """Test ScenarioValidationStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioValidationStatus()  # noqa: E501
+    def test_send_scenario_run_result(self) -> None:
+        """Test case for send_scenario_run_result
+
+        Create a new ScenarioRunResult in the Organization
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_scenariorun_api.py` & `cosmotech_api-3.2.0/test/test_scenariorun_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,130 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import unittest
 
-import cosmotech_api
-from cosmotech_api.api.scenariorun_api import ScenariorunApi  # noqa: E501
+from cosmotech_api.api.scenariorun_api import ScenariorunApi
 
 
 class TestScenariorunApi(unittest.TestCase):
     """ScenariorunApi unit test stubs"""
 
-    def setUp(self):
-        self.api = ScenariorunApi()  # noqa: E501
+    def setUp(self) -> None:
+        self.api = ScenariorunApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    def test_delete_historical_data_organization(self):
+    def test_delete_historical_data_organization(self) -> None:
         """Test case for delete_historical_data_organization
 
-        Delete all historical ScenarioRuns in the Organization  # noqa: E501
+        Delete all historical ScenarioRuns in the Organization
         """
         pass
 
-    def test_delete_historical_data_scenario(self):
+    def test_delete_historical_data_scenario(self) -> None:
         """Test case for delete_historical_data_scenario
 
-        Delete all historical ScenarioRuns in the Scenario  # noqa: E501
+        Delete all historical ScenarioRuns in the Scenario
         """
         pass
 
-    def test_delete_historical_data_workspace(self):
+    def test_delete_historical_data_workspace(self) -> None:
         """Test case for delete_historical_data_workspace
 
-        Delete all historical ScenarioRuns in the Workspace  # noqa: E501
+        Delete all historical ScenarioRuns in the Workspace
         """
         pass
 
-    def test_delete_scenario_run(self):
+    def test_delete_scenario_run(self) -> None:
         """Test case for delete_scenario_run
 
-        Delete a scenariorun  # noqa: E501
+        Delete a scenariorun
         """
         pass
 
-    def test_find_scenario_run_by_id(self):
+    def test_find_scenario_run_by_id(self) -> None:
         """Test case for find_scenario_run_by_id
 
-        Get the details of a scenariorun  # noqa: E501
+        Get the details of a scenariorun
         """
         pass
 
-    def test_get_scenario_run_cumulated_logs(self):
+    def test_get_scenario_run_cumulated_logs(self) -> None:
         """Test case for get_scenario_run_cumulated_logs
 
-        Get the cumulated logs of a scenariorun  # noqa: E501
+        Get the cumulated logs of a scenariorun
         """
         pass
 
-    def test_get_scenario_run_logs(self):
+    def test_get_scenario_run_logs(self) -> None:
         """Test case for get_scenario_run_logs
 
-        get the logs for the ScenarioRun  # noqa: E501
+        get the logs for the ScenarioRun
         """
         pass
 
-    def test_get_scenario_run_status(self):
+    def test_get_scenario_run_status(self) -> None:
         """Test case for get_scenario_run_status
 
-        get the status for the ScenarioRun  # noqa: E501
+        get the status for the ScenarioRun
         """
         pass
 
-    def test_get_scenario_runs(self):
+    def test_get_scenario_runs(self) -> None:
         """Test case for get_scenario_runs
 
-        get the list of ScenarioRuns for the Scenario  # noqa: E501
+        get the list of ScenarioRuns for the Scenario
         """
         pass
 
-    def test_get_workspace_scenario_runs(self):
+    def test_get_workspace_scenario_runs(self) -> None:
         """Test case for get_workspace_scenario_runs
 
-        get the list of ScenarioRuns for the Workspace  # noqa: E501
+        get the list of ScenarioRuns for the Workspace
         """
         pass
 
-    def test_run_scenario(self):
+    def test_run_scenario(self) -> None:
         """Test case for run_scenario
 
-        run a ScenarioRun for the Scenario  # noqa: E501
+        run a ScenarioRun for the Scenario
         """
         pass
 
-    def test_search_scenario_runs(self):
+    def test_search_scenario_runs(self) -> None:
         """Test case for search_scenario_runs
 
-        Search ScenarioRuns  # noqa: E501
+        Search ScenarioRuns
         """
         pass
 
-    def test_start_scenario_run_containers(self):
+    def test_start_scenario_run_containers(self) -> None:
         """Test case for start_scenario_run_containers
 
-        Start a new scenariorun with raw containers definition  # noqa: E501
+        Start a new scenariorun with raw containers definition
         """
         pass
 
-    def test_stop_scenario_run(self):
+    def test_stop_scenario_run(self) -> None:
         """Test case for stop_scenario_run
 
-        stop a ScenarioRun for the Scenario  # noqa: E501
+        stop a ScenarioRun for the Scenario
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_sub_dataset_graph_query.py` & `cosmotech_api-3.2.0/test/test_sub_dataset_graph_query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,57 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.sub_dataset_graph_query import SubDatasetGraphQuery
+import unittest
 
+from cosmotech_api.models.sub_dataset_graph_query import SubDatasetGraphQuery
 
 class TestSubDatasetGraphQuery(unittest.TestCase):
     """SubDatasetGraphQuery unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> SubDatasetGraphQuery:
+        """Test SubDatasetGraphQuery
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SubDatasetGraphQuery`
+        """
+        model = SubDatasetGraphQuery()
+        if include_optional:
+            return SubDatasetGraphQuery(
+                name = '',
+                description = '',
+                queries = [
+                    ''
+                    ],
+                main = True
+            )
+        else:
+            return SubDatasetGraphQuery(
+        )
+        """
+
     def testSubDatasetGraphQuery(self):
         """Test SubDatasetGraphQuery"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = SubDatasetGraphQuery()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_twin_graph_query.py` & `cosmotech_api-3.2.0/test/test_twin_graph_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,54 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.twin_graph_query import TwinGraphQuery
+import unittest
 
+from cosmotech_api.models.twin_graph_query import TwinGraphQuery
 
 class TestTwinGraphQuery(unittest.TestCase):
     """TwinGraphQuery unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> TwinGraphQuery:
+        """Test TwinGraphQuery
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TwinGraphQuery`
+        """
+        model = TwinGraphQuery()
+        if include_optional:
+            return TwinGraphQuery(
+                version = '',
+                query = ''
+            )
+        else:
+            return TwinGraphQuery(
+                query = '',
+        )
+        """
+
     def testTwinGraphQuery(self):
         """Test TwinGraphQuery"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphQuery()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_user_api.py` & `cosmotech_api-3.2.0/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-api-3.1.1/test/test_validator_api.py` & `cosmotech_api-3.2.0/test/test_validator_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,95 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import unittest
 
-import cosmotech_api
-from cosmotech_api.api.validator_api import ValidatorApi  # noqa: E501
+from cosmotech_api.api.validator_api import ValidatorApi
 
 
 class TestValidatorApi(unittest.TestCase):
     """ValidatorApi unit test stubs"""
 
-    def setUp(self):
-        self.api = ValidatorApi()  # noqa: E501
+    def setUp(self) -> None:
+        self.api = ValidatorApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    def test_create_validator(self):
+    def test_create_validator(self) -> None:
         """Test case for create_validator
 
-        Register a new validator  # noqa: E501
+        Register a new validator
         """
         pass
 
-    def test_create_validator_run(self):
+    def test_create_validator_run(self) -> None:
         """Test case for create_validator_run
 
-        Register a new validator run  # noqa: E501
+        Register a new validator run
         """
         pass
 
-    def test_delete_validator(self):
+    def test_delete_validator(self) -> None:
         """Test case for delete_validator
 
-        Delete a validator  # noqa: E501
+        Delete a validator
         """
         pass
 
-    def test_delete_validator_run(self):
+    def test_delete_validator_run(self) -> None:
         """Test case for delete_validator_run
 
-        Delete a validator run  # noqa: E501
+        Delete a validator run
         """
         pass
 
-    def test_find_all_validator_runs(self):
+    def test_find_all_validator_runs(self) -> None:
         """Test case for find_all_validator_runs
 
-        List all Validator Runs  # noqa: E501
+        List all Validator Runs
         """
         pass
 
-    def test_find_all_validators(self):
+    def test_find_all_validators(self) -> None:
         """Test case for find_all_validators
 
-        List all Validators  # noqa: E501
+        List all Validators
         """
         pass
 
-    def test_find_validator_by_id(self):
+    def test_find_validator_by_id(self) -> None:
         """Test case for find_validator_by_id
 
-        Get the details of a validator  # noqa: E501
+        Get the details of a validator
         """
         pass
 
-    def test_find_validator_run_by_id(self):
+    def test_find_validator_run_by_id(self) -> None:
         """Test case for find_validator_run_by_id
 
-        Get the details of a validator run  # noqa: E501
+        Get the details of a validator run
         """
         pass
 
-    def test_run_validator(self):
+    def test_run_validator(self) -> None:
         """Test case for run_validator
 
-        Run a Validator  # noqa: E501
+        Run a Validator
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-3.1.1/test/test_workspace_security.py` & `cosmotech_api-3.2.0/test/test_workspace_security.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,63 @@
+# coding: utf-8
+
 """
     Cosmo Tech Platform API
 
-    Cosmo Tech Platform API  # noqa: E501
+    Cosmo Tech Platform API
 
-    The version of the OpenAPI document: 3.1.1
+    The version of the OpenAPI document: 3.1.1-SNAPSHOT
     Contact: platform@cosmotech.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import sys
-import unittest
 
-import cosmotech_api
-from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
-globals()['WorkspaceAccessControl'] = WorkspaceAccessControl
-from cosmotech_api.model.workspace_security import WorkspaceSecurity
+import unittest
 
+from cosmotech_api.models.workspace_security import WorkspaceSecurity
 
 class TestWorkspaceSecurity(unittest.TestCase):
     """WorkspaceSecurity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
+    def make_instance(self, include_optional) -> WorkspaceSecurity:
+        """Test WorkspaceSecurity
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `WorkspaceSecurity`
+        """
+        model = WorkspaceSecurity()
+        if include_optional:
+            return WorkspaceSecurity(
+                default = '',
+                access_control_list = [
+                    cosmotech_api.models.workspace_access_control.WorkspaceAccessControl(
+                        id = '', 
+                        role = '', )
+                    ]
+            )
+        else:
+            return WorkspaceSecurity(
+                default = '',
+                access_control_list = [
+                    cosmotech_api.models.workspace_access_control.WorkspaceAccessControl(
+                        id = '', 
+                        role = '', )
+                    ],
+        )
+        """
+
     def testWorkspaceSecurity(self):
         """Test WorkspaceSecurity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceSecurity()  # noqa: E501
-        pass
-
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```


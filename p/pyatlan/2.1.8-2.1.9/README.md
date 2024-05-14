# Comparing `tmp/pyatlan-2.1.8.tar.gz` & `tmp/pyatlan-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-2.1.8.tar", last modified: Wed May  8 12:28:24 2024, max compression
+gzip compressed data, was "pyatlan-2.1.9.tar", last modified: Tue May 14 15:10:41 2024, max compression
```

## Comparing `pyatlan-2.1.8.tar` & `pyatlan-2.1.9.tar`

### file list

```diff
@@ -1,481 +1,492 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.508564 pyatlan-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-08 12:28:18.000000 pyatlan-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 12:28:18.000000 pyatlan-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 12:28:18.000000 pyatlan-2.1.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 12:28:24.508564 pyatlan-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-08 12:28:18.000000 pyatlan-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.436564 pyatlan-2.1.8/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.436564 pyatlan-2.1.8/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.440564 pyatlan-2.1.8/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.444564 pyatlan-2.1.8/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/events/atlan_lambda_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.444564 pyatlan-2.1.8/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32114 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/create_typedefs_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.444564 pyatlan-2.1.8/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/enums.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/globals.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/properties.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/referenceable_attributes.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/referenceable_methods.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/generator/templates/structs.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.448564 pyatlan-2.1.8/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/api_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.488564 pyatlan-2.1.8/pyatlan/model/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_p_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_p_i_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_p_i_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/a_w_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)   122057 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/auth_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/azure_event_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/azure_event_hub_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/b_i_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/calculation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite3_d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cognite_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cube_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cube_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/cube_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/data_studio_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_model_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/domo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/domo_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/domo_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/domo_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/domo_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/dynamo_dbtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/event_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/g_c_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/g_c_s_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/g_c_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/kafka_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_look.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/looker_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/m_c_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/m_c_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/materialised_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/matillion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/matillion_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/matillion_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/matillion_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/matillion_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/metabase_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/metabase_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/metabase_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_dossier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mode_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/multi_dimensional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/no_s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/power_b_i_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/preset_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/preset_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/preset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/preset_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/process_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/qlik_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_analysis_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dataset_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/quick_sight_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/readme_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/redash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/redash_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/redash_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/redash_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/s3_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/saa_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/salesforce_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/schema_registry_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_data_element_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sigma_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense_datamodel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/sisense_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/snowflake_dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/snowflake_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/snowflake_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/snowflake_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/soda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/soda_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/spark_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/table_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_calculated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_datasource_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tableau_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/tag_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_dashlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/assets/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    76409 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.488564 pyatlan-2.1.8/pyatlan/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/fields/atlan_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/fluent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/fluent_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.492564 pyatlan-2.1.8/pyatlan/model/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.492564 pyatlan-2.1.8/pyatlan/model/packages/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/base/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/base/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/base/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/confluent_kafka_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/dbt_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/glue_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/powerbi_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/sigma_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/snowflake_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/snowflake_miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/sql_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/packages/tableau_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/model/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/multipart_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.492564 pyatlan-2.1.8/pyatlan/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/create_package_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.492564 pyatlan-2.1.8/pyatlan/pkg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/templates/default_configmap.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/templates/default_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/templates/package_config.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/pkg/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 12:28:18.000000 pyatlan-2.1.8/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.508564 pyatlan-2.1.8/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 12:28:24.000000 pyatlan-2.1.8/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 12:28:18.000000 pyatlan-2.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 12:28:18.000000 pyatlan-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:28:24.508564 pyatlan-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-08 12:28:18.000000 pyatlan-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.492564 pyatlan-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.500564 pyatlan-2.1.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/adls_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/airflow_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/api_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/custom_package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/data_mesh_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/gcs_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/owner_propagator_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/preset_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/requests_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_sql_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/test_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.504564 pyatlan-2.1.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.508564 pyatlan-2.1.8/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/a_d_l_s_account_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/a_d_l_s_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/a_d_l_s_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/a_p_i_path_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/a_p_i_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/column_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/data_domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/data_product_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/database_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.508564 pyatlan-2.1.8/tests/unit/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/fields/atlan_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/gcs_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/gcs_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/preset_chart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/preset_dashboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/preset_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/preset_workspace_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/model/view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:24.508564 pyatlan-2.1.8/tests/unit/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/pkg/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    68515 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_credential_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_query_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-08 12:28:18.000000 pyatlan-2.1.8/tests/unit/test_workflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-14 15:10:35.000000 pyatlan-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 15:10:35.000000 pyatlan-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-14 15:10:41.929864 pyatlan-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 15:10:35.000000 pyatlan-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.841863 pyatlan-2.1.9/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.845864 pyatlan-2.1.9/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/atlan_lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/create_typedefs_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/enums.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/globals.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/properties.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/referenceable_attributes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/referenceable_methods.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/structs.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.857864 pyatlan-2.1.9/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/api_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.905864 pyatlan-2.1.9/pyatlan/model/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_w_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/auth_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/b_i_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/calculation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite3_d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_studio_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_model_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_dbtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/event_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_look.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/m_c_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/m_c_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/materialised_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_dossier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/multi_dimensional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/no_s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/process_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/readme_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/saa_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema_registry_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/soda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/soda_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/spark_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/table_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_calculated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tag_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_dashlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.905864 pyatlan-2.1.9/pyatlan/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fields/atlan_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fluent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fluent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/model/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/model/packages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/big_query_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/confluent_kafka_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/dbt_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/dynamo_d_b_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/postgres_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/powerbi_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/s_q_l_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/sigma_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/snowflake_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/snowflake_miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/sql_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/tableau_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/multipart_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/create_package_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.913864 pyatlan-2.1.9/pyatlan/pkg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/default_configmap.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/default_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/package_config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 15:10:35.000000 pyatlan-2.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:10:35.000000 pyatlan-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:10:41.929864 pyatlan-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-14 15:10:35.000000 pyatlan-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.913864 pyatlan-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.917864 pyatlan-2.1.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/adls_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/airflow_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/api_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/custom_package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/data_mesh_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/gcs_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/owner_propagator_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/preset_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/requests_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_sql_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.921864 pyatlan-2.1.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_account_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_p_i_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_p_i_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/column_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/fields/atlan_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/gcs_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/gcs_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_chart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_dashboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_workspace_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68514 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_credential_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_query_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_workflow_client.py
```

### Comparing `pyatlan-2.1.8/LICENSE` & `pyatlan-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/PKG-INFO` & `pyatlan-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.8
+Version: 2.1.9
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.8/README.md` & `pyatlan-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-2.1.9/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-2.1.9/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/enum_cache.py` & `pyatlan-2.1.9/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/group_cache.py` & `pyatlan-2.1.9/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/role_cache.py` & `pyatlan-2.1.9/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/cache/user_cache.py` & `pyatlan-2.1.9/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/admin.py` & `pyatlan-2.1.9/pyatlan/client/admin.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/asset.py` & `pyatlan-2.1.9/pyatlan/client/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/atlan.py` & `pyatlan-2.1.9/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/audit.py` & `pyatlan-2.1.9/pyatlan/client/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/common.py` & `pyatlan-2.1.9/pyatlan/client/common.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/constants.py` & `pyatlan-2.1.9/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/credential.py` & `pyatlan-2.1.9/pyatlan/client/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/file.py` & `pyatlan-2.1.9/pyatlan/client/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/group.py` & `pyatlan-2.1.9/pyatlan/client/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/impersonate.py` & `pyatlan-2.1.9/pyatlan/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/query.py` & `pyatlan-2.1.9/pyatlan/client/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/role.py` & `pyatlan-2.1.9/pyatlan/client/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/search_log.py` & `pyatlan-2.1.9/pyatlan/client/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/sso.py` & `pyatlan-2.1.9/pyatlan/client/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/task.py` & `pyatlan-2.1.9/pyatlan/client/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/token.py` & `pyatlan-2.1.9/pyatlan/client/token.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/typedef.py` & `pyatlan-2.1.9/pyatlan/client/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/user.py` & `pyatlan-2.1.9/pyatlan/client/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/client/workflow.py` & `pyatlan-2.1.9/pyatlan/client/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/errors.py` & `pyatlan-2.1.9/pyatlan/errors.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/events/atlan_event_handler.py` & `pyatlan-2.1.9/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-2.1.9/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/class_generator.py` & `pyatlan-2.1.9/pyatlan/generator/class_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 # helping to prevent inconsistencies
 # across Python versions (e.g: 3.8 and 3.9).
 PARENT = Path(__file__).resolve().parent
 ASSETS_DIR = PARENT.parent / "model" / "assets"
 MODEL_DIR = PARENT.parent / "model"
 DOCS_DIR = PARENT.parent / "documentation"
 SPHINX_DIR = PARENT.parent.parent / "docs"
+TEMPLATES_DIR = PARENT / "templates"
 
 
 def get_type(type_: str):
     ret_value = type_
     for field, replacement in TYPE_REPLACEMENTS:
         ret_value = ret_value.replace(field, replacement)
     return ret_value
@@ -631,20 +632,22 @@
             ),
             ancestor_relationship_defs,
         )
 
     def render_modules(self, modules: List[ModuleInfo]):
         self.render_init(modules)  # type: ignore
 
-    def render_module(self, asset_info: AssetInfo):
+    def render_module(self, asset_info: AssetInfo, enum_defs: List["EnumDefInfo"]):
         template = self.environment.get_template("module.jinja2")
         content = template.render(
             {
                 "asset_info": asset_info,
                 "existz": os.path.exists,
+                "enum_defs": enum_defs,
+                "templates_path": TEMPLATES_DIR.absolute().as_posix(),
             }
         )
         with (ASSETS_DIR / f"{asset_info.module_name}.py").open("w") as script:
             script.write(content)
 
     def render_init(self, assets: List[AssetInfo]):
         asset_names = [asset.name for asset in assets]
@@ -826,17 +829,17 @@
     AssetInfo.sub_type_names_to_ignore = type_defs.custom_entity_def_names
     AssetInfo.set_entity_defs(type_defs.reserved_entity_defs)
     AssetInfo.update_all_circular_dependencies()
     AssetInfo.create_modules()
     for file in (ASSETS_DIR).glob("*.py"):
         file.unlink()
     generator = Generator()
+    EnumDefInfo.create(type_defs.enum_defs)
     for asset_info in ModuleInfo.assets.values():
-        generator.render_module(asset_info)
+        generator.render_module(asset_info, EnumDefInfo.enum_def_info)
     generator.render_init(ModuleInfo.assets.values())  # type: ignore
     generator.render_structs(type_defs.struct_defs)
-    EnumDefInfo.create(type_defs.enum_defs)
     generator.render_enums(EnumDefInfo.enum_def_info)
     generator.render_docs_struct_snippets(type_defs.struct_defs)
     generator.render_docs_entity_properties(type_defs.reserved_entity_defs)
     generator.render_docs_entity_relationships(type_defs.reserved_entity_defs)
     generator.render_sphinx_docs(type_defs.reserved_entity_defs)
```

### Comparing `pyatlan-2.1.8/pyatlan/generator/create_typedefs_file.py` & `pyatlan-2.1.9/pyatlan/generator/create_typedefs_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/globals.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/globals.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/imports.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/imports.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/macros.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/module.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/module.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # Copyright 2022 Atlan Pte. Ltd.
 {% from 'macros.jinja2' import gen_properties %}
 {% from 'macros.jinja2' import gen_property_class_vars %}
 {% from 'macros.jinja2' import gen_property_relationship_class_vars %}
 
 {% include 'imports.jinja2' %}
 
+from pyatlan.model.enums import (
+{% for enum in enum_defs %}
+{{ enum.name }},
+{% endfor %}
+)
+
 {% if asset_info.name != 'Referenceable' and asset_info.name != 'Asset' %}
 from .asset import SelfAsset
 {% endif %}
 
 {% set entity_def = asset_info.entity_def %}
 
 {% set file_name = 'methods/imports/' + entity_def.name | to_snake_case + '.jinja2' %}
-{%  if existz('templates/' + file_name) %}
+{%  if existz(templates_path + '/' + file_name) %}
 {% include file_name %}
 {% endif %}
 
 {% set entity_def = asset_info.entity_def %}
 {%- set super_classes = ['AtlanObject'] if not entity_def.super_types else entity_def.super_types %}
 
 {{ asset_info.import_super_class }}
@@ -30,15 +36,15 @@
     """Description"""
 {% if entity_def.name == "Referenceable" %}
     {% include 'referenceable_methods.jinja2' %}
     {% include 'properties.jinja2' %}
     {% include 'referenceable_attributes.jinja2' %}
 {%- else %}
     {% set file_name = 'methods/asset/' + entity_def.name | to_snake_case + '.jinja2' %}
-    {%  if existz('templates/' + file_name) %}
+    {%  if existz(templates_path + '/' + file_name) %}
         {% include file_name %}
     {% endif %}
 
     type_name: str = Field(default="{{ entity_def.name }}", allow_mutation=False)
 
     @validator('type_name')
     def validate_type_name(cls, v):
@@ -54,15 +60,15 @@
         {{attribute_def.name | to_snake_case }}: Optional[{{type}}] = Field(default=None, description='')
         {%- endfor %}
         {%- for attribute_def in entity_def.relationship_attribute_defs %}
         {%- set type = attribute_def.typeName | get_type %}
         {{attribute_def.name | to_snake_case }}: Optional[{{type}}]= Field(default=None, description='') # relationship
         {%- endfor %}
         {% set file_name = 'methods/attribute/' + entity_def.name | to_snake_case + '.jinja2' %}
-        {%  if existz('templates/' + file_name) %}
+        {%  if existz(templates_path + '/' + file_name) %}
             {% include file_name %}
         {% endif %}
     attributes: {{entity_def.name}}.Attributes = Field(
         default_factory = lambda: {{entity_def.name}}.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
```

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/properties.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/properties.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/referenceable_attributes.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/referenceable_attributes.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/referenceable_methods.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/referenceable_methods.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     def set_custom_metadata(self, custom_metadata: CustomMetadataDict):
         return self._metadata_proxy.set_custom_metadata(custom_metadata=custom_metadata)
 
     def flush_custom_metadata(self):
         self.business_attributes = self._metadata_proxy.business_attributes
 
     @classmethod
+    def __get_validators__(cls):
+        yield cls._convert_to_real_type_
+
+    @classmethod
+    def _convert_to_real_type_(cls, data):
+        return Asset._convert_to_real_type_(data)
+
+    @classmethod
     def can_be_archived(self) -> bool:
         """
         Indicates if an asset can be archived via the asset.delete_by_guid method.
         :returns: True if archiving is supported
         """
         return True
```

### Comparing `pyatlan-2.1.8/pyatlan/generator/templates/structs.jinja2` & `pyatlan-2.1.9/pyatlan/generator/templates/structs.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/logging.conf` & `pyatlan-2.1.9/pyatlan/logging.conf`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/aggregation.py` & `pyatlan-2.1.9/pyatlan/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/api_tokens.py` & `pyatlan-2.1.9/pyatlan/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/__init__.py` & `pyatlan-2.1.9/pyatlan/model/assets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .dbt_process import DbtProcess
 from .column_process import ColumnProcess
 from .persona import Persona
 from .purpose import Purpose
 from .collection import Collection
 from .folder import Folder
 from .airflow import Airflow
+from .data_contract import DataContract
 from .object_store import ObjectStore
 from .data_quality import DataQuality
 from .b_i import BI
 from .saa_s import SaaS
 from .resource import Resource
 from .multi_dimensional_dataset import MultiDimensionalDataset
 from .data_mesh import DataMesh
@@ -88,19 +89,21 @@
 from .snowflake_pipe import SnowflakePipe
 from .view import View
 from .materialised_view import MaterialisedView
 from .function import Function
 from .table_partition import TablePartition
 from .column import Column
 from .snowflake_stream import SnowflakeStream
-from .calculation_view import CalculationView
 from .database import Database
+from .calculation_view import CalculationView
 from .procedure import Procedure
 from .snowflake_tag import SnowflakeTag
 from .kafka import Kafka
+from .azure_service_bus import AzureServiceBus
+from .cosmos_mongo_d_b import CosmosMongoDB
 from .dynamo_d_b import DynamoDB
 from .mongo_d_b import MongoDB
 from .matillion_group import MatillionGroup
 from .matillion_job import MatillionJob
 from .matillion_project import MatillionProject
 from .matillion_component import MatillionComponent
 from .dbt_model_column import DbtModelColumn
@@ -227,14 +230,18 @@
 from .snowflake_dynamic_table import SnowflakeDynamicTable
 from .mongo_d_b_collection import MongoDBCollection
 from .dynamo_d_b_secondary_index import DynamoDBSecondaryIndex
 from .dynamo_dbtable import DynamoDBTable
 from .mongo_d_b_database import MongoDBDatabase
 from .kafka_topic import KafkaTopic
 from .kafka_consumer_group import KafkaConsumerGroup
+from .azure_service_bus_namespace import AzureServiceBusNamespace
+from .azure_service_bus_topic import AzureServiceBusTopic
+from .cosmos_mongo_d_b_collection import CosmosMongoDBCollection
+from .cosmos_mongo_d_b_database import CosmosMongoDBDatabase
 from .qlik_stream import QlikStream
 from .dynamo_d_b_local_secondary_index import DynamoDBLocalSecondaryIndex
 from .dynamo_d_b_global_secondary_index import DynamoDBGlobalSecondaryIndex
 from .azure_event_hub import AzureEventHub
 from .azure_event_hub_consumer_group import AzureEventHubConsumerGroup
 
 
@@ -262,14 +269,15 @@
 DbtProcess.Attributes.update_forward_refs(**localns)
 ColumnProcess.Attributes.update_forward_refs(**localns)
 Persona.Attributes.update_forward_refs(**localns)
 Purpose.Attributes.update_forward_refs(**localns)
 Collection.Attributes.update_forward_refs(**localns)
 Folder.Attributes.update_forward_refs(**localns)
 Airflow.Attributes.update_forward_refs(**localns)
+DataContract.Attributes.update_forward_refs(**localns)
 ObjectStore.Attributes.update_forward_refs(**localns)
 DataQuality.Attributes.update_forward_refs(**localns)
 BI.Attributes.update_forward_refs(**localns)
 SaaS.Attributes.update_forward_refs(**localns)
 Resource.Attributes.update_forward_refs(**localns)
 MultiDimensionalDataset.Attributes.update_forward_refs(**localns)
 DataMesh.Attributes.update_forward_refs(**localns)
@@ -328,19 +336,21 @@
 SnowflakePipe.Attributes.update_forward_refs(**localns)
 View.Attributes.update_forward_refs(**localns)
 MaterialisedView.Attributes.update_forward_refs(**localns)
 Function.Attributes.update_forward_refs(**localns)
 TablePartition.Attributes.update_forward_refs(**localns)
 Column.Attributes.update_forward_refs(**localns)
 SnowflakeStream.Attributes.update_forward_refs(**localns)
-CalculationView.Attributes.update_forward_refs(**localns)
 Database.Attributes.update_forward_refs(**localns)
+CalculationView.Attributes.update_forward_refs(**localns)
 Procedure.Attributes.update_forward_refs(**localns)
 SnowflakeTag.Attributes.update_forward_refs(**localns)
 Kafka.Attributes.update_forward_refs(**localns)
+AzureServiceBus.Attributes.update_forward_refs(**localns)
+CosmosMongoDB.Attributes.update_forward_refs(**localns)
 DynamoDB.Attributes.update_forward_refs(**localns)
 MongoDB.Attributes.update_forward_refs(**localns)
 MatillionGroup.Attributes.update_forward_refs(**localns)
 MatillionJob.Attributes.update_forward_refs(**localns)
 MatillionProject.Attributes.update_forward_refs(**localns)
 MatillionComponent.Attributes.update_forward_refs(**localns)
 DbtModelColumn.Attributes.update_forward_refs(**localns)
@@ -467,12 +477,16 @@
 SnowflakeDynamicTable.Attributes.update_forward_refs(**localns)
 MongoDBCollection.Attributes.update_forward_refs(**localns)
 DynamoDBSecondaryIndex.Attributes.update_forward_refs(**localns)
 DynamoDBTable.Attributes.update_forward_refs(**localns)
 MongoDBDatabase.Attributes.update_forward_refs(**localns)
 KafkaTopic.Attributes.update_forward_refs(**localns)
 KafkaConsumerGroup.Attributes.update_forward_refs(**localns)
+AzureServiceBusNamespace.Attributes.update_forward_refs(**localns)
+AzureServiceBusTopic.Attributes.update_forward_refs(**localns)
+CosmosMongoDBCollection.Attributes.update_forward_refs(**localns)
+CosmosMongoDBDatabase.Attributes.update_forward_refs(**localns)
 QlikStream.Attributes.update_forward_refs(**localns)
 DynamoDBLocalSecondaryIndex.Attributes.update_forward_refs(**localns)
 DynamoDBGlobalSecondaryIndex.Attributes.update_forward_refs(**localns)
 AzureEventHub.Attributes.update_forward_refs(**localns)
 AzureEventHubConsumerGroup.Attributes.update_forward_refs(**localns)
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s.py` & `pyatlan-2.1.9/pyatlan/model/assets/view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,290 +1,299 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 
 
 from __future__ import annotations
 
-from typing import ClassVar, List, Optional
+from typing import ClassVar, Dict, List, Optional
+from warnings import warn
 
 from pydantic.v1 import Field, validator
 
+from pyatlan.model.enums import AtlanConnectorType
 from pyatlan.model.fields.atlan_fields import (
+    BooleanField,
     KeywordField,
-    KeywordTextField,
+    NumericField,
     RelationField,
 )
-from pyatlan.model.structs import AzureTag
+from pyatlan.utils import init_guid, validate_required_fields
 
-from .azure import Azure
+from .s_q_l import SQL
 
 
-class ADLS(Azure):
+class View(SQL):
     """Description"""
 
-    type_name: str = Field(default="ADLS", allow_mutation=False)
+    @classmethod
+    @init_guid
+    def creator(cls, *, name: str, schema_qualified_name: str) -> View:
+        validate_required_fields(
+            ["name", "schema_qualified_name"], [name, schema_qualified_name]
+        )
+        attributes = View.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
+        return cls(attributes=attributes)
+
+    @classmethod
+    @init_guid
+    def create(cls, *, name: str, schema_qualified_name: str) -> View:
+        warn(
+            (
+                "This method is deprecated, please use 'creator' "
+                "instead, which offers identical functionality."
+            ),
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return cls.creator(
+            name=name,
+            schema_qualified_name=schema_qualified_name,
+        )
+
+    type_name: str = Field(default="View", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "ADLS":
-            raise ValueError("must be ADLS")
+        if v != "View":
+            raise ValueError("must be View")
         return v
 
     def __setattr__(self, name, value):
-        if name in ADLS._convenience_properties:
+        if name in View._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    ADLS_ACCOUNT_QUALIFIED_NAME: ClassVar[KeywordTextField] = KeywordTextField(
-        "adlsAccountQualifiedName",
-        "adlsAccountQualifiedName",
-        "adlsAccountQualifiedName.text",
-    )
+    COLUMN_COUNT: ClassVar[NumericField] = NumericField("columnCount", "columnCount")
     """
-    Unique name of the account for this ADLS asset.
+    Number of columns in this view.
     """
-    AZURE_RESOURCE_ID: ClassVar[KeywordTextField] = KeywordTextField(
-        "azureResourceId", "azureResourceId", "azureResourceId.text"
-    )
+    ROW_COUNT: ClassVar[NumericField] = NumericField("rowCount", "rowCount")
     """
-    Resource identifier of this asset in Azure.
+    Number of rows in this view.
     """
-    AZURE_LOCATION: ClassVar[KeywordField] = KeywordField(
-        "azureLocation", "azureLocation"
-    )
+    SIZE_BYTES: ClassVar[NumericField] = NumericField("sizeBytes", "sizeBytes")
     """
-    Location of this asset in Azure.
+    Size of this view, in bytes.
     """
-    ADLS_ACCOUNT_SECONDARY_LOCATION: ClassVar[KeywordField] = KeywordField(
-        "adlsAccountSecondaryLocation", "adlsAccountSecondaryLocation"
+    IS_QUERY_PREVIEW: ClassVar[BooleanField] = BooleanField(
+        "isQueryPreview", "isQueryPreview"
     )
     """
-    Secondary location of the ADLS account.
+    Whether preview queries are allowed on this view (true) or not (false).
     """
-    AZURE_TAGS: ClassVar[KeywordField] = KeywordField("azureTags", "azureTags")
+    QUERY_PREVIEW_CONFIG: ClassVar[KeywordField] = KeywordField(
+        "queryPreviewConfig", "queryPreviewConfig"
+    )
     """
-    Tags that have been applied to this asset in Azure.
+    Configuration for preview queries on this view.
     """
-
-    INPUT_TO_PROCESSES: ClassVar[RelationField] = RelationField("inputToProcesses")
+    ALIAS: ClassVar[KeywordField] = KeywordField("alias", "alias")
     """
-    TBC
+    Alias for this view.
     """
-    OUTPUT_FROM_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
-        "outputFromAirflowTasks"
-    )
+    IS_TEMPORARY: ClassVar[BooleanField] = BooleanField("isTemporary", "isTemporary")
     """
-    TBC
+    Whether this view is temporary (true) or not (false).
     """
-    INPUT_TO_SPARK_JOBS: ClassVar[RelationField] = RelationField("inputToSparkJobs")
+    DEFINITION: ClassVar[KeywordField] = KeywordField("definition", "definition")
     """
-    TBC
+    SQL definition of this view.
     """
-    OUTPUT_FROM_SPARK_JOBS: ClassVar[RelationField] = RelationField(
-        "outputFromSparkJobs"
-    )
+
+    COLUMNS: ClassVar[RelationField] = RelationField("columns")
     """
     TBC
     """
-    INPUT_TO_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
-        "inputToAirflowTasks"
-    )
+    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
     """
     TBC
     """
-    OUTPUT_FROM_PROCESSES: ClassVar[RelationField] = RelationField(
-        "outputFromProcesses"
-    )
+    QUERIES: ClassVar[RelationField] = RelationField("queries")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "adls_account_qualified_name",
-        "azure_resource_id",
-        "azure_location",
-        "adls_account_secondary_location",
-        "azure_tags",
-        "input_to_processes",
-        "output_from_airflow_tasks",
-        "input_to_spark_jobs",
-        "output_from_spark_jobs",
-        "input_to_airflow_tasks",
-        "output_from_processes",
+        "column_count",
+        "row_count",
+        "size_bytes",
+        "is_query_preview",
+        "query_preview_config",
+        "alias",
+        "is_temporary",
+        "definition",
+        "columns",
+        "atlan_schema",
+        "queries",
     ]
 
     @property
-    def adls_account_qualified_name(self) -> Optional[str]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.adls_account_qualified_name
-        )
+    def column_count(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.column_count
 
-    @adls_account_qualified_name.setter
-    def adls_account_qualified_name(self, adls_account_qualified_name: Optional[str]):
+    @column_count.setter
+    def column_count(self, column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.adls_account_qualified_name = adls_account_qualified_name
+        self.attributes.column_count = column_count
 
     @property
-    def azure_resource_id(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.azure_resource_id
+    def row_count(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.row_count
 
-    @azure_resource_id.setter
-    def azure_resource_id(self, azure_resource_id: Optional[str]):
+    @row_count.setter
+    def row_count(self, row_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_resource_id = azure_resource_id
+        self.attributes.row_count = row_count
 
     @property
-    def azure_location(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.azure_location
+    def size_bytes(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.size_bytes
 
-    @azure_location.setter
-    def azure_location(self, azure_location: Optional[str]):
+    @size_bytes.setter
+    def size_bytes(self, size_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_location = azure_location
+        self.attributes.size_bytes = size_bytes
 
     @property
-    def adls_account_secondary_location(self) -> Optional[str]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.adls_account_secondary_location
-        )
+    def is_query_preview(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_query_preview
 
-    @adls_account_secondary_location.setter
-    def adls_account_secondary_location(
-        self, adls_account_secondary_location: Optional[str]
-    ):
+    @is_query_preview.setter
+    def is_query_preview(self, is_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.adls_account_secondary_location = (
-            adls_account_secondary_location
-        )
+        self.attributes.is_query_preview = is_query_preview
 
     @property
-    def azure_tags(self) -> Optional[List[AzureTag]]:
-        return None if self.attributes is None else self.attributes.azure_tags
+    def query_preview_config(self) -> Optional[Dict[str, str]]:
+        return None if self.attributes is None else self.attributes.query_preview_config
 
-    @azure_tags.setter
-    def azure_tags(self, azure_tags: Optional[List[AzureTag]]):
+    @query_preview_config.setter
+    def query_preview_config(self, query_preview_config: Optional[Dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_tags = azure_tags
+        self.attributes.query_preview_config = query_preview_config
 
     @property
-    def input_to_processes(self) -> Optional[List[Process]]:
-        return None if self.attributes is None else self.attributes.input_to_processes
+    def alias(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.alias
 
-    @input_to_processes.setter
-    def input_to_processes(self, input_to_processes: Optional[List[Process]]):
+    @alias.setter
+    def alias(self, alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.input_to_processes = input_to_processes
+        self.attributes.alias = alias
 
     @property
-    def output_from_airflow_tasks(self) -> Optional[List[AirflowTask]]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.output_from_airflow_tasks
-        )
+    def is_temporary(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_temporary
 
-    @output_from_airflow_tasks.setter
-    def output_from_airflow_tasks(
-        self, output_from_airflow_tasks: Optional[List[AirflowTask]]
-    ):
+    @is_temporary.setter
+    def is_temporary(self, is_temporary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.output_from_airflow_tasks = output_from_airflow_tasks
+        self.attributes.is_temporary = is_temporary
 
     @property
-    def input_to_spark_jobs(self) -> Optional[List[SparkJob]]:
-        return None if self.attributes is None else self.attributes.input_to_spark_jobs
+    def definition(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.definition
 
-    @input_to_spark_jobs.setter
-    def input_to_spark_jobs(self, input_to_spark_jobs: Optional[List[SparkJob]]):
+    @definition.setter
+    def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.input_to_spark_jobs = input_to_spark_jobs
+        self.attributes.definition = definition
 
     @property
-    def output_from_spark_jobs(self) -> Optional[List[SparkJob]]:
-        return (
-            None if self.attributes is None else self.attributes.output_from_spark_jobs
-        )
+    def columns(self) -> Optional[List[Column]]:
+        return None if self.attributes is None else self.attributes.columns
 
-    @output_from_spark_jobs.setter
-    def output_from_spark_jobs(self, output_from_spark_jobs: Optional[List[SparkJob]]):
+    @columns.setter
+    def columns(self, columns: Optional[List[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.output_from_spark_jobs = output_from_spark_jobs
+        self.attributes.columns = columns
 
     @property
-    def input_to_airflow_tasks(self) -> Optional[List[AirflowTask]]:
-        return (
-            None if self.attributes is None else self.attributes.input_to_airflow_tasks
-        )
+    def atlan_schema(self) -> Optional[Schema]:
+        return None if self.attributes is None else self.attributes.atlan_schema
 
-    @input_to_airflow_tasks.setter
-    def input_to_airflow_tasks(
-        self, input_to_airflow_tasks: Optional[List[AirflowTask]]
-    ):
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.input_to_airflow_tasks = input_to_airflow_tasks
+        self.attributes.atlan_schema = atlan_schema
 
     @property
-    def output_from_processes(self) -> Optional[List[Process]]:
-        return (
-            None if self.attributes is None else self.attributes.output_from_processes
-        )
+    def queries(self) -> Optional[List[Query]]:
+        return None if self.attributes is None else self.attributes.queries
 
-    @output_from_processes.setter
-    def output_from_processes(self, output_from_processes: Optional[List[Process]]):
+    @queries.setter
+    def queries(self, queries: Optional[List[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.output_from_processes = output_from_processes
+        self.attributes.queries = queries
 
-    class Attributes(Azure.Attributes):
-        adls_account_qualified_name: Optional[str] = Field(default=None, description="")
-        azure_resource_id: Optional[str] = Field(default=None, description="")
-        azure_location: Optional[str] = Field(default=None, description="")
-        adls_account_secondary_location: Optional[str] = Field(
+    class Attributes(SQL.Attributes):
+        column_count: Optional[int] = Field(default=None, description="")
+        row_count: Optional[int] = Field(default=None, description="")
+        size_bytes: Optional[int] = Field(default=None, description="")
+        is_query_preview: Optional[bool] = Field(default=None, description="")
+        query_preview_config: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
-        azure_tags: Optional[List[AzureTag]] = Field(default=None, description="")
-        input_to_processes: Optional[List[Process]] = Field(
-            default=None, description=""
-        )  # relationship
-        output_from_airflow_tasks: Optional[List[AirflowTask]] = Field(
-            default=None, description=""
-        )  # relationship
-        input_to_spark_jobs: Optional[List[SparkJob]] = Field(
-            default=None, description=""
-        )  # relationship
-        output_from_spark_jobs: Optional[List[SparkJob]] = Field(
+        alias: Optional[str] = Field(default=None, description="")
+        is_temporary: Optional[bool] = Field(default=None, description="")
+        definition: Optional[str] = Field(default=None, description="")
+        columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
-        input_to_airflow_tasks: Optional[List[AirflowTask]] = Field(
+        atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
-        output_from_processes: Optional[List[Process]] = Field(
+        queries: Optional[List[Query]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: ADLS.Attributes = Field(
-        default_factory=lambda: ADLS.Attributes(),
+        @classmethod
+        @init_guid
+        def create(cls, *, name: str, schema_qualified_name: str) -> View.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
+            fields = schema_qualified_name.split("/")
+            if len(fields) != 5:
+                raise ValueError("Invalid schema_qualified_name")
+            try:
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+            except ValueError as e:
+                raise ValueError("Invalid schema_qualified_name") from e
+            return View.Attributes(
+                name=name,
+                database_name=fields[3],
+                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
+                qualified_name=f"{schema_qualified_name}/{name}",
+                schema_qualified_name=schema_qualified_name,
+                schema_name=fields[4],
+                connector_name=connector_type.value,
+                atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
+            )
+
+    attributes: View.Attributes = Field(
+        default_factory=lambda: View.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
     )
 
 
-from .airflow_task import AirflowTask  # noqa
-from .process import Process  # noqa
-from .spark_job import SparkJob  # noqa
+from .column import Column  # noqa
+from .query import Query  # noqa
+from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_account.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_account.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_container.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_container.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_d_l_s_object.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_p_i.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_p_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_p_i_path.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_p_i_path.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_p_i_spec.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_p_i_spec.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/a_w_s.py` & `pyatlan-2.1.9/pyatlan/model/assets/a_w_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/access_control.py` & `pyatlan-2.1.9/pyatlan/model/assets/access_control.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/airflow.py` & `pyatlan-2.1.9/pyatlan/model/assets/airflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/airflow_dag.py` & `pyatlan-2.1.9/pyatlan/model/assets/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/airflow_task.py` & `pyatlan-2.1.9/pyatlan/model/assets/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/asset.py` & `pyatlan-2.1.9/pyatlan/model/assets/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -985,31 +985,49 @@
     """
     ASSET_THEME_HEX: ClassVar[KeywordField] = KeywordField(
         "assetThemeHex", "assetThemeHex"
     )
     """
     Color (in hexadecimal RGB) to use to represent this asset.
     """
+    HAS_CONTRACT: ClassVar[BooleanField] = BooleanField("hasContract", "hasContract")
+    """
+    Whether this asset has contract (true) or not (false).
+    """
 
     SCHEMA_REGISTRY_SUBJECTS: ClassVar[RelationField] = RelationField(
         "schemaRegistrySubjects"
     )
     """
     TBC
     """
-    MC_MONITORS: ClassVar[RelationField] = RelationField("mcMonitors")
+    DATA_CONTRACT_LATEST_CERTIFIED: ClassVar[RelationField] = RelationField(
+        "dataContractLatestCertified"
+    )
     """
     TBC
     """
     OUTPUT_PORT_DATA_PRODUCTS: ClassVar[RelationField] = RelationField(
         "outputPortDataProducts"
     )
     """
     TBC
     """
+    README: ClassVar[RelationField] = RelationField("readme")
+    """
+    TBC
+    """
+    DATA_CONTRACT_LATEST: ClassVar[RelationField] = RelationField("dataContractLatest")
+    """
+    TBC
+    """
+    MC_MONITORS: ClassVar[RelationField] = RelationField("mcMonitors")
+    """
+    TBC
+    """
     FILES: ClassVar[RelationField] = RelationField("files")
     """
     TBC
     """
     MC_INCIDENTS: ClassVar[RelationField] = RelationField("mcIncidents")
     """
     TBC
@@ -1018,18 +1036,14 @@
     """
     TBC
     """
     METRICS: ClassVar[RelationField] = RelationField("metrics")
     """
     TBC
     """
-    README: ClassVar[RelationField] = RelationField("readme")
-    """
-    TBC
-    """
     INPUT_PORT_DATA_PRODUCTS: ClassVar[RelationField] = RelationField(
         "inputPortDataProducts"
     )
     """
     TBC
     """
     SODA_CHECKS: ClassVar[RelationField] = RelationField("sodaChecks")
@@ -1160,25 +1174,28 @@
         "asset_soda_check_statuses",
         "asset_soda_source_url",
         "asset_icon",
         "is_partial",
         "is_a_i_generated",
         "asset_cover_image",
         "asset_theme_hex",
+        "has_contract",
         "schema_registry_subjects",
-        "mc_monitors",
+        "data_contract_latest_certified",
         "output_port_data_products",
+        "readme",
+        "data_contract_latest",
+        "assigned_terms",
+        "mc_monitors",
         "files",
         "mc_incidents",
         "links",
         "metrics",
-        "readme",
         "input_port_data_products",
         "soda_checks",
-        "assigned_terms",
     ]
 
     @property
     def name(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.name
 
     @name.setter
@@ -2831,14 +2848,24 @@
     @asset_theme_hex.setter
     def asset_theme_hex(self, asset_theme_hex: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_theme_hex = asset_theme_hex
 
     @property
+    def has_contract(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.has_contract
+
+    @has_contract.setter
+    def has_contract(self, has_contract: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.has_contract = has_contract
+
+    @property
     def schema_registry_subjects(self) -> Optional[List[SchemaRegistrySubject]]:
         return (
             None
             if self.attributes is None
             else self.attributes.schema_registry_subjects
         )
 
@@ -2847,22 +2874,28 @@
         self, schema_registry_subjects: Optional[List[SchemaRegistrySubject]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_registry_subjects = schema_registry_subjects
 
     @property
-    def mc_monitors(self) -> Optional[List[MCMonitor]]:
-        return None if self.attributes is None else self.attributes.mc_monitors
+    def data_contract_latest_certified(self) -> Optional[DataContract]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.data_contract_latest_certified
+        )
 
-    @mc_monitors.setter
-    def mc_monitors(self, mc_monitors: Optional[List[MCMonitor]]):
+    @data_contract_latest_certified.setter
+    def data_contract_latest_certified(
+        self, data_contract_latest_certified: Optional[DataContract]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mc_monitors = mc_monitors
+        self.attributes.data_contract_latest_certified = data_contract_latest_certified
 
     @property
     def output_port_data_products(self) -> Optional[List[DataProduct]]:
         return (
             None
             if self.attributes is None
             else self.attributes.output_port_data_products
@@ -2873,14 +2906,54 @@
         self, output_port_data_products: Optional[List[DataProduct]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_port_data_products = output_port_data_products
 
     @property
+    def readme(self) -> Optional[Readme]:
+        return None if self.attributes is None else self.attributes.readme
+
+    @readme.setter
+    def readme(self, readme: Optional[Readme]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.readme = readme
+
+    @property
+    def data_contract_latest(self) -> Optional[DataContract]:
+        return None if self.attributes is None else self.attributes.data_contract_latest
+
+    @data_contract_latest.setter
+    def data_contract_latest(self, data_contract_latest: Optional[DataContract]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.data_contract_latest = data_contract_latest
+
+    @property
+    def assigned_terms(self) -> Optional[List[AtlasGlossaryTerm]]:
+        return None if self.attributes is None else self.attributes.meanings
+
+    @assigned_terms.setter
+    def assigned_terms(self, assigned_terms: Optional[List[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = assigned_terms
+
+    @property
+    def mc_monitors(self) -> Optional[List[MCMonitor]]:
+        return None if self.attributes is None else self.attributes.mc_monitors
+
+    @mc_monitors.setter
+    def mc_monitors(self, mc_monitors: Optional[List[MCMonitor]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitors = mc_monitors
+
+    @property
     def files(self) -> Optional[List[File]]:
         return None if self.attributes is None else self.attributes.files
 
     @files.setter
     def files(self, files: Optional[List[File]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -2913,24 +2986,14 @@
     @metrics.setter
     def metrics(self, metrics: Optional[List[Metric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metrics = metrics
 
     @property
-    def readme(self) -> Optional[Readme]:
-        return None if self.attributes is None else self.attributes.readme
-
-    @readme.setter
-    def readme(self, readme: Optional[Readme]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.readme = readme
-
-    @property
     def input_port_data_products(self) -> Optional[List[DataProduct]]:
         return (
             None
             if self.attributes is None
             else self.attributes.input_port_data_products
         )
 
@@ -2948,24 +3011,14 @@
 
     @soda_checks.setter
     def soda_checks(self, soda_checks: Optional[List[SodaCheck]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.soda_checks = soda_checks
 
-    @property
-    def assigned_terms(self) -> Optional[List[AtlasGlossaryTerm]]:
-        return None if self.attributes is None else self.attributes.meanings
-
-    @assigned_terms.setter
-    def assigned_terms(self, assigned_terms: Optional[List[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.meanings = assigned_terms
-
     class Attributes(Referenceable.Attributes):
         name: Optional[str] = Field(default=None, description="")
         display_name: Optional[str] = Field(default=None, description="")
         description: Optional[str] = Field(default=None, description="")
         user_description: Optional[str] = Field(default=None, description="")
         tenant_id: Optional[str] = Field(default=None, description="")
         certificate_status: Optional[CertificateStatus] = Field(
@@ -3187,45 +3240,52 @@
         asset_soda_check_statuses: Optional[str] = Field(default=None, description="")
         asset_soda_source_url: Optional[str] = Field(default=None, description="")
         asset_icon: Optional[str] = Field(default=None, description="")
         is_partial: Optional[bool] = Field(default=None, description="")
         is_a_i_generated: Optional[bool] = Field(default=None, description="")
         asset_cover_image: Optional[str] = Field(default=None, description="")
         asset_theme_hex: Optional[str] = Field(default=None, description="")
+        has_contract: Optional[bool] = Field(default=None, description="")
         schema_registry_subjects: Optional[List[SchemaRegistrySubject]] = Field(
             default=None, description=""
         )  # relationship
-        mc_monitors: Optional[List[MCMonitor]] = Field(
+        data_contract_latest_certified: Optional[DataContract] = Field(
             default=None, description=""
         )  # relationship
         output_port_data_products: Optional[List[DataProduct]] = Field(
             default=None, description=""
         )  # relationship
+        readme: Optional[Readme] = Field(default=None, description="")  # relationship
+        data_contract_latest: Optional[DataContract] = Field(
+            default=None, description=""
+        )  # relationship
+        meanings: Optional[List[AtlasGlossaryTerm]] = Field(
+            default=None, description=""
+        )  # relationship
+        mc_monitors: Optional[List[MCMonitor]] = Field(
+            default=None, description=""
+        )  # relationship
         files: Optional[List[File]] = Field(
             default=None, description=""
         )  # relationship
         mc_incidents: Optional[List[MCIncident]] = Field(
             default=None, description=""
         )  # relationship
         links: Optional[List[Link]] = Field(
             default=None, description=""
         )  # relationship
         metrics: Optional[List[Metric]] = Field(
             default=None, description=""
         )  # relationship
-        readme: Optional[Readme] = Field(default=None, description="")  # relationship
         input_port_data_products: Optional[List[DataProduct]] = Field(
             default=None, description=""
         )  # relationship
         soda_checks: Optional[List[SodaCheck]] = Field(
             default=None, description=""
         )  # relationship
-        meanings: Optional[List[AtlasGlossaryTerm]] = Field(
-            default=None, description=""
-        )  # relationship
 
         def remove_description(self):
             self.description = None
 
         def remove_user_description(self):
             self.user_description = None
 
@@ -3249,14 +3309,15 @@
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
     )
 
 
 from .atlas_glossary_term import AtlasGlossaryTerm  # noqa
+from .data_contract import DataContract  # noqa
 from .data_product import DataProduct  # noqa
 from .file import File  # noqa
 from .link import Link  # noqa
 from .m_c_incident import MCIncident  # noqa
 from .m_c_monitor import MCMonitor  # noqa
 from .metric import Metric  # noqa
 from .readme import Readme  # noqa
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary.py` & `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary_category.py` & `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_category.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/atlas_glossary_term.py` & `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/auth_policy.py` & `pyatlan-2.1.9/pyatlan/model/assets/auth_policy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/auth_service.py` & `pyatlan-2.1.9/pyatlan/model/assets/auth_service.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/azure.py` & `pyatlan-2.1.9/pyatlan/model/assets/azure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/azure_event_hub.py` & `pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/azure_event_hub_consumer_group.py` & `pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/b_i.py` & `pyatlan-2.1.9/pyatlan/model/assets/b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/b_i_process.py` & `pyatlan-2.1.9/pyatlan/model/assets/b_i_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/badge.py` & `pyatlan-2.1.9/pyatlan/model/assets/badge.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/calculation_view.py` & `pyatlan-2.1.9/pyatlan/model/assets/calculation_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/catalog.py` & `pyatlan-2.1.9/pyatlan/model/assets/catalog.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cloud.py` & `pyatlan-2.1.9/pyatlan/model/assets/cloud.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite3_d_model.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite3_d_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite_asset.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite_event.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite_event.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite_file.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite_sequence.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite_sequence.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cognite_time_series.py` & `pyatlan-2.1.9/pyatlan/model/assets/cognite_time_series.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/collection.py` & `pyatlan-2.1.9/pyatlan/model/assets/collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/column.py` & `pyatlan-2.1.9/pyatlan/model/assets/column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/column_process.py` & `pyatlan-2.1.9/pyatlan/model/assets/column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/connection.py` & `pyatlan-2.1.9/pyatlan/model/assets/connection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cube.py` & `pyatlan-2.1.9/pyatlan/model/assets/cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cube_dimension.py` & `pyatlan-2.1.9/pyatlan/model/assets/cube_dimension.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cube_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/cube_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/cube_hierarchy.py` & `pyatlan-2.1.9/pyatlan/model/assets/cube_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_domain.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_domain.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_mesh.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_product.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_product.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_quality.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_quality.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_set.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_set.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_studio.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_studio.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/data_studio_asset.py` & `pyatlan-2.1.9/pyatlan/model/assets/data_studio_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/database.py` & `pyatlan-2.1.9/pyatlan/model/assets/database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_column_process.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_column_process.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,18 @@
     SQL query that ran to produce the outputs.
     """
     AST: ClassVar[KeywordField] = KeywordField("ast", "ast")
     """
     Parsed AST of the code or SQL statements that describe the logic of this process.
     """
 
+    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
+    """
+    TBC
+    """
     MATILLION_COMPONENT: ClassVar[RelationField] = RelationField("matillionComponent")
     """
     TBC
     """
     PROCESS: ClassVar[RelationField] = RelationField("process")
     """
     TBC
@@ -176,18 +180,14 @@
     """
     TBC
     """
     COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
     """
     TBC
     """
-    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
-    """
-    TBC
-    """
 
     _convenience_properties: ClassVar[List[str]] = [
         "dbt_column_process_job_status",
         "dbt_alias",
         "dbt_meta",
         "dbt_unique_id",
         "dbt_account_name",
@@ -206,19 +206,19 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
+        "spark_jobs",
         "matillion_component",
         "process",
         "airflow_tasks",
         "column_processes",
-        "spark_jobs",
     ]
 
     @property
     def dbt_column_process_job_status(self) -> Optional[str]:
         return (
             None
             if self.attributes is None
@@ -482,14 +482,24 @@
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
+    def spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.spark_jobs
+
+    @spark_jobs.setter
+    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.spark_jobs = spark_jobs
+
+    @property
     def matillion_component(self) -> Optional[MatillionComponent]:
         return None if self.attributes is None else self.attributes.matillion_component
 
     @matillion_component.setter
     def matillion_component(self, matillion_component: Optional[MatillionComponent]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -521,24 +531,14 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[List[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
-    @property
-    def spark_jobs(self) -> Optional[List[SparkJob]]:
-        return None if self.attributes is None else self.attributes.spark_jobs
-
-    @spark_jobs.setter
-    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.spark_jobs = spark_jobs
-
     class Attributes(Dbt.Attributes):
         dbt_column_process_job_status: Optional[str] = Field(
             default=None, description=""
         )
         dbt_alias: Optional[str] = Field(default=None, description="")
         dbt_meta: Optional[str] = Field(default=None, description="")
         dbt_unique_id: Optional[str] = Field(default=None, description="")
@@ -562,27 +562,27 @@
             default=None, description=""
         )
         inputs: Optional[List[Catalog]] = Field(default=None, description="")
         outputs: Optional[List[Catalog]] = Field(default=None, description="")
         code: Optional[str] = Field(default=None, description="")
         sql: Optional[str] = Field(default=None, description="")
         ast: Optional[str] = Field(default=None, description="")
+        spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
         matillion_component: Optional[MatillionComponent] = Field(
             default=None, description=""
         )  # relationship
         process: Optional[Process] = Field(default=None, description="")  # relationship
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         column_processes: Optional[List[ColumnProcess]] = Field(
             default=None, description=""
         )  # relationship
-        spark_jobs: Optional[List[SparkJob]] = Field(
-            default=None, description=""
-        )  # relationship
 
     attributes: DbtColumnProcess.Attributes = Field(
         default_factory=lambda: DbtColumnProcess.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_metric.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_model.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_model_column.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_model_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_process.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_process.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -160,27 +160,27 @@
     SQL query that ran to produce the outputs.
     """
     AST: ClassVar[KeywordField] = KeywordField("ast", "ast")
     """
     Parsed AST of the code or SQL statements that describe the logic of this process.
     """
 
-    MATILLION_COMPONENT: ClassVar[RelationField] = RelationField("matillionComponent")
+    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
     """
     TBC
     """
-    AIRFLOW_TASKS: ClassVar[RelationField] = RelationField("airflowTasks")
+    MATILLION_COMPONENT: ClassVar[RelationField] = RelationField("matillionComponent")
     """
     TBC
     """
-    COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
+    AIRFLOW_TASKS: ClassVar[RelationField] = RelationField("airflowTasks")
     """
     TBC
     """
-    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
+    COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "dbt_process_job_status",
         "dbt_alias",
@@ -202,18 +202,18 @@
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
+        "spark_jobs",
         "matillion_component",
         "airflow_tasks",
         "column_processes",
-        "spark_jobs",
     ]
 
     @property
     def dbt_process_job_status(self) -> Optional[str]:
         return (
             None if self.attributes is None else self.attributes.dbt_process_job_status
         )
@@ -473,14 +473,24 @@
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
+    def spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.spark_jobs
+
+    @spark_jobs.setter
+    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.spark_jobs = spark_jobs
+
+    @property
     def matillion_component(self) -> Optional[MatillionComponent]:
         return None if self.attributes is None else self.attributes.matillion_component
 
     @matillion_component.setter
     def matillion_component(self, matillion_component: Optional[MatillionComponent]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -502,24 +512,14 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[List[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
-    @property
-    def spark_jobs(self) -> Optional[List[SparkJob]]:
-        return None if self.attributes is None else self.attributes.spark_jobs
-
-    @spark_jobs.setter
-    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.spark_jobs = spark_jobs
-
     class Attributes(Dbt.Attributes):
         dbt_process_job_status: Optional[str] = Field(default=None, description="")
         dbt_alias: Optional[str] = Field(default=None, description="")
         dbt_meta: Optional[str] = Field(default=None, description="")
         dbt_unique_id: Optional[str] = Field(default=None, description="")
         dbt_account_name: Optional[str] = Field(default=None, description="")
         dbt_project_name: Optional[str] = Field(default=None, description="")
@@ -541,26 +541,26 @@
             default=None, description=""
         )
         inputs: Optional[List[Catalog]] = Field(default=None, description="")
         outputs: Optional[List[Catalog]] = Field(default=None, description="")
         code: Optional[str] = Field(default=None, description="")
         sql: Optional[str] = Field(default=None, description="")
         ast: Optional[str] = Field(default=None, description="")
+        spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
         matillion_component: Optional[MatillionComponent] = Field(
             default=None, description=""
         )  # relationship
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         column_processes: Optional[List[ColumnProcess]] = Field(
             default=None, description=""
         )  # relationship
-        spark_jobs: Optional[List[SparkJob]] = Field(
-            default=None, description=""
-        )  # relationship
 
     attributes: DbtProcess.Attributes = Field(
         default_factory=lambda: DbtProcess.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_source.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_source.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_tag.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dbt_test.py` & `pyatlan-2.1.9/pyatlan/model/assets/dbt_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/domo.py` & `pyatlan-2.1.9/pyatlan/model/assets/domo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/domo_card.py` & `pyatlan-2.1.9/pyatlan/model/assets/domo_card.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/domo_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/domo_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/domo_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/domo_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/domo_dataset_column.py` & `pyatlan-2.1.9/pyatlan/model/assets/domo_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b.py` & `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py` & `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py` & `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dynamo_d_b_secondary_index.py` & `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/dynamo_dbtable.py` & `pyatlan-2.1.9/pyatlan/model/assets/dynamo_dbtable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/event_store.py` & `pyatlan-2.1.9/pyatlan/model/assets/event_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/file.py` & `pyatlan-2.1.9/pyatlan/model/assets/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/folder.py` & `pyatlan-2.1.9/pyatlan/model/assets/folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/function.py` & `pyatlan-2.1.9/pyatlan/model/assets/function.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/g_c_s.py` & `pyatlan-2.1.9/pyatlan/model/assets/g_c_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/g_c_s_bucket.py` & `pyatlan-2.1.9/pyatlan/model/assets/g_c_s_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/g_c_s_object.py` & `pyatlan-2.1.9/pyatlan/model/assets/g_c_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/google.py` & `pyatlan-2.1.9/pyatlan/model/assets/google.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/infrastructure.py` & `pyatlan-2.1.9/pyatlan/model/assets/infrastructure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/insight.py` & `pyatlan-2.1.9/pyatlan/model/assets/insight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/kafka.py` & `pyatlan-2.1.9/pyatlan/model/assets/kafka.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/kafka_consumer_group.py` & `pyatlan-2.1.9/pyatlan/model/assets/kafka_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/kafka_topic.py` & `pyatlan-2.1.9/pyatlan/model/assets/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/link.py` & `pyatlan-2.1.9/pyatlan/model/assets/link.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_explore.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_explore.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_folder.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_look.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_look.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_model.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_project.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_project.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,19 +25,23 @@
         return v
 
     def __setattr__(self, name, value):
         if name in LookerProject._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    MODELS: ClassVar[RelationField] = RelationField("models")
+    EXPLORES: ClassVar[RelationField] = RelationField("explores")
     """
     TBC
     """
-    EXPLORES: ClassVar[RelationField] = RelationField("explores")
+    VIEWS: ClassVar[RelationField] = RelationField("views")
+    """
+    TBC
+    """
+    MODELS: ClassVar[RelationField] = RelationField("models")
     """
     TBC
     """
     LOOKER_PARENT_PROJECTS: ClassVar[RelationField] = RelationField(
         "lookerParentProjects"
     )
     """
@@ -49,49 +53,55 @@
     """
     TBC
     """
     FIELDS: ClassVar[RelationField] = RelationField("fields")
     """
     TBC
     """
-    VIEWS: ClassVar[RelationField] = RelationField("views")
-    """
-    TBC
-    """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "models",
         "explores",
+        "views",
+        "models",
         "looker_parent_projects",
         "looker_child_projects",
         "fields",
-        "views",
     ]
 
     @property
-    def models(self) -> Optional[List[LookerModel]]:
-        return None if self.attributes is None else self.attributes.models
-
-    @models.setter
-    def models(self, models: Optional[List[LookerModel]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.models = models
-
-    @property
     def explores(self) -> Optional[List[LookerExplore]]:
         return None if self.attributes is None else self.attributes.explores
 
     @explores.setter
     def explores(self, explores: Optional[List[LookerExplore]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.explores = explores
 
     @property
+    def views(self) -> Optional[List[LookerView]]:
+        return None if self.attributes is None else self.attributes.views
+
+    @views.setter
+    def views(self, views: Optional[List[LookerView]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.views = views
+
+    @property
+    def models(self) -> Optional[List[LookerModel]]:
+        return None if self.attributes is None else self.attributes.models
+
+    @models.setter
+    def models(self, models: Optional[List[LookerModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.models = models
+
+    @property
     def looker_parent_projects(self) -> Optional[List[LookerProject]]:
         return (
             None if self.attributes is None else self.attributes.looker_parent_projects
         )
 
     @looker_parent_projects.setter
     def looker_parent_projects(
@@ -121,43 +131,33 @@
 
     @fields.setter
     def fields(self, fields: Optional[List[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
-    @property
-    def views(self) -> Optional[List[LookerView]]:
-        return None if self.attributes is None else self.attributes.views
-
-    @views.setter
-    def views(self, views: Optional[List[LookerView]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.views = views
-
     class Attributes(Looker.Attributes):
-        models: Optional[List[LookerModel]] = Field(
+        explores: Optional[List[LookerExplore]] = Field(
             default=None, description=""
         )  # relationship
-        explores: Optional[List[LookerExplore]] = Field(
+        views: Optional[List[LookerView]] = Field(
+            default=None, description=""
+        )  # relationship
+        models: Optional[List[LookerModel]] = Field(
             default=None, description=""
         )  # relationship
         looker_parent_projects: Optional[List[LookerProject]] = Field(
             default=None, description=""
         )  # relationship
         looker_child_projects: Optional[List[LookerProject]] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[LookerField]] = Field(
             default=None, description=""
         )  # relationship
-        views: Optional[List[LookerView]] = Field(
-            default=None, description=""
-        )  # relationship
 
     attributes: LookerProject.Attributes = Field(
         default_factory=lambda: LookerProject.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_query.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_tile.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/looker_view.py` & `pyatlan-2.1.9/pyatlan/model/assets/looker_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/m_c_incident.py` & `pyatlan-2.1.9/pyatlan/model/assets/m_c_incident.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/m_c_monitor.py` & `pyatlan-2.1.9/pyatlan/model/assets/m_c_monitor.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/materialised_view.py` & `pyatlan-2.1.9/pyatlan/model/assets/materialised_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/matillion.py` & `pyatlan-2.1.9/pyatlan/model/assets/matillion.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/matillion_component.py` & `pyatlan-2.1.9/pyatlan/model/assets/matillion_component.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/matillion_group.py` & `pyatlan-2.1.9/pyatlan/model/assets/matillion_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/matillion_job.py` & `pyatlan-2.1.9/pyatlan/model/assets/matillion_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/matillion_project.py` & `pyatlan-2.1.9/pyatlan/model/assets/matillion_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/metabase.py` & `pyatlan-2.1.9/pyatlan/model/assets/metabase.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/metabase_collection.py` & `pyatlan-2.1.9/pyatlan/model/assets/metabase_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/metabase_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/metabase_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/metabase_question.py` & `pyatlan-2.1.9/pyatlan/model/assets/metabase_question.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/metric.py` & `pyatlan-2.1.9/pyatlan/model/assets/metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_attribute.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_attribute.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_cube.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_document.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_document.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_dossier.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_dossier.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_fact.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_fact.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_metric.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_project.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_report.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/micro_strategy_visualization.py` & `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode_chart.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode_collection.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode_query.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode_report.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mode_workspace.py` & `pyatlan-2.1.9/pyatlan/model/assets/mode_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b.py` & `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b_collection.py` & `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/mongo_d_b_database.py` & `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/monte_carlo.py` & `pyatlan-2.1.9/pyatlan/model/assets/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/multi_dimensional_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/multi_dimensional_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/namespace.py` & `pyatlan-2.1.9/pyatlan/model/assets/namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/no_s_q_l.py` & `pyatlan-2.1.9/pyatlan/model/assets/no_s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/object_store.py` & `pyatlan-2.1.9/pyatlan/model/assets/object_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/persona.py` & `pyatlan-2.1.9/pyatlan/model/assets/persona.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_column.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dataflow.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,39 +44,39 @@
     """
     TBC
     """
     WORKSPACE: ClassVar[RelationField] = RelationField("workspace")
     """
     TBC
     """
-    DATAFLOWS: ClassVar[RelationField] = RelationField("dataflows")
+    TILES: ClassVar[RelationField] = RelationField("tiles")
     """
     TBC
     """
-    TILES: ClassVar[RelationField] = RelationField("tiles")
+    TABLES: ClassVar[RelationField] = RelationField("tables")
     """
     TBC
     """
-    TABLES: ClassVar[RelationField] = RelationField("tables")
+    DATAFLOWS: ClassVar[RelationField] = RelationField("dataflows")
     """
     TBC
     """
     DATASOURCES: ClassVar[RelationField] = RelationField("datasources")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "workspace_qualified_name",
         "web_url",
         "reports",
         "workspace",
-        "dataflows",
         "tiles",
         "tables",
+        "dataflows",
         "datasources",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return (
             None
@@ -117,24 +117,14 @@
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
     @property
-    def dataflows(self) -> Optional[List[PowerBIDataflow]]:
-        return None if self.attributes is None else self.attributes.dataflows
-
-    @dataflows.setter
-    def dataflows(self, dataflows: Optional[List[PowerBIDataflow]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataflows = dataflows
-
-    @property
     def tiles(self) -> Optional[List[PowerBITile]]:
         return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[List[PowerBITile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -147,14 +137,24 @@
     @tables.setter
     def tables(self, tables: Optional[List[PowerBITable]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tables = tables
 
     @property
+    def dataflows(self) -> Optional[List[PowerBIDataflow]]:
+        return None if self.attributes is None else self.attributes.dataflows
+
+    @dataflows.setter
+    def dataflows(self, dataflows: Optional[List[PowerBIDataflow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflows = dataflows
+
+    @property
     def datasources(self) -> Optional[List[PowerBIDatasource]]:
         return None if self.attributes is None else self.attributes.datasources
 
     @datasources.setter
     def datasources(self, datasources: Optional[List[PowerBIDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -165,23 +165,23 @@
         web_url: Optional[str] = Field(default=None, description="")
         reports: Optional[List[PowerBIReport]] = Field(
             default=None, description=""
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             default=None, description=""
         )  # relationship
-        dataflows: Optional[List[PowerBIDataflow]] = Field(
-            default=None, description=""
-        )  # relationship
         tiles: Optional[List[PowerBITile]] = Field(
             default=None, description=""
         )  # relationship
         tables: Optional[List[PowerBITable]] = Field(
             default=None, description=""
         )  # relationship
+        dataflows: Optional[List[PowerBIDataflow]] = Field(
+            default=None, description=""
+        )  # relationship
         datasources: Optional[List[PowerBIDatasource]] = Field(
             default=None, description=""
         )  # relationship
 
     attributes: PowerBIDataset.Attributes = Field(
         default_factory=lambda: PowerBIDataset.Attributes(),
         description=(
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_datasource.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_measure.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_measure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_page.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_report.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_table.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_tile.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/power_b_i_workspace.py` & `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/preset.py` & `pyatlan-2.1.9/pyatlan/model/assets/preset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/preset_chart.py` & `pyatlan-2.1.9/pyatlan/model/assets/preset_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/preset_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/preset_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/preset_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/preset_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/preset_workspace.py` & `pyatlan-2.1.9/pyatlan/model/assets/preset_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/procedure.py` & `pyatlan-2.1.9/pyatlan/model/assets/procedure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/process.py` & `pyatlan-2.1.9/pyatlan/model/assets/process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/process_execution.py` & `pyatlan-2.1.9/pyatlan/model/assets/process_execution.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/purpose.py` & `pyatlan-2.1.9/pyatlan/model/assets/purpose.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_app.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_app.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_chart.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_sheet.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_sheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_space.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_space.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/qlik_stream.py` & `pyatlan-2.1.9/pyatlan/model/assets/qlik_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/query.py` & `pyatlan-2.1.9/pyatlan/model/assets/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_analysis.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_analysis_visual.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dashboard_visual.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_dataset_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/quick_sight_folder.py` & `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/readme.py` & `pyatlan-2.1.9/pyatlan/model/assets/readme.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/readme_template.py` & `pyatlan-2.1.9/pyatlan/model/assets/readme_template.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/redash.py` & `pyatlan-2.1.9/pyatlan/model/assets/redash.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/redash_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/redash_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/redash_query.py` & `pyatlan-2.1.9/pyatlan/model/assets/redash_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/redash_visualization.py` & `pyatlan-2.1.9/pyatlan/model/assets/redash_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/referenceable.py` & `pyatlan-2.1.9/pyatlan/model/assets/referenceable.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,22 @@
     def set_custom_metadata(self, custom_metadata: CustomMetadataDict):
         return self._metadata_proxy.set_custom_metadata(custom_metadata=custom_metadata)
 
     def flush_custom_metadata(self):
         self.business_attributes = self._metadata_proxy.business_attributes
 
     @classmethod
+    def __get_validators__(cls):
+        yield cls._convert_to_real_type_
+
+    @classmethod
+    def _convert_to_real_type_(cls, data):
+        return Asset._convert_to_real_type_(data)
+
+    @classmethod
     def can_be_archived(self) -> bool:
         """
         Indicates if an asset can be archived via the asset.delete_by_guid method.
         :returns: True if archiving is supported
         """
         return True
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/resource.py` & `pyatlan-2.1.9/pyatlan/model/assets/resource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/s3.py` & `pyatlan-2.1.9/pyatlan/model/assets/s3.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/s3_bucket.py` & `pyatlan-2.1.9/pyatlan/model/assets/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/s3_object.py` & `pyatlan-2.1.9/pyatlan/model/assets/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/s_q_l.py` & `pyatlan-2.1.9/pyatlan/model/assets/s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/saa_s.py` & `pyatlan-2.1.9/pyatlan/model/assets/saa_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce_object.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce_organization.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce_organization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/salesforce_report.py` & `pyatlan-2.1.9/pyatlan/model/assets/salesforce_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/schema.py` & `pyatlan-2.1.9/pyatlan/model/assets/schema.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/schema_registry.py` & `pyatlan-2.1.9/pyatlan/model/assets/schema_registry.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/schema_registry_subject.py` & `pyatlan-2.1.9/pyatlan/model/assets/schema_registry_subject.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_data_element.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_data_element_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_dataset.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_dataset_column.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_page.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sigma_workbook.py` & `pyatlan-2.1.9/pyatlan/model/assets/sigma_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense_datamodel.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense_datamodel_table.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense_folder.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/sisense_widget.py` & `pyatlan-2.1.9/pyatlan/model/assets/sisense_widget.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/snowflake_dynamic_table.py` & `pyatlan-2.1.9/pyatlan/model/assets/snowflake_dynamic_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/snowflake_pipe.py` & `pyatlan-2.1.9/pyatlan/model/assets/snowflake_pipe.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/snowflake_stream.py` & `pyatlan-2.1.9/pyatlan/model/assets/snowflake_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/snowflake_tag.py` & `pyatlan-2.1.9/pyatlan/model/assets/snowflake_tag.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -156,27 +156,27 @@
     """
     TBC
     """
     SQL_DBT_MODELS: ClassVar[RelationField] = RelationField("sqlDbtModels")
     """
     TBC
     """
-    SQL_DBT_SOURCES: ClassVar[RelationField] = RelationField("sqlDBTSources")
+    DBT_TESTS: ClassVar[RelationField] = RelationField("dbtTests")
     """
     TBC
     """
-    DBT_MODELS: ClassVar[RelationField] = RelationField("dbtModels")
+    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
     """
     TBC
     """
-    DBT_TESTS: ClassVar[RelationField] = RelationField("dbtTests")
+    SQL_DBT_SOURCES: ClassVar[RelationField] = RelationField("sqlDBTSources")
     """
     TBC
     """
-    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
+    DBT_MODELS: ClassVar[RelationField] = RelationField("dbtModels")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "tag_id",
         "tag_attributes",
@@ -196,18 +196,18 @@
         "view_qualified_name",
         "calculation_view_name",
         "calculation_view_qualified_name",
         "is_profiled",
         "last_profiled_at",
         "dbt_sources",
         "sql_dbt_models",
-        "sql_dbt_sources",
-        "dbt_models",
         "dbt_tests",
         "atlan_schema",
+        "sql_dbt_sources",
+        "dbt_models",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.tag_id
 
     @tag_id.setter
@@ -441,34 +441,14 @@
     @sql_dbt_models.setter
     def sql_dbt_models(self, sql_dbt_models: Optional[List[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_dbt_models = sql_dbt_models
 
     @property
-    def sql_dbt_sources(self) -> Optional[List[DbtSource]]:
-        return None if self.attributes is None else self.attributes.sql_dbt_sources
-
-    @sql_dbt_sources.setter
-    def sql_dbt_sources(self, sql_dbt_sources: Optional[List[DbtSource]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sql_dbt_sources = sql_dbt_sources
-
-    @property
-    def dbt_models(self) -> Optional[List[DbtModel]]:
-        return None if self.attributes is None else self.attributes.dbt_models
-
-    @dbt_models.setter
-    def dbt_models(self, dbt_models: Optional[List[DbtModel]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dbt_models = dbt_models
-
-    @property
     def dbt_tests(self) -> Optional[List[DbtTest]]:
         return None if self.attributes is None else self.attributes.dbt_tests
 
     @dbt_tests.setter
     def dbt_tests(self, dbt_tests: Optional[List[DbtTest]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -480,14 +460,34 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
+    @property
+    def sql_dbt_sources(self) -> Optional[List[DbtSource]]:
+        return None if self.attributes is None else self.attributes.sql_dbt_sources
+
+    @sql_dbt_sources.setter
+    def sql_dbt_sources(self, sql_dbt_sources: Optional[List[DbtSource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sql_dbt_sources = sql_dbt_sources
+
+    @property
+    def dbt_models(self) -> Optional[List[DbtModel]]:
+        return None if self.attributes is None else self.attributes.dbt_models
+
+    @dbt_models.setter
+    def dbt_models(self, dbt_models: Optional[List[DbtModel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dbt_models = dbt_models
+
     class Attributes(Tag.Attributes):
         tag_id: Optional[str] = Field(default=None, description="")
         tag_attributes: Optional[List[SourceTagAttribute]] = Field(
             default=None, description=""
         )
         tag_allowed_values: Optional[Set[str]] = Field(default=None, description="")
         mapped_atlan_tag_name: Optional[str] = Field(default=None, description="")
@@ -511,24 +511,24 @@
         last_profiled_at: Optional[datetime] = Field(default=None, description="")
         dbt_sources: Optional[List[DbtSource]] = Field(
             default=None, description=""
         )  # relationship
         sql_dbt_models: Optional[List[DbtModel]] = Field(
             default=None, description=""
         )  # relationship
-        sql_dbt_sources: Optional[List[DbtSource]] = Field(
+        dbt_tests: Optional[List[DbtTest]] = Field(
             default=None, description=""
         )  # relationship
-        dbt_models: Optional[List[DbtModel]] = Field(
+        atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
-        dbt_tests: Optional[List[DbtTest]] = Field(
+        sql_dbt_sources: Optional[List[DbtSource]] = Field(
             default=None, description=""
         )  # relationship
-        atlan_schema: Optional[Schema] = Field(
+        dbt_models: Optional[List[DbtModel]] = Field(
             default=None, description=""
         )  # relationship
 
     attributes: SnowflakeTag.Attributes = Field(
         default_factory=lambda: SnowflakeTag.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/soda.py` & `pyatlan-2.1.9/pyatlan/model/assets/soda.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/soda_check.py` & `pyatlan-2.1.9/pyatlan/model/assets/soda_check.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/spark.py` & `pyatlan-2.1.9/pyatlan/model/assets/spark.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/spark_job.py` & `pyatlan-2.1.9/pyatlan/model/assets/spark_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/table.py` & `pyatlan-2.1.9/pyatlan/model/assets/table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/table_partition.py` & `pyatlan-2.1.9/pyatlan/model/assets/table_partition.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_calculated_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_calculated_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_dashboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_datasource.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_datasource_field.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_flow.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_flow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_metric.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_project.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_project.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,50 +50,50 @@
     PROJECT_HIERARCHY: ClassVar[KeywordField] = KeywordField(
         "projectHierarchy", "projectHierarchy"
     )
     """
     List of top-level projects with their nested child projects.
     """
 
-    PARENT_PROJECT: ClassVar[RelationField] = RelationField("parentProject")
+    WORKBOOKS: ClassVar[RelationField] = RelationField("workbooks")
     """
     TBC
     """
-    WORKBOOKS: ClassVar[RelationField] = RelationField("workbooks")
+    FLOWS: ClassVar[RelationField] = RelationField("flows")
     """
     TBC
     """
-    SITE: ClassVar[RelationField] = RelationField("site")
+    CHILD_PROJECTS: ClassVar[RelationField] = RelationField("childProjects")
     """
     TBC
     """
-    DATASOURCES: ClassVar[RelationField] = RelationField("datasources")
+    PARENT_PROJECT: ClassVar[RelationField] = RelationField("parentProject")
     """
     TBC
     """
-    FLOWS: ClassVar[RelationField] = RelationField("flows")
+    SITE: ClassVar[RelationField] = RelationField("site")
     """
     TBC
     """
-    CHILD_PROJECTS: ClassVar[RelationField] = RelationField("childProjects")
+    DATASOURCES: ClassVar[RelationField] = RelationField("datasources")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "site_qualified_name",
         "top_level_project_qualified_name",
         "is_top_level_project",
         "project_hierarchy",
-        "parent_project",
         "workbooks",
-        "site",
-        "datasources",
         "flows",
         "child_projects",
+        "parent_project",
+        "site",
+        "datasources",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
@@ -137,54 +137,24 @@
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[List[Dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
-    def parent_project(self) -> Optional[TableauProject]:
-        return None if self.attributes is None else self.attributes.parent_project
-
-    @parent_project.setter
-    def parent_project(self, parent_project: Optional[TableauProject]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.parent_project = parent_project
-
-    @property
     def workbooks(self) -> Optional[List[TableauWorkbook]]:
         return None if self.attributes is None else self.attributes.workbooks
 
     @workbooks.setter
     def workbooks(self, workbooks: Optional[List[TableauWorkbook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbooks = workbooks
 
     @property
-    def site(self) -> Optional[TableauSite]:
-        return None if self.attributes is None else self.attributes.site
-
-    @site.setter
-    def site(self, site: Optional[TableauSite]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.site = site
-
-    @property
-    def datasources(self) -> Optional[List[TableauDatasource]]:
-        return None if self.attributes is None else self.attributes.datasources
-
-    @datasources.setter
-    def datasources(self, datasources: Optional[List[TableauDatasource]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.datasources = datasources
-
-    @property
     def flows(self) -> Optional[List[TableauFlow]]:
         return None if self.attributes is None else self.attributes.flows
 
     @flows.setter
     def flows(self, flows: Optional[List[TableauFlow]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -196,39 +166,69 @@
 
     @child_projects.setter
     def child_projects(self, child_projects: Optional[List[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.child_projects = child_projects
 
+    @property
+    def parent_project(self) -> Optional[TableauProject]:
+        return None if self.attributes is None else self.attributes.parent_project
+
+    @parent_project.setter
+    def parent_project(self, parent_project: Optional[TableauProject]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_project = parent_project
+
+    @property
+    def site(self) -> Optional[TableauSite]:
+        return None if self.attributes is None else self.attributes.site
+
+    @site.setter
+    def site(self, site: Optional[TableauSite]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.site = site
+
+    @property
+    def datasources(self) -> Optional[List[TableauDatasource]]:
+        return None if self.attributes is None else self.attributes.datasources
+
+    @datasources.setter
+    def datasources(self, datasources: Optional[List[TableauDatasource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasources = datasources
+
     class Attributes(Tableau.Attributes):
         site_qualified_name: Optional[str] = Field(default=None, description="")
         top_level_project_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         is_top_level_project: Optional[bool] = Field(default=None, description="")
         project_hierarchy: Optional[List[Dict[str, str]]] = Field(
             default=None, description=""
         )
-        parent_project: Optional[TableauProject] = Field(
+        workbooks: Optional[List[TableauWorkbook]] = Field(
             default=None, description=""
         )  # relationship
-        workbooks: Optional[List[TableauWorkbook]] = Field(
+        flows: Optional[List[TableauFlow]] = Field(
             default=None, description=""
         )  # relationship
-        site: Optional[TableauSite] = Field(
+        child_projects: Optional[List[TableauProject]] = Field(
             default=None, description=""
         )  # relationship
-        datasources: Optional[List[TableauDatasource]] = Field(
+        parent_project: Optional[TableauProject] = Field(
             default=None, description=""
         )  # relationship
-        flows: Optional[List[TableauFlow]] = Field(
+        site: Optional[TableauSite] = Field(
             default=None, description=""
         )  # relationship
-        child_projects: Optional[List[TableauProject]] = Field(
+        datasources: Optional[List[TableauDatasource]] = Field(
             default=None, description=""
         )  # relationship
 
     attributes: TableauProject.Attributes = Field(
         default_factory=lambda: TableauProject.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
```

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_site.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_site.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_workbook.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tableau_worksheet.py` & `pyatlan-2.1.9/pyatlan/model/assets/tableau_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tag.py` & `pyatlan-2.1.9/pyatlan/model/assets/tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/tag_attachment.py` & `pyatlan-2.1.9/pyatlan/model/assets/tag_attachment.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_answer.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_answer.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_column.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_dashlet.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_dashlet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_liveboard.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_liveboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_table.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_view.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/assets/thoughtspot_worksheet.py` & `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/atlan_image.py` & `pyatlan-2.1.9/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/audit.py` & `pyatlan-2.1.9/pyatlan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/core.py` & `pyatlan-2.1.9/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/credential.py` & `pyatlan-2.1.9/pyatlan/model/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/custom_metadata.py` & `pyatlan-2.1.9/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/data_mesh.py` & `pyatlan-2.1.9/pyatlan/model/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/enums.py` & `pyatlan-2.1.9/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1836,14 +1836,15 @@
     AWS_LAMBDA_TRIGGER = "atlan-aws-lambda-trigger"
     AZURE_EVENT_HUB = "atlan-azure-event-hub"
     BIGQUERY = "atlan-bigquery"
     BIGQUERY_MINER = "atlan-bigquery-miner"
     CONNECTION_DELETE = "atlan-connection-delete"
     DATABRICKS = "atlan-databricks"
     DATABRICKS_LINEAGE = "atlan-databricks-lineage"
+    DYNAMODB = "atlan-dynamodb"
     DBT = "atlan-dbt"
     FIVETRAN = "atlan-fivetran"
     GLUE = "atlan-glue"
     HIVE = "atlan-hive"
     HIVE_MINER = "atlan-hive-miner"
     KAFKA = "atlan-kafka"
     KAFKA_AIVEN = "atlan-kafka-aiven"
```

### Comparing `pyatlan-2.1.8/pyatlan/model/events.py` & `pyatlan-2.1.9/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/fields/atlan_fields.py` & `pyatlan-2.1.9/pyatlan/model/fields/atlan_fields.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/fluent_search.py` & `pyatlan-2.1.9/pyatlan/model/fluent_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/fluent_tasks.py` & `pyatlan-2.1.9/pyatlan/model/fluent_tasks.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/group.py` & `pyatlan-2.1.9/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/keycloak_events.py` & `pyatlan-2.1.9/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/lineage.py` & `pyatlan-2.1.9/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/base/crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/base/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     group, or user defined as an admin (or any of them are invalid)
     """
 
     def __init__(
         self,
         connection_name: str,
         connection_type: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
         source_logo: str = "",
     ):
         super().__init__()
         self._connection_name = connection_name
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/base/miner.py` & `pyatlan-2.1.9/pyatlan/model/packages/base/miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/base/package.py` & `pyatlan-2.1.9/pyatlan/model/packages/base/package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/confluent_kafka_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/confluent_kafka_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     _CONNECTOR_TYPE = AtlanConnectorType.CONFLUENT_KAFKA
     _PACKAGE_ICON = "https://cdn.confluent.io/wp-content/uploads/apache-kafka-icon-2021-e1638496305992.jpg"
     _PACKAGE_LOGO = "https://cdn.confluent.io/wp-content/uploads/apache-kafka-icon-2021-e1638496305992.jpg"
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/dbt_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/dbt_crawler.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     _CONNECTOR_TYPE = AtlanConnectorType.DBT
     _PACKAGE_ICON = "https://assets.atlan.com/assets/dbt-new.svg"
     _PACKAGE_LOGO = "https://assets.atlan.com/assets/dbt-new.svg"
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/glue_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/glue_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     _PACKAGE_LOGO = (
         "https://atlan-public.s3.eu-west-1.amazonaws.com/atlan/logos/aws-glue.png"
     )
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/powerbi_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/powerbi_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     _PACKAGE_LOGO = (
         "https://powerbi.microsoft.com/pictures/application-logos/svg/powerbi.svg"
     )
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
@@ -62,15 +62,15 @@
 
         :returns: rawler, set up to extract directly from Power BI
         """
         local_creds = {
             "name": f"default-{self._NAME}-{self._epoch}-0",
             "host": "api.powerbi.com",
             "port": 443,
-            "connectorConfigName": f"atlan-connectors-{self._NAME}",
+            "connector_config_name": f"atlan-connectors-{self._NAME}",
         }
         self._credentials_body.update(local_creds)
         return self
 
     def delegated_user(
         self,
         username: str,
@@ -133,32 +133,30 @@
         :return: crawler, set to include only those workspaces specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         include_workspaces = workspaces or []
         to_include = self.build_flat_filter(include_workspaces)
         self._parameters.append(
-            dict(name="include-filter", value=to_include if to_include else "{}")
+            dict(dict(name="include-filter", value=to_include or "{}"))
         )
         return self
 
     def exclude(self, workspaces: List[str]) -> PowerBICrawler:
         """
         Defines the filter for workspaces to exclude when crawling.
 
         :param workspaces: the GUIDs of workspaces to exclude when crawling
         :return: crawler, set to exclude only those workspaces specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         exclude_workspaces = workspaces or []
         to_exclude = self.build_flat_filter(exclude_workspaces)
-        self._parameters.append(
-            dict(name="exclude-filter", value=to_exclude if to_exclude else "{}")
-        )
+        self._parameters.append(dict(name="exclude-filter", value=to_exclude or "{}"))
         return self
 
     def direct_endorsements(self, enabled: bool = True) -> PowerBICrawler:
         """
         Whether to directly attach endorsements as
         certificates (True), or instead raise these as requests
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/sigma_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/sigma_crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         AWS = "aws-api.sigmacomputing.com"
         AWS_CANADA = "api.ca.aws.sigmacomputing.com"
         AWS_EUROPE = "api.eu.aws.sigmacomputing.com"
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
@@ -107,15 +107,15 @@
         :returns: crawler, set to include only those workbooks specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         include_workbooks = workbooks or []
         to_include = self.build_flat_filter(include_workbooks)
         self._parameters.append(
-            dict(name="include-filter", value=to_include if to_include else "{}")
+            dict(dict(name="include-filter", value=to_include or "{}"))
         )
         return self
 
     def exclude(self, workbooks: List[str]) -> SigmaCrawler:
         """
         Defines the filter for Sigma workbooks to exclude when crawling.
 
@@ -123,17 +123,15 @@
         default to no workbooks if `None` are specified
         :returns: crawler, set to exclude only those workbooks specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         exclude_workbooks = workbooks or []
         to_exclude = self.build_flat_filter(exclude_workbooks)
-        self._parameters.append(
-            dict(name="exclude-filter", value=to_exclude if to_exclude else "{}")
-        )
+        self._parameters.append(dict(name="exclude-filter", value=to_exclude or "{}"))
         return self
 
     def _set_required_metadata_params(self):
         self._parameters.append(
             {"name": "credential-guid", "value": "{{credentialGuid}}"}
         )
         self._parameters.append(
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/snowflake_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/snowflake_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     _CONNECTOR_TYPE = AtlanConnectorType.SNOWFLAKE
     _PACKAGE_ICON = "https://docs.snowflake.com/en/_images/logo-snowflake-sans-text.png"
     _PACKAGE_LOGO = "https://1amiydhcmj36tz3733v94f15-wpengine.netdna-ssl.com/wp-content/themes/snowflake/assets/img/logo-blue.svg"  # noqa
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = True,
         allow_query_preview: bool = True,
         row_limit: int = 10000,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
@@ -182,32 +182,30 @@
         :returns: crawler, set to include only those assets specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         include_assets = assets or {}
         to_include = self.build_hierarchical_filter(include_assets)
         self._parameters.append(
-            dict(name="include-filter", value=to_include if to_include else "{}")
+            dict(dict(name="include-filter", value=to_include or "{}"))
         )
         return self
 
     def exclude(self, assets: dict) -> SnowflakeCrawler:
         """
         Defines the filter for assets to exclude when crawling.
 
         :param assets: Map keyed by database name with each value being a list of schemas
         :returns: crawler, set to exclude only those assets specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         exclude_assets = assets or {}
         to_exclude = self.build_hierarchical_filter(exclude_assets)
-        self._parameters.append(
-            dict(name="exclude-filter", value=to_exclude if to_exclude else "{}")
-        )
+        self._parameters.append(dict(name="exclude-filter", value=to_exclude or "{}"))
         return self
 
     def _set_required_metadata_params(self):
         self._parameters.append(
             {"name": "credential-guid", "value": "{{credentialGuid}}"}
         )
         self._parameters.append(dict(name="control-config-strategy", value="default"))
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/snowflake_miner.py` & `pyatlan-2.1.9/pyatlan/model/packages/snowflake_miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/sql_server_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/sql_server_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     _CONNECTOR_TYPE = AtlanConnectorType.MSSQL
     _PACKAGE_ICON = "https://user-images.githubusercontent.com/4249331/52232852-e2c4f780-28bd-11e9-835d-1e3cf3e43888.png"  # noqa
     _PACKAGE_LOGO = "https://user-images.githubusercontent.com/4249331/52232852-e2c4f780-28bd-11e9-835d-1e3cf3e43888.png"  # noqa
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = True,
         allow_query_preview: bool = True,
         row_limit: int = 10000,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
@@ -98,15 +98,15 @@
         :returns: crawler, set to include only those assets specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         include_assets = assets or {}
         to_include = self.build_hierarchical_filter(include_assets)
         self._parameters.append(
-            dict(name="include-filter", value=to_include if to_include else "{}")
+            dict(dict(name="include-filter", value=to_include or "{}"))
         )
         return self
 
     def exclude(self, assets: dict) -> SQLServerCrawler:
         """
         Defines the filter for assets to exclude when crawling.
 
@@ -114,17 +114,15 @@
         with each value being a list of schemas
         :returns: crawler, set to exclude only those assets specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         exclude_assets = assets or {}
         to_exclude = self.build_hierarchical_filter(exclude_assets)
-        self._parameters.append(
-            dict(name="exclude-filter", value=to_exclude if to_exclude else "{}")
-        )
+        self._parameters.append(dict(name="exclude-filter", value=to_exclude or "{}"))
         return self
 
     def _set_required_metadata_params(self):
         self._parameters.append(
             {"name": "credential-guid", "value": "{{credentialGuid}}"}
         )
         self._parameters.append(dict(name="publish-mode", value="production"))
```

### Comparing `pyatlan-2.1.8/pyatlan/model/packages/tableau_crawler.py` & `pyatlan-2.1.9/pyatlan/model/packages/tableau_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     _CONNECTOR_TYPE = AtlanConnectorType.TABLEAU
     _PACKAGE_ICON = "https://img.icons8.com/color/480/000000/tableau-software.png"
     _PACKAGE_LOGO = "https://img.icons8.com/color/480/000000/tableau-software.png"
 
     def __init__(
         self,
         connection_name: str,
-        admin_roles: Optional[List[str]],
-        admin_groups: Optional[List[str]],
-        admin_users: Optional[List[str]],
+        admin_roles: Optional[List[str]] = None,
+        admin_groups: Optional[List[str]] = None,
+        admin_users: Optional[List[str]] = None,
         allow_query: bool = False,
         allow_query_preview: bool = False,
         row_limit: int = 0,
     ):
         super().__init__(
             connection_name=connection_name,
             connection_type=self._CONNECTOR_TYPE,
@@ -72,15 +72,15 @@
             "name": f"default-{self._NAME}-{self._epoch}-0",
             "host": hostname,
             "port": port,
             "extra": {
                 "protocol": "https" if ssl_enabled else "http",
                 "defaultSite": site,
             },
-            "connectorConfigName": f"atlan-connectors-{self._NAME}",
+            "connector_config_name": f"atlan-connectors-{self._NAME}",
         }
         self._credentials_body.update(local_creds)
         self._parameters.append({"name": "extraction-method", "value": "direct"})
         return self
 
     def basic_auth(self, username: str, password: str) -> TableauCrawler:
         """
@@ -122,32 +122,30 @@
         :returns: crawler, set to include only those projects specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         include_projects = projects or []
         to_include = self.build_flat_filter(include_projects)
         self._parameters.append(
-            dict(name="include-filter", value=to_include if to_include else "{}")
+            dict(dict(name="include-filter", value=to_include or "{}"))
         )
         return self
 
     def exclude(self, projects: List[str]) -> TableauCrawler:
         """
         Defines the filter for projects to exclude when crawling.
 
         :param projects: the GUIDs of projects to exclude when crawling
         :returns: crawler, set to exclude only those projects specified
         :raises InvalidRequestException: In the unlikely
         event the provided filter cannot be translated
         """
         exclude_projects = projects or []
         to_exclude = self.build_flat_filter(exclude_projects)
-        self._parameters.append(
-            dict(name="exclude-filter", value=to_exclude if to_exclude else "{}")
-        )
+        self._parameters.append(dict(name="exclude-filter", value=to_exclude or "{}"))
         return self
 
     def crawl_hidden_fields(self, enabled: bool = True) -> TableauCrawler:
         """
         Whether to crawl hidden datasource fields (True) or not.
 
         :param enabled: If True, hidden datasource fields
```

### Comparing `pyatlan-2.1.8/pyatlan/model/query.py` & `pyatlan-2.1.9/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/response.py` & `pyatlan-2.1.9/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/role.py` & `pyatlan-2.1.9/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/search.py` & `pyatlan-2.1.9/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/search_log.py` & `pyatlan-2.1.9/pyatlan/model/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/sso.py` & `pyatlan-2.1.9/pyatlan/model/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/structs.py` & `pyatlan-2.1.9/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,57 +54,35 @@
 class AwsCloudWatchMetric(AtlanObject):
     """Description"""
 
     aws_cloud_watch_metric_name: str = Field(description="")
     aws_cloud_watch_metric_scope: str = Field(description="")
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    boundaries: Set[float] = Field(description="")
-    frequencies: Set[float] = Field(description="")
-
-
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     topic_name: Optional[str] = Field(default=None, description="")
     topic_partition: Optional[str] = Field(default=None, description="")
     topic_lag: Optional[int] = Field(default=None, description="")
     topic_current_offset: Optional[int] = Field(default=None, description="")
 
 
-class ColumnValueFrequencyMap(AtlanObject):
-    """Description"""
-
-    column_value: Optional[str] = Field(default=None, description="")
-    column_value_frequency: Optional[int] = Field(default=None, description="")
-
-
-class SourceTagAttachmentValue(AtlanObject):
+class Histogram(AtlanObject):
     """Description"""
 
-    tag_attachment_key: Optional[str] = Field(default=None, description="")
-    tag_attachment_value: Optional[str] = Field(default=None, description="")
+    boundaries: Set[float] = Field(description="")
+    frequencies: Set[float] = Field(description="")
 
 
-class SourceTagAttachment(AtlanObject):
+class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
-    source_tag_name: Optional[str] = Field(default=None, description="")
-    source_tag_qualified_name: Optional[str] = Field(default=None, description="")
-    source_tag_guid: Optional[str] = Field(default=None, description="")
-    source_tag_connector_name: Optional[str] = Field(default=None, description="")
-    source_tag_value: Optional[List[SourceTagAttachmentValue]] = Field(
-        default=None, description=""
-    )
-    is_source_tag_synced: Optional[bool] = Field(default=None, description="")
-    source_tag_sync_timestamp: Optional[datetime] = Field(default=None, description="")
-    source_tag_sync_error: Optional[str] = Field(default=None, description="")
+    column_value: Optional[str] = Field(default=None, description="")
+    column_value_frequency: Optional[int] = Field(default=None, description="")
 
 
 class BadgeCondition(AtlanObject):
     """Description"""
 
     @classmethod
     def create(
@@ -133,28 +111,50 @@
         )
 
     badge_condition_operator: Optional[str] = Field(default=None, description="")
     badge_condition_value: Optional[str] = Field(default=None, description="")
     badge_condition_colorhex: Optional[str] = Field(default=None, description="")
 
 
-class StarredDetails(AtlanObject):
+class SourceTagAttachment(AtlanObject):
     """Description"""
 
-    asset_starred_by: Optional[str] = Field(default=None, description="")
-    asset_starred_at: Optional[datetime] = Field(default=None, description="")
+    source_tag_name: Optional[str] = Field(default=None, description="")
+    source_tag_qualified_name: Optional[str] = Field(default=None, description="")
+    source_tag_guid: Optional[str] = Field(default=None, description="")
+    source_tag_connector_name: Optional[str] = Field(default=None, description="")
+    source_tag_value: Optional[List[SourceTagAttachmentValue]] = Field(
+        default=None, description=""
+    )
+    is_source_tag_synced: Optional[bool] = Field(default=None, description="")
+    source_tag_sync_timestamp: Optional[datetime] = Field(default=None, description="")
+    source_tag_sync_error: Optional[str] = Field(default=None, description="")
+
+
+class SourceTagAttachmentValue(AtlanObject):
+    """Description"""
+
+    tag_attachment_key: Optional[str] = Field(default=None, description="")
+    tag_attachment_value: Optional[str] = Field(default=None, description="")
 
 
 class AzureTag(AtlanObject):
     """Description"""
 
     azure_tag_key: str = Field(description="")
     azure_tag_value: str = Field(description="")
 
 
+class StarredDetails(AtlanObject):
+    """Description"""
+
+    asset_starred_by: Optional[str] = Field(default=None, description="")
+    asset_starred_at: Optional[datetime] = Field(default=None, description="")
+
+
 class AuthPolicyCondition(AtlanObject):
     """Description"""
 
     policy_condition_type: str = Field(description="")
     policy_condition_values: Set[str] = Field(description="")
 
 
@@ -238,30 +238,30 @@
     )
 
 
 MCRuleSchedule.update_forward_refs()
 
 AwsCloudWatchMetric.update_forward_refs()
 
-Histogram.update_forward_refs()
-
 KafkaTopicConsumption.update_forward_refs()
 
+Histogram.update_forward_refs()
+
 ColumnValueFrequencyMap.update_forward_refs()
 
-SourceTagAttachmentValue.update_forward_refs()
+BadgeCondition.update_forward_refs()
 
 SourceTagAttachment.update_forward_refs()
 
-BadgeCondition.update_forward_refs()
-
-StarredDetails.update_forward_refs()
+SourceTagAttachmentValue.update_forward_refs()
 
 AzureTag.update_forward_refs()
 
+StarredDetails.update_forward_refs()
+
 AuthPolicyCondition.update_forward_refs()
 
 AwsTag.update_forward_refs()
 
 DbtMetricFilter.update_forward_refs()
 
 GoogleTag.update_forward_refs()
```

### Comparing `pyatlan-2.1.8/pyatlan/model/task.py` & `pyatlan-2.1.9/pyatlan/model/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/typedef.py` & `pyatlan-2.1.9/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/user.py` & `pyatlan-2.1.9/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/utils.py` & `pyatlan-2.1.9/pyatlan/model/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/model/workflow.py` & `pyatlan-2.1.9/pyatlan/model/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/multipart_data_generator.py` & `pyatlan-2.1.9/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/create_package_files.py` & `pyatlan-2.1.9/pyatlan/pkg/create_package_files.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/models.py` & `pyatlan-2.1.9/pyatlan/pkg/models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/templates/default_configmap.jinja2` & `pyatlan-2.1.9/pyatlan/pkg/templates/default_configmap.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/templates/default_template.jinja2` & `pyatlan-2.1.9/pyatlan/pkg/templates/default_template.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/templates/package_config.jinja2` & `pyatlan-2.1.9/pyatlan/pkg/templates/package_config.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/ui.py` & `pyatlan-2.1.9/pyatlan/pkg/ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/utils.py` & `pyatlan-2.1.9/pyatlan/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/pkg/widgets.py` & `pyatlan-2.1.9/pyatlan/pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan/utils.py` & `pyatlan-2.1.9/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/pyatlan.egg-info/PKG-INFO` & `pyatlan-2.1.9/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.8
+Version: 2.1.9
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.8/pyatlan.egg-info/SOURCES.txt` & `pyatlan-2.1.9/pyatlan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,17 @@
 pyatlan/model/assets/atlas_glossary_category.py
 pyatlan/model/assets/atlas_glossary_term.py
 pyatlan/model/assets/auth_policy.py
 pyatlan/model/assets/auth_service.py
 pyatlan/model/assets/azure.py
 pyatlan/model/assets/azure_event_hub.py
 pyatlan/model/assets/azure_event_hub_consumer_group.py
+pyatlan/model/assets/azure_service_bus.py
+pyatlan/model/assets/azure_service_bus_namespace.py
+pyatlan/model/assets/azure_service_bus_topic.py
 pyatlan/model/assets/b_i.py
 pyatlan/model/assets/b_i_process.py
 pyatlan/model/assets/badge.py
 pyatlan/model/assets/calculation_view.py
 pyatlan/model/assets/catalog.py
 pyatlan/model/assets/cloud.py
 pyatlan/model/assets/cognite.py
@@ -128,18 +131,22 @@
 pyatlan/model/assets/cognite_file.py
 pyatlan/model/assets/cognite_sequence.py
 pyatlan/model/assets/cognite_time_series.py
 pyatlan/model/assets/collection.py
 pyatlan/model/assets/column.py
 pyatlan/model/assets/column_process.py
 pyatlan/model/assets/connection.py
+pyatlan/model/assets/cosmos_mongo_d_b.py
+pyatlan/model/assets/cosmos_mongo_d_b_collection.py
+pyatlan/model/assets/cosmos_mongo_d_b_database.py
 pyatlan/model/assets/cube.py
 pyatlan/model/assets/cube_dimension.py
 pyatlan/model/assets/cube_field.py
 pyatlan/model/assets/cube_hierarchy.py
+pyatlan/model/assets/data_contract.py
 pyatlan/model/assets/data_domain.py
 pyatlan/model/assets/data_mesh.py
 pyatlan/model/assets/data_product.py
 pyatlan/model/assets/data_quality.py
 pyatlan/model/assets/data_set.py
 pyatlan/model/assets/data_studio.py
 pyatlan/model/assets/data_studio_asset.py
@@ -329,18 +336,22 @@
 pyatlan/model/assets/thoughtspot_table.py
 pyatlan/model/assets/thoughtspot_view.py
 pyatlan/model/assets/thoughtspot_worksheet.py
 pyatlan/model/assets/view.py
 pyatlan/model/fields/__init__.py
 pyatlan/model/fields/atlan_fields.py
 pyatlan/model/packages/__init__.py
+pyatlan/model/packages/big_query_crawler.py
 pyatlan/model/packages/confluent_kafka_crawler.py
 pyatlan/model/packages/dbt_crawler.py
+pyatlan/model/packages/dynamo_d_b_crawler.py
 pyatlan/model/packages/glue_crawler.py
+pyatlan/model/packages/postgres_crawler.py
 pyatlan/model/packages/powerbi_crawler.py
+pyatlan/model/packages/s_q_l_server_crawler.py
 pyatlan/model/packages/sigma_crawler.py
 pyatlan/model/packages/snowflake_crawler.py
 pyatlan/model/packages/snowflake_miner.py
 pyatlan/model/packages/sql_server_crawler.py
 pyatlan/model/packages/tableau_crawler.py
 pyatlan/model/packages/base/__init__.py
 pyatlan/model/packages/base/crawler.py
```

### Comparing `pyatlan-2.1.8/setup.py` & `pyatlan-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/adls_asset_test.py` & `pyatlan-2.1.9/tests/integration/adls_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/admin_test.py` & `pyatlan-2.1.9/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/airflow_asset_test.py` & `pyatlan-2.1.9/tests/integration/airflow_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/api_asset_test.py` & `pyatlan-2.1.9/tests/integration/api_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/atlan_tag_test.py` & `pyatlan-2.1.9/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/client.py` & `pyatlan-2.1.9/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/connection_test.py` & `pyatlan-2.1.9/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/custom_metadata_test.py` & `pyatlan-2.1.9/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/custom_package_test.py` & `pyatlan-2.1.9/tests/integration/custom_package_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/data_mesh_test.py` & `pyatlan-2.1.9/tests/integration/data_mesh_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/data_studio_asset_test.py` & `pyatlan-2.1.9/tests/integration/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/file_test.py` & `pyatlan-2.1.9/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/gcs_asset_test.py` & `pyatlan-2.1.9/tests/integration/gcs_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/glossary_test.py` & `pyatlan-2.1.9/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/lineage_test.py` & `pyatlan-2.1.9/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/owner_propagator_cfg.py` & `pyatlan-2.1.9/tests/integration/owner_propagator_cfg.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/persona_test.py` & `pyatlan-2.1.9/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/preset_asset_test.py` & `pyatlan-2.1.9/tests/integration/preset_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/purpose_test.py` & `pyatlan-2.1.9/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/query_parser_test.py` & `pyatlan-2.1.9/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/requests_test.py` & `pyatlan-2.1.9/tests/integration/requests_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/s3_asset_test.py` & `pyatlan-2.1.9/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_client.py` & `pyatlan-2.1.9/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_file_client.py` & `pyatlan-2.1.9/tests/integration/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_index_search.py` & `pyatlan-2.1.9/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_sql_assets.py` & `pyatlan-2.1.9/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_sso_client.py` & `pyatlan-2.1.9/tests/integration/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_task_client.py` & `pyatlan-2.1.9/tests/integration/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/test_workflow_client.py` & `pyatlan-2.1.9/tests/integration/test_workflow_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/integration/utils.py` & `pyatlan-2.1.9/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/conftest.py` & `pyatlan-2.1.9/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/constants.py` & `pyatlan-2.1.9/tests/unit/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/a_d_l_s_account_test.py` & `pyatlan-2.1.9/tests/unit/model/a_d_l_s_account_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/a_d_l_s_container_test.py` & `pyatlan-2.1.9/tests/unit/model/a_d_l_s_container_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/a_d_l_s_object_test.py` & `pyatlan-2.1.9/tests/unit/model/a_d_l_s_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/a_p_i_path_test.py` & `pyatlan-2.1.9/tests/unit/model/a_p_i_path_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/a_p_i_spec_test.py` & `pyatlan-2.1.9/tests/unit/model/a_p_i_spec_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/airflow_dag.py` & `pyatlan-2.1.9/tests/unit/model/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/airflow_task.py` & `pyatlan-2.1.9/tests/unit/model/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/badge_condition_test.py` & `pyatlan-2.1.9/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/badge_test.py` & `pyatlan-2.1.9/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/column_process_test.py` & `pyatlan-2.1.9/tests/unit/model/column_process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/column_test.py` & `pyatlan-2.1.9/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/connection_test.py` & `pyatlan-2.1.9/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/constants.py` & `pyatlan-2.1.9/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/data_domain_test.py` & `pyatlan-2.1.9/tests/unit/model/data_domain_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/data_product_test.py` & `pyatlan-2.1.9/tests/unit/model/data_product_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/data_studio_asset_test.py` & `pyatlan-2.1.9/tests/unit/model/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/database_test.py` & `pyatlan-2.1.9/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/fields/atlan_fields_test.py` & `pyatlan-2.1.9/tests/unit/model/fields/atlan_fields_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/file_test.py` & `pyatlan-2.1.9/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/gcs_bucket_test.py` & `pyatlan-2.1.9/tests/unit/model/gcs_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/gcs_object_test.py` & `pyatlan-2.1.9/tests/unit/model/gcs_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/glossary_category_test.py` & `pyatlan-2.1.9/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/glossary_term_test.py` & `pyatlan-2.1.9/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/glossary_test.py` & `pyatlan-2.1.9/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/materialised_view_test.py` & `pyatlan-2.1.9/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/preset_chart_test.py` & `pyatlan-2.1.9/tests/unit/model/preset_chart_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/preset_dashboard_test.py` & `pyatlan-2.1.9/tests/unit/model/preset_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/preset_dataset_test.py` & `pyatlan-2.1.9/tests/unit/model/preset_dataset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/preset_workspace_test.py` & `pyatlan-2.1.9/tests/unit/model/preset_workspace_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/process_test.py` & `pyatlan-2.1.9/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/readme_test.py` & `pyatlan-2.1.9/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/s3_bucket_test.py` & `pyatlan-2.1.9/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/s3object_test.py` & `pyatlan-2.1.9/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/schema_test.py` & `pyatlan-2.1.9/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/table_test.py` & `pyatlan-2.1.9/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/model/view_test.py` & `pyatlan-2.1.9/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/pkg/conftest.py` & `pyatlan-2.1.9/tests/unit/pkg/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/pkg/test_models.py` & `pyatlan-2.1.9/tests/unit/pkg/test_models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/pkg/test_ui.py` & `pyatlan-2.1.9/tests/unit/pkg/test_ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/pkg/test_utils.py` & `pyatlan-2.1.9/tests/unit/pkg/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/pkg/test_widgets.py` & `pyatlan-2.1.9/tests/unit/pkg/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_atlan_tag_name.py` & `pyatlan-2.1.9/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_client.py` & `pyatlan-2.1.9/tests/unit/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -881,15 +881,14 @@
         assert mock_find_category_fast_by_name.return_value == category
 
 
 @patch.object(AssetClient, "find_glossary_by_name")
 def test_find_category_by_name_qn_guid_correctly_populated(
     mock_find_glossary_by_name, mock_api_caller, glossary_category_by_name_json
 ):
-
     client = AssetClient(mock_api_caller)
     mock_find_glossary_by_name.return_value.qualified_name = GLOSSARY_QUALIFIED_NAME
     mock_api_caller._call_api.side_effect = [glossary_category_by_name_json]
 
     category = client.find_category_by_name(
         name="test-cat-1-1",
         glossary_name="test-glossary",
```

### Comparing `pyatlan-2.1.8/tests/unit/test_core.py` & `pyatlan-2.1.9/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_credential_client.py` & `pyatlan-2.1.9/tests/unit/test_credential_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_custom_metadata.py` & `pyatlan-2.1.9/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_deprecated.py` & `pyatlan-2.1.9/tests/unit/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_events.py` & `pyatlan-2.1.9/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_file_client.py` & `pyatlan-2.1.9/tests/unit/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_glossary_term.py` & `pyatlan-2.1.9/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_lineage.py` & `pyatlan-2.1.9/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_model.py` & `pyatlan-2.1.9/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_packages.py` & `pyatlan-2.1.9/tests/unit/test_packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 
 from pyatlan.errors import InvalidRequestError
 from pyatlan.model.packages import (
+    BigQueryCrawler,
     ConfluentKafkaCrawler,
     DbtCrawler,
+    DynamoDBCrawler,
     GlueCrawler,
+    PostgresCrawler,
     PowerBICrawler,
     SigmaCrawler,
     SnowflakeCrawler,
     SnowflakeMiner,
     SQLServerCrawler,
     TableauCrawler,
 )
@@ -29,14 +32,21 @@
 POWERBI_DELEGATED_USER = "powerbi_delegated_user.json"
 POWEBI_SERVICE_PRINCIPAL = "powerbi_service_principal.json"
 CONFLUENT_KAFKA_DIRECT = "confluent_kafka_direct.json"
 DBT_CORE = "dbt_core.json"
 DBT_CLOUD = "dbt_cloud.json"
 SIGMA_API_TOKEN = "sigma_api_token.json"
 SQL_SERVER_BASIC = "sql_server_basic.json"
+BIG_QUERY_DIRECT = "big_query_direct.json"
+DYNAMO_DB_IAM_USER = "dynamo_db_iam_user.json"
+DYNAMO_DB_IAM_USER_ROLE = "dynamo_db_iam_user_role.json"
+POSTGRES_DIRECT_BASIC = "postgres_direct_basic.json"
+POSTGRES_DIRECT_IAM_USER = "postgres_direct_iam_user.json"
+POSTGRES_DIRECT_IAM_ROLE = "postgres_direct_iam_role.json"
+POSTGRES_S3_OFFLINE = "postgres_s3_offline.json"
 
 
 class NonSerializable:
     pass
 
 
 INVALID_REQ_ERROR = (
@@ -74,14 +84,37 @@
 ):
     mock_role_cache.validate_idstrs
     mock_user_cache.validate_names
     mock_group_cache.validate_aliases
 
 
 def test_snowflake_package(mock_package_env):
+    snowflake_with_connection_default = (
+        SnowflakeCrawler(
+            connection_name="test-snowflake-basic-conn",
+            admin_roles=["admin-guid-1234"],
+        )
+        .information_schema(hostname="test-hostname")
+        .basic_auth(
+            username="test-user",
+            password="test-pass",
+            role="test-role",
+            warehouse="test-warehouse",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .lineage(True)
+        .tags(True)
+        .to_workflow()
+    )
+    request_json = loads(
+        snowflake_with_connection_default.json(by_alias=True, exclude_none=True)
+    )
+    assert request_json == load_json(SNOWFLAKE_BASIC)
+
     snowflake_basic_auth = (
         SnowflakeCrawler(
             connection_name="test-snowflake-basic-conn",
             admin_roles=["admin-guid-1234"],
             admin_groups=None,
             admin_users=None,
         )
@@ -392,14 +425,160 @@
     )
     request_json = loads(
         snowflake_miner_s3_offline.json(by_alias=True, exclude_none=True)
     )
     assert request_json == load_json(SNOWFLAKE_MINER_S3_OFFLINE)
 
 
+def test_big_query_package(mock_package_env):
+    big_query_direct = (
+        BigQueryCrawler(
+            connection_name="test-big-query-conn", admin_roles=["admin-guid-1234"]
+        )
+        .service_account_auth(
+            project_id="test-project-id",
+            service_account_json="test-account-json",
+            service_account_email="test@test.com",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .exclude_regex(regex=".*_TEST")
+        .custom_config(config={"test": True, "feature": 1234})
+        .to_workflow()
+    )
+    request_json = loads(big_query_direct.json(by_alias=True, exclude_none=True))
+    assert request_json == load_json(BIG_QUERY_DIRECT)
+
+
+def test_dynamo_db_package(mock_package_env):
+    dynamo_db_direct_iam_user = (
+        DynamoDBCrawler(
+            connection_name="test-dynamodb-conn", admin_roles=["admin-guid-1234"]
+        )
+        .direct(region="test-region")
+        .iam_user_auth(access_key="test-access-key", secret_key="test-secret-key")
+        .include_regex(regex=".*_TEST_INCLUDE")
+        .exclude_regex(regex=".*_TEST_EXCLUDE")
+        .to_workflow()
+    )
+    request_json = loads(
+        dynamo_db_direct_iam_user.json(by_alias=True, exclude_none=True)
+    )
+    assert request_json == load_json(DYNAMO_DB_IAM_USER)
+
+    dynamo_db_direct_iam_user_role = (
+        DynamoDBCrawler(
+            connection_name="test-dynamodb-conn", admin_roles=["admin-guid-1234"]
+        )
+        .direct(region="test-region")
+        .iam_user_role_auth(
+            arn="arn:aws:iam::123456789012:user/test", external_id="test-ext-id"
+        )
+        .include_regex(regex=".*_TEST_INCLUDE")
+        .exclude_regex(regex=".*_TEST_EXCLUDE")
+        .to_workflow()
+    )
+    request_json = loads(
+        dynamo_db_direct_iam_user_role.json(by_alias=True, exclude_none=True)
+    )
+    assert request_json == load_json(DYNAMO_DB_IAM_USER_ROLE)
+
+
+def test_postgres_package(mock_package_env):
+    postgres_direct_basic = (
+        PostgresCrawler(
+            connection_name="test-sdk-postgresql",
+            admin_roles=["admin-guid-1234"],
+        )
+        .direct(hostname="test.com", database="test-db")
+        .basic_auth(
+            username="test-user",
+            password="test-password",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .exclude_regex(regex=".*_TEST")
+        .source_level_filtering(enable=True)
+        .jdbc_internal_methods(enable=True)
+        .to_workflow()
+    )
+
+    request_json = loads(postgres_direct_basic.json(by_alias=True, exclude_none=True))
+    assert request_json == load_json(POSTGRES_DIRECT_BASIC)
+
+    postgres_direct_iam_user = (
+        PostgresCrawler(
+            connection_name="test-sdk-postgresql",
+            admin_roles=["admin-guid-1234"],
+        )
+        .direct(hostname="test.com", database="test-db")
+        .iam_user_auth(
+            username="test-user",
+            access_key="test-access-key",
+            secret_key="test-secret-key",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .exclude_regex(regex=".*_TEST")
+        .source_level_filtering(enable=True)
+        .jdbc_internal_methods(enable=True)
+        .to_workflow()
+    )
+
+    request_json = loads(
+        postgres_direct_iam_user.json(by_alias=True, exclude_none=True)
+    )
+    assert request_json == load_json(POSTGRES_DIRECT_IAM_USER)
+
+    postgres_direct_iam_role = (
+        PostgresCrawler(
+            connection_name="test-sdk-postgresql",
+            admin_roles=["admin-guid-1234"],
+        )
+        .direct(hostname="test.com", database="test-db")
+        .iam_user_role_auth(
+            username="test-user",
+            arn="arn:aws:iam::123456789012:user/test",
+            external_id="test-ext-id",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .exclude_regex(regex=".*_TEST")
+        .source_level_filtering(enable=True)
+        .jdbc_internal_methods(enable=True)
+        .to_workflow()
+    )
+
+    request_json = loads(
+        postgres_direct_iam_role.json(by_alias=True, exclude_none=True)
+    )
+    assert request_json == load_json(POSTGRES_DIRECT_IAM_ROLE)
+
+    postgres_s3_offline = (
+        PostgresCrawler(
+            connection_name="test-sdk-postgresql",
+            admin_roles=["admin-guid-1234"],
+        )
+        .s3(
+            bucket_name="test-bucket",
+            bucket_prefix="test-prefix",
+            bucket_region="test-region",
+        )
+        .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
+        .exclude(assets=None)
+        .exclude_regex(regex=".*_TEST")
+        .source_level_filtering(enable=True)
+        .jdbc_internal_methods(enable=True)
+        .to_workflow()
+    )
+
+    request_json = loads(postgres_s3_offline.json(by_alias=True, exclude_none=True))
+    assert request_json == load_json(POSTGRES_S3_OFFLINE)
+
+
 @pytest.mark.parametrize(
     "test_assets",
     [
         "abc",
         123,
         {"abc": 123},
         [123],
@@ -407,15 +586,14 @@
         [NonSerializable()],
         {"abc": NonSerializable()},
     ],
 )
 def test_wrong_hierarchical_filter_raises_invalid_req_err(
     test_assets, mock_package_env
 ):
-
     with pytest.raises(
         InvalidRequestError,
         match=INVALID_REQ_ERROR,
     ):
         SnowflakeCrawler(
             connection_name="test-snowflake-conn",
             admin_roles=["admin-guid-1234"],
@@ -425,15 +603,14 @@
 
 
 @pytest.mark.parametrize(
     "test_projects",
     [[NonSerializable()], NonSerializable()],
 )
 def test_wrong_flat_filter_raises_invalid_req_err(test_projects, mock_package_env):
-
     with pytest.raises(
         InvalidRequestError,
         match=INVALID_REQ_ERROR,
     ):
         TableauCrawler(
             connection_name="test-tableau-conn",
             admin_roles=["admin-guid-1234"],
@@ -445,15 +622,14 @@
 @pytest.mark.parametrize(
     "test_assets",
     [NonSerializable(), [NonSerializable()]],
 )
 def test_wrong_glue_package_filter_raises_invalid_req_err(
     test_assets, mock_package_env
 ):
-
     with pytest.raises(
         InvalidRequestError,
         match=INVALID_REQ_ERROR,
     ):
         GlueCrawler(
             connection_name="test-glue-conn",
             admin_roles=["admin-guid-1234"],
```

### Comparing `pyatlan-2.1.8/tests/unit/test_query_client.py` & `pyatlan-2.1.9/tests/unit/test_query_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_search_model.py` & `pyatlan-2.1.9/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_sso_client.py` & `pyatlan-2.1.9/tests/unit/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_structs.py` & `pyatlan-2.1.9/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_task_client.py` & `pyatlan-2.1.9/tests/unit/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_typedef_model.py` & `pyatlan-2.1.9/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_utils.py` & `pyatlan-2.1.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.8/tests/unit/test_workflow_client.py` & `pyatlan-2.1.9/tests/unit/test_workflow_client.py`

 * *Files identical despite different names*


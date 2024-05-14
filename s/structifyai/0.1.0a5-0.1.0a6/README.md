# Comparing `tmp/structifyai-0.1.0a5.tar.gz` & `tmp/structifyai-0.1.0a6.tar.gz`

## Comparing `structifyai-0.1.0a5.tar` & `structifyai-0.1.0a6.tar`

### file list

```diff
@@ -1,81 +1,77 @@
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/__init__.py
--rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_base_client.py
--rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_constants.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_qs.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_resource.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_response.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_types.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/lib/.keep
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/__init__.py
--rw-r--r--   0        0        0    17961 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/datasets.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/documents.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/runs.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/sources.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/user.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/__init__.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/admin.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/users.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/server.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/version.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/__init__.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/is_complete.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/job_status.py
--rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/run.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/run_async.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/structure.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/__init__.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/get_job_info.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/usage.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_delete_params.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_descriptor.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_retrieve_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_view_params.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_view_response.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_download_response.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_list_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_upload_params.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/kg_entity.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/new_token.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/run_list_response.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/source.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/source_list_params.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/user_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/user.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/user_list_response.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/server/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/server/server_information.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/is_complete.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/is_complete_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/job_status_create_params.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/llm.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/run_async_create_params.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/run_create_params.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/usage/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/usage/get_job_info_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/__init__.py
+-rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_base_client.py
+-rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_constants.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_qs.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_resource.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_response.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_streaming.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_types.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/lib/.keep
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/__init__.py
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/datasets.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/documents.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/runs.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/server.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/sources.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/user.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/admin.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/users.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/__init__.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/is_complete.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/job_status.py
+-rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/run.py
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/run_async.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/structure.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/__init__.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/get_job_info.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/usage.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_delete_params.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_descriptor.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_list_response.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_node.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_retrieve_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_view_params.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_view_response.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_download_response.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_list_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_upload_params.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/kg_entity.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/new_token.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/run_list_response.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/server_information.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/source.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/source_list_params.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/user_info.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/user_list_response.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/user_node.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/is_complete.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/is_complete_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/job_status_create_params.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/run_async_create_params.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/run_create_params.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/usage/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/usage/get_job_info_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/PKG-INFO
```

### Comparing `structifyai-0.1.0a5/src/structify/__init__.py` & `structifyai-0.1.0a6/src/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_base_client.py` & `structifyai-0.1.0a6/src/structify/_base_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_client.py` & `structifyai-0.1.0a6/src/structify/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_compat.py` & `structifyai-0.1.0a6/src/structify/_compat.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_exceptions.py` & `structifyai-0.1.0a6/src/structify/_exceptions.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_files.py` & `structifyai-0.1.0a6/src/structify/_files.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_models.py` & `structifyai-0.1.0a6/src/structify/_models.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_qs.py` & `structifyai-0.1.0a6/src/structify/_qs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_resource.py` & `structifyai-0.1.0a6/src/structify/_resource.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_response.py` & `structifyai-0.1.0a6/src/structify/_response.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_streaming.py` & `structifyai-0.1.0a6/src/structify/_streaming.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_types.py` & `structifyai-0.1.0a6/src/structify/_types.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/__init__.py` & `structifyai-0.1.0a6/src/structify/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_logs.py` & `structifyai-0.1.0a6/src/structify/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_proxy.py` & `structifyai-0.1.0a6/src/structify/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_sync.py` & `structifyai-0.1.0a6/src/structify/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_transform.py` & `structifyai-0.1.0a6/src/structify/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_typing.py` & `structifyai-0.1.0a6/src/structify/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/_utils/_utils.py` & `structifyai-0.1.0a6/src/structify/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/__init__.py` & `structifyai-0.1.0a6/src/structify/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/datasets.py` & `structifyai-0.1.0a6/src/structify/resources/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,14 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> None:
         """
-        Create a Dataset
-
         Creates a dataset.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -131,19 +129,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> DatasetListResponse:
-        """
-        List datasets
-
-        Gets all datasets owned by the current user
-        """
+        """Gets all datasets owned by the current user"""
         return self._get(
             "/dataset/list",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DatasetListResponse,
         )
@@ -252,16 +246,14 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> None:
         """
-        Create a Dataset
-
         Creates a dataset.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -329,19 +321,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> DatasetListResponse:
-        """
-        List datasets
-
-        Gets all datasets owned by the current user
-        """
+        """Gets all datasets owned by the current user"""
         return await self._get(
             "/dataset/list",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DatasetListResponse,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/documents.py` & `structifyai-0.1.0a6/src/structify/resources/documents.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/runs.py` & `structifyai-0.1.0a6/src/structify/resources/runs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/sources.py` & `structifyai-0.1.0a6/src/structify/resources/sources.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/user.py` & `structifyai-0.1.0a6/src/structify/resources/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> NewToken:
-        """TODO: Move to admin. Creates a test token."""
+        """Creates a test token."""
         return self._post(
             "/user/create_test_token",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NewToken,
         )
@@ -85,15 +85,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> NewToken:
-        """TODO: Move to admin. Creates a test token."""
+        """Creates a test token."""
         return await self._post(
             "/user/create_test_token",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NewToken,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/admin/__init__.py` & `structifyai-0.1.0a6/src/structify/resources/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/admin/admin.py` & `structifyai-0.1.0a6/src/structify/resources/admin/admin.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/admin/users.py` & `structifyai-0.1.0a6/src/structify/resources/admin/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> UserListResponse:
-        """
-        Gets all the users.
-
-        Lists all the users in the system.
-        """
+        """Lists all the users in the system."""
         return self._get(
             "/admin/users/list",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=UserListResponse,
         )
@@ -69,19 +65,15 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> UserListResponse:
-        """
-        Gets all the users.
-
-        Lists all the users in the system.
-        """
+        """Lists all the users in the system."""
         return await self._get(
             "/admin/users/list",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=UserListResponse,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/server/version.py` & `structifyai-0.1.0a6/src/structify/resources/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,123 +1,115 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._compat import cached_property
-from ..._resource import SyncAPIResource, AsyncAPIResource
-from ..._response import (
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._compat import cached_property
+from .._resource import SyncAPIResource, AsyncAPIResource
+from .._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ..._base_client import (
+from .._base_client import (
     make_request_options,
 )
-from ...types.server.server_information import ServerInformation
+from ..types.server_information import ServerInformation
 
-__all__ = ["VersionResource", "AsyncVersionResource"]
+__all__ = ["ServerResource", "AsyncServerResource"]
 
 
-class VersionResource(SyncAPIResource):
+class ServerResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> VersionResourceWithRawResponse:
-        return VersionResourceWithRawResponse(self)
+    def with_raw_response(self) -> ServerResourceWithRawResponse:
+        return ServerResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> VersionResourceWithStreamingResponse:
-        return VersionResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> ServerResourceWithStreamingResponse:
+        return ServerResourceWithStreamingResponse(self)
 
-    def retrieve(
+    def version(
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ServerInformation:
-        """
-        Version
-
-        Gets the version of the API server.
-        """
+        """Gets the version of the API server."""
         return self._get(
             "/server/version",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ServerInformation,
         )
 
 
-class AsyncVersionResource(AsyncAPIResource):
+class AsyncServerResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncVersionResourceWithRawResponse:
-        return AsyncVersionResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncServerResourceWithRawResponse:
+        return AsyncServerResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncVersionResourceWithStreamingResponse:
-        return AsyncVersionResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncServerResourceWithStreamingResponse:
+        return AsyncServerResourceWithStreamingResponse(self)
 
-    async def retrieve(
+    async def version(
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ServerInformation:
-        """
-        Version
-
-        Gets the version of the API server.
-        """
+        """Gets the version of the API server."""
         return await self._get(
             "/server/version",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ServerInformation,
         )
 
 
-class VersionResourceWithRawResponse:
-    def __init__(self, version: VersionResource) -> None:
-        self._version = version
+class ServerResourceWithRawResponse:
+    def __init__(self, server: ServerResource) -> None:
+        self._server = server
 
-        self.retrieve = to_raw_response_wrapper(
-            version.retrieve,
+        self.version = to_raw_response_wrapper(
+            server.version,
         )
 
 
-class AsyncVersionResourceWithRawResponse:
-    def __init__(self, version: AsyncVersionResource) -> None:
-        self._version = version
+class AsyncServerResourceWithRawResponse:
+    def __init__(self, server: AsyncServerResource) -> None:
+        self._server = server
 
-        self.retrieve = async_to_raw_response_wrapper(
-            version.retrieve,
+        self.version = async_to_raw_response_wrapper(
+            server.version,
         )
 
 
-class VersionResourceWithStreamingResponse:
-    def __init__(self, version: VersionResource) -> None:
-        self._version = version
+class ServerResourceWithStreamingResponse:
+    def __init__(self, server: ServerResource) -> None:
+        self._server = server
 
-        self.retrieve = to_streamed_response_wrapper(
-            version.retrieve,
+        self.version = to_streamed_response_wrapper(
+            server.version,
         )
 
 
-class AsyncVersionResourceWithStreamingResponse:
-    def __init__(self, version: AsyncVersionResource) -> None:
-        self._version = version
+class AsyncServerResourceWithStreamingResponse:
+    def __init__(self, server: AsyncServerResource) -> None:
+        self._server = server
 
-        self.retrieve = async_to_streamed_response_wrapper(
-            version.retrieve,
+        self.version = async_to_streamed_response_wrapper(
+            server.version,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/__init__.py` & `structifyai-0.1.0a6/src/structify/resources/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/is_complete.py` & `structifyai-0.1.0a6/src/structify/resources/structure/is_complete.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/job_status.py` & `structifyai-0.1.0a6/src/structify/resources/structure/job_status.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/run.py` & `structifyai-0.1.0a6/src/structify/resources/structure/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ..._base_client import (
     make_request_options,
 )
-from ...types.structure import Llm, run_create_params
-from ...types.structure.llm import Llm
+from ...types.structure import run_create_params
 
 __all__ = ["RunResource", "AsyncRunResource"]
 
 
 class RunResource(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> RunResourceWithRawResponse:
@@ -39,28 +38,26 @@
         return RunResourceWithStreamingResponse(self)
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_create_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -72,28 +69,26 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         document: run_create_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -105,28 +100,26 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         web: run_create_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -138,28 +131,26 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         sec_filing: run_create_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -167,24 +158,20 @@
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
-        ["dataset_name", "llm", "text"],
-        ["dataset_name", "llm", "document"],
-        ["dataset_name", "llm", "web"],
-        ["dataset_name", "llm", "sec_filing"],
+        ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_create_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         document: run_create_params.Variant1Document | NotGiven = NOT_GIVEN,
         web: run_create_params.Variant2Web | NotGiven = NOT_GIVEN,
         sec_filing: run_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -208,15 +195,14 @@
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "dataset_name": dataset_name,
-                        "llm": llm,
                         "custom_instruction": custom_instruction,
                     },
                     run_create_params.RunCreateParams,
                 ),
             ),
             cast_to=object,
         )
@@ -232,28 +218,26 @@
         return AsyncRunResourceWithStreamingResponse(self)
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_create_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -265,28 +249,26 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         document: run_create_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -298,28 +280,26 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         web: run_create_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -331,28 +311,26 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         sec_filing: run_create_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """
-        Structure an unstructured data source into the given dataset.
+        """There's a couple of different types of sources.
 
-        There's a couple of different types of sources. Right now, you can either add a
+        Right now, you can either add a
         file path or the internet as a whole. In the future, we'll allow you to pare
         down the internet to a specific domain or criterium.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -360,24 +338,20 @@
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
-        ["dataset_name", "llm", "text"],
-        ["dataset_name", "llm", "document"],
-        ["dataset_name", "llm", "web"],
-        ["dataset_name", "llm", "sec_filing"],
+        ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_create_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         document: run_create_params.Variant1Document | NotGiven = NOT_GIVEN,
         web: run_create_params.Variant2Web | NotGiven = NOT_GIVEN,
         sec_filing: run_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -401,15 +375,14 @@
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "dataset_name": dataset_name,
-                        "llm": llm,
                         "custom_instruction": custom_instruction,
                     },
                     run_create_params.RunCreateParams,
                 ),
             ),
             cast_to=object,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/run_async.py` & `structifyai-0.1.0a6/src/structify/resources/structure/run_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ..._base_client import (
     make_request_options,
 )
-from ...types.structure import Llm, run_async_create_params
-from ...types.structure.llm import Llm
+from ...types.structure import run_async_create_params
 
 __all__ = ["RunAsyncResource", "AsyncRunAsyncResource"]
 
 
 class RunAsyncResource(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> RunAsyncResourceWithRawResponse:
@@ -39,28 +38,24 @@
         return RunAsyncResourceWithStreamingResponse(self)
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_async_create_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -71,28 +66,24 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         document: run_async_create_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -103,28 +94,24 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         web: run_async_create_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -135,52 +122,44 @@
         ...
 
     @overload
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         sec_filing: run_async_create_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
-        ["dataset_name", "llm", "text"],
-        ["dataset_name", "llm", "document"],
-        ["dataset_name", "llm", "web"],
-        ["dataset_name", "llm", "sec_filing"],
+        ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
     def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_async_create_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         document: run_async_create_params.Variant1Document | NotGiven = NOT_GIVEN,
         web: run_async_create_params.Variant2Web | NotGiven = NOT_GIVEN,
         sec_filing: run_async_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -204,15 +183,14 @@
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "dataset_name": dataset_name,
-                        "llm": llm,
                         "custom_instruction": custom_instruction,
                     },
                     run_async_create_params.RunAsyncCreateParams,
                 ),
             ),
             cast_to=object,
         )
@@ -228,28 +206,24 @@
         return AsyncRunAsyncResourceWithStreamingResponse(self)
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_async_create_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -260,28 +234,24 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         document: run_async_create_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -292,28 +262,24 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         web: run_async_create_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -324,52 +290,44 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         sec_filing: run_async_create_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
-        ["dataset_name", "llm", "text"],
-        ["dataset_name", "llm", "document"],
-        ["dataset_name", "llm", "web"],
-        ["dataset_name", "llm", "sec_filing"],
+        ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
     async def create(
         self,
         *,
         dataset_name: str,
-        llm: Llm,
         text: run_async_create_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         document: run_async_create_params.Variant1Document | NotGiven = NOT_GIVEN,
         web: run_async_create_params.Variant2Web | NotGiven = NOT_GIVEN,
         sec_filing: run_async_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -393,15 +351,14 @@
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "dataset_name": dataset_name,
-                        "llm": llm,
                         "custom_instruction": custom_instruction,
                     },
                     run_async_create_params.RunAsyncCreateParams,
                 ),
             ),
             cast_to=object,
         )
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/structure/structure.py` & `structifyai-0.1.0a6/src/structify/resources/structure/structure.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/usage/__init__.py` & `structifyai-0.1.0a6/src/structify/resources/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/resources/usage/get_job_info.py` & `structifyai-0.1.0a6/src/structify/resources/usage/get_job_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,14 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -90,17 +87,14 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         """
-        Structure an unstructured data source into the given dataset in an async
-        fashion.
-
         Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
```

### Comparing `structifyai-0.1.0a5/src/structify/resources/usage/usage.py` & `structifyai-0.1.0a6/src/structify/resources/usage/usage.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/types/__init__.py` & `structifyai-0.1.0a6/src/structify/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from .source import Source as Source
-from .dataset import Dataset as Dataset
 from .kg_entity import KgEntity as KgEntity
 from .new_token import NewToken as NewToken
 from .user_info import UserInfo as UserInfo
+from .dataset_node import DatasetNode as DatasetNode
 from .run_list_response import RunListResponse as RunListResponse
 from .dataset_descriptor import DatasetDescriptor as DatasetDescriptor
+from .server_information import ServerInformation as ServerInformation
 from .source_list_params import SourceListParams as SourceListParams
 from .dataset_view_params import DatasetViewParams as DatasetViewParams
 from .dataset_create_params import DatasetCreateParams as DatasetCreateParams
 from .dataset_delete_params import DatasetDeleteParams as DatasetDeleteParams
 from .dataset_list_response import DatasetListResponse as DatasetListResponse
 from .dataset_view_response import DatasetViewResponse as DatasetViewResponse
 from .document_list_response import DocumentListResponse as DocumentListResponse
```

### Comparing `structifyai-0.1.0a5/src/structify/types/dataset_create_params.py` & `structifyai-0.1.0a6/src/structify/types/dataset_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/types/dataset_descriptor.py` & `structifyai-0.1.0a6/src/structify/types/dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/types/source.py` & `structifyai-0.1.0a6/src/structify/types/source.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/src/structify/types/structure/run_async_create_params.py` & `structifyai-0.1.0a6/src/structify/types/structure/run_create_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Union, Optional
 from typing_extensions import Required, Annotated, TypedDict
 
-from .llm import Llm
 from ..._utils import PropertyInfo
 
 __all__ = [
-    "RunAsyncCreateParams",
+    "RunCreateParams",
     "Variant0",
     "Variant0Text",
     "Variant1",
     "Variant1Document",
     "Variant2",
     "Variant2Web",
     "Variant3",
     "Variant3SecFiling",
 ]
 
 
 class Variant0(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     text: Required[Annotated[Variant0Text, PropertyInfo(alias="Text")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant0Text(TypedDict, total=False):
     text_content: Required[str]
 
 
 class Variant1(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     document: Required[Annotated[Variant1Document, PropertyInfo(alias="Document")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant1Document(TypedDict, total=False):
     path: Required[str]
 
 
 class Variant2(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     web: Required[Annotated[Variant2Web, PropertyInfo(alias="Web")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant2Web(TypedDict, total=False):
     phrase: Required[str]
 
     starting_website: Optional[str]
 
 
 class Variant3(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     sec_filing: Required[Annotated[Variant3SecFiling, PropertyInfo(alias="SECFiling")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant3SecFiling(TypedDict, total=False):
     accession_number: Optional[str]
 
     quarter: Optional[int]
 
     year: Optional[int]
 
 
-RunAsyncCreateParams = Union[Variant0, Variant1, Variant2, Variant3]
+RunCreateParams = Union[Variant0, Variant1, Variant2, Variant3]
```

### Comparing `structifyai-0.1.0a5/src/structify/types/structure/run_create_params.py` & `structifyai-0.1.0a6/src/structify/types/structure/run_async_create_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Union, Optional
 from typing_extensions import Required, Annotated, TypedDict
 
-from .llm import Llm
 from ..._utils import PropertyInfo
 
 __all__ = [
-    "RunCreateParams",
+    "RunAsyncCreateParams",
     "Variant0",
     "Variant0Text",
     "Variant1",
     "Variant1Document",
     "Variant2",
     "Variant2Web",
     "Variant3",
     "Variant3SecFiling",
 ]
 
 
 class Variant0(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     text: Required[Annotated[Variant0Text, PropertyInfo(alias="Text")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant0Text(TypedDict, total=False):
     text_content: Required[str]
 
 
 class Variant1(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     document: Required[Annotated[Variant1Document, PropertyInfo(alias="Document")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant1Document(TypedDict, total=False):
     path: Required[str]
 
 
 class Variant2(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     web: Required[Annotated[Variant2Web, PropertyInfo(alias="Web")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant2Web(TypedDict, total=False):
     phrase: Required[str]
 
     starting_website: Optional[str]
 
 
 class Variant3(TypedDict, total=False):
     dataset_name: Required[str]
 
-    llm: Required[Llm]
-
     sec_filing: Required[Annotated[Variant3SecFiling, PropertyInfo(alias="SECFiling")]]
 
     custom_instruction: Optional[str]
 
 
 class Variant3SecFiling(TypedDict, total=False):
     accession_number: Optional[str]
 
     quarter: Optional[int]
 
     year: Optional[int]
 
 
-RunCreateParams = Union[Variant0, Variant1, Variant2, Variant3]
+RunAsyncCreateParams = Union[Variant0, Variant1, Variant2, Variant3]
```

### Comparing `structifyai-0.1.0a5/LICENSE` & `structifyai-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a5/pyproject.toml` & `structifyai-0.1.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "structifyai"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "The official Python library for the structify API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Structify", email = "team@structify.ai" },
 ]
 dependencies = [
```

### Comparing `structifyai-0.1.0a5/PKG-INFO` & `structifyai-0.1.0a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structifyai
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: The official Python library for the structify API
 Project-URL: Homepage, https://github.com/StructifyAI/structify-python
 Project-URL: Repository, https://github.com/StructifyAI/structify-python
 Author-email: Structify <team@structify.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -63,15 +63,15 @@
 client = Structify(
     # This is the default and can be omitted
     api_key=os.environ.get("STRUCTIFY_API_TOKEN"),
     # defaults to "production".
     environment="deployment",
 )
 
-server_information = client.server.version.retrieve()
+server_information = client.server.version()
 print(server_information.version)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `STRUCTIFY_API_TOKEN="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
@@ -90,15 +90,15 @@
     api_key=os.environ.get("STRUCTIFY_API_TOKEN"),
     # defaults to "production".
     environment="deployment",
 )
 
 
 async def main() -> None:
-    server_information = await client.server.version.retrieve()
+    server_information = await client.server.version()
     print(server_information.version)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
@@ -124,15 +124,15 @@
 ```python
 import structify
 from structify import Structify
 
 client = Structify()
 
 try:
-    client.server.version.retrieve()
+    client.server.version()
 except structify.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except structify.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except structify.APIStatusError as e:
     print("Another non-200-range status code was received")
@@ -167,15 +167,15 @@
 # Configure the default for all requests:
 client = Structify(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).server.version.retrieve()
+client.with_options(max_retries=5).server.version()
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
@@ -190,15 +190,15 @@
 
 # More granular control:
 client = Structify(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5.0).server.version.retrieve()
+client.with_options(timeout=5.0).server.version()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/StructifyAI/structify-python/tree/main/#retries).
 
 ## Advanced
@@ -229,33 +229,33 @@
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from structify import Structify
 
 client = Structify()
-response = client.server.version.with_raw_response.retrieve()
+response = client.server.with_raw_response.version()
 print(response.headers.get('X-My-Header'))
 
-version = response.parse()  # get the object that `server.version.retrieve()` would have returned
-print(version.version)
+server = response.parse()  # get the object that `server.version()` would have returned
+print(server.version)
 ```
 
 These methods return an [`APIResponse`](https://github.com/StructifyAI/structify-python/tree/main/src/structify/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/StructifyAI/structify-python/tree/main/src/structify/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.server.version.with_streaming_response.retrieve() as response:
+with client.server.with_streaming_response.version() as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
```


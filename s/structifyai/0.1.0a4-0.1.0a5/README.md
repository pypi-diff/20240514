# Comparing `tmp/structifyai-0.1.0a4.tar.gz` & `tmp/structifyai-0.1.0a5.tar.gz`

## Comparing `structifyai-0.1.0a4.tar` & `structifyai-0.1.0a5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/__init__.py
--rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_base_client.py
--rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_constants.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_qs.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_resource.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_response.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_types.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/lib/.keep
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/__init__.py
--rw-r--r--   0        0        0    17961 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/datasets.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/documents.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/runs.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/sources.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/user.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/admin/__init__.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/admin/admin.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/admin/users.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/server/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/server/server.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/server/version.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/__init__.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/is_complete.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/job_status.py
--rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/run.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/run_async.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/structure/structure.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/usage/__init__.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/usage/get_job_info.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/resources/usage/usage.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_delete_params.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_descriptor.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_retrieve_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_view_params.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/dataset_view_response.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/document_download_response.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/document_list_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/document_upload_params.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/kg_entity.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/new_token.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/run_list_response.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/source.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/source_list_params.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/user_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/admin/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/admin/user.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/admin/user_list_response.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/server/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/server/server_information.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/is_complete.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/is_complete_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/job_status_create_params.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/llm.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/run_async_create_params.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/structure/run_create_params.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/usage/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/src/structify/types/usage/get_job_info_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0    12145 2020-02-02 00:00:00.000000 structifyai-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/__init__.py
+-rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_base_client.py
+-rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_constants.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_qs.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_resource.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_response.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_streaming.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_types.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/lib/.keep
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/__init__.py
+-rw-r--r--   0        0        0    17961 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/datasets.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/documents.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/runs.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/sources.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/user.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/admin.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/admin/users.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/server.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/server/version.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/__init__.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/is_complete.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/job_status.py
+-rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/run.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/run_async.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/structure/structure.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/__init__.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/get_job_info.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/resources/usage/usage.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_delete_params.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_descriptor.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_retrieve_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_view_params.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/dataset_view_response.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_download_response.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_list_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/document_upload_params.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/kg_entity.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/new_token.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/run_list_response.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/source.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/source_list_params.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/user_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/user.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/admin/user_list_response.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/server/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/server/server_information.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/is_complete.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/is_complete_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/job_status_create_params.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/llm.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/run_async_create_params.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/structure/run_create_params.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/usage/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/src/structify/types/usage/get_job_info_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 structifyai-0.1.0a5/PKG-INFO
```

### Comparing `structifyai-0.1.0a4/src/structify/__init__.py` & `structifyai-0.1.0a5/src/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_base_client.py` & `structifyai-0.1.0a5/src/structify/_base_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_client.py` & `structifyai-0.1.0a5/src/structify/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_compat.py` & `structifyai-0.1.0a5/src/structify/_compat.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_exceptions.py` & `structifyai-0.1.0a5/src/structify/_exceptions.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_files.py` & `structifyai-0.1.0a5/src/structify/_files.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_models.py` & `structifyai-0.1.0a5/src/structify/_models.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_qs.py` & `structifyai-0.1.0a5/src/structify/_qs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_resource.py` & `structifyai-0.1.0a5/src/structify/_resource.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_response.py` & `structifyai-0.1.0a5/src/structify/_response.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_streaming.py` & `structifyai-0.1.0a5/src/structify/_streaming.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_types.py` & `structifyai-0.1.0a5/src/structify/_types.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/__init__.py` & `structifyai-0.1.0a5/src/structify/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_logs.py` & `structifyai-0.1.0a5/src/structify/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_proxy.py` & `structifyai-0.1.0a5/src/structify/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_sync.py` & `structifyai-0.1.0a5/src/structify/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_transform.py` & `structifyai-0.1.0a5/src/structify/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_typing.py` & `structifyai-0.1.0a5/src/structify/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/_utils/_utils.py` & `structifyai-0.1.0a5/src/structify/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/__init__.py` & `structifyai-0.1.0a5/src/structify/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/datasets.py` & `structifyai-0.1.0a5/src/structify/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/documents.py` & `structifyai-0.1.0a5/src/structify/resources/documents.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/runs.py` & `structifyai-0.1.0a5/src/structify/resources/runs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/sources.py` & `structifyai-0.1.0a5/src/structify/resources/sources.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/user.py` & `structifyai-0.1.0a5/src/structify/resources/user.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/admin/__init__.py` & `structifyai-0.1.0a5/src/structify/resources/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/admin/admin.py` & `structifyai-0.1.0a5/src/structify/resources/admin/admin.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/admin/users.py` & `structifyai-0.1.0a5/src/structify/resources/admin/users.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/server/__init__.py` & `structifyai-0.1.0a5/src/structify/resources/server/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/server/server.py` & `structifyai-0.1.0a5/src/structify/resources/server/server.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/server/version.py` & `structifyai-0.1.0a5/src/structify/resources/server/version.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/__init__.py` & `structifyai-0.1.0a5/src/structify/resources/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/is_complete.py` & `structifyai-0.1.0a5/src/structify/resources/structure/is_complete.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/job_status.py` & `structifyai-0.1.0a5/src/structify/resources/structure/job_status.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/run.py` & `structifyai-0.1.0a5/src/structify/resources/structure/run.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/run_async.py` & `structifyai-0.1.0a5/src/structify/resources/structure/run_async.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/structure/structure.py` & `structifyai-0.1.0a5/src/structify/resources/structure/structure.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/usage/__init__.py` & `structifyai-0.1.0a5/src/structify/resources/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/usage/get_job_info.py` & `structifyai-0.1.0a5/src/structify/resources/usage/get_job_info.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/resources/usage/usage.py` & `structifyai-0.1.0a5/src/structify/resources/usage/usage.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/__init__.py` & `structifyai-0.1.0a5/src/structify/types/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/dataset_create_params.py` & `structifyai-0.1.0a5/src/structify/types/dataset_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/dataset_descriptor.py` & `structifyai-0.1.0a5/src/structify/types/dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/source.py` & `structifyai-0.1.0a5/src/structify/types/source.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/structure/__init__.py` & `structifyai-0.1.0a5/src/structify/types/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/structure/run_async_create_params.py` & `structifyai-0.1.0a5/src/structify/types/structure/run_async_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/src/structify/types/structure/run_create_params.py` & `structifyai-0.1.0a5/src/structify/types/structure/run_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/LICENSE` & `structifyai-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a4/pyproject.toml` & `structifyai-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "structifyai"
-version = "0.1.0-alpha.4"
+version = "0.1.0-alpha.5"
 description = "The official Python library for the structify API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Structify", email = "team@structify.ai" },
 ]
 dependencies = [
```

### Comparing `structifyai-0.1.0a4/PKG-INFO` & `structifyai-0.1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structifyai
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: The official Python library for the structify API
 Project-URL: Homepage, https://github.com/StructifyAI/structify-python
 Project-URL: Repository, https://github.com/StructifyAI/structify-python
 Author-email: Structify <team@structify.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -31,24 +31,23 @@
 Requires-Dist: sniffio
 Requires-Dist: typing-extensions<5,>=4.7
 Description-Content-Type: text/markdown
 
 # Structify Python API library
 
 [![PyPI version](https://img.shields.io/pypi/v/structifyai.svg)](https://pypi.org/project/structifyai/)
+[![Documentation Status](https://readthedocs.org/projects/structify/badge/?version=latest)](https://structify.readthedocs.io/en/latest/?badge=latest)
 
 The Structify Python library provides convenient access to the Structify REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
-It is generated with [Stainless](https://www.stainlessapi.com/).
-
 ## Documentation
 
-The REST API documentation can be found [on api.structify.ai](https://api.structify.ai/). The full API of this library can be found in [api.md](https://github.com/StructifyAI/structify-python/tree/main/api.md).
+The REST API documentation can be found on [ReadTheDocs](https://structify.readthedocs.io/en/latest/). The full API of this library can be found in [api.md](https://github.com/StructifyAI/structify-python/tree/main/api.md).
 
 ## Installation
 
 ```sh
 # install from PyPI
 pip install --pre structifyai
 ```
```


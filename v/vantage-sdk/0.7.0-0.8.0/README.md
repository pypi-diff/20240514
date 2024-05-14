# Comparing `tmp/vantage_sdk-0.7.0.tar.gz` & `tmp/vantage_sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage_sdk-0.7.0.tar", max compression
+gzip compressed data, was "vantage_sdk-0.8.0.tar", max compression
```

## Comparing `vantage_sdk-0.7.0.tar` & `vantage_sdk-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,77 @@
--rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.7.0/LICENSE
--rw-r--r--   0        0        0     2766 2024-04-25 01:26:48.214195 vantage_sdk-0.7.0/README.md
--rw-r--r--   0        0        0     2924 2024-04-25 01:26:48.216977 vantage_sdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.7.0/tests/data/documents.jsonl
--rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.7.0/tests/data/hello_world.parquet
--rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.7.0/tests/integration_tests/.env-example
--rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.7.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0     9406 2024-04-25 01:26:48.217716 vantage_sdk-0.7.0/tests/integration_tests/conftest.py
--rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.7.0/tests/integration_tests/test_account.py
--rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.7.0/tests/integration_tests/test_api_keys.py
--rw-r--r--   0        0        0    12673 2024-04-25 01:26:48.218029 vantage_sdk-0.7.0/tests/integration_tests/test_collection.py
--rw-r--r--   0        0        0     2080 2024-04-25 01:26:48.218088 vantage_sdk-0.7.0/tests/integration_tests/test_documents.py
--rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.7.0/tests/integration_tests/test_search.py
--rw-r--r--   0        0        0      671 2024-04-25 01:26:48.218254 vantage_sdk-0.7.0/vantage_sdk/__init__.py
--rw-r--r--   0        0        0    64968 2024-04-25 01:27:40.386067 vantage_sdk-0.7.0/vantage_sdk/client.py
--rw-r--r--   0        0        0      170 2024-04-25 01:27:40.386339 vantage_sdk-0.7.0/vantage_sdk/config.py
--rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.7.0/vantage_sdk/core/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.7.0/vantage_sdk/core/base.py
--rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.7.0/vantage_sdk/core/exceptions.py
--rw-r--r--   0        0        0     4478 2024-04-25 01:27:40.386560 vantage_sdk-0.7.0/vantage_sdk/core/http/__init__.py
--rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.7.0/vantage_sdk/core/http/api/__init__.py
--rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.7.0/vantage_sdk/core/http/api/account_management_api.py
--rw-r--r--   0        0        0    75292 2024-04-25 01:27:40.386926 vantage_sdk-0.7.0/vantage_sdk/core/http/api/collection_management_api.py
--rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.7.0/vantage_sdk/core/http/api/documents_api.py
--rw-r--r--   0        0        0    57921 2024-04-25 01:27:40.387280 vantage_sdk-0.7.0/vantage_sdk/core/http/api/external_api_keys_api.py
--rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.7.0/vantage_sdk/core/http/api/search_api.py
--rw-r--r--   0        0        0    22790 2024-04-25 01:27:40.387561 vantage_sdk-0.7.0/vantage_sdk/core/http/api/vantage_api_keys_api.py
--rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.7.0/vantage_sdk/core/http/api_client.py
--rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.7.0/vantage_sdk/core/http/api_response.py
--rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.7.0/vantage_sdk/core/http/configuration.py
--rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.7.0/vantage_sdk/core/http/exceptions.py
--rw-r--r--   0        0        0     3594 2024-04-25 01:27:40.387750 vantage_sdk-0.7.0/vantage_sdk/core/http/models/__init__.py
--rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.7.0/vantage_sdk/core/http/models/account.py
--rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.7.0/vantage_sdk/core/http/models/account_modifiable.py
--rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.7.0/vantage_sdk/core/http/models/account_read_only.py
--rw-r--r--   0        0        0     7026 2024-04-25 01:27:40.387925 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection.py
--rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_immutable.py
--rw-r--r--   0        0        0     3525 2024-04-25 01:27:40.388136 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_modifiable.py
--rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_read_only.py
--rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_upload_url.py
--rw-r--r--   0        0        0     5192 2024-04-25 01:27:40.388274 vantage_sdk-0.7.0/vantage_sdk/core/http/models/collections_result_inner.py
--rw-r--r--   0        0        0     5377 2024-04-25 01:27:40.388459 vantage_sdk-0.7.0/vantage_sdk/core/http/models/create_collection_request.py
--rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.7.0/vantage_sdk/core/http/models/document_batch.py
--rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.7.0/vantage_sdk/core/http/models/embedding_search_query.py
--rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key.py
--rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key_modifiable.py
--rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key_read_only.py
--rw-r--r--   0        0        0     5290 2024-04-25 01:27:40.388563 vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_keys_result_inner.py
--rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties.py
--rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_collection.py
--rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
--rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_filter.py
--rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_pagination.py
--rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_sort.py
--rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.7.0/vantage_sdk/core/http/models/ml_these.py
--rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.7.0/vantage_sdk/core/http/models/ml_these_these_inner.py
--rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.7.0/vantage_sdk/core/http/models/more_like_these_query.py
--rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.7.0/vantage_sdk/core/http/models/more_like_this_query.py
--rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.7.0/vantage_sdk/core/http/models/search_result.py
--rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.7.0/vantage_sdk/core/http/models/search_result_results_inner.py
--rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.7.0/vantage_sdk/core/http/models/semantic_search_query.py
--rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.7.0/vantage_sdk/core/http/models/vantage_api_key.py
--rw-r--r--   0        0        0     5266 2024-04-25 01:27:40.388653 vantage_sdk-0.7.0/vantage_sdk/core/http/models/vantage_api_keys_result_inner.py
--rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.7.0/vantage_sdk/core/http/models/weighted_field_values.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.7.0/vantage_sdk/core/http/py.typed
--rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.7.0/vantage_sdk/core/http/rest.py
--rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.7.0/vantage_sdk/core/management/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.7.0/vantage_sdk/core/management/management.py
--rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.7.0/vantage_sdk/core/search/__init__.py
--rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.7.0/vantage_sdk/core/search/search.py
--rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.7.0/vantage_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.7.0/vantage_sdk/model/__init__.py
--rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.7.0/vantage_sdk/model/account.py
--rw-r--r--   0        0        0      916 2024-04-25 01:27:40.388843 vantage_sdk-0.7.0/vantage_sdk/model/collection.py
--rw-r--r--   0        0        0      767 2024-04-25 01:27:40.389033 vantage_sdk-0.7.0/vantage_sdk/model/keys.py
--rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.7.0/vantage_sdk/model/search.py
--rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 vantage_sdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3974 2024-05-14 15:00:04.643283 vantage_sdk-0.8.0/README.md
+-rw-r--r--   0        0        0     2924 2024-05-14 15:00:04.643589 vantage_sdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.8.0/tests/data/documents.jsonl
+-rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.8.0/tests/data/hello_world.parquet
+-rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.8.0/tests/integration_tests/.env-example
+-rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.8.0/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0    10571 2024-05-14 15:00:04.643899 vantage_sdk-0.8.0/tests/integration_tests/conftest.py
+-rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.8.0/tests/integration_tests/test_account.py
+-rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.8.0/tests/integration_tests/test_api_keys.py
+-rw-r--r--   0        0        0    12709 2024-05-14 15:00:04.644178 vantage_sdk-0.8.0/tests/integration_tests/test_collection.py
+-rw-r--r--   0        0        0     4219 2024-05-14 15:00:04.644424 vantage_sdk-0.8.0/tests/integration_tests/test_documents.py
+-rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.8.0/tests/integration_tests/test_search.py
+-rw-r--r--   0        0        0      671 2024-05-14 15:00:04.644679 vantage_sdk-0.8.0/vantage_sdk/__init__.py
+-rw-r--r--   0        0        0    66114 2024-05-14 15:00:04.645142 vantage_sdk-0.8.0/vantage_sdk/client.py
+-rw-r--r--   0        0        0      239 2024-05-14 15:00:04.645361 vantage_sdk-0.8.0/vantage_sdk/config.py
+-rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.8.0/vantage_sdk/core/__init__.py
+-rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.8.0/vantage_sdk/core/base.py
+-rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.8.0/vantage_sdk/core/exceptions.py
+-rw-r--r--   0        0        0     4268 2024-05-14 15:00:04.645589 vantage_sdk-0.8.0/vantage_sdk/core/http/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.8.0/vantage_sdk/core/http/api/__init__.py
+-rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.8.0/vantage_sdk/core/http/api/account_management_api.py
+-rw-r--r--   0        0        0    75134 2024-05-14 15:00:04.645955 vantage_sdk-0.8.0/vantage_sdk/core/http/api/collection_management_api.py
+-rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.8.0/vantage_sdk/core/http/api/documents_api.py
+-rw-r--r--   0        0        0    57753 2024-05-14 15:00:04.646292 vantage_sdk-0.8.0/vantage_sdk/core/http/api/external_api_keys_api.py
+-rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.8.0/vantage_sdk/core/http/api/search_api.py
+-rw-r--r--   0        0        0    22624 2024-05-14 15:00:04.646500 vantage_sdk-0.8.0/vantage_sdk/core/http/api/vantage_api_keys_api.py
+-rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.8.0/vantage_sdk/core/http/api_client.py
+-rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.8.0/vantage_sdk/core/http/api_response.py
+-rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.8.0/vantage_sdk/core/http/configuration.py
+-rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.8.0/vantage_sdk/core/http/exceptions.py
+-rw-r--r--   0        0        0     3384 2024-05-14 15:00:04.646724 vantage_sdk-0.8.0/vantage_sdk/core/http/models/__init__.py
+-rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account.py
+-rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_modifiable.py
+-rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_read_only.py
+-rw-r--r--   0        0        0     7946 2024-05-14 15:00:04.646949 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection.py
+-rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_immutable.py
+-rw-r--r--   0        0        0     4445 2024-05-14 15:00:04.647162 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_modifiable.py
+-rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_read_only.py
+-rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_upload_url.py
+-rw-r--r--   0        0        0     6297 2024-05-14 15:00:04.647434 vantage_sdk-0.8.0/vantage_sdk/core/http/models/create_collection_request.py
+-rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.8.0/vantage_sdk/core/http/models/document_batch.py
+-rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.8.0/vantage_sdk/core/http/models/embedding_search_query.py
+-rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key.py
+-rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_modifiable.py
+-rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_read_only.py
+-rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties.py
+-rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_collection.py
+-rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
+-rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_filter.py
+-rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_pagination.py
+-rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_sort.py
+-rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these.py
+-rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these_these_inner.py
+-rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_these_query.py
+-rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_this_query.py
+-rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result.py
+-rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result_results_inner.py
+-rw-r--r--   0        0        0     3445 2024-05-14 15:00:04.647571 vantage_sdk-0.8.0/vantage_sdk/core/http/models/secondary_external_account.py
+-rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.8.0/vantage_sdk/core/http/models/semantic_search_query.py
+-rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.8.0/vantage_sdk/core/http/models/vantage_api_key.py
+-rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.8.0/vantage_sdk/core/http/models/weighted_field_values.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.8.0/vantage_sdk/core/http/py.typed
+-rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.8.0/vantage_sdk/core/http/rest.py
+-rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.8.0/vantage_sdk/core/management/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.8.0/vantage_sdk/core/management/management.py
+-rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.8.0/vantage_sdk/core/search/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.8.0/vantage_sdk/core/search/search.py
+-rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.8.0/vantage_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.8.0/vantage_sdk/model/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.8.0/vantage_sdk/model/account.py
+-rw-r--r--   0        0        0     2563 2024-05-14 15:00:04.647772 vantage_sdk-0.8.0/vantage_sdk/model/collection.py
+-rw-r--r--   0        0        0     1670 2024-05-14 15:00:04.647963 vantage_sdk-0.8.0/vantage_sdk/model/document.py
+-rw-r--r--   0        0        0      910 2024-05-14 15:00:04.648235 vantage_sdk-0.8.0/vantage_sdk/model/keys.py
+-rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.8.0/vantage_sdk/model/search.py
+-rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 vantage_sdk-0.8.0/PKG-INFO
```

### Comparing `vantage_sdk-0.7.0/LICENSE` & `vantage_sdk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/README.md` & `vantage_sdk-0.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Vantage Discovery Python SDK
 
 The Vantage Discovery Python SDK provides an easy-to-use interface to interact with the Vantage vector database, enabling developers to seamlessly integrate vector search and collection management capabilities into their Python applications.
 
 ## Installation
 
-To install the Vantage Python SDK, run the following command:
+To install the [Vantage Python SDK](https://pypi.org/project/vantage-sdk/), run the following command:
 
 ```bash
 pip install vantage-sdk
 ```
 
 ## Quickstart
 
@@ -34,44 +34,78 @@
 
 #### Key Features
 - __Collection Management__: Easily create, update, list, and delete collections.
 - __Documents Upload__: Upload your data easily to your collections.
 - __Search__: Perform semantic, embedding and "more like this/these" searches within your collections.
 - __LLM Keys Management__: Keep your LLM provider secrets safe and up-to-date.
 
-## Examples
+## 🔍 Examples
 
 ### Creating a Collection
 
+To create a new collection for storing documents, specify the collection ID, the dimension of the embeddings, and the LLM (language learning model) details. Here, we use `text-embedding-ada-002` from OpenAI with the necessary secret key. 
+
+📚 Visit [management-api](https://docs.vantagediscovery.com/docs/management-api) documentation for more details.
+
 ```python
-collection = vantage_client.create_collection(
-    collection_id="my_collection",
-    collection_name="My Test Collection",
+collection = OpenAICollection(
+    collection_id="my-collection",
     embeddings_dimension=1536,
     llm="text-embedding-ada-002",
-    external_key_id="YOUR_EXTERNAL_KEY_ID" # Get from Vantage Console UI or using the SDK
+    llm_secret="YOUR_OPENAI_SECRET_KEY",
 )
-print(f"Created collection: {collection.name}")
+
+created_collection = vantage_client.create_collection(collection=collection)
+
+print(f"Created collection: {created_collection.collection_name}")
 ```
 
 ### Uploading Documents
+
+To upload documents to your collection, provide a list of document IDs and corresponding text. Each document is wrapped in a `VantageManagedEmbeddingsDocument` object. This example demonstrates uploading a batch of documents. 
+
+📚 Visit [management-api](https://docs.vantagediscovery.com/docs/management-api) documentation for more details.
+
 ```python
-documents_jsonl = '{"id": "1", "text": "Example text"}\\n{"id": "2", "text": "Another example"}'
-vantage_client.upload_documents_from_jsonl(
-    collection_id="my_collection",
-    documents=documents_jsonl
+ids = [
+    "1",
+    "2",
+    "3",
+    "4",
+]
+
+texts = [
+    "First text",
+    "Second text",
+    "Third text",
+    "Fourth text",
+]
+
+documents = [
+    VantageManagedEmbeddingsDocument(text=text, id=id)
+    for id, text in zip(ids, texts)
+]
+
+instance.upsert_documents(
+    collection_id="my-collection",
+    documents=documents,
 )
 ```
 
 ### Performing a Search
+
+To perform a semantic search within your collection, specify the text you want to find similar documents for. This example retrieves documents similar to the provided text, printing out each document's ID and its similarity score. 
+
+📚 Visit [search-api](https://docs.vantagediscovery.com/docs/search-api) documentation for more details.
+
 ```python
 search_result = vantage_client.semantic_search(
     text="Find documents similar to this text",
-    collection_id="my_collection"
+    collection_id="my-collection"
 )
 for result in search_result.results:
     print(result.id, result.score)
 ```
 
-## Documentation
+## 📚 Documentation
 
 For detailed documentation on all methods and their parameters, please refer to the [Vantage Discovery official documentation](https://docs.vantagediscovery.com/docs/concepts).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vantage_sdk-0.7.0/pyproject.toml` & `vantage_sdk-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "vantage-sdk"
-version = "0.7.0"
+version = "0.8.0"
 description = "Vantage Python SDK."
 authors = ["Vantage <none@vantage.com>"]
 readme = "README.md"
 repository = "https://github.com/VantageDiscovery/vantage-sdk-python"
 documentation = "https://docs.vantagediscovery.com/docs/concepts"
 classifiers=[
     'Programming Language :: Python :: 3.10',
@@ -114,15 +114,15 @@
     "D107"
 ]
 
 [tool.mypy]
 exclude = "vantage_sdk/core/http"
 
 [bumpver]
-current_version = "0.7.0"
+current_version = "0.8.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "vantage_sdk/__init__.py" = [
```

### Comparing `vantage_sdk-0.7.0/tests/data/documents.jsonl` & `vantage_sdk-0.8.0/tests/data/documents.jsonl`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/tests/data/hello_world.parquet` & `vantage_sdk-0.8.0/tests/data/hello_world.parquet`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/.env-example` & `vantage_sdk-0.8.0/tests/integration_tests/.env-example`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/conftest.py` & `vantage_sdk-0.8.0/tests/integration_tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import os
 import random
 import string
 import uuid
-from typing import Callable
+from typing import Callable, List
 
 import pytest
 
 from vantage_sdk.client import VantageClient
 from vantage_sdk.exceptions import VantageNotFoundError
+from vantage_sdk.model.document import (
+    UserProvidedEmbeddingsDocument,
+    VantageManagedEmbeddingsDocument,
+)
 
 
 ABS_PATH = os.path.dirname(os.path.abspath(__file__))
 PROJECT_DIR = os.path.abspath(os.path.join(ABS_PATH, os.pardir, os.pardir))
 DISABLE_EXTERNAL_API_KEYS_TESTS = True
 
 
@@ -318,7 +322,61 @@
 def jsonl_documents_path() -> str:
     return "tests/data/documents.jsonl"
 
 
 @pytest.fixture(scope="module")
 def parquet_file_path() -> str:
     return "tests/data/hello_world.parquet"
+
+
+@pytest.fixture(scope="module")
+def vantage_upe_documents() -> List[UserProvidedEmbeddingsDocument]:
+    ids = [
+        "1",
+        "2",
+        "3",
+        "4",
+    ]
+
+    texts = [
+        "First text",
+        "Second text",
+        "Third text",
+        "Fourth text",
+    ]
+
+    embeddings = [
+        [0.123, 0.234, 0.345],
+        [0.456, 0.567, 0.678],
+        [0.789, 0.891, 0.912],
+        [0.257, 0.389, 0.468],
+    ]
+    documents = [
+        UserProvidedEmbeddingsDocument(text=text, id=id, embeddings=emb)
+        for id, text, emb in zip(ids, texts, embeddings)
+    ]
+
+    return documents
+
+
+@pytest.fixture(scope="module")
+def vantage_vme_documents() -> List[VantageManagedEmbeddingsDocument]:
+    ids = [
+        "1",
+        "2",
+        "3",
+        "4",
+    ]
+
+    texts = [
+        "First text",
+        "Second text",
+        "Third text",
+        "Fourth text",
+    ]
+
+    documents = [
+        VantageManagedEmbeddingsDocument(text=text, id=id)
+        for id, text in zip(ids, texts)
+    ]
+
+    return documents
```

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/test_account.py` & `vantage_sdk-0.8.0/tests/integration_tests/test_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/test_api_keys.py` & `vantage_sdk-0.8.0/tests/integration_tests/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/test_collection.py` & `vantage_sdk-0.8.0/tests/integration_tests/test_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             collection_id=collection_id,
             collection_name=collection_name,
             user_provided_embeddings=True,
             embeddings_dimension=1536,
         )
 
         # When
-        status = client.upload_embeddings_from_parquet(
+        status = client.upsert_documents_from_parquet_file(
             collection_id=collection_id,
-            file_path=test_parquet_file_path,
+            parquet_file_path=test_parquet_file_path,
             account_id=account_params["id"],
         )
 
         # Then
         assert status == 200
 
     def test_upload_user_embeddings_to_a_non_existing_collection(
@@ -87,17 +87,17 @@
         """
         Tests uploading user embeddings to a non-existing collection.
         """
         # Given
         collection_id = random_string_generator(10)
 
         with pytest.raises(NotFoundException) as exception:
-            client.upload_embeddings_from_parquet(
+            client.upsert_documents_from_parquet_file(
                 collection_id=collection_id,
-                file_path=test_parquet_file_path,
+                parquet_file_path=test_parquet_file_path,
                 account_id=account_params["id"],
             )
 
         # Then
         assert exception.type is NotFoundException
 
     def test_upload_non_existing_user_embeddings(
@@ -112,17 +112,17 @@
         Tests uploading non existing user embeddings file.
         """
         # Given
         collection_id = random_string_generator(10)
         non_existing_file_path = random_string_generator(10)
 
         with pytest.raises(FileNotFoundError) as exception:
-            client.upload_embeddings_from_parquet(
+            client.upsert_documents_from_parquet_file(
                 collection_id=collection_id,
-                file_path=non_existing_file_path,
+                parquet_file_path=non_existing_file_path,
                 account_id=account_params["id"],
             )
 
         # Then
         assert exception.type is FileNotFoundError
 
     def test_upload_user_embeddings_with_wrong_file_size(
@@ -148,15 +148,15 @@
             collection_name=collection_name,
             user_provided_embeddings=True,
             embeddings_dimension=1536,
         )
 
         # When
         with pytest.raises(VantageFileUploadError) as exception:
-            client.upload_embeddings_from_bytes(
+            client._upsert_documents_from_bytes(
                 collection_id=collection_id,
                 content=file_content,
                 file_size=file_size,
                 batch_identifier="test-batch",
                 account_id=account_params["id"],
             )
```

### Comparing `vantage_sdk-0.7.0/tests/integration_tests/test_search.py` & `vantage_sdk-0.8.0/tests/integration_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/__init__.py` & `vantage_sdk-0.8.0/vantage_sdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SearchResult,
     SearchResultItem,
 )
 
 
 __author__ = """Vantage"""
 __email__ = 'none@vantage.com'
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 __all__ = [
     "VantageClient",
     "Collection",
     "CollectionUploadURL",
     "Account",
     "VantageAPIKey",
     "ExternalAPIKey",
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/client.py` & `vantage_sdk-0.8.0/vantage_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import json
 import ntpath
 import uuid
 from os.path import exists
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import requests
 
 from vantage_sdk.config import (
     API_HOST_VERSION,
     AUTH_ENDPOINT,
     DEFAULT_API_HOST,
@@ -25,22 +26,40 @@
     GlobalSearchPropertiesCollection,
     GlobalSearchPropertiesFilter,
     GlobalSearchPropertiesPagination,
     GlobalSearchPropertiesSort,
     MLTheseTheseInner,
     MoreLikeTheseQuery,
     MoreLikeThisQuery,
-    SemanticSearchQuery,
 )
+from vantage_sdk.core.http.models import (
+    SecondaryExternalAccount as OpenAPISecondaryExternalAccount,
+)
+from vantage_sdk.core.http.models import SemanticSearchQuery
 from vantage_sdk.core.management import ManagementAPI
 from vantage_sdk.core.search import SearchAPI
 from vantage_sdk.exceptions import VantageFileUploadError, VantageValueError
 from vantage_sdk.model.account import Account
-from vantage_sdk.model.collection import Collection, CollectionUploadURL
-from vantage_sdk.model.keys import ExternalAPIKey, LLMProvider, VantageAPIKey
+from vantage_sdk.model.collection import (
+    Collection,
+    CollectionUploadURL,
+    HuggingFaceCollection,
+    OpenAICollection,
+    UserProvidedEmbeddingsCollection,
+)
+from vantage_sdk.model.document import (
+    UserProvidedEmbeddingsDocument,
+    VantageManagedEmbeddingsDocument,
+)
+from vantage_sdk.model.keys import (
+    ExternalAPIKey,
+    LLMProvider,
+    SecondaryExternalAccount,
+    VantageAPIKey,
+)
 from vantage_sdk.model.search import (
     GlobalSearchProperties,
     MoreLikeTheseItem,
     SearchResult,
 )
 
 
@@ -274,20 +293,15 @@
             Defaults to None.
 
         Returns
         -------
         Account
             An Account object containing the details of the requested account.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> account = vantage_client.get_account()
-        >>> print(account.name)
-        "Example Account Name"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         result = self.management_api.account_api.get_account(
             account_id=account_id or self.account_id
         )
         return Account.model_validate(result.model_dump())
 
@@ -313,20 +327,15 @@
             Defaults to None.
 
         Returns
         -------
         Account
             An updated Account object reflecting the changes made.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> updated_account = vantage_client.update_account(account_name="New Account Name")
-        >>> print(updated_account.name)
-        "New Account Name"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         account_modifiable = AccountModifiable(account_name=account_name)
 
         result = self.management_api.account_api.update_account(
             account_id=account_id or self.account_id,
             account_modifiable=account_modifiable,
@@ -356,32 +365,22 @@
             Defaults to None.
 
         Returns
         -------
         List[VantageAPIKey]
             A list of VantageAPIKey objects, each representing a Vantage API key associated with the account.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_api_keys = vantage_client.get_vantage_api_keys()
-        >>> for key in vantage_api_keys:
-        ...     print(key.value)
-        "12345"
-        "54321"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         keys = self.management_api.vantage_api_keys_api.get_vantage_api_keys(
             account_id=account_id or self.account_id,
         )
 
-        return [
-            VantageAPIKey.model_validate(key.actual_instance.model_dump())
-            for key in keys
-        ]
+        return [VantageAPIKey.model_validate(key.model_dump()) for key in keys]
 
     def get_vantage_api_key(
         self,
         vantage_api_key_id: str,
         account_id: Optional[str] = None,
     ) -> VantageAPIKey:
         """
@@ -402,20 +401,15 @@
             Defaults to None.
 
         Returns
         -------
         VantageAPIKey
             A VantageAPIKey object containing the details of the requested API key.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_api_key = vantage_client.get_vantage_api_key(vantage_api_key_id="api_key_12345")
-        >>> print(vantage_api_key.value)
-        "12345"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         key = self.management_api.vantage_api_keys_api.get_vantage_api_key(
             account_id=account_id or self.account_id,
             vantage_api_key_id=vantage_api_key_id,
         )
         return VantageAPIKey.model_validate(key.model_dump())
@@ -443,30 +437,22 @@
             Defaults to None.
 
         Returns
         -------
         List[ExternalAPIKey]
             A list of ExternalAPIKey objects, each representing an external API key associated with the account.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> external_api_keys = vantage_client.get_external_api_keys()
-        >>> for key in external_api_keys:
-        ...     print(key.id)
-        "external_key_123"
-        "external_key_321"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         keys = self.management_api.external_api_keys_api.get_external_api_keys(
             account_id=account_id or self.account_id,
         )
         return [
-            ExternalAPIKey.model_validate(key.actual_instance.model_dump())
-            for key in keys
+            ExternalAPIKey.model_validate(key.model_dump()) for key in keys
         ]
 
     def get_external_api_key(
         self,
         external_key_id: str,
         account_id: Optional[str] = None,
     ) -> ExternalAPIKey:
@@ -489,20 +475,15 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the details of the requested external API key.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> external_api_key = vantage_client.get_external_api_key(external_key_id="external_key_123")
-        >>> print(external_api_key.llm_provider)
-        "OpenAI"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         key = self.management_api.external_api_keys_api.get_external_api_key(
             account_id=account_id or self.account_id,
             external_key_id=external_key_id,
         )
 
@@ -536,23 +517,15 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the details of the newly created API key.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> external_api_key = vantage_client.create_external_api_key(
-        ...     llm_provider="OpenAI",
-        ...     llm_secret="secret123",
-        ... )
-        >>> print(external_api_key.id)
-        "external_key_123"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         external_api_key_modifiable = ExternalAPIKeyModifiable(
             llm_provider=llm_provider, llm_secret=llm_secret
         )
 
         key = (
@@ -593,24 +566,15 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the updated details of the external API key.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> updated_external_api_key = vantage_client.update_external_api_key(
-        ...     external_key_id="external_key_123",
-        ...     llm_provider="OpenAI",
-        ...     llm_secret="new_secret_123",
-        ... )
-        >>> print(updated_external_api_key.llm_secret)
-        "new_secret_123"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         external_api_key_modifiable = ExternalAPIKeyModifiable(
             llm_provider=llm_provider, llm_secret=llm_secret
         )
 
         key = (
@@ -641,50 +605,44 @@
         external_key_id : str
             The unique identifier of the external API key to be deleted.
         account_id : Optional[str], optional
             The unique identifier of the account to which the external API key is associated.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_client.delete_external_api_key(external_key_id="external_key_123")
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.external_api_keys_api.delete_external_api_key(
             account_id=account_id or self.account_id,
             external_key_id=external_key_id,
         )
 
     # endregion
 
-    # region Collections
+    # region Collections Helper Functions
 
     def _existing_collection_ids(
         self,
         account_id: Optional[str] = None,
     ) -> List[str]:
         """
         Retrieves a list of existing collection IDs associated with a given account.
 
-        This private method fetches the IDs of all collections linked to the account specified by `account_id`.
-        If `account_id` is not provided, it defaults to the account ID of the current instance.
-
         Parameters
         ----------
         account_id : Optional[str], optional
-            The unique identifier of the account for which the collection IDs are to be retrieved.
-            If not provided, the instance's account ID is used.
+            The account identifier under which to look for collections.
+            If not provided, the default account ID associated with the user is used.
             Defaults to None.
 
         Returns
         -------
         List[str]
-            A list of strings, each representing the unique ID of a collection associated with the account.
+            A list of collection IDs that are available under the specified or default account.
         """
 
         collections = self.list_collections(
             account_id=account_id or self.account_id
         )
         return [col.model_dump()["collection_id"] for col in collections]
 
@@ -693,47 +651,78 @@
         collection_id: str,
         file_size: int,
         parquet_file_name: str,
         account_id: Optional[str] = None,
     ) -> CollectionUploadURL:
         """
         Retrieves a browser upload URL for uploading files to a specified collection.
-        It verifies the existence of the collection within the specified account and
-        raises an exception if the collection does not exist.
-        The method generates a URL that can be used to upload files directly from a browser,
-        using specified file sizes and an optional customer batch identifier for tracking.
 
         Parameters
         ----------
         collection_id : str
-            The unique identifier of the collection to which the file will be uploaded.
+            The identifier of the collection to which the file is being uploaded.
         file_size : int
             The size of the file to be uploaded, in bytes.
         parquet_file_name : str
-            Name of the parquet file being uploaded.
+            The name of the parquet file being uploaded, used as a customer batch identifier.
         account_id : Optional[str], optional
-            The account ID to which the collection belongs.
-            If not provided, the instance's account ID is used.
+            The account identifier under which the collection exists.
+            If not provided, the default account associated with the user is used.
             Defaults to None.
 
         Returns
         -------
         CollectionUploadURL
-            An object containing the URL for browser-based file uploads.
+            An object representing the upload URL and any other relevant data needed for the upload process.
         """
 
         url = self.management_api.collection_api.get_browser_upload_url(
             collection_id=collection_id,
             file_size=file_size,
             customer_batch_identifier=parquet_file_name,
             account_id=account_id or self.account_id,
         )
 
         return CollectionUploadURL.model_validate(url.model_dump())
 
+    def _validate_create_collection_parameters(
+        self,
+        llm_provider: str,
+        url: Optional[str] = None,
+        llm: Optional[str] = None,
+    ) -> None:
+        """
+        Validates the parameters required for creating a collection based on the specified LLM provider.
+
+        Parameters
+        ----------
+        llm_provider : str
+            The name of the LLM provider, which dictates the specific parameters required for the collection.
+        url : Optional[str], optional
+            Endpoint of the HuggingFace model.
+            Required if the LLM provider is HuggingFace and not provided otherwise.
+            Defaults to None.
+        llm : Optional[str], optional
+            OpenAI model identifier.
+            Required if the LLM provider is OpenAI and not provided otherwise.
+            Defaults to None.
+        """
+        if llm_provider == LLMProvider.HuggingFace.value and not url:
+            raise ValueError(
+                f"URL parameter is required if {llm_provider} is used as LLM provider."
+            )
+        elif llm_provider == LLMProvider.OpenAI.value and not llm:
+            raise ValueError(
+                f"LLM parameter is required if {llm_provider} is used as LLM provider."
+            )
+
+    # endregion
+
+    # region Collections
+
     def list_collections(
         self,
         account_id: Optional[str] = None,
     ) -> List[Collection]:
         """
         Retrieves a list of collections associated with a given account.
 
@@ -750,30 +739,23 @@
             Defaults to None.
 
         Returns
         -------
         List[Collection]
             A list of Collection objects, each representing a collection associated with the account.
 
-        Examples
-        --------
-        >>> vantage_client = VantageClient(...)
-        >>> collections = vantage_client.list_collections(account_id="12345")
-        >>> for collection in collections:
-        ...     print(collection.name)
-        "Collection 1"
-        "Collection 2"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         collections = self.management_api.collection_api.list_collections(
             account_id=account_id or self.account_id
         )
 
         return [
-            Collection.model_validate(collection.actual_instance.model_dump())
+            Collection.model_validate(collection.model_dump())
             for collection in collections
         ]
 
     def get_collection(
         self,
         collection_id: str,
         account_id: Optional[str] = None,
@@ -798,236 +780,158 @@
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object containing the details of the specified collection.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient()
-        >>> collection = vantage_client.get_collection(collection_id="unique_collection_id")
-        >>> print(collection.name)
-        "My Collection"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         collection = self.management_api.collection_api.get_collection(
             collection_id=collection_id,
             account_id=account_id or self.account_id,
         )
 
         return Collection.model_validate(collection.model_dump())
 
-    def _validate_create_collection_parameters(
-        self,
-        llm_provider: str,
-        url: Optional[str] = None,
-        llm: Optional[str] = None,
-    ) -> None:
-        if llm_provider == LLMProvider.HuggingFace.value and not url:
-            raise ValueError(
-                f"URL parameter is required if {llm_provider} is used as LLM provider."
-            )
-        elif llm_provider == LLMProvider.OpenAI.value and not llm:
-            raise ValueError(
-                f"LLM parameter is required if {llm_provider} is used as LLM provider."
-            )
-
     def create_collection(
         self,
-        collection_id: str,
-        embeddings_dimension: int,
-        collection_name: Optional[str] = None,
-        user_provided_embeddings: Optional[bool] = False,
-        external_key_id: Optional[str] = None,
-        llm_provider: Optional[str] = None,
-        llm_secret: Optional[str] = None,
-        llm: Optional[str] = None,
-        external_url: Optional[str] = None,
-        collection_preview_url_pattern: Optional[str] = None,
-        account_id: Optional[str] = None,
-    ) -> Collection:
-        """
-        Creates a new collection with the specified parameters.
-
-        This method creates a new collection identified by a unique collection ID.
-        It checks for the uniqueness of the collection ID within the specified account
-        and raises an exception if a collection with the given ID already exists.
-        The collection can optionally be configured to use user-provided embeddings
-        or leverage a Large Language Model (LLM) for embeddings generation.
-        Additional parameters allow specifying an external key for API integration,
-        a preview URL pattern for collection items, and the dimensionality of embeddings.
+        collection: Union[
+            UserProvidedEmbeddingsCollection,
+            OpenAICollection,
+            HuggingFaceCollection,
+        ],
+        account_id: Optional[str] = None,
+    ) -> Union[
+        UserProvidedEmbeddingsCollection,
+        OpenAICollection,
+        HuggingFaceCollection,
+    ]:
+        """
+        Creates a new collection based on the provided collection object.
 
         Parameters
         ----------
-        collection_id : str
-            The unique identifier for the new collection.
-            It can only contain lowercase letters [a-z], digits [0-9] and a hypen [-].
-            The maximum length for a colleciton ID is 36 characters.
-            It can not be changed after the collection is created.
-        embeddings_dimension : int
-            The dimensionality of the embeddings for the collection items.
-        collection_name : Optional[str], optional
-            The name of the new collection.
-            If not provided, value will be 'Colllection [<collection_id>]'
-        user_provided_embeddings : Optional[bool], optional
-            Indicates whether embeddings are provided by the user (True)
-            or managed by Vantage (False). Defaults to False.
-        external_key_id : Optional[str], optional
-            The external key ID used for API integration, if applicable.
-        llm_provider: Optional[str], optional
-            The provider of the Large Language Model (LLM).
-            Supported options are: OpenAI and HuggingFace (Hugging)
-        llm_secret: Optional[str], optional
-            The secret key for accessing the LLM.
-        llm : Optional[str], optional
-            The identifier of the Large Language Model used for generating embeddings, if applicable.
-        external_url : Optional[str], optional
-            Link to the deployed model. Required when llm_provider is set to [Hugging].
-        collection_preview_url_pattern : Optional[str], optional
-            A URL pattern for previewing items in the collection, if applicable.
-        account_id : Optional[str], optional
-            The account ID to which the collection belongs.
-            If not provided, the instance's account ID is used.
-            Defaults to None.
+        collection : Collection
+            Instance of a UserProvidedEmbeddingsCollection, which creates and uses
+            embeddings provided by the user, or instance of OpenAICollection /
+            HuggingFaceCollection, both of which create and use Vantage-managed embeddings.
 
         Returns
         -------
         Collection
             A Collection object representing the newly created collection.
 
-        Example
-        -------
-        User-Provided:
-        >>> vantage_client = VantageClient(...)
-        >>> new_collection = vantage_client.create_collection(
-                collection_id="user-provided",
-                collection_name="My Collection",
-                embeddings_dimension=1536,
-                user_provided_embeddings=True,
-                llm="text-embedding-ada-002",
-                external_key_id="external_key_123",
-            )
-        >>> print(new_collection.id)
-        "user-provided"
-
-        Vantage-Managed:
-        >>> vantage_client = VantageClient(...)
-        >>> new_collection = vantage_client.create_collection(
-                collection_id="vantage-managed",
-                collection_name="My Collection",
-                embeddings_dimension=1536,
-                user_provided_embeddings=False,
-            )
-        >>> print(new_collection.id)
-        "vantage-managed"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
-        collection_name = collection_name or f"Collection [{collection_id}]"
-
-        if not user_provided_embeddings:
-            if external_key_id:
-                if llm_provider or llm_secret:
-                    raise ValueError(
-                        "Please provide either external API key or LLM provider and secret, but not both."
-                    )
-
-                external_key = self.get_external_api_key(
-                    external_key_id=external_key_id
+        if (
+            hasattr(collection, "secondary_external_accounts")
+            and collection.secondary_external_accounts is not None
+        ):
+            collection.secondary_external_accounts = [
+                OpenAPISecondaryExternalAccount(
+                    external_account_id=account.external_account_id,
+                    external_type=account.external_type,
                 )
-
-                llm_provider = external_key.llm_provider
-            else:
-                llm_providers = [el.value for el in LLMProvider]
-
-                if not llm_provider or not llm_secret:
-                    raise ValueError(
-                        "Both LLM provider and LLM secret need to be provided if External API key ID is None."
-                    )
-
-                if llm_provider not in llm_providers:
-                    raise ValueError(
-                        f"LLM provider needs to take one of the following values: {llm_providers}."
-                    )
-
-            self._validate_create_collection_parameters(
-                llm_provider,
-                external_url,
-                llm,
-            )
+                for account in collection.secondary_external_accounts
+            ]
 
         create_collection_request = CreateCollectionRequest(
-            collection_id=collection_id,
-            collection_name=collection_name,
-            embeddings_dimension=int(embeddings_dimension),
-            user_provided_embeddings=bool(user_provided_embeddings),
-            external_key_id=(
-                None if user_provided_embeddings else external_key_id
+            collection_id=collection.collection_id,
+            collection_name=collection.collection_name,
+            user_provided_embeddings=bool(collection.user_provided_embeddings),
+            embeddings_dimension=int(collection.embeddings_dimension),
+            external_key_id=getattr(collection, 'external_account_id', None),
+            secondary_external_accounts=getattr(
+                collection, 'secondary_external_accounts', None
+            ),
+            llm=getattr(collection, 'llm', None),
+            llm_secret=getattr(collection, 'llm_secret', None),
+            llm_provider=getattr(collection, 'llm_provider', None),
+            external_url=getattr(collection, 'external_url', None),
+            collection_preview_url_pattern=getattr(
+                collection, 'collection_preview_url_pattern', None
             ),
-            llm=None if user_provided_embeddings else llm,
-            llm_secret=None if user_provided_embeddings else llm_secret,
-            llm_provider=None if user_provided_embeddings else llm_provider,
-            external_url=None if user_provided_embeddings else external_url,
-            collection_preview_url_pattern=collection_preview_url_pattern,
         )
 
         collection = self.management_api.collection_api.create_collection(
             create_collection_request=create_collection_request,
             account_id=account_id or self.account_id,
         )
 
-        return Collection.model_validate(collection.model_dump())
+        return collection.model_validate(collection.model_dump())
 
     def update_collection(
         self,
         collection_id: str,
         collection_name: Optional[str] = None,
         external_key_id: Optional[str] = None,
-        collection_preview_url_pattern: Optional[str] = None,
+        secondary_external_accounts: Optional[
+            List[SecondaryExternalAccount]
+        ] = None,
         account_id: Optional[str] = None,
     ) -> Collection:
         """
-        Updates an existing collection's details such as its name, associated external key ID, and preview URL pattern.
+        Updates an existing collection's details such as its name, associated external key ID, and secondary accounts.
         It checks for the existence of the collection within the specified account and raises an exception if the
         collection does not exist. Upon successful update, it returns an updated Collection object.
 
         Parameters
         ----------
         collection_id : str
             Unique identifier of the collection to be updated.
         collection_name : Optional[str], optional
             New name for the collection, if updating.
         external_key_id : Optional[str], optional
             New external key ID, if updating.
-        collection_preview_url_pattern : Optional[str], optional
-            New URL pattern for previewing items in the collection, if updating.
+        secondary_external_accounts: Optional[List[SecondaryExternalAccount]], optional
+            Additional external accounts/keys used for indexing, search or both.
+            Applicable if llm_provider is set to OpenAI.
         account_id : Optional[str], optional
             Account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object representing the updated collection.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient(...)
-        >>> updated_collection = vantage_client.update_collection(
-                collection_id="my-collection",
-                collection_name="Updated Collection Name",
-            )
-        >>> print(updated_collection.name)
-        "Updated Collection Name"
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
+        collection = self.management_api.collection_api.get_collection(
+            collection_id=collection_id,
+            account_id=account_id or self.account_id,
+        )
+
+        if secondary_external_accounts:
+            if collection.user_provided_embeddings:
+                raise ValueError(
+                    "Collections with user-provided embeddings cannot have secondary external accounts."
+                )
+
+            if collection.llm_provider is not LLMProvider.OpenAI.value:
+                raise ValueError(
+                    f"Only collections which are using {LLMProvider.OpenAI.value} as LLM provider can have secondary external accounts."  # noqa: E501
+                )
+
+            secondary_external_accounts = [
+                OpenAPISecondaryExternalAccount(
+                    external_account_id=account.external_account_id,
+                    external_type=account.external_type,
+                )
+                for account in secondary_external_accounts
+            ]
+
         collection_modifiable = CollectionModifiable(
             external_key_id=external_key_id,
-            collection_preview_url_pattern=collection_preview_url_pattern,
+            secondary_external_accounts=secondary_external_accounts,
             collection_name=collection_name,
         )
 
         collection = self.management_api.collection_api.update_collection(
             collection_id=collection_id,
             collection_modifiable=collection_modifiable,
             account_id=account_id or self.account_id,
@@ -1055,28 +959,25 @@
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object representing the collection that was deleted.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_client.delete_collection(collection_id="my-collection")
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.collection_api.delete_collection(
             collection_id=collection_id,
             account_id=account_id if account_id else self.account_id,
         )
 
     # endregion
 
-    # region Search
+    # region Search Helper Functions
 
     def _prepare_search_query(
         self,
         collection_id: str,
         accuracy: float = 0.3,
         page: Optional[int] = None,
         page_count: Optional[int] = None,
@@ -1134,14 +1035,18 @@
         if not vantage_api_key:
             raise VantageValueError(
                 "Vantage API Key is missing. Please provide the 'vantage_api_key' parameter to authenticate with the Search API."  # noqa: E501
             )
 
         return vantage_api_key
 
+    # endregion
+
+    # region Search
+
     def semantic_search(
         self,
         text: str,
         collection_id: str,
         accuracy: float = 0.3,
         page: Optional[int] = None,
         page_count: Optional[int] = None,
@@ -1194,16 +1099,25 @@
             If not provided, the instance's account ID is used.
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results.
+
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
+        collection = self.get_collection(collection_id=collection_id)
+
+        if collection.user_provided_embeddings:
+            raise ValueError(
+                "Semantic search is not possible on a collection of user-provided embeddings (UPE)."
+            )
+
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
             accuracy,
             page,
             page_count,
@@ -1287,14 +1201,16 @@
             If not provided, the instance's account ID is used.
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results.
+
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
             accuracy,
@@ -1380,14 +1296,16 @@
             If not provided, the instance's account ID is used.
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results similar to the specified document.
+
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
             accuracy,
@@ -1473,14 +1391,16 @@
             If not provided, the instance's account ID is used.
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results similar to the specified document.
+
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
             accuracy,
@@ -1511,260 +1431,357 @@
             _headers={"authorization": f"Bearer {vantage_api_key}"},
         )
 
         return SearchResult.model_validate(result.model_dump())
 
     # endregion
 
-    # region Upload - Documents
+    # region Documents - Upsert Helper Functions
 
-    def upload_documents_from_jsonl(
+    def _document_to_collection_compatibility_check(
+        self,
+        collection: Collection,
+        document: Union[
+            UserProvidedEmbeddingsDocument, VantageManagedEmbeddingsDocument
+        ],
+    ) -> None:
+        """
+        Checks if a document is compatible with the type of the specified collection.
+
+        Parameters
+        ----------
+        collection : Collection
+            The collection to which the document is intended to be added. This object should specify whether it
+            expects user-provided embeddings or Vantage-managed embeddings.
+        document : Union[UserProvidedEmbeddingsDocument, VantageManagedEmbeddingsDocument]
+            The document to be checked for compatibility with the collection. This must be an instance of either
+            UserProvidedEmbeddingsDocument or VantageManagedEmbeddingsDocument.
+        """
+        if collection.user_provided_embeddings and isinstance(
+            document, VantageManagedEmbeddingsDocument
+        ):
+            raise ValueError(
+                f"Embeddings are required for User-provided embeddings collection. Please provide a list of {UserProvidedEmbeddingsDocument.__name__} objects."  # noqa: E501
+            )
+        elif not collection.user_provided_embeddings and isinstance(
+            document, UserProvidedEmbeddingsDocument
+        ):
+            raise ValueError(
+                f"Embeddings are not required for Vantage-managed embeddings collection. Please provide a list of {VantageManagedEmbeddingsDocument.__name__} objects."  # noqa: E501
+            )
+
+    def _upsert_documents_using_browser_upload_url(
+        self,
+        browser_upload_url: str,
+        upload_content,
+    ) -> int:
+        """
+        Uploads content to a specified collection using a browser upload URL.
+
+        Parameters
+        ----------
+        browser_upload_url : str
+            The URL to which the content should be uploaded. This URL should be pre-configured to
+            accept uploads for a specific collection.
+        upload_content
+            The content to be uploaded.
+
+        Returns
+        -------
+        int
+            The HTTP status code returned by the server after attempting the upload.
+        """
+        response = requests.put(
+            browser_upload_url,
+            data=upload_content,
+        )
+
+        if response.status_code != 200:
+            raise VantageFileUploadError(response.reason, response.status_code)
+
+        return response.status_code
+
+    def _upsert_documents_from_bytes(
         self,
         collection_id: str,
-        documents: str,
+        content: bytes,
+        file_size: int,
+        batch_identifier: Optional[str],
+        account_id: Optional[str] = None,
+    ) -> int:
+        """
+        Upserts documents as bytes to a collection.
+
+        Parameters
+        ----------
+        collection_id : str
+            The identifier of the collection to which the documents are being upserted.
+        content : bytes
+            The binary content (documents in bytes) to be uploaded.
+        file_size : int
+            The size of the content to be uploaded, in bytes.
+        batch_identifier : Optional[str], optional
+            An optional identifier for the batch upload. If not provided, a unique identifier is generated.
+            If provided without a '.parquet' extension, it will be appended. Defaults to None.
+        account_id : Optional[str], optional
+            The account identifier under which the collection exists. If not provided, the default account
+            associated with the user is used. Defaults to None.
+
+        Returns
+        -------
+        int
+            The HTTP status code returned by the server after attempting the upload.
+        """
+
+        if batch_identifier is None:
+            batch_identifier = f"{uuid.uuid4}.parquet"
+        elif not batch_identifier.endswith(".parquet"):
+            batch_identifier = f"{batch_identifier}.parquet"
+
+        browser_upload_url = self._get_browser_upload_url(
+            collection_id=collection_id,
+            file_size=file_size,
+            parquet_file_name=batch_identifier,
+            account_id=account_id,
+        )
+
+        return self._upsert_documents_using_browser_upload_url(
+            browser_upload_url=browser_upload_url.upload_url,
+            upload_content=content,
+        )
+
+    # endregion
+
+    # region Documents - Upsert
+
+    def upsert_documents(
+        self,
+        collection_id: str,
+        documents: Union[
+            List[VantageManagedEmbeddingsDocument],
+            List[UserProvidedEmbeddingsDocument],
+        ],
+        account_id: Optional[str] = None,
+    ):
+        """
+        Upserts documents to a specified collection from a list of Vantage
+        documents. The `documents` object should be a list of one type of Vantage
+        document objects—either VantageManagedEmbeddingsDocument or UserProvidedEmbeddingsDocument,
+        depending on the type of the collection to which you are upserting.
+
+        Parameters
+        ----------
+        collection_id : str
+            The unique identifier for the collection to which the documents will be upserted.
+        documents : Union[List[VantageManagedEmbeddingsDocument], List[UserProvidedEmbeddingsDocument]]
+            A list of documents to upsert. This list should contain only one type of document,
+            either VantageManagedEmbeddingsDocument or UserProvidedEmbeddingsDocument,
+            depending on the collection's type.
+        account_id : Optional[str], optional
+            The account ID to which the collection belongs.
+            If not provided, the instance's account ID is used.
+            Defaults to None.
+
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
+        """
+        if not documents:
+            raise ValueError("Documents object can't be empty.")
+
+        collection = self.get_collection(
+            collection_id=collection_id,
+            account_id=account_id or self.account_id,
+        )
+
+        self._document_to_collection_compatibility_check(
+            collection=collection,
+            document=documents[0],
+        )
+
+        vantage_documents_jsonl = "\n".join(
+            map(
+                json.dumps,
+                [document.to_vantage_dict() for document in documents],
+            )
+        )
+
+        self.upsert_documents_from_jsonl_string(
+            collection_id=collection_id,
+            documents_jsonl=vantage_documents_jsonl,
+            account_id=account_id or self.account_id,
+        )
+
+    def upsert_documents_from_jsonl_string(
+        self,
+        collection_id: str,
+        documents_jsonl: str,
         batch_identifier: Optional[str] = None,
         account_id: Optional[str] = None,
     ) -> None:
         """
-        Uploads documents to a specified collection from a string containing JSONL-formatted documents.
+        Upserts documents to a specified collection from a string containing JSONL-formatted documents.
         The `documents` string is expected to be in JSONL format, where each line is a valid JSON
         document.
 
         Parameters
         ----------
         collection_id : str
             The unique identifier of the collection to which the documents will be uploaded.
-        documents : str
+        documents_jsonl : str
             A string containing the documents to be uploaded, formatted as JSONL.
         batch_identifier : Optional[str], optional
             An optional identifier provided by the user to track the batch of document uploads.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient(...)
-        >>> documents_jsonl = '{"id": "1", "text": "Example text", "meta_color": "green", "meta_something": "value", "embeddings": [1,2,3, ...]}\\n{"id": "2", "text": "Lorem ipsum", "meta_color": "blue", "meta_something": "value", "embeddings": [4,5,6, ...]}' # noqa: E501
-        >>> vantage_client.upload_documents_from_jsonl(
-                collection_id="my-collection",
-                documents=documents_jsonl,
-            )
-        # This will upload two documents to "my-collection".
-
-        Note
-        -------
-        Documents in the JSONL file should be in the right format:
-
-        Uploading to user-provided collection (`embeddings` field is included):
-        {"id": "1", "text": "Example text", "meta_color": "green", "meta_something": "value", "embeddings": [1,2,3, ...]}
-
-
-        Uploading to vantage-managed collection (`embeddings` field is excluded):
-        {"id": "1", "text": "Example text", "meta_color": "green", "meta_something": "value"}
-
-        Metadata fields should all have `meta_` prefix.
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.documents_api.upload_documents(
-            body=documents,
+            body=documents_jsonl,
             account_id=account_id if account_id else self.account_id,
             collection_id=collection_id,
             customer_batch_identifier=batch_identifier,
         )
 
-    def upload_documents_from_path(
+    def upsert_documents_from_jsonl_file(
         self,
         collection_id: str,
-        file_path: str,
+        jsonl_file_path: str,
         batch_identifier: Optional[str] = None,
         account_id: Optional[str] = None,
     ) -> None:
         """
-        Uploads documents to a specified collection from a JSONL file located at a given file path.
+        Upserts documents to a specified collection from a JSONL file located at a given file path.
         This method checks if the file exists at the specified path and raises a FileNotFoundError if it does not.
         It then reads the file and uploads the documents contained within the file to the specified
-        collection using the `upload_documents_from_jsonl` method.
+        collection using the `upsert_documents_from_jsonl_string` method.
 
         Parameters
         ----------
         collection_id : str
             The unique identifier of the collection to which the documents will be uploaded.
         file_path : str
             The path to the JSONL file containing the documents to be uploaded.
         batch_identifier : Optional[str], optional
             An optional identifier provided by the user to track the batch of document uploads.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient()
-        >>> vantage_client.upload_documents_from_path(
-                collection_id="my-collection",
-                file_path="/path/to/documents.jsonl",
-            )
-        # This will upload documents from "/path/to/documents.jsonl" to "my-collection".
-
-        Note
-        -------
-        Documents in the JSONL file should be in the right format:
-
-        Uploading to user-provided collection (`embeddings` field is included):
-        {"id": "1", "text": "Example text", "meta_color": "green", "meta_something": "value", "embeddings": [1,2,3, ...]} # noqa: E501
-
-
-        Uploading to vantage-managed collection (`embeddings` field is excluded):
-        {"id": "1", "text": "Example text", "meta_color": "green", "meta_something": "value"}
-
-        Metadata fields should all have `meta_` prefix.
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
-        if not exists(file_path):
-            raise FileNotFoundError(f"File \"{file_path}\" not found.")
+        if not exists(jsonl_file_path):
+            raise FileNotFoundError(f"File \"{jsonl_file_path}\" not found.")
 
-        file = open(file_path, "rb")
+        file = open(jsonl_file_path, "rb")
         file_content = file.read().decode(self._default_encoding)
-        self.upload_documents_from_jsonl(
+        self.upsert_documents_from_jsonl_string(
             collection_id=collection_id,
-            documents=file_content,
+            documents_jsonl=file_content,
             batch_identifier=batch_identifier,
             account_id=account_id,
         )
 
-    # endregion
-
-    # region Upload - Embeddings
-
-    def _upload_embedding(self, upload_url: str, upload_content) -> int:
-        response = requests.put(
-            upload_url,
-            data=upload_content,
-        )
-
-        if response.status_code != 200:
-            raise VantageFileUploadError(response.reason, response.status_code)
-
-        return response.status_code
-
-    def upload_embeddings_from_bytes(
+    def upsert_documents_from_parquet_file(
         self,
         collection_id: str,
-        content: bytes,
-        file_size: int,
-        batch_identifier: Optional[str],
+        parquet_file_path: str,
         account_id: Optional[str] = None,
     ) -> int:
         """
-        Uploads embeddings in parquet format to a collection.
+        Upserts embeddings from a parquet file to a collection.
+        This upsert method is available for user-provided embeddings collections only.
 
         Parameters
         ----------
         collection_id : str
-            The unique identifier of the collection embeddings are being uploaded.
+            The unique identifier of the collection
+            embeddings are being uploaded to.
+        parquet_file_path : str, optional
+            Path to the parquet file in a filesystem.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None
-        content: bytes
-            Embeddings content as bytes.
-        file_size: int
-            Size of contents being uploaded, in bytes.
-        parquet_file_name: str
-        batch_identifier : Optional[str], optional
-            An optional identifier provided by the user to track the batch of document uploads.
-            Identifier needs to end with '.parquet',if it doesn't, it will be
-            automatically added.
-            If none is provided, it will be generated automatically.
 
         Returns
         -------
         int
             HTTP status of upload execution.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_client.upload_parquet_embedding(
-            collection_id="my-collection",
-            content=parquet_content_as_bytes,
-            file_size=1000,
-            batch_identifier="my-embeddings.parquet"
-        )
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
-        if batch_identifier is None:
-            batch_identifier = f"{uuid.uuid4}.parquet"
-        elif not batch_identifier.endswith(".parquet"):
-            batch_identifier = f"{batch_identifier}.parquet"
+        collection = self.get_collection(collection_id=collection_id)
 
-        browser_upload_url = self._get_browser_upload_url(
+        if not collection.user_provided_embeddings:
+            raise ValueError(
+                "Upsert using parquet file is available only for user-provided embeddings (UPE) collections."
+            )
+
+        if not exists(parquet_file_path):
+            raise FileNotFoundError(f"File \"{parquet_file_path}\" not found.")
+        file_name = ntpath.basename(parquet_file_path)
+
+        if not parquet_file_path.endswith(".parquet"):
+            raise ValueError("File mast be a parquet file.")
+
+        file_size = Path(parquet_file_path).stat().st_size
+        file = open(parquet_file_path, "rb")
+        file_content = file.read()
+        return self._upsert_documents_from_bytes(
             collection_id=collection_id,
+            content=file_content,
             file_size=file_size,
-            parquet_file_name=batch_identifier,
+            batch_identifier=file_name,
             account_id=account_id,
         )
 
-        return self._upload_embedding(
-            upload_url=browser_upload_url.upload_url,
-            upload_content=content,
-        )
+    # endregion
+
+    # region Documents - Delete
 
-    def upload_embeddings_from_parquet(
+    def delete_documents(
         self,
         collection_id: str,
-        file_path: str,
+        document_ids: List[str],
         account_id: Optional[str] = None,
-    ) -> int:
+    ) -> None:
         """
-        Uploads embeddings from a parquet file to a collection.
+        Deletes a list of documents from a specified collection.
 
         Parameters
         ----------
         collection_id : str
-            The unique identifier of the collection
-            embeddings are being uploaded to.
-        file_path : str, optional
-            Path to the parquet file in a filesystem.
+            The unique identifier of the collection from which documents are to be deleted.
+        document_ids : List[str]
+            A list of document IDs that need to be deleted from the collection.
         account_id : Optional[str], optional
-            The account ID to which the collection belongs.
+            The account identifier under which the collection exists.
             If not provided, the instance's account ID is used.
-            Defaults to None
-
-        Returns
-        -------
-        int
-            HTTP status of upload execution.
+            Defaults to None.
 
-        Example
-        -------
-        >>> vantage_client = VantageClient(...)
-        >>> vantage_client.upload_parquet_embedding(
-            collection_id="my-collection",
-            content=parquet_content_as_bytes,
-            file_size=1000,
-            batch_identifier="my-embeddings.parquet"
-        )
+        Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
-        if not exists(file_path):
-            raise FileNotFoundError(f"File \"{file_path}\" not found.")
-        file_name = ntpath.basename(file_path)
+        documents_to_delete = [
+            {"id": id, "operation": "delete"} for id in document_ids
+        ]
 
-        if not file_path.endswith(".parquet"):
-            raise ValueError("File mast be a parquet file.")
+        vantage_documents_jsonl = "\n".join(
+            map(
+                json.dumps,
+                [document for document in documents_to_delete],
+            )
+        )
 
-        file_size = Path(file_path).stat().st_size
-        file = open(file_path, "rb")
-        file_content = file.read()
-        return self.upload_embeddings_from_bytes(
+        self.upsert_documents_from_jsonl_string(
             collection_id=collection_id,
-            content=file_content,
-            file_size=file_size,
-            batch_identifier=file_name,
-            account_id=account_id,
+            documents_jsonl=vantage_documents_jsonl,
+            account_id=account_id or self.account_id,
         )
 
     # endregion
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/base.py` & `vantage_sdk-0.8.0/vantage_sdk/core/base.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/exceptions.py` & `vantage_sdk-0.8.0/vantage_sdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/__init__.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,34 +55,28 @@
 )
 from vantage_sdk.core.http.models.collection_read_only import (
     CollectionReadOnly,
 )
 from vantage_sdk.core.http.models.collection_upload_url import (
     CollectionUploadURL,
 )
-from vantage_sdk.core.http.models.collections_result_inner import (
-    CollectionsResultInner,
-)
 from vantage_sdk.core.http.models.create_collection_request import (
     CreateCollectionRequest,
 )
 from vantage_sdk.core.http.models.document_batch import DocumentBatch
 from vantage_sdk.core.http.models.embedding_search_query import (
     EmbeddingSearchQuery,
 )
 from vantage_sdk.core.http.models.external_api_key import ExternalAPIKey
 from vantage_sdk.core.http.models.external_api_key_modifiable import (
     ExternalAPIKeyModifiable,
 )
 from vantage_sdk.core.http.models.external_api_key_read_only import (
     ExternalAPIKeyReadOnly,
 )
-from vantage_sdk.core.http.models.external_api_keys_result_inner import (
-    ExternalAPIKeysResultInner,
-)
 from vantage_sdk.core.http.models.global_search_properties import (
     GlobalSearchProperties,
 )
 from vantage_sdk.core.http.models.global_search_properties_collection import (
     GlobalSearchPropertiesCollection,
 )
 from vantage_sdk.core.http.models.global_search_properties_field_value_weighting import (
@@ -103,17 +97,17 @@
     MoreLikeTheseQuery,
 )
 from vantage_sdk.core.http.models.more_like_this_query import MoreLikeThisQuery
 from vantage_sdk.core.http.models.search_result import SearchResult
 from vantage_sdk.core.http.models.search_result_results_inner import (
     SearchResultResultsInner,
 )
+from vantage_sdk.core.http.models.secondary_external_account import (
+    SecondaryExternalAccount,
+)
 from vantage_sdk.core.http.models.semantic_search_query import (
     SemanticSearchQuery,
 )
 from vantage_sdk.core.http.models.vantage_api_key import VantageAPIKey
-from vantage_sdk.core.http.models.vantage_api_keys_result_inner import (
-    VantageAPIKeysResultInner,
-)
 from vantage_sdk.core.http.models.weighted_field_values import (
     WeightedFieldValues,
 )
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/__init__.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/account_management_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/account_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/collection_management_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/collection_management_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 from vantage_sdk.core.http.models.collection import Collection
 from vantage_sdk.core.http.models.collection_modifiable import (
     CollectionModifiable,
 )
 from vantage_sdk.core.http.models.collection_upload_url import (
     CollectionUploadURL,
 )
-from vantage_sdk.core.http.models.collections_result_inner import (
-    CollectionsResultInner,
-)
 from vantage_sdk.core.http.models.create_collection_request import (
     CreateCollectionRequest,
 )
 from vantage_sdk.core.http.rest import RESTResponseType
 
 
 class CollectionManagementApi:
@@ -1291,15 +1288,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[CollectionsResultInner]:
+    ) -> List[Collection]:
         """List Collections
 
         List the collections in account_id
 
         :param account_id: The account id (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -1329,15 +1326,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[CollectionsResultInner]",
+            '200': "List[Collection]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1357,15 +1354,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[CollectionsResultInner]]:
+    ) -> ApiResponse[List[Collection]]:
         """List Collections
 
         List the collections in account_id
 
         :param account_id: The account id (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -1395,15 +1392,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[CollectionsResultInner]",
+            '200': "List[Collection]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1461,15 +1458,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[CollectionsResultInner]",
+            '200': "List[Collection]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/documents_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/external_api_keys_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/external_api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 
 from vantage_sdk.core.http.api_client import ApiClient
 from vantage_sdk.core.http.api_response import ApiResponse
 from vantage_sdk.core.http.models.external_api_key import ExternalAPIKey
 from vantage_sdk.core.http.models.external_api_key_modifiable import (
     ExternalAPIKeyModifiable,
 )
-from vantage_sdk.core.http.models.external_api_keys_result_inner import (
-    ExternalAPIKeysResultInner,
-)
 from vantage_sdk.core.http.rest import RESTResponseType
 
 
 class ExternalAPIKeysApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -889,15 +886,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ExternalAPIKeysResultInner]:
+    ) -> List[ExternalAPIKey]:
         """Get external API keys
 
         Get external API keys
 
         :param account_id: The account these keys are within (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -927,15 +924,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ExternalAPIKeysResultInner]",
+            '200': "List[ExternalAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -957,15 +954,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ExternalAPIKeysResultInner]]:
+    ) -> ApiResponse[List[ExternalAPIKey]]:
         """Get external API keys
 
         Get external API keys
 
         :param account_id: The account these keys are within (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -995,15 +992,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ExternalAPIKeysResultInner]",
+            '200': "List[ExternalAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1063,15 +1060,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ExternalAPIKeysResultInner]",
+            '200': "List[ExternalAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/search_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/search_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api/vantage_api_keys_api.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api/vantage_api_keys_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 
 from pydantic import Field, StrictStr
 from typing_extensions import Annotated
 
 from vantage_sdk.core.http.api_client import ApiClient
 from vantage_sdk.core.http.api_response import ApiResponse
 from vantage_sdk.core.http.models.vantage_api_key import VantageAPIKey
-from vantage_sdk.core.http.models.vantage_api_keys_result_inner import (
-    VantageAPIKeysResultInner,
-)
 from vantage_sdk.core.http.rest import RESTResponseType
 
 
 class VantageAPIKeysApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -336,15 +333,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[VantageAPIKeysResultInner]:
+    ) -> List[VantageAPIKey]:
         """Get Vantage API keys
 
         Get Vantage API keys
 
         :param account_id: The account these keys are within (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -374,15 +371,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[VantageAPIKeysResultInner]",
+            '200': "List[VantageAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -404,15 +401,15 @@
                 Annotated[StrictFloat, Field(gt=0)],
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[VantageAPIKeysResultInner]]:
+    ) -> ApiResponse[List[VantageAPIKey]]:
         """Get Vantage API keys
 
         Get Vantage API keys
 
         :param account_id: The account these keys are within (required)
         :type account_id: str
         :param _request_timeout: timeout setting for this request. If one
@@ -442,15 +439,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[VantageAPIKeysResultInner]",
+            '200': "List[VantageAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -510,15 +507,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[VantageAPIKeysResultInner]",
+            '200': "List[VantageAPIKey]",
             '405': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api_client.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api_client.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/api_response.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/api_response.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/configuration.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/configuration.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/exceptions.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/__init__.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,34 +27,28 @@
 )
 from vantage_sdk.core.http.models.collection_read_only import (
     CollectionReadOnly,
 )
 from vantage_sdk.core.http.models.collection_upload_url import (
     CollectionUploadURL,
 )
-from vantage_sdk.core.http.models.collections_result_inner import (
-    CollectionsResultInner,
-)
 from vantage_sdk.core.http.models.create_collection_request import (
     CreateCollectionRequest,
 )
 from vantage_sdk.core.http.models.document_batch import DocumentBatch
 from vantage_sdk.core.http.models.embedding_search_query import (
     EmbeddingSearchQuery,
 )
 from vantage_sdk.core.http.models.external_api_key import ExternalAPIKey
 from vantage_sdk.core.http.models.external_api_key_modifiable import (
     ExternalAPIKeyModifiable,
 )
 from vantage_sdk.core.http.models.external_api_key_read_only import (
     ExternalAPIKeyReadOnly,
 )
-from vantage_sdk.core.http.models.external_api_keys_result_inner import (
-    ExternalAPIKeysResultInner,
-)
 from vantage_sdk.core.http.models.global_search_properties import (
     GlobalSearchProperties,
 )
 from vantage_sdk.core.http.models.global_search_properties_collection import (
     GlobalSearchPropertiesCollection,
 )
 from vantage_sdk.core.http.models.global_search_properties_field_value_weighting import (
@@ -75,17 +69,17 @@
     MoreLikeTheseQuery,
 )
 from vantage_sdk.core.http.models.more_like_this_query import MoreLikeThisQuery
 from vantage_sdk.core.http.models.search_result import SearchResult
 from vantage_sdk.core.http.models.search_result_results_inner import (
     SearchResultResultsInner,
 )
+from vantage_sdk.core.http.models.secondary_external_account import (
+    SecondaryExternalAccount,
+)
 from vantage_sdk.core.http.models.semantic_search_query import (
     SemanticSearchQuery,
 )
 from vantage_sdk.core.http.models.vantage_api_key import VantageAPIKey
-from vantage_sdk.core.http.models.vantage_api_keys_result_inner import (
-    VantageAPIKeysResultInner,
-)
 from vantage_sdk.core.http.models.weighted_field_values import (
     WeightedFieldValues,
 )
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/account.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/account_modifiable.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/account_read_only.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     Field,
     StrictBool,
     StrictInt,
     StrictStr,
     field_validator,
 )
 
+from vantage_sdk.core.http.models.secondary_external_account import (
+    SecondaryExternalAccount,
+)
+
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
@@ -60,14 +64,17 @@
         default=None,
         description="The dimensionality or vector size of the embeddings.  Applies to both user provided embeddings and vantage managed embeddings.",
     )
     external_key_id: Optional[StrictStr] = Field(
         default=None,
         description="The external API key, for the llm_provider to use for the collection",
     )
+    secondary_external_accounts: Optional[
+        List[SecondaryExternalAccount]
+    ] = None
     collection_name: Optional[StrictStr] = None
     collection_preview_url_pattern: Optional[StrictStr] = Field(
         default=None,
         description="To be able to preview items in test on the test collection page, enter in a URL that supports the open graph extensions for previewing links.",
     )
     __properties: ClassVar[List[str]] = [
         "collection_created_time",
@@ -77,14 +84,15 @@
         "user_provided_embeddings",
         "llm",
         "llm_provider",
         "llm_secret",
         "external_url",
         "embeddings_dimension",
         "external_key_id",
+        "secondary_external_accounts",
         "collection_name",
         "collection_preview_url_pattern",
     ]
 
     @field_validator('collection_status')
     def collection_status_validate_enum(cls, value):
         """Validates the enum"""
@@ -165,14 +173,21 @@
             exclude={
                 "collection_created_time",
                 "collection_status",
                 "collection_state",
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in secondary_external_accounts (list)
+        _items = []
+        if self.secondary_external_accounts:
+            for _item in self.secondary_external_accounts:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['secondary_external_accounts'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Collection from a dict"""
         if obj is None:
             return None
@@ -191,14 +206,20 @@
                 else False,
                 "llm": obj.get("llm"),
                 "llm_provider": obj.get("llm_provider"),
                 "llm_secret": obj.get("llm_secret"),
                 "external_url": obj.get("external_url"),
                 "embeddings_dimension": obj.get("embeddings_dimension"),
                 "external_key_id": obj.get("external_key_id"),
+                "secondary_external_accounts": [
+                    SecondaryExternalAccount.from_dict(_item)
+                    for _item in obj.get("secondary_external_accounts")
+                ]
+                if obj.get("secondary_external_accounts") is not None
+                else None,
                 "collection_name": obj.get("collection_name"),
                 "collection_preview_url_pattern": obj.get(
                     "collection_preview_url_pattern"
                 ),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_immutable.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_immutable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_modifiable.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_upload_url.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,43 +16,49 @@
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr, field_validator
 
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class CollectionModifiable(BaseModel):
+class CollectionUploadURL(BaseModel):
     """
-    CollectionModifiable
+    CollectionUploadURL
     """  # noqa: E501
 
-    external_key_id: Optional[StrictStr] = Field(
-        default=None,
-        description="The external API key, for the llm_provider to use for the collection",
-    )
-    collection_name: Optional[StrictStr] = None
-    collection_preview_url_pattern: Optional[StrictStr] = Field(
-        default=None,
-        description="To be able to preview items in test on the test collection page, enter in a URL that supports the open graph extensions for previewing links.",
-    )
+    collection_id: Optional[StrictStr] = None
+    customer_batch_identifier: Optional[StrictStr] = None
+    upload_url_type: Optional[StrictStr] = None
+    upload_url: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = [
-        "external_key_id",
-        "collection_name",
-        "collection_preview_url_pattern",
+        "collection_id",
+        "customer_batch_identifier",
+        "upload_url_type",
+        "upload_url",
     ]
 
+    @field_validator('upload_url_type')
+    def upload_url_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PUT'):
+            raise ValueError("must be one of enum values ('PUT')")
+        return value
+
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def to_str(self) -> str:
@@ -62,46 +68,50 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CollectionModifiable from a JSON string"""
+        """Create an instance of CollectionUploadURL from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         _dict = self.model_dump(
             by_alias=True,
-            exclude={},
+            exclude={
+                "collection_id",
+            },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of CollectionModifiable from a dict"""
+        """Create an instance of CollectionUploadURL from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "external_key_id": obj.get("external_key_id"),
-                "collection_name": obj.get("collection_name"),
-                "collection_preview_url_pattern": obj.get(
-                    "collection_preview_url_pattern"
+                "collection_id": obj.get("collection_id"),
+                "customer_batch_identifier": obj.get(
+                    "customer_batch_identifier"
                 ),
+                "upload_url_type": obj.get("upload_url_type"),
+                "upload_url": obj.get("upload_url"),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_read_only.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collection_upload_url.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_read_only.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,49 +16,43 @@
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, StrictStr, field_validator
+from pydantic import BaseModel, Field, StrictStr
 
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class CollectionUploadURL(BaseModel):
+class ExternalAPIKeyReadOnly(BaseModel):
     """
-    CollectionUploadURL
+    ExternalAPIKeyReadOnly
     """  # noqa: E501
 
-    collection_id: Optional[StrictStr] = None
-    customer_batch_identifier: Optional[StrictStr] = None
-    upload_url_type: Optional[StrictStr] = None
-    upload_url: Optional[StrictStr] = None
+    external_key_id: Optional[StrictStr] = Field(
+        default=None, description="The unique id of the key"
+    )
+    account_id: Optional[StrictStr] = Field(
+        default=None, description="The account this key is contained within"
+    )
+    external_key_created_date: Optional[StrictStr] = Field(
+        default=None, description="date this key was created"
+    )
     __properties: ClassVar[List[str]] = [
-        "collection_id",
-        "customer_batch_identifier",
-        "upload_url_type",
-        "upload_url",
+        "external_key_id",
+        "account_id",
+        "external_key_created_date",
     ]
 
-    @field_validator('upload_url_type')
-    def upload_url_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('PUT'):
-            raise ValueError("must be one of enum values ('PUT')")
-        return value
-
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def to_str(self) -> str:
@@ -68,50 +62,53 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CollectionUploadURL from a JSON string"""
+        """Create an instance of ExternalAPIKeyReadOnly from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
-                "collection_id",
+                "external_key_id",
+                "account_id",
+                "external_key_created_date",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of CollectionUploadURL from a dict"""
+        """Create an instance of ExternalAPIKeyReadOnly from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "collection_id": obj.get("collection_id"),
-                "customer_batch_identifier": obj.get(
-                    "customer_batch_identifier"
+                "external_key_id": obj.get("external_key_id"),
+                "account_id": obj.get("account_id"),
+                "external_key_created_date": obj.get(
+                    "external_key_created_date"
                 ),
-                "upload_url_type": obj.get("upload_url_type"),
-                "upload_url": obj.get("upload_url"),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/collections_result_inner.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/embedding_search_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,145 +14,151 @@
 
 
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from inspect import getfullargspec
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Union
 
-from pydantic import (
-    BaseModel,
-    Field,
-    StrictStr,
-    ValidationError,
-    field_validator,
-)
-from typing_extensions import Literal
+from pydantic import BaseModel, StrictFloat, StrictInt
 
-from vantage_sdk.core.http.models.collection import Collection
+from vantage_sdk.core.http.models.global_search_properties_collection import (
+    GlobalSearchPropertiesCollection,
+)
+from vantage_sdk.core.http.models.global_search_properties_field_value_weighting import (
+    GlobalSearchPropertiesFieldValueWeighting,
+)
+from vantage_sdk.core.http.models.global_search_properties_filter import (
+    GlobalSearchPropertiesFilter,
+)
+from vantage_sdk.core.http.models.global_search_properties_pagination import (
+    GlobalSearchPropertiesPagination,
+)
+from vantage_sdk.core.http.models.global_search_properties_sort import (
+    GlobalSearchPropertiesSort,
+)
 
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-COLLECTIONSRESULTINNER_ONE_OF_SCHEMAS = ["Collection"]
 
-
-class CollectionsResultInner(BaseModel):
-    """
-    CollectionsResultInner
+class EmbeddingSearchQuery(BaseModel):
     """
+    EmbeddingSearchQuery
+    """  # noqa: E501
 
-    # data type: Collection
-    oneof_schema_1_validator: Optional[Collection] = None
-    actual_instance: Optional[Union[Collection]] = None
-    one_of_schemas: List[str] = Literal["Collection"]
+    collection: Optional[GlobalSearchPropertiesCollection] = None
+    request_id: Optional[StrictInt] = None
+    filter: Optional[GlobalSearchPropertiesFilter] = None
+    field_value_weighting: Optional[
+        GlobalSearchPropertiesFieldValueWeighting
+    ] = None
+    pagination: Optional[GlobalSearchPropertiesPagination] = None
+    sort: Optional[GlobalSearchPropertiesSort] = None
+    embedding: Optional[List[Union[StrictFloat, StrictInt]]] = None
+    __properties: ClassVar[List[str]] = [
+        "collection",
+        "request_id",
+        "filter",
+        "field_value_weighting",
+        "pagination",
+        "sort",
+        "embedding",
+    ]
 
     model_config = {
+        "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
-    def __init__(self, *args, **kwargs) -> None:
-        if args:
-            if len(args) > 1:
-                raise ValueError(
-                    "If a position argument is used, only 1 is allowed to set `actual_instance`"
-                )
-            if kwargs:
-                raise ValueError(
-                    "If a position argument is used, keyword arguments cannot be used."
-                )
-            super().__init__(actual_instance=args[0])
-        else:
-            super().__init__(**kwargs)
-
-    @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = CollectionsResultInner.model_construct()
-        error_messages = []
-        match = 0
-        # validate data type: Collection
-        if not isinstance(v, Collection):
-            error_messages.append(
-                f"Error! Input type `{type(v)}` is not `Collection`"
-            )
-        else:
-            match += 1
-        if match > 1:
-            # more than 1 match
-            raise ValueError(
-                "Multiple matches found when setting `actual_instance` in CollectionsResultInner with oneOf schemas: Collection. Details: "
-                + ", ".join(error_messages)
-            )
-        elif match == 0:
-            # no match
-            raise ValueError(
-                "No match found when setting `actual_instance` in CollectionsResultInner with oneOf schemas: Collection. Details: "
-                + ", ".join(error_messages)
-            )
-        else:
-            return v
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
 
-    @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        return cls.from_json(json.dumps(obj))
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Returns the object represented by the json string"""
-        instance = cls.model_construct()
-        error_messages = []
-        match = 0
-
-        # deserialize data into Collection
-        try:
-            instance.actual_instance = Collection.from_json(json_str)
-            match += 1
-        except (ValidationError, ValueError) as e:
-            error_messages.append(str(e))
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError(
-                "Multiple matches found when deserializing the JSON string into CollectionsResultInner with oneOf schemas: Collection. Details: "
-                + ", ".join(error_messages)
-            )
-        elif match == 0:
-            # no match
-            raise ValueError(
-                "No match found when deserializing the JSON string into CollectionsResultInner with oneOf schemas: Collection. Details: "
-                + ", ".join(error_messages)
-            )
-        else:
-            return instance
+        """Create an instance of EmbeddingSearchQuery from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
 
-    def to_json(self) -> str:
-        """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is None:
-            return "null"
-
-        to_json = getattr(self.actual_instance, "to_json", None)
-        if callable(to_json):
-            return self.actual_instance.to_json()
-        else:
-            return json.dumps(self.actual_instance)
-
-    def to_dict(self) -> Dict:
-        """Returns the dict representation of the actual instance"""
-        if self.actual_instance is None:
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude={},
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of collection
+        if self.collection:
+            _dict['collection'] = self.collection.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of filter
+        if self.filter:
+            _dict['filter'] = self.filter.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of field_value_weighting
+        if self.field_value_weighting:
+            _dict[
+                'field_value_weighting'
+            ] = self.field_value_weighting.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of sort
+        if self.sort:
+            _dict['sort'] = self.sort.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of EmbeddingSearchQuery from a dict"""
+        if obj is None:
             return None
 
-        to_dict = getattr(self.actual_instance, "to_dict", None)
-        if callable(to_dict):
-            return self.actual_instance.to_dict()
-        else:
-            # primitive type
-            return self.actual_instance
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
 
-    def to_str(self) -> str:
-        """Returns the string representation of the actual instance"""
-        return pprint.pformat(self.model_dump())
+        _obj = cls.model_validate(
+            {
+                "collection": GlobalSearchPropertiesCollection.from_dict(
+                    obj.get("collection")
+                )
+                if obj.get("collection") is not None
+                else None,
+                "request_id": obj.get("request_id"),
+                "filter": GlobalSearchPropertiesFilter.from_dict(
+                    obj.get("filter")
+                )
+                if obj.get("filter") is not None
+                else None,
+                "field_value_weighting": GlobalSearchPropertiesFieldValueWeighting.from_dict(
+                    obj.get("field_value_weighting")
+                )
+                if obj.get("field_value_weighting") is not None
+                else None,
+                "pagination": GlobalSearchPropertiesPagination.from_dict(
+                    obj.get("pagination")
+                )
+                if obj.get("pagination") is not None
+                else None,
+                "sort": GlobalSearchPropertiesSort.from_dict(obj.get("sort"))
+                if obj.get("sort") is not None
+                else None,
+                "embedding": obj.get("embedding"),
+            }
+        )
+        return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/create_collection_request.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/create_collection_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     Field,
     StrictBool,
     StrictInt,
     StrictStr,
     field_validator,
 )
 
+from vantage_sdk.core.http.models.secondary_external_account import (
+    SecondaryExternalAccount,
+)
+
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
@@ -55,28 +59,32 @@
     embeddings_dimension: StrictInt = Field(
         description="The dimensionality or vector size of the embeddings.  Applies to both user provided embeddings and vantage managed embeddings."
     )
     external_key_id: Optional[StrictStr] = Field(
         default=None,
         description="The external API key, for the llm_provider to use for the collection",
     )
+    secondary_external_accounts: Optional[
+        List[SecondaryExternalAccount]
+    ] = None
     collection_name: StrictStr
     collection_preview_url_pattern: Optional[StrictStr] = Field(
         default=None,
         description="To be able to preview items in test on the test collection page, enter in a URL that supports the open graph extensions for previewing links.",
     )
     __properties: ClassVar[List[str]] = [
         "collection_id",
         "user_provided_embeddings",
         "llm",
         "llm_provider",
         "llm_secret",
         "external_url",
         "embeddings_dimension",
         "external_key_id",
+        "secondary_external_accounts",
         "collection_name",
         "collection_preview_url_pattern",
     ]
 
     @field_validator('llm_provider')
     def llm_provider_validate_enum(cls, value):
         """Validates the enum"""
@@ -120,14 +128,21 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in secondary_external_accounts (list)
+        _items = []
+        if self.secondary_external_accounts:
+            for _item in self.secondary_external_accounts:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['secondary_external_accounts'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateCollectionRequest from a dict"""
         if obj is None:
             return None
@@ -143,14 +158,20 @@
                 else False,
                 "llm": obj.get("llm"),
                 "llm_provider": obj.get("llm_provider"),
                 "llm_secret": obj.get("llm_secret"),
                 "external_url": obj.get("external_url"),
                 "embeddings_dimension": obj.get("embeddings_dimension"),
                 "external_key_id": obj.get("external_key_id"),
+                "secondary_external_accounts": [
+                    SecondaryExternalAccount.from_dict(_item)
+                    for _item in obj.get("secondary_external_accounts")
+                ]
+                if obj.get("secondary_external_accounts") is not None
+                else None,
                 "collection_name": obj.get("collection_name"),
                 "collection_preview_url_pattern": obj.get(
                     "collection_preview_url_pattern"
                 ),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/document_batch.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/document_batch.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/embedding_search_query.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/semantic_search_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, StrictFloat, StrictInt
+from pydantic import BaseModel, StrictInt, StrictStr
 
 from vantage_sdk.core.http.models.global_search_properties_collection import (
     GlobalSearchPropertiesCollection,
 )
 from vantage_sdk.core.http.models.global_search_properties_field_value_weighting import (
     GlobalSearchPropertiesFieldValueWeighting,
 )
@@ -41,36 +41,36 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class EmbeddingSearchQuery(BaseModel):
+class SemanticSearchQuery(BaseModel):
     """
-    EmbeddingSearchQuery
+    SemanticSearchQuery
     """  # noqa: E501
 
     collection: Optional[GlobalSearchPropertiesCollection] = None
     request_id: Optional[StrictInt] = None
     filter: Optional[GlobalSearchPropertiesFilter] = None
     field_value_weighting: Optional[
         GlobalSearchPropertiesFieldValueWeighting
     ] = None
     pagination: Optional[GlobalSearchPropertiesPagination] = None
     sort: Optional[GlobalSearchPropertiesSort] = None
-    embedding: Optional[List[Union[StrictFloat, StrictInt]]] = None
+    text: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = [
         "collection",
         "request_id",
         "filter",
         "field_value_weighting",
         "pagination",
         "sort",
-        "embedding",
+        "text",
     ]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -82,15 +82,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of EmbeddingSearchQuery from a JSON string"""
+        """Create an instance of SemanticSearchQuery from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -121,15 +121,15 @@
         # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
             _dict['sort'] = self.sort.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of EmbeddingSearchQuery from a dict"""
+        """Create an instance of SemanticSearchQuery from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
@@ -154,11 +154,11 @@
                     obj.get("pagination")
                 )
                 if obj.get("pagination") is not None
                 else None,
                 "sort": GlobalSearchPropertiesSort.from_dict(obj.get("sort"))
                 if obj.get("sort") is not None
                 else None,
-                "embedding": obj.get("embedding"),
+                "text": obj.get("text"),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key_modifiable.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/external_api_key_read_only.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/secondary_external_account.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,43 +16,49 @@
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictStr, field_validator
 
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class ExternalAPIKeyReadOnly(BaseModel):
+class SecondaryExternalAccount(BaseModel):
     """
-    ExternalAPIKeyReadOnly
+    SecondaryExternalAccount
     """  # noqa: E501
 
-    external_key_id: Optional[StrictStr] = Field(
-        default=None, description="The unique id of the key"
-    )
-    account_id: Optional[StrictStr] = Field(
-        default=None, description="The account this key is contained within"
-    )
-    external_key_created_date: Optional[StrictStr] = Field(
-        default=None, description="date this key was created"
+    external_account_id: Optional[StrictStr] = Field(
+        default=None, description="The external API key ID"
     )
+    external_type: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = [
-        "external_key_id",
-        "account_id",
-        "external_key_created_date",
+        "external_account_id",
+        "external_type",
     ]
 
+    @field_validator('external_type')
+    def external_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('index', 'search', 'both'):
+            raise ValueError(
+                "must be one of enum values ('index', 'search', 'both')"
+            )
+        return value
+
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def to_str(self) -> str:
@@ -62,53 +68,43 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ExternalAPIKeyReadOnly from a JSON string"""
+        """Create an instance of SecondaryExternalAccount from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-                "external_key_id",
-                "account_id",
-                "external_key_created_date",
-            },
+            exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ExternalAPIKeyReadOnly from a dict"""
+        """Create an instance of SecondaryExternalAccount from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "external_key_id": obj.get("external_key_id"),
-                "account_id": obj.get("account_id"),
-                "external_key_created_date": obj.get(
-                    "external_key_created_date"
-                ),
+                "external_account_id": obj.get("external_account_id"),
+                "external_type": obj.get("external_type"),
             }
         )
         return _obj
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_collection.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_filter.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_filter.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_pagination.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_pagination.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/global_search_properties_sort.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_sort.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/ml_these.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/ml_these_these_inner.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these_these_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/more_like_these_query.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_these_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/more_like_this_query.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_this_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/search_result.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/search_result_results_inner.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result_results_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/vantage_api_key.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/vantage_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/models/weighted_field_values.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/models/weighted_field_values.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/http/rest.py` & `vantage_sdk-0.8.0/vantage_sdk/core/http/rest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/core/management/management.py` & `vantage_sdk-0.8.0/vantage_sdk/core/management/management.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/exceptions.py` & `vantage_sdk-0.8.0/vantage_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/vantage_sdk/model/collection.py` & `vantage_sdk-0.8.0/vantage_sdk/model/keys.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+from enum import Enum
 from typing import Optional
 
-from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, StrictStr
 
 
-class Collection(BaseModel):
-    collection_created_time: Optional[StrictStr] = None
-    collection_status: Optional[StrictStr] = None
-    collection_state: Optional[StrictStr] = None
-    collection_id: Optional[StrictStr] = None
-    user_provided_embeddings: Optional[StrictBool] = None
-    llm: Optional[StrictStr] = None
-    external_url: Optional[StrictStr] = None
-    embeddings_dimension: Optional[StrictInt] = None
-    external_account_id: Optional[StrictStr] = None
-    collection_name: Optional[StrictStr] = None
-    collection_preview_url_pattern: Optional[StrictStr] = None
+class VantageAPIKey(BaseModel):
+    vantage_api_key_id: Optional[StrictStr] = None
+    account_id: Optional[StrictStr] = None
+    vantage_api_key_created_date: Optional[StrictStr] = None
+    vantage_api_key_obfuscated: Optional[StrictStr] = None
+    status: Optional[StrictStr] = None
+
+
+class LLMProvider(Enum):
+    HuggingFace = "Hugging"
+    OpenAI = "OpenAI"
 
 
-class CollectionUploadURL(BaseModel):
-    collection_id: Optional[StrictStr] = None
-    customer_batch_identifier: Optional[StrictStr] = None
-    upload_url_type: Optional[StrictStr] = None
-    upload_url: Optional[StrictStr] = None
+class ExternalAPIKey(BaseModel):
+    external_key_id: Optional[StrictStr] = None
+    account_id: Optional[StrictStr] = None
+    external_key_created_date: Optional[StrictStr] = None
+    llm_provider: Optional[StrictStr] = None
+    llm_secret: Optional[StrictStr] = None
+    state: Optional[StrictStr] = None
+
+
+class SecondaryExternalAccount(BaseModel):
+    external_account_id: Optional[StrictStr] = None
+    external_type: Optional[StrictStr] = None
```

### Comparing `vantage_sdk-0.7.0/vantage_sdk/model/search.py` & `vantage_sdk-0.8.0/vantage_sdk/model/search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.7.0/PKG-INFO` & `vantage_sdk-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: Vantage Python SDK.
 Home-page: https://github.com/VantageDiscovery/vantage-sdk-python
 Author: Vantage
 Author-email: none@vantage.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -46,15 +46,15 @@
 
 # Vantage Discovery Python SDK
 
 The Vantage Discovery Python SDK provides an easy-to-use interface to interact with the Vantage vector database, enabling developers to seamlessly integrate vector search and collection management capabilities into their Python applications.
 
 ## Installation
 
-To install the Vantage Python SDK, run the following command:
+To install the [Vantage Python SDK](https://pypi.org/project/vantage-sdk/), run the following command:
 
 ```bash
 pip install vantage-sdk
 ```
 
 ## Quickstart
 
@@ -78,45 +78,79 @@
 
 #### Key Features
 - __Collection Management__: Easily create, update, list, and delete collections.
 - __Documents Upload__: Upload your data easily to your collections.
 - __Search__: Perform semantic, embedding and "more like this/these" searches within your collections.
 - __LLM Keys Management__: Keep your LLM provider secrets safe and up-to-date.
 
-## Examples
+## 🔍 Examples
 
 ### Creating a Collection
 
+To create a new collection for storing documents, specify the collection ID, the dimension of the embeddings, and the LLM (language learning model) details. Here, we use `text-embedding-ada-002` from OpenAI with the necessary secret key. 
+
+📚 Visit [management-api](https://docs.vantagediscovery.com/docs/management-api) documentation for more details.
+
 ```python
-collection = vantage_client.create_collection(
-    collection_id="my_collection",
-    collection_name="My Test Collection",
+collection = OpenAICollection(
+    collection_id="my-collection",
     embeddings_dimension=1536,
     llm="text-embedding-ada-002",
-    external_key_id="YOUR_EXTERNAL_KEY_ID" # Get from Vantage Console UI or using the SDK
+    llm_secret="YOUR_OPENAI_SECRET_KEY",
 )
-print(f"Created collection: {collection.name}")
+
+created_collection = vantage_client.create_collection(collection=collection)
+
+print(f"Created collection: {created_collection.collection_name}")
 ```
 
 ### Uploading Documents
+
+To upload documents to your collection, provide a list of document IDs and corresponding text. Each document is wrapped in a `VantageManagedEmbeddingsDocument` object. This example demonstrates uploading a batch of documents. 
+
+📚 Visit [management-api](https://docs.vantagediscovery.com/docs/management-api) documentation for more details.
+
 ```python
-documents_jsonl = '{"id": "1", "text": "Example text"}\\n{"id": "2", "text": "Another example"}'
-vantage_client.upload_documents_from_jsonl(
-    collection_id="my_collection",
-    documents=documents_jsonl
+ids = [
+    "1",
+    "2",
+    "3",
+    "4",
+]
+
+texts = [
+    "First text",
+    "Second text",
+    "Third text",
+    "Fourth text",
+]
+
+documents = [
+    VantageManagedEmbeddingsDocument(text=text, id=id)
+    for id, text in zip(ids, texts)
+]
+
+instance.upsert_documents(
+    collection_id="my-collection",
+    documents=documents,
 )
 ```
 
 ### Performing a Search
+
+To perform a semantic search within your collection, specify the text you want to find similar documents for. This example retrieves documents similar to the provided text, printing out each document's ID and its similarity score. 
+
+📚 Visit [search-api](https://docs.vantagediscovery.com/docs/search-api) documentation for more details.
+
 ```python
 search_result = vantage_client.semantic_search(
     text="Find documents similar to this text",
-    collection_id="my_collection"
+    collection_id="my-collection"
 )
 for result in search_result.results:
     print(result.id, result.score)
 ```
 
-## Documentation
+## 📚 Documentation
 
 For detailed documentation on all methods and their parameters, please refer to the [Vantage Discovery official documentation](https://docs.vantagediscovery.com/docs/concepts).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


# Comparing `tmp/pinecone_client-4.0.0.tar.gz` & `tmp/pinecone_client-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_client-4.0.0.tar", max compression
+gzip compressed data, was "pinecone_client-4.1.0.tar", max compression
```

## Comparing `pinecone_client-4.0.0.tar` & `pinecone_client-4.1.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
--rw-r--r--   0        0        0    11356 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/LICENSE.txt
--rw-r--r--   0        0        0    14522 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/README.md
--rw-r--r--   0        0        0      394 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/__init__.py
--rw-r--r--   0        0        0        5 2024-05-01 03:31:12.978757 pinecone_client-4.0.0/pinecone/__version__
--rw-r--r--   0        0        0      199 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/config.py
--rw-r--r--   0        0        0     4258 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/openapi.py
--rw-r--r--   0        0        0      934 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/pinecone_config.py
--rw-r--r--   0        0        0       30 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/index_host_store.py
--rw-r--r--   0        0        0    24453 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/pinecone.py
--rw-r--r--   0        0        0        0 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/__init__.py
--rw-r--r--   0        0        0      907 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/client/__init__.py
--rw-r--r--   0        0        0      226 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/client/api/__init__.py
--rw-r--r--   0        0        0    44178 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api/data_plane_api.py
--rw-r--r--   0        0        0    42885 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api/manage_indexes_api.py
--rw-r--r--   0        0        0    37006 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17137 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/configuration.py
--rw-r--r--   0        0        0     5270 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/__init__.py
--rw-r--r--   0        0        0    11433 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/collection_list.py
--rw-r--r--   0        0        0    13032 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/collection_model.py
--rw-r--r--   0        0        0    11527 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request.py
--rw-r--r--   0        0        0    11550 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec.py
--rw-r--r--   0        0        0    12263 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec_pod.py
--rw-r--r--   0        0        0    12063 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0        0        0    13925 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/create_index_request.py
--rw-r--r--   0        0        0    12887 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/delete_request.py
--rw-r--r--   0        0        0    11726 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0        0        0    12925 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0        0        0    11746 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/error_response.py
--rw-r--r--   0        0        0    12829 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/error_response_error.py
--rw-r--r--   0        0        0    11910 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0        0        0    11363 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_list.py
--rw-r--r--   0        0        0    14018 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model.py
--rw-r--r--   0        0        0    11695 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model_spec.py
--rw-r--r--   0        0        0    11825 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model_status.py
--rw-r--r--   0        0        0    11137 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/list_item.py
--rw-r--r--   0        0        0    12233 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/list_response.py
--rw-r--r--   0        0        0    11542 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0        0        0    11153 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pagination.py
--rw-r--r--   0        0        0    14766 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pod_spec.py
--rw-r--r--   0        0        0    11495 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pod_spec_metadata_config.py
--rw-r--r--   0        0        0    11358 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0        0        0    12395 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0        0        0    15451 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_request.py
--rw-r--r--   0        0        0    12553 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_response.py
--rw-r--r--   0        0        0    13170 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_vector.py
--rw-r--r--   0        0        0    11741 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0        0        0    12974 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0        0        0    12063 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/serverless_spec.py
--rw-r--r--   0        0        0    11731 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0        0        0    11533 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0        0        0    12778 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/update_request.py
--rw-r--r--   0        0        0    11918 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0        0        0    11280 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0        0        0    11275 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/usage.py
--rw-r--r--   0        0        0    12589 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/vector.py
--rw-r--r--   0        0        0    80537 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model_utils.py
--rw-r--r--   0        0        0     3104 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/models/__init__.py
--rw-r--r--   0        0        0    14204 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/rest.py
--rw-r--r--   0        0        0    26761 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0        0        0    30075 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.pyi
--rw-r--r--   0        0        0    14276 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0      291 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/data/__init__.py
--rw-r--r--   0        0        0     2125 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/data/errors.py
--rw-r--r--   0        0        0    27458 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/index.py
--rw-r--r--   0        0        0     1730 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/sparse_vector_factory.py
--rw-r--r--   0        0        0     2815 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/vector_factory.py
--rw-r--r--   0        0        0     4027 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/deprecation_warnings.py
--rw-r--r--   0        0        0     1033 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/exceptions.py
--rw-r--r--   0        0        0     1300 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/__init__.py
--rw-r--r--   0        0        0     5875 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/base.py
--rw-r--r--   0        0        0     1728 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/config.py
--rw-r--r--   0        0        0      961 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/future.py
--rw-r--r--   0        0        0    28020 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/index_grpc.py
--rw-r--r--   0        0        0     4166 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/pinecone.py
--rw-r--r--   0        0        0     3193 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/retry.py
--rw-r--r--   0        0        0     2000 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/sparse_values_factory.py
--rw-r--r--   0        0        0     2996 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/utils.py
--rw-r--r--   0        0        0     4220 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/vector_factory_grpc.py
--rw-r--r--   0        0        0      534 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/__init__.py
--rw-r--r--   0        0        0      277 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/collection_description.py
--rw-r--r--   0        0        0      852 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/collection_list.py
--rw-r--r--   0        0        0     1330 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/index_description.py
--rw-r--r--   0        0        0      718 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/index_list.py
--rw-r--r--   0        0        0      198 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/list_response.py
--rw-r--r--   0        0        0     2189 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/pod_spec.py
--rw-r--r--   0        0        0      164 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/serverless_spec.py
--rw-r--r--   0        0        0      348 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/__init__.py
--rw-r--r--   0        0        0      288 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/check_kwargs.py
--rw-r--r--   0        0        0      722 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/constants.py
--rw-r--r--   0        0        0      785 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/convert_to_list.py
--rw-r--r--   0        0        0      263 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/deprecation_notice.py
--rw-r--r--   0        0        0      750 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/error_handling.py
--rw-r--r--   0        0        0      193 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/fix_tuple_length.py
--rw-r--r--   0        0        0      206 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/normalize_host.py
--rw-r--r--   0        0        0      527 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/setup_openapi_client.py
--rw-r--r--   0        0        0     1011 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/user_agent.py
--rw-r--r--   0        0        0      157 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/version.py
--rw-r--r--   0        0        0     3266 2024-05-01 03:40:20.894214 pinecone_client-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    16625 1970-01-01 00:00:00.000000 pinecone_client-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-13 22:23:59.620042 pinecone_client-4.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    14501 2024-05-13 22:23:59.620042 pinecone_client-4.1.0/README.md
+-rw-r--r--   0        0        0      394 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/__init__.py
+-rw-r--r--   0        0        0        5 2024-05-13 22:23:59.696043 pinecone_client-4.1.0/pinecone/__version__
+-rw-r--r--   0        0        0      199 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/config/config.py
+-rw-r--r--   0        0        0     4258 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/config/openapi.py
+-rw-r--r--   0        0        0      934 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/config/pinecone_config.py
+-rw-r--r--   0        0        0       30 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/control/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/control/index_host_store.py
+-rw-r--r--   0        0        0      600 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/control/langchain_import_warnings.py
+-rw-r--r--   0        0        0    24826 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/control/pinecone.py
+-rw-r--r--   0        0        0        0 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/__init__.py
+-rw-r--r--   0        0        0      907 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/api/__init__.py
+-rw-r--r--   0        0        0    44178 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/api/data_plane_api.py
+-rw-r--r--   0        0        0    42885 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/api/manage_indexes_api.py
+-rw-r--r--   0        0        0    37006 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17137 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/configuration.py
+-rw-r--r--   0        0        0     5270 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11433 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/collection_list.py
+-rw-r--r--   0        0        0    13032 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/collection_model.py
+-rw-r--r--   0        0        0    11527 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request.py
+-rw-r--r--   0        0        0    11550 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request_spec.py
+-rw-r--r--   0        0        0    12263 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request_spec_pod.py
+-rw-r--r--   0        0        0    12063 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0        0        0    13925 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/create_index_request.py
+-rw-r--r--   0        0        0    12887 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0        0        0    11726 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0        0        0    12925 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0        0        0    11746 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/error_response.py
+-rw-r--r--   0        0        0    12829 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/error_response_error.py
+-rw-r--r--   0        0        0    11910 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0        0        0    11363 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/index_list.py
+-rw-r--r--   0        0        0    14018 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/index_model.py
+-rw-r--r--   0        0        0    11695 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/index_model_spec.py
+-rw-r--r--   0        0        0    11825 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/index_model_status.py
+-rw-r--r--   0        0        0    11137 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/list_item.py
+-rw-r--r--   0        0        0    12233 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/list_response.py
+-rw-r--r--   0        0        0    11542 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0        0        0    11153 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/pagination.py
+-rw-r--r--   0        0        0    14766 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/pod_spec.py
+-rw-r--r--   0        0        0    11495 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/pod_spec_metadata_config.py
+-rw-r--r--   0        0        0    11358 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0        0        0    12395 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0        0        0    15451 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/query_request.py
+-rw-r--r--   0        0        0    12553 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/query_response.py
+-rw-r--r--   0        0        0    13170 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0        0        0    11741 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0        0        0    12974 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0        0        0    12063 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/serverless_spec.py
+-rw-r--r--   0        0        0    11731 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0        0        0    11533 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0        0        0    12778 2024-05-13 22:23:59.624042 pinecone_client-4.1.0/pinecone/core/client/model/update_request.py
+-rw-r--r--   0        0        0    11918 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0        0        0    11280 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0        0        0    11275 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/model/usage.py
+-rw-r--r--   0        0        0    12589 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/model/vector.py
+-rw-r--r--   0        0        0    80537 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/model_utils.py
+-rw-r--r--   0        0        0     3104 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14204 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/client/rest.py
+-rw-r--r--   0        0        0    26761 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0        0        0    30075 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    14276 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0      291 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/data/__init__.py
+-rw-r--r--   0        0        0     2125 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/data/errors.py
+-rw-r--r--   0        0        0    27458 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/data/index.py
+-rw-r--r--   0        0        0     1730 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/data/sparse_vector_factory.py
+-rw-r--r--   0        0        0     2815 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/data/vector_factory.py
+-rw-r--r--   0        0        0     4027 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/deprecation_warnings.py
+-rw-r--r--   0        0        0     1033 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/exceptions.py
+-rw-r--r--   0        0        0     1300 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/__init__.py
+-rw-r--r--   0        0        0     6070 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/base.py
+-rw-r--r--   0        0        0     1728 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/config.py
+-rw-r--r--   0        0        0      961 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/future.py
+-rw-r--r--   0        0        0    28020 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/index_grpc.py
+-rw-r--r--   0        0        0     4312 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/pinecone.py
+-rw-r--r--   0        0        0     3193 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/retry.py
+-rw-r--r--   0        0        0     2000 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/sparse_values_factory.py
+-rw-r--r--   0        0        0     2996 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/utils.py
+-rw-r--r--   0        0        0     4220 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/grpc/vector_factory_grpc.py
+-rw-r--r--   0        0        0      534 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/collection_description.py
+-rw-r--r--   0        0        0      852 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/collection_list.py
+-rw-r--r--   0        0        0     1330 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/index_description.py
+-rw-r--r--   0        0        0      718 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/index_list.py
+-rw-r--r--   0        0        0      198 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/list_response.py
+-rw-r--r--   0        0        0     2189 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/pod_spec.py
+-rw-r--r--   0        0        0      164 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/models/serverless_spec.py
+-rw-r--r--   0        0        0      381 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/check_kwargs.py
+-rw-r--r--   0        0        0      722 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/constants.py
+-rw-r--r--   0        0        0      785 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/convert_to_list.py
+-rw-r--r--   0        0        0      263 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/deprecation_notice.py
+-rw-r--r--   0        0        0      210 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/docslinks.py
+-rw-r--r--   0        0        0      750 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/error_handling.py
+-rw-r--r--   0        0        0      193 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/fix_tuple_length.py
+-rw-r--r--   0        0        0      206 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/normalize_host.py
+-rw-r--r--   0        0        0      527 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/setup_openapi_client.py
+-rw-r--r--   0        0        0     1011 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/user_agent.py
+-rw-r--r--   0        0        0      157 2024-05-13 22:23:59.628043 pinecone_client-4.1.0/pinecone/utils/version.py
+-rw-r--r--   0        0        0     3266 2024-05-13 22:32:58.150294 pinecone_client-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16604 1970-01-01 00:00:00.000000 pinecone_client-4.1.0/PKG-INFO
```

### Comparing `pinecone_client-4.0.0/LICENSE.txt` & `pinecone_client-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/README.md` & `pinecone_client-4.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 pc = Pinecone(api_key=os.environ.get('CUSTOM_VAR'))
 ```
 
 ### Proxy configuration
 
 If your network setup requires you to interact with Pinecone via a proxy, you will need
-to pass additional configuration using optional keyword parameters. These optional parameters are forwarded to `urllib3`, which is the underlying library currently used by the Pinecone client to make HTTP requests. You may find it helpful to refer to the  [urllib3 documentation on working with proxies](https://urllib3.readthedocs.io/en/stable/advanced-usage.html#http-and-https-proxies) while troubleshooting these settings. 
+to pass additional configuration using optional keyword parameters. These optional parameters are forwarded to `urllib3`, which is the underlying library currently used by the Pinecone client to make HTTP requests. You may find it helpful to refer to the [urllib3 documentation on working with proxies](https://urllib3.readthedocs.io/en/stable/advanced-usage.html#http-and-https-proxies) while troubleshooting these settings.
 
 Here is a basic example:
 
 ```python
 from pinecone import Pinecone
 
 pc = Pinecone(
@@ -118,15 +118,15 @@
 )
 
 pc.list_indexes()
 ```
 
 ### Using proxies with self-signed certificates
 
-By default the Pinecone Python client will perform SSL certificate verification 
+By default the Pinecone Python client will perform SSL certificate verification
 using the CA bundle maintained by Mozilla in the [certifi](https://pypi.org/project/certifi/) package.
 
 If your proxy server is using a self-signed certificate, you will need to pass the path to the certificate in PEM format using the `ssl_ca_certs` parameter.
 
 ```python
 from pinecone import Pinecone
 import urllib3 import make_headers
@@ -139,15 +139,15 @@
 )
 
 pc.list_indexes()
 ```
 
 ### Disabling SSL verification
 
-If you would like to disable SSL verification, you can pass the `ssl_verify` 
+If you would like to disable SSL verification, you can pass the `ssl_verify`
 parameter with a value of `False`. We do not recommend going to production with SSL verification disabled.
 
 ```python
 from pinecone import Pinecone
 import urllib3 import make_headers
 
 pc = Pinecone(
@@ -181,17 +181,16 @@
 
 # Indexes
 
 ## Create Index
 
 ### Create a serverless index
 
-> [!WARNING]  
-> Serverless indexes are in **public preview** and are available only on AWS in the
-> `us-west-2` region. Check the [current limitations](https://docs.pinecone.io/docs/limits#serverless-index-limitations) and test thoroughly before using it in production.
+The following example creates a serverless index in the `us-west-2`
+region of AWS. For more information on serverless and regional availability, see [Understanding indexes](https://docs.pinecone.io/guides/indexes/understanding-indexes#serverless-indexes).
 
 ```python
 from pinecone import Pinecone, ServerlessSpec
 
 pc = Pinecone(api_key='<<PINECONE_API_KEY>>')
 pc.create_index(
     name='my-index',
@@ -412,17 +411,17 @@
     set_metadata={"genre": "drama"},
     namespace="example-namespace"
 )
 ```
 
 ## List vectors
 
-The `list` and `list_paginated` methods can be used to list vector ids matching a particular id prefix. 
+The `list` and `list_paginated` methods can be used to list vector ids matching a particular id prefix.
 With clever assignment of vector ids, this can be used to help model hierarchical relationships between
-different vectors such as when there are embeddings for multiple chunks or fragments related to the 
+different vectors such as when there are embeddings for multiple chunks or fragments related to the
 same document.
 
 The `list` method returns a generator that handles pagination on your behalf.
 
 ```python
 from pinecone import Pinecone
```

### Comparing `pinecone_client-4.0.0/pinecone/config/config.py` & `pinecone_client-4.1.0/pinecone/config/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/config/openapi.py` & `pinecone_client-4.1.0/pinecone/config/openapi.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/config/pinecone_config.py` & `pinecone_client-4.1.0/pinecone/config/pinecone_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/control/index_host_store.py` & `pinecone_client-4.1.0/pinecone/control/index_host_store.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/control/pinecone.py` & `pinecone_client-4.1.0/pinecone/control/pinecone.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CreateCollectionRequest,
     CreateIndexRequest,
     ConfigureIndexRequest,
     ConfigureIndexRequestSpec,
     ConfigureIndexRequestSpecPod
 )
 from pinecone.models import ServerlessSpec, PodSpec, IndexList, CollectionList
+from .langchain_import_warnings import _build_langchain_attribute_error_message
 
 from pinecone.data import Index
 
 class Pinecone:
 
     def __init__(
         self,
@@ -541,14 +542,21 @@
         return api_instance.describe_collection(name).to_dict()
 
     def _get_status(self, name: str):
         api_instance = self.index_api
         response = api_instance.describe_index(name)
         return response["status"]
 
+    @staticmethod
+    def from_texts(*args, **kwargs):
+        raise AttributeError(_build_langchain_attribute_error_message("from_texts"))
+    
+    @staticmethod
+    def from_documents(*args, **kwargs):
+        raise AttributeError(_build_langchain_attribute_error_message("from_documents"))
 
     def Index(self, name: str = '', host: str = '', **kwargs):
         """
         Target an index for data operations.
 
         ### Target an index by host url
```

### Comparing `pinecone_client-4.0.0/pinecone/core/client/__init__.py` & `pinecone_client-4.1.0/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/api/data_plane_api.py` & `pinecone_client-4.1.0/pinecone/core/client/api/data_plane_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/api/manage_indexes_api.py` & `pinecone_client-4.1.0/pinecone/core/client/api/manage_indexes_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/api_client.py` & `pinecone_client-4.1.0/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/apis/__init__.py` & `pinecone_client-4.1.0/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/configuration.py` & `pinecone_client-4.1.0/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/exceptions.py` & `pinecone_client-4.1.0/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/collection_list.py` & `pinecone_client-4.1.0/pinecone/core/client/model/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/collection_model.py` & `pinecone_client-4.1.0/pinecone/core/client/model/collection_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec.py` & `pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec_pod.py` & `pinecone_client-4.1.0/pinecone/core/client/model/configure_index_request_spec_pod.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/create_collection_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/create_index_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/create_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/delete_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/error_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/error_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/error_response_error.py` & `pinecone_client-4.1.0/pinecone/core/client/model/error_response_error.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/fetch_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/index_list.py` & `pinecone_client-4.1.0/pinecone/core/client/model/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/index_model.py` & `pinecone_client-4.1.0/pinecone/core/client/model/index_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/index_model_spec.py` & `pinecone_client-4.1.0/pinecone/core/client/model/index_model_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/index_model_status.py` & `pinecone_client-4.1.0/pinecone/core/client/model/index_model_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/list_item.py` & `pinecone_client-4.1.0/pinecone/core/client/model/list_item.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/list_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/list_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/namespace_summary.py` & `pinecone_client-4.1.0/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/pagination.py` & `pinecone_client-4.1.0/pinecone/core/client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/pod_spec.py` & `pinecone_client-4.1.0/pinecone/core/client/model/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/pod_spec_metadata_config.py` & `pinecone_client-4.1.0/pinecone/core/client/model/pod_spec_metadata_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/protobuf_any.py` & `pinecone_client-4.1.0/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/protobuf_null_value.py` & `pinecone_client-4.1.0/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/query_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/query_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/query_vector.py` & `pinecone_client-4.1.0/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/rpc_status.py` & `pinecone_client-4.1.0/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/scored_vector.py` & `pinecone_client-4.1.0/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/serverless_spec.py` & `pinecone_client-4.1.0/pinecone/core/client/model/serverless_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/single_query_results.py` & `pinecone_client-4.1.0/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/sparse_values.py` & `pinecone_client-4.1.0/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/update_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/upsert_request.py` & `pinecone_client-4.1.0/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/upsert_response.py` & `pinecone_client-4.1.0/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/usage.py` & `pinecone_client-4.1.0/pinecone/core/client/model/usage.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model/vector.py` & `pinecone_client-4.1.0/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/model_utils.py` & `pinecone_client-4.1.0/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/models/__init__.py` & `pinecone_client-4.1.0/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/client/rest.py` & `pinecone_client-4.1.0/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.py` & `pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.pyi` & `pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `pinecone_client-4.1.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/data/errors.py` & `pinecone_client-4.1.0/pinecone/data/errors.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/data/index.py` & `pinecone_client-4.1.0/pinecone/data/index.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/data/sparse_vector_factory.py` & `pinecone_client-4.1.0/pinecone/data/sparse_vector_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/data/vector_factory.py` & `pinecone_client-4.1.0/pinecone/data/vector_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/deprecation_warnings.py` & `pinecone_client-4.1.0/pinecone/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/exceptions.py` & `pinecone_client-4.1.0/pinecone/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/__init__.py` & `pinecone_client-4.1.0/pinecone/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/base.py` & `pinecone_client-4.1.0/pinecone/grpc/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,23 +97,26 @@
             "grpc.max_send_message_length": MAX_MSG_SIZE,
             "grpc.max_receive_message_length": MAX_MSG_SIZE,
             "grpc.service_config": self.method_config,
             "grpc.enable_retries": True,
         }
         if self.grpc_client_config.secure:
             default_options["grpc.ssl_target_name_override"] = target.split(":")[0]
+        if self.config.proxy_url:
+            default_options["grpc.http_proxy"] = self.config.proxy_url
         user_provided_options = options or {}
         _options = tuple((k, v) for k, v in {**default_options, **user_provided_options}.items())
         _logger.debug(
             "creating new channel with endpoint %s options %s and config %s", target, _options, self.grpc_client_config
         )
         if not self.grpc_client_config.secure:
             channel = grpc.insecure_channel(target, options=_options)
         else:
-            root_cas = open(certifi.where(), "rb").read()
+            ca_certs = self.config.ssl_ca_certs if self.config.ssl_ca_certs else certifi.where()
+            root_cas = open(ca_certs, "rb").read()
             tls = grpc.ssl_channel_credentials(root_certificates=root_cas)
             channel = grpc.secure_channel(target, tls, options=_options)
 
         return channel
 
     @property
     def channel(self):
```

### Comparing `pinecone_client-4.0.0/pinecone/grpc/config.py` & `pinecone_client-4.1.0/pinecone/grpc/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/future.py` & `pinecone_client-4.1.0/pinecone/grpc/future.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/index_grpc.py` & `pinecone_client-4.1.0/pinecone/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/pinecone.py` & `pinecone_client-4.1.0/pinecone/grpc/pinecone.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,9 +121,11 @@
             raise ValueError("Either name or host must be specified")
 
         # Use host if it is provided, otherwise get host from describe_index
         index_host = host or self.index_host_store.get_host(self.index_api, self.config, name)
 
         config = ConfigBuilder.build(api_key=self.config.api_key,
                                      host=index_host,
-                                     source_tag=self.config.source_tag)
+                                     source_tag=self.config.source_tag,
+                                     proxy_url=self.config.proxy_url,
+                                     ssl_ca_certs=self.config.ssl_ca_certs)
         return GRPCIndex(index_name=name, config=config, **kwargs)
```

### Comparing `pinecone_client-4.0.0/pinecone/grpc/retry.py` & `pinecone_client-4.1.0/pinecone/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/sparse_values_factory.py` & `pinecone_client-4.1.0/pinecone/grpc/sparse_values_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/utils.py` & `pinecone_client-4.1.0/pinecone/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/grpc/vector_factory_grpc.py` & `pinecone_client-4.1.0/pinecone/grpc/vector_factory_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/models/__init__.py` & `pinecone_client-4.1.0/pinecone/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/models/collection_list.py` & `pinecone_client-4.1.0/pinecone/models/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/models/index_description.py` & `pinecone_client-4.1.0/pinecone/models/index_description.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/models/index_list.py` & `pinecone_client-4.1.0/pinecone/models/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/models/pod_spec.py` & `pinecone_client-4.1.0/pinecone/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/utils/constants.py` & `pinecone_client-4.1.0/pinecone/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/utils/convert_to_list.py` & `pinecone_client-4.1.0/pinecone/utils/convert_to_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/utils/error_handling.py` & `pinecone_client-4.1.0/pinecone/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/utils/setup_openapi_client.py` & `pinecone_client-4.1.0/pinecone/utils/setup_openapi_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pinecone/utils/user_agent.py` & `pinecone_client-4.1.0/pinecone/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-4.0.0/pyproject.toml` & `pinecone_client-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "pinecone-client"
-version = "4.0.0"
+version = "4.1.0"
 packages = [
     { include="pinecone", from="." },
 ]
 description = "Pinecone client and SDK"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pinecone_client-4.0.0/PKG-INFO` & `pinecone_client-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-client
-Version: 4.0.0
+Version: 4.1.0
 Summary: Pinecone client and SDK
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Keywords: Pinecone,vector,database,cloud
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.8,<4.0
@@ -129,15 +129,15 @@
 
 pc = Pinecone(api_key=os.environ.get('CUSTOM_VAR'))
 ```
 
 ### Proxy configuration
 
 If your network setup requires you to interact with Pinecone via a proxy, you will need
-to pass additional configuration using optional keyword parameters. These optional parameters are forwarded to `urllib3`, which is the underlying library currently used by the Pinecone client to make HTTP requests. You may find it helpful to refer to the  [urllib3 documentation on working with proxies](https://urllib3.readthedocs.io/en/stable/advanced-usage.html#http-and-https-proxies) while troubleshooting these settings. 
+to pass additional configuration using optional keyword parameters. These optional parameters are forwarded to `urllib3`, which is the underlying library currently used by the Pinecone client to make HTTP requests. You may find it helpful to refer to the [urllib3 documentation on working with proxies](https://urllib3.readthedocs.io/en/stable/advanced-usage.html#http-and-https-proxies) while troubleshooting these settings.
 
 Here is a basic example:
 
 ```python
 from pinecone import Pinecone
 
 pc = Pinecone(
@@ -161,15 +161,15 @@
 )
 
 pc.list_indexes()
 ```
 
 ### Using proxies with self-signed certificates
 
-By default the Pinecone Python client will perform SSL certificate verification 
+By default the Pinecone Python client will perform SSL certificate verification
 using the CA bundle maintained by Mozilla in the [certifi](https://pypi.org/project/certifi/) package.
 
 If your proxy server is using a self-signed certificate, you will need to pass the path to the certificate in PEM format using the `ssl_ca_certs` parameter.
 
 ```python
 from pinecone import Pinecone
 import urllib3 import make_headers
@@ -182,15 +182,15 @@
 )
 
 pc.list_indexes()
 ```
 
 ### Disabling SSL verification
 
-If you would like to disable SSL verification, you can pass the `ssl_verify` 
+If you would like to disable SSL verification, you can pass the `ssl_verify`
 parameter with a value of `False`. We do not recommend going to production with SSL verification disabled.
 
 ```python
 from pinecone import Pinecone
 import urllib3 import make_headers
 
 pc = Pinecone(
@@ -224,17 +224,16 @@
 
 # Indexes
 
 ## Create Index
 
 ### Create a serverless index
 
-> [!WARNING]  
-> Serverless indexes are in **public preview** and are available only on AWS in the
-> `us-west-2` region. Check the [current limitations](https://docs.pinecone.io/docs/limits#serverless-index-limitations) and test thoroughly before using it in production.
+The following example creates a serverless index in the `us-west-2`
+region of AWS. For more information on serverless and regional availability, see [Understanding indexes](https://docs.pinecone.io/guides/indexes/understanding-indexes#serverless-indexes).
 
 ```python
 from pinecone import Pinecone, ServerlessSpec
 
 pc = Pinecone(api_key='<<PINECONE_API_KEY>>')
 pc.create_index(
     name='my-index',
@@ -455,17 +454,17 @@
     set_metadata={"genre": "drama"},
     namespace="example-namespace"
 )
 ```
 
 ## List vectors
 
-The `list` and `list_paginated` methods can be used to list vector ids matching a particular id prefix. 
+The `list` and `list_paginated` methods can be used to list vector ids matching a particular id prefix.
 With clever assignment of vector ids, this can be used to help model hierarchical relationships between
-different vectors such as when there are embeddings for multiple chunks or fragments related to the 
+different vectors such as when there are embeddings for multiple chunks or fragments related to the
 same document.
 
 The `list` method returns a generator that handles pagination on your behalf.
 
 ```python
 from pinecone import Pinecone
```


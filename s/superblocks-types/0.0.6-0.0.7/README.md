# Comparing `tmp/superblocks-types-0.0.6.tar.gz` & `tmp/superblocks-types-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.6.tar", last modified: Mon May 13 15:02:42 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.7.tar", last modified: Tue May 14 13:08:59 2024, max compression
```

## Comparing `superblocks-types-0.0.6.tar` & `superblocks-types-0.0.7.tar`

### file list

```diff
@@ -1,424 +1,425 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.082513 superblocks-types-0.0.6/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 15:02:42.082352 superblocks-types-0.0.6/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.6/README.md
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.015854 superblocks-types-0.0.6/gen/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.015945 superblocks-types-0.0.6/gen/py/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.030243 superblocks-types-0.0.6/gen/py/superblocks_types/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.031350 superblocks-types-0.0.6/gen/py/superblocks_types/agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.031996 superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11149 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4565 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.032206 superblocks-types-0.0.6/gen/py/superblocks_types/ai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.034001 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8400 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/ai_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/ai_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3053 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4325 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5300 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/vector_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/vector_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.034202 superblocks-types-0.0.6/gen/py/superblocks_types/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.036930 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    39242 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2900 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/blocks_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/blocks_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7262 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8593 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10701 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7444 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    27119 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    28883 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.037156 superblocks-types-0.0.6/gen/py/superblocks_types/auth/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/auth/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.037598 superblocks-types-0.0.6/gen/py/superblocks_types/auth/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/auth/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/auth/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/auth/v1/auth_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.037754 superblocks-types-0.0.6/gen/py/superblocks_types/buf/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.038638 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/expression_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.039099 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/priv/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/priv/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/priv/private_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)   136639 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.039256 superblocks-types-0.0.6/gen/py/superblocks_types/cache/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/cache/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.039663 superblocks-types-0.0.6/gen/py/superblocks_types/cache/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/cache/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/cache/v1/cache_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/cache/v1/cache_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.039831 superblocks-types-0.0.6/gen/py/superblocks_types/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.042139 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3864 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/common_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/common_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/errors_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/errors_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/health_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/health_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/language_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/language_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/plugin_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.042297 superblocks-types-0.0.6/gen/py/superblocks_types/event/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.043330 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5954 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.044059 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.044215 superblocks-types-0.0.6/gen/py/superblocks_types/google/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.045006 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1591 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/http_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.045163 superblocks-types-0.0.6/gen/py/superblocks_types/intake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/intake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.045606 superblocks-types-0.0.6/gen/py/superblocks_types/intake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/intake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/intake/v1/logs_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/intake/v1/logs_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.045787 superblocks-types-0.0.6/gen/py/superblocks_types/integration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/integration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.046309 superblocks-types-0.0.6/gen/py/superblocks_types/integration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/integration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3690 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/integration/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/integration/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.046480 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.046961 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/v1/kafka_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/kafka/v1/kafka_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.047148 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.047306 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.047795 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5374 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.048020 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.048574 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2940 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.048775 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.049304 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.049498 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.050028 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.050233 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.051519 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/auth_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6530 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.051724 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.052210 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6310 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.052401 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.052904 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4120 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.053100 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.053555 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.053737 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.054181 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2601 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.054360 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.055089 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.055350 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.055940 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.056164 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.056764 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.056959 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.057472 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2008 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.057697 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.058192 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.058409 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.058896 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.059082 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.059611 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     9925 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.059779 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.060263 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.060435 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.060893 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.061079 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.061569 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.061765 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.062226 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.062395 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.062842 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.063006 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.063450 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.063610 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.064038 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2461 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.064199 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.064620 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3186 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.064779 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.065218 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.065382 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.065849 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.066015 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.066561 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13989 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.066737 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.067209 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.067394 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.067866 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2103 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.068021 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.068472 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2509 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.068628 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.069042 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.069209 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.069650 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.069824 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.070280 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5293 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.070469 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.070917 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2551 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.071094 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.071687 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.071982 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.072504 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2680 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.073013 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1462 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.073180 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.074065 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2316 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.074260 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.075124 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7599 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/secrets_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/secrets_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4880 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.075312 superblocks-types-0.0.6/gen/py/superblocks_types/security/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.076063 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3141 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4830 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4519 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.076220 superblocks-types-0.0.6/gen/py/superblocks_types/store/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.077079 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3608 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4413 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1671 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.077239 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.077683 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/v1/options_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.078563 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 15:02:41.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)    16226 2024-05-13 15:02:41.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 15:02:41.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)      176 2024-05-13 15:02:41.000000 superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.078731 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.079572 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8935 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11806 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3390 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/syncer_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.079756 superblocks-types-0.0.6/gen/py/superblocks_types/transport/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/transport/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.080312 superblocks-types-0.0.6/gen/py/superblocks_types/transport/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/transport/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13244 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/transport/v1/transport_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/transport/v1/transport_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.080485 superblocks-types-0.0.6/gen/py/superblocks_types/utils/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/utils/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.080915 superblocks-types-0.0.6/gen/py/superblocks_types/utils/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/utils/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/utils/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/utils/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.081456 superblocks-types-0.0.6/gen/py/superblocks_types/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.081633 superblocks-types-0.0.6/gen/py/superblocks_types/worker/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/worker/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:02:42.082070 superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1980 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/step_executor_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10056 2024-05-13 15:01:55.000000 superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 15:02:42.082579 superblocks-types-0.0.6/setup.cfg
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.647208 superblocks-types-0.0.7/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:08:59.646986 superblocks-types-0.0.7/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.7/README.md
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.569200 superblocks-types-0.0.7/gen/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.569404 superblocks-types-0.0.7/gen/py/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.584973 superblocks-types-0.0.7/gen/py/superblocks_types/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.586101 superblocks-types-0.0.7/gen/py/superblocks_types/agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.586818 superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11149 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4565 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.587050 superblocks-types-0.0.7/gen/py/superblocks_types/ai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.588784 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8400 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/ai_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/ai_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3053 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4325 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5300 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/vector_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/vector_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.588958 superblocks-types-0.0.7/gen/py/superblocks_types/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.592091 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    39242 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2900 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/blocks_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/blocks_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7262 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8593 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10701 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7444 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    27119 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    28883 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.592382 superblocks-types-0.0.7/gen/py/superblocks_types/auth/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/auth/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.592893 superblocks-types-0.0.7/gen/py/superblocks_types/auth/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/auth/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/auth/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/auth/v1/auth_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.593098 superblocks-types-0.0.7/gen/py/superblocks_types/buf/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.594275 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/expression_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.595100 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/priv/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/priv/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)   136639 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.595340 superblocks-types-0.0.7/gen/py/superblocks_types/cache/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/cache/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.595927 superblocks-types-0.0.7/gen/py/superblocks_types/cache/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/cache/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/cache/v1/cache_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/cache/v1/cache_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.596121 superblocks-types-0.0.7/gen/py/superblocks_types/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.599390 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3864 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/common_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/common_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/errors_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/errors_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/health_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/health_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/language_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/language_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/plugin_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.599583 superblocks-types-0.0.7/gen/py/superblocks_types/event/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.600987 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5954 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.601878 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.602076 superblocks-types-0.0.7/gen/py/superblocks_types/google/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.603003 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1591 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/http_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.603214 superblocks-types-0.0.7/gen/py/superblocks_types/intake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/intake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.603728 superblocks-types-0.0.7/gen/py/superblocks_types/intake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/intake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/intake/v1/logs_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/intake/v1/logs_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.604161 superblocks-types-0.0.7/gen/py/superblocks_types/integration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/integration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.604822 superblocks-types-0.0.7/gen/py/superblocks_types/integration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/integration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3690 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/integration/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/integration/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.605035 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.605641 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/v1/kafka_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/kafka/v1/kafka_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.605935 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.606126 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.606684 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5374 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.606914 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.607513 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2940 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.607733 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.608364 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.608570 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.609228 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.609441 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.610772 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/auth_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6530 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.610970 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.611531 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6310 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.611734 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.612259 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4120 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.612446 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.614168 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.614423 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.614977 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2601 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.615202 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.615749 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.616249 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.616816 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.617052 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.617664 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.617862 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.618541 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2008 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.618731 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.619353 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.619561 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.620132 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.620327 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.620909 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     9925 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.621132 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.621670 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.621877 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.622401 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.622623 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.623176 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.623650 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.624300 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.624568 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.625148 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.625348 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.625866 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.626189 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.626911 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2461 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.627163 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.627713 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3186 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.627910 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.628521 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.628740 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.629358 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.629594 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.630306 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13989 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.630530 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.631101 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.631339 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.631895 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2103 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.632066 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.632545 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2509 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.632727 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.633386 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.633583 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.634117 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.634324 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.634881 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5293 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.635102 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.635585 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2551 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.635794 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.636345 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.636564 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.637079 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2680 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.637594 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1462 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.637820 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.638797 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2316 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.638993 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.639846 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7599 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/secrets_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/secrets_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4880 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.640047 superblocks-types-0.0.7/gen/py/superblocks_types/security/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.640932 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3141 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4830 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4519 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.641128 superblocks-types-0.0.7/gen/py/superblocks_types/store/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.641985 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3608 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4413 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1671 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.642189 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.642674 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/v1/options_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.642874 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.643749 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8935 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11806 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3390 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/syncer_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.643947 superblocks-types-0.0.7/gen/py/superblocks_types/transport/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/transport/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.644522 superblocks-types-0.0.7/gen/py/superblocks_types/transport/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/transport/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13244 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/transport/v1/transport_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/transport/v1/transport_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.644719 superblocks-types-0.0.7/gen/py/superblocks_types/utils/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/utils/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.645210 superblocks-types-0.0.7/gen/py/superblocks_types/utils/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/utils/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/utils/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/utils/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.645832 superblocks-types-0.0.7/gen/py/superblocks_types/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.646019 superblocks-types-0.0.7/gen/py/superblocks_types/worker/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/worker/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.646546 superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1980 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/step_executor_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10056 2024-05-14 13:06:42.000000 superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:08:59.585885 superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:08:59.000000 superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)    16191 2024-05-14 13:08:59.000000 superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-14 13:08:59.000000 superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       18 2024-05-14 13:08:59.000000 superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/top_level.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-14 13:08:59.647312 superblocks-types-0.0.7/setup.cfg
```

### Comparing `superblocks-types-0.0.6/PKG-INFO` & `superblocks-types-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.6/README.md` & `superblocks-types-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/ai_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/ai_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/metadata_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/ai/v1/vector_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/ai/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/api_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/blocks_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/blocks_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/event_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/requests_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/requests_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/api/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/api/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/auth/v1/auth_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/auth/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/expression_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/priv/private_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/buf/validate/validate_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/cache/v1/cache_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/cache/v1/cache_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/api_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/common_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/errors_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/health_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/language_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/language_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/common/v1/utils_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/common/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/cloudevent_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/event_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/cloudevent_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/event/v2/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/event/v2/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/google/api/annotations_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/google/api/http_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/intake/v1/logs_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/intake/v1/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/integration/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/integration/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/kafka/v1/kafka_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/kafka/v1/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/secrets_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/store_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/store_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/requests_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/requests_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/security/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/security/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/store/v1/store_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/store/v1/store_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/superblocks/v1/options_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/superblocks/v1/options_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/PKG-INFO` & `superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/superblocks_types.egg-info/SOURCES.txt` & `superblocks-types-0.0.7/gen/py/superblocks_types.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 README.md
+gen/py/superblocks_types/__init__.py
+gen/py/superblocks_types.egg-info/PKG-INFO
+gen/py/superblocks_types.egg-info/SOURCES.txt
+gen/py/superblocks_types.egg-info/dependency_links.txt
+gen/py/superblocks_types.egg-info/top_level.txt
 gen/py/superblocks_types/agent/__init__.py
 gen/py/superblocks_types/agent/v1/__init__.py
 gen/py/superblocks_types/agent/v1/service_pb2.py
 gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
 gen/py/superblocks_types/ai/__init__.py
 gen/py/superblocks_types/ai/v1/__init__.py
 gen/py/superblocks_types/ai/v1/ai_pb2.py
@@ -267,18 +272,14 @@
 gen/py/superblocks_types/store/v1/service_pb2_grpc.py
 gen/py/superblocks_types/store/v1/store_pb2.py
 gen/py/superblocks_types/store/v1/store_pb2_grpc.py
 gen/py/superblocks_types/superblocks/__init__.py
 gen/py/superblocks_types/superblocks/v1/__init__.py
 gen/py/superblocks_types/superblocks/v1/options_pb2.py
 gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
-gen/py/superblocks_types/superblocks_types.egg-info/PKG-INFO
-gen/py/superblocks_types/superblocks_types.egg-info/SOURCES.txt
-gen/py/superblocks_types/superblocks_types.egg-info/dependency_links.txt
-gen/py/superblocks_types/superblocks_types.egg-info/top_level.txt
 gen/py/superblocks_types/syncer/__init__.py
 gen/py/superblocks_types/syncer/v1/__init__.py
 gen/py/superblocks_types/syncer/v1/service_pb2.py
 gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
 gen/py/superblocks_types/syncer/v1/syncer_pb2.py
 gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
 gen/py/superblocks_types/transport/__init__.py
```

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/service_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/syncer/v1/syncer_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/syncer/v1/syncer_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/transport/v1/transport_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/transport/v1/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/utils/v1/utils_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/utils/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/validate/validate_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/step_executor_pb2.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/step_executor_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.6/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py` & `superblocks-types-0.0.7/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py`

 * *Files identical despite different names*


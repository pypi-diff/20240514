# Comparing `tmp/zep_cloud-1.0.0rc1.tar.gz` & `tmp/zep_cloud-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_cloud-1.0.0rc1.tar", max compression
+gzip compressed data, was "zep_cloud-1.0.1.tar", max compression
```

## Comparing `zep_cloud-1.0.0rc1.tar` & `zep_cloud-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5078 2024-05-08 18:32:22.377254 zep_cloud-1.0.0rc1/README.md
--rw-r--r--   0        0        0      675 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1610 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/__init__.py
--rw-r--r--   0        0        0     6052 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/base_client.py
--rw-r--r--   0        0        0     2188 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/client.py
--rw-r--r--   0        0        0      853 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/api_error.py
--rw-r--r--   0        0        0     1501 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/request_options.py
--rw-r--r--   0        0        0       65 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/document/__init__.py
--rw-r--r--   0        0        0    93354 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/document/client.py
--rw-r--r--   0        0        0      158 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/environment.py
--rw-r--r--   0        0        0      352 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/bad_request_error.py
--rw-r--r--   0        0        0      360 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/internal_server_error.py
--rw-r--r--   0        0        0      354 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/not_found_error.py
--rw-r--r--   0        0        0      358 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/unauthorized_error.py
--rw-r--r--   0        0        0      581 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/document.py
--rw-r--r--   0        0        0      563 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/memory.py
--rw-r--r--   0        0        0      545 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/user.py
--rw-r--r--   0        0        0      186 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/__init__.py
--rw-r--r--   0        0        0      380 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/helpers.py
--rw-r--r--   0        0        0     6905 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/history.py
--rw-r--r--   0        0        0    19893 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/vectorstore.py
--rw-r--r--   0        0        0      153 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/__init__.py
--rw-r--r--   0        0        0   101724 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/client.py
--rw-r--r--   0        0        0      178 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/types/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/types/memory_get_request_memory_type.py
--rw-r--r--   0        0        0        0 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/py.typed
--rw-r--r--   0        0        0     1730 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/__init__.py
--rw-r--r--   0        0        0      872 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/api_error.py
--rw-r--r--   0        0        0     1044 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/classify_session_response.py
--rw-r--r--   0        0        0     1055 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/create_document_request.py
--rw-r--r--   0        0        0     1772 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_collection_response.py
--rw-r--r--   0        0        0     1342 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_response.py
--rw-r--r--   0        0        0     1387 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result.py
--rw-r--r--   0        0        0     1173 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result_page.py
--rw-r--r--   0        0        0     1549 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/memory.py
--rw-r--r--   0        0        0     1155 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/memory_search_result.py
--rw-r--r--   0        0        0     2061 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/message.py
--rw-r--r--   0        0        0     1251 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/message_list_response.py
--rw-r--r--   0        0        0      962 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/models_zep_data_class.py
--rw-r--r--   0        0        0      873 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/question.py
--rw-r--r--   0        0        0      193 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/role_type.py
--rw-r--r--   0        0        0      158 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/search_scope.py
--rw-r--r--   0        0        0      155 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/search_type.py
--rw-r--r--   0        0        0     1564 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/session.py
--rw-r--r--   0        0        0     1023 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/session_list_response.py
--rw-r--r--   0        0        0      879 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/success_response.py
--rw-r--r--   0        0        0     1567 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/summary.py
--rw-r--r--   0        0        0     1019 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/summary_list_response.py
--rw-r--r--   0        0        0     1087 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/update_document_list_request.py
--rw-r--r--   0        0        0     1480 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/user.py
--rw-r--r--   0        0        0     1003 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/user_list_response.py
--rw-r--r--   0        0        0       65 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/user/__init__.py
--rw-r--r--   0        0        0    37852 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/user/client.py
--rw-r--r--   0        0        0       77 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/version.py
--rw-r--r--   0        0        0     5576 1970-01-01 00:00:00.000000 zep_cloud-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     5078 2024-05-14 00:47:42.014451 zep_cloud-1.0.1/README.md
+-rw-r--r--   0        0        0      670 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1610 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/__init__.py
+-rw-r--r--   0        0        0     6052 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/base_client.py
+-rw-r--r--   0        0        0     2188 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/client.py
+-rw-r--r--   0        0        0      853 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/api_error.py
+-rw-r--r--   0        0        0     1501 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/document/__init__.py
+-rw-r--r--   0        0        0    93354 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/document/client.py
+-rw-r--r--   0        0        0      158 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/environment.py
+-rw-r--r--   0        0        0      352 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/errors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/errors/bad_request_error.py
+-rw-r--r--   0        0        0      360 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/errors/internal_server_error.py
+-rw-r--r--   0        0        0      354 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/errors/not_found_error.py
+-rw-r--r--   0        0        0      358 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      581 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/external_clients/document.py
+-rw-r--r--   0        0        0      563 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/external_clients/memory.py
+-rw-r--r--   0        0        0      545 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/external_clients/user.py
+-rw-r--r--   0        0        0      186 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/langchain/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/langchain/helpers.py
+-rw-r--r--   0        0        0     6905 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/langchain/history.py
+-rw-r--r--   0        0        0    19893 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/langchain/vectorstore.py
+-rw-r--r--   0        0        0      153 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/memory/__init__.py
+-rw-r--r--   0        0        0   102256 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/memory/client.py
+-rw-r--r--   0        0        0      178 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/memory/types/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/memory/types/memory_get_request_memory_type.py
+-rw-r--r--   0        0        0        0 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/py.typed
+-rw-r--r--   0        0        0     1730 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/api_error.py
+-rw-r--r--   0        0        0     1044 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/classify_session_response.py
+-rw-r--r--   0        0        0     1055 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/create_document_request.py
+-rw-r--r--   0        0        0     1772 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/document_collection_response.py
+-rw-r--r--   0        0        0     1342 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/document_response.py
+-rw-r--r--   0        0        0     1387 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/document_search_result.py
+-rw-r--r--   0        0        0     1173 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/document_search_result_page.py
+-rw-r--r--   0        0        0     1549 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/memory.py
+-rw-r--r--   0        0        0     1155 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/memory_search_result.py
+-rw-r--r--   0        0        0     2061 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/message.py
+-rw-r--r--   0        0        0     1251 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/message_list_response.py
+-rw-r--r--   0        0        0      962 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/models_zep_data_class.py
+-rw-r--r--   0        0        0      873 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/question.py
+-rw-r--r--   0        0        0      193 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/role_type.py
+-rw-r--r--   0        0        0      158 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/search_scope.py
+-rw-r--r--   0        0        0      155 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/search_type.py
+-rw-r--r--   0        0        0     1564 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/session.py
+-rw-r--r--   0        0        0     1023 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/session_list_response.py
+-rw-r--r--   0        0        0      879 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/success_response.py
+-rw-r--r--   0        0        0     1567 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/summary.py
+-rw-r--r--   0        0        0     1019 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/summary_list_response.py
+-rw-r--r--   0        0        0     1087 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/update_document_list_request.py
+-rw-r--r--   0        0        0     1480 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/user.py
+-rw-r--r--   0        0        0     1003 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/types/user_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/user/__init__.py
+-rw-r--r--   0        0        0    37852 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/user/client.py
+-rw-r--r--   0        0        0       77 2024-05-14 00:47:42.022451 zep_cloud-1.0.1/src/zep_cloud/version.py
+-rw-r--r--   0        0        0     5573 1970-01-01 00:00:00.000000 zep_cloud-1.0.1/PKG-INFO
```

### Comparing `zep_cloud-1.0.0rc1/README.md` & `zep_cloud-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/pyproject.toml` & `zep_cloud-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-cloud"
-version = "1.0.0-rc.1"
+version = "1.0.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "zep_cloud", from = "src"}
 ]
```

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/__init__.py` & `zep_cloud-1.0.1/src/zep_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/base_client.py` & `zep_cloud-1.0.1/src/zep_cloud/base_client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/client.py` & `zep_cloud-1.0.1/src/zep_cloud/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/__init__.py` & `zep_cloud-1.0.1/src/zep_cloud/core/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/client_wrapper.py` & `zep_cloud-1.0.1/src/zep_cloud/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "zep-cloud",
-            "X-Fern-SDK-Version": "1.0.0",
+            "X-Fern-SDK-Version": "1.0.1",
         }
         headers["Authorization"] = f"Api-Key {self.api_key}"
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/datetime_utils.py` & `zep_cloud-1.0.1/src/zep_cloud/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/file.py` & `zep_cloud-1.0.1/src/zep_cloud/core/file.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/http_client.py` & `zep_cloud-1.0.1/src/zep_cloud/core/http_client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/jsonable_encoder.py` & `zep_cloud-1.0.1/src/zep_cloud/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/core/request_options.py` & `zep_cloud-1.0.1/src/zep_cloud/core/request_options.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/document/client.py` & `zep_cloud-1.0.1/src/zep_cloud/document/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/document.py` & `zep_cloud-1.0.1/src/zep_cloud/external_clients/document.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/memory.py` & `zep_cloud-1.0.1/src/zep_cloud/external_clients/memory.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/user.py` & `zep_cloud-1.0.1/src/zep_cloud/external_clients/user.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/langchain/history.py` & `zep_cloud-1.0.1/src/zep_cloud/langchain/history.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/langchain/vectorstore.py` & `zep_cloud-1.0.1/src/zep_cloud/langchain/vectorstore.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/memory/client.py` & `zep_cloud-1.0.1/src/zep_cloud/memory/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,28 +636,32 @@
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def add(
         self,
         session_id: str,
         *,
         messages: typing.Sequence[Message],
+        fact_instruction: typing.Optional[str] = OMIT,
         summary_instruction: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SuccessResponse:
         """
         Add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
 
         messages : typing.Sequence[Message]
             A list of message objects, where each message contains a role and content.
 
+        fact_instruction : typing.Optional[str]
+            Additional instruction for generating the facts.
+
         summary_instruction : typing.Optional[str]
             Additional instruction for generating the summary.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
@@ -675,14 +679,16 @@
         )
         client.memory.add(
             session_id="sessionId",
             messages=[Message()],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"messages": messages}
+        if fact_instruction is not OMIT:
+            _request["fact_instruction"] = fact_instruction
         if summary_instruction is not OMIT:
             _request["summary_instruction"] = summary_instruction
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{jsonable_encoder(session_id)}/memory"
             ),
@@ -1902,28 +1908,32 @@
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add(
         self,
         session_id: str,
         *,
         messages: typing.Sequence[Message],
+        fact_instruction: typing.Optional[str] = OMIT,
         summary_instruction: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SuccessResponse:
         """
         Add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
 
         messages : typing.Sequence[Message]
             A list of message objects, where each message contains a role and content.
 
+        fact_instruction : typing.Optional[str]
+            Additional instruction for generating the facts.
+
         summary_instruction : typing.Optional[str]
             Additional instruction for generating the summary.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
@@ -1941,14 +1951,16 @@
         )
         await client.memory.add(
             session_id="sessionId",
             messages=[Message()],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"messages": messages}
+        if fact_instruction is not OMIT:
+            _request["fact_instruction"] = fact_instruction
         if summary_instruction is not OMIT:
             _request["summary_instruction"] = summary_instruction
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{jsonable_encoder(session_id)}/memory"
             ),
```

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/__init__.py` & `zep_cloud-1.0.1/src/zep_cloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/api_error.py` & `zep_cloud-1.0.1/src/zep_cloud/types/api_error.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/classify_session_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/classify_session_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/create_document_request.py` & `zep_cloud-1.0.1/src/zep_cloud/types/create_document_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_collection_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/document_collection_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/document_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result.py` & `zep_cloud-1.0.1/src/zep_cloud/types/document_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result_page.py` & `zep_cloud-1.0.1/src/zep_cloud/types/document_search_result_page.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/memory.py` & `zep_cloud-1.0.1/src/zep_cloud/types/memory.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/memory_search_result.py` & `zep_cloud-1.0.1/src/zep_cloud/types/memory_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/message.py` & `zep_cloud-1.0.1/src/zep_cloud/types/message.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/message_list_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/message_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/models_zep_data_class.py` & `zep_cloud-1.0.1/src/zep_cloud/types/models_zep_data_class.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/question.py` & `zep_cloud-1.0.1/src/zep_cloud/types/question.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/session.py` & `zep_cloud-1.0.1/src/zep_cloud/types/session.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/session_list_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/session_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/success_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/success_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/summary.py` & `zep_cloud-1.0.1/src/zep_cloud/types/summary.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/summary_list_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/summary_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/update_document_list_request.py` & `zep_cloud-1.0.1/src/zep_cloud/types/update_document_list_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/user.py` & `zep_cloud-1.0.1/src/zep_cloud/types/user.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/types/user_list_response.py` & `zep_cloud-1.0.1/src/zep_cloud/types/user_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/src/zep_cloud/user/client.py` & `zep_cloud-1.0.1/src/zep_cloud/user/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.0rc1/PKG-INFO` & `zep_cloud-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-cloud
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: 
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: zep-cloud Version: 1.0.0rc1 Summary: Requires-
-Python: >=3.8.1,<4.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Requires-Dist: httpx
-(>=0.21.2) Requires-Dist: pydantic (>=1.9.2) Requires-Dist: typing_extensions
-(>=4.0.0) Description-Content-Type: text/markdown [![Release to PyPI](https://
-github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://
-github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://
+Metadata-Version: 2.1 Name: zep-cloud Version: 1.0.1 Summary: Requires-Python:
+>=3.8.1,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Dist: httpx (>=0.21.2)
+Requires-Dist: pydantic (>=1.9.2) Requires-Dist: typing_extensions (>=4.0.0)
+Description-Content-Type: text/markdown [![Release to PyPI](https://github.com/
+getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/
+getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://
 img.shields.io/github/license/getzep/zep-python?color=blue) [![fern shield]
 (https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-
 brightgreen)](https://github.com/fern-api/fern)
                                   _[_Z_e_p_ _L_o_g_o_]
            ************ ZZeepp:: LLoonngg--TTeerrmm MMeemmoorryy ffoorr ?â??AAII AAssssiissttaannttss.. ************
      ********** RReeccaallll,, uunnddeerrssttaanndd,, aanndd eexxttrraacctt ddaattaa ffrroomm cchhaatt hhiissttoorriieess.. PPoowweerr
                       ppeerrssoonnaalliizzeedd AAII eexxppeerriieenncceess.. **********
```


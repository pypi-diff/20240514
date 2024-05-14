# Comparing `tmp/pytest_aws_apigateway-0.3.0.tar.gz` & `tmp/pytest_aws_apigateway-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.3.0.tar", last modified: Mon May 13 09:37:04 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.4.0.tar", last modified: Tue May 14 20:14:15 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.3.0.tar` & `pytest_aws_apigateway-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.381175 pytest_aws_apigateway-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.373175 pytest_aws_apigateway-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:37:04.381175 pytest_aws_apigateway-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.373175 pytest_aws_apigateway-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 09:37:04.000000 pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:37:04.377175 pytest_aws_apigateway-0.3.0/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/examples/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 09:36:54.000000 pytest_aws_apigateway-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tox.ini
```

### Comparing `pytest_aws_apigateway-0.3.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.3.0/LICENSE` & `pytest_aws_apigateway-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.3.0/PKG-INFO` & `pytest_aws_apigateway-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.3.0
+Version: 0.4.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -49,25 +49,21 @@
 ```console
 pip install pytest-aws-apigateway
 ```
 
 ## Usage
 
 ```python
-import httpx
-
-from pytest_aws_apigateway import ApiGateway
-
-def test_handler(apigateway: ApiGateway):
-
+def test_root_resource(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
-        return httpx.Response(200, json={"body": "hello"})
-
-    apigateway.add_integration("/", handler=handler, method="GET", endpoint="https://some/")
+        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
+    apigateway_mock.add_integration(
+        "/", handler=handler, method="GET", endpoint="https://some/"
+    )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
         assert resp.json() == {"body": "hello"}
 ```
```

### Comparing `pytest_aws_apigateway-0.3.0/README.md` & `pytest_aws_apigateway-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,21 @@
 ```console
 pip install pytest-aws-apigateway
 ```
 
 ## Usage
 
 ```python
-import httpx
-
-from pytest_aws_apigateway import ApiGateway
-
-def test_handler(apigateway: ApiGateway):
-
+def test_root_resource(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
-        return httpx.Response(200, json={"body": "hello"})
-
-    apigateway.add_integration("/", handler=handler, method="GET", endpoint="https://some/")
+        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
+    apigateway_mock.add_integration(
+        "/", handler=handler, method="GET", endpoint="https://some/"
+    )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
         assert resp.json() == {"body": "hello"}
 ```
```

### Comparing `pytest_aws_apigateway-0.3.0/pyproject.toml` & `pytest_aws_apigateway-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/apigateway.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import json
 import re
-from typing import Callable
+from typing import Any, Callable
 from typing import Union
 
 import httpx
 import pytest_httpx
 
 from pytest_aws_apigateway.context import LambdaContext, create_context
-from pytest_aws_apigateway.event import OutputFormatError
-from pytest_aws_apigateway.event import request_to_event
-from pytest_aws_apigateway.event import transform_response
+from pytest_aws_apigateway.integration import ResponseFormatError
+from pytest_aws_apigateway.integration import IntegrationResponse
+from pytest_aws_apigateway.integration import build_integration_request
+from pytest_aws_apigateway.integration import transform_integration_response
 
 __all__ = ["ApiGatewayMock"]
 
 
 class ApiGatewayMock:
     def __init__(self, httpx_mock: pytest_httpx.HTTPXMock):
         self.httpx_mock = httpx_mock
         ...
 
     def add_integration(
         self,
         resource: str,
         method: str,
         endpoint: str,
-        handler: Callable[[dict, LambdaContext], Union[dict, httpx.Response]],
+        handler: Callable[[dict[str, Any], LambdaContext], IntegrationResponse],
     ):
         resource = self._normalize_resource(resource)
         endpoint = self._normalize_endpoint(endpoint)
 
         url = self._url_expression(endpoint, resource)
-        print(resource)
-        print(url)
 
         def integration(request: httpx.Request) -> httpx.Response:
-            event = request_to_event(request, resource)
+            event = build_integration_request(request, resource)
             context = create_context(handler)
             resp = handler(event, context)
             try:
-                return transform_response(resp)
-            except OutputFormatError:
+                return transform_integration_response(resp)
+            except ResponseFormatError:
                 return httpx.Response(
                     status_code=500,
                     json=json.dumps({"message": "Internal server error"}),
                 )
 
         self.httpx_mock.add_callback(callback=integration, url=url, method=method)
```

### Comparing `pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/context.py` & `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/context.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway/event.py` & `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import Any, TypedDict, Union
 import httpx
 import re
 
 PATH_PARAMETER_EXPRESSION = r"\{([^\/]+)\}"
 
 
-class OutputFormatError(Exception): ...
+class ResponseFormatError(Exception): ...
 
 
-def request_to_event(request: httpx.Request, resource: str) -> dict[str, Any]:
+class IntegrationResponse(TypedDict):
+    isBase64Encoded: bool
+    statusCode: int
+    headers: dict[str, str]
+    multiValueHeaders: dict[str, list[str]]
+    body: str
+
+
+def build_integration_request(request: httpx.Request, resource: str) -> dict[str, Any]:
     # TODO isBase64Encoded depends on content-type header
 
     path = request.url.path
     path_parameters = _extract_path_parameters(path, resource)
 
     event = {
         "resource": resource,
@@ -22,32 +30,22 @@
         "queryStringParameters": request.url.params,
         "body": request.content.decode(),
         "pathParameters": path_parameters,
     }
     return event
 
 
-class OutputFormat(TypedDict):
-    isBase64Encoded: bool
-    statusCode: int
-    headers: dict[str, str]
-    multiValueHeaders: dict[str, list[str]]
-    body: str
-
-
-def transform_response(output: Union[dict[str, Any], httpx.Response]) -> httpx.Response:
-    if isinstance(output, httpx.Response):
-        return output
+def transform_integration_response(output: IntegrationResponse) -> httpx.Response:
     if not isinstance(output, dict):
         raise ValueError
     if "statusCode" not in output:
         raise ValueError
     status_code = output["statusCode"]
     if not isinstance(status_code, int):
-        raise OutputFormatError
+        raise ResponseFormatError
     headers = output.get("headers")
     body = output.get("body")
     return httpx.Response(status_code=status_code, headers=headers, content=body)
 
 
 def _extract_path_parameters(path: str, resource: str) -> Union[dict[str, str], None]:
     """Extract path parameters by comparing the URL path with the resource path.
```

### Comparing `pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.3.0
+Version: 0.4.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -49,25 +49,21 @@
 ```console
 pip install pytest-aws-apigateway
 ```
 
 ## Usage
 
 ```python
-import httpx
-
-from pytest_aws_apigateway import ApiGateway
-
-def test_handler(apigateway: ApiGateway):
-
+def test_root_resource(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
-        return httpx.Response(200, json={"body": "hello"})
-
-    apigateway.add_integration("/", handler=handler, method="GET", endpoint="https://some/")
+        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
+    apigateway_mock.add_integration(
+        "/", handler=handler, method="GET", endpoint="https://some/"
+    )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
         assert resp.json() == {"body": "hello"}
 ```
```

### Comparing `pytest_aws_apigateway-0.3.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 requirements-dev.txt
 tox.ini
 .github/workflows/main.yml
 changes/.gitignore
 src/pytest_aws_apigateway/__init__.py
 src/pytest_aws_apigateway/apigateway.py
 src/pytest_aws_apigateway/context.py
-src/pytest_aws_apigateway/event.py
+src/pytest_aws_apigateway/integration.py
 src/pytest_aws_apigateway/plugin.py
 src/pytest_aws_apigateway.egg-info/PKG-INFO
 src/pytest_aws_apigateway.egg-info/SOURCES.txt
 src/pytest_aws_apigateway.egg-info/dependency_links.txt
 src/pytest_aws_apigateway.egg-info/entry_points.txt
 src/pytest_aws_apigateway.egg-info/requires.txt
 src/pytest_aws_apigateway.egg-info/top_level.txt
 tasks/release.py
 tests/__init__.py
 tests/conftest.py
-tests/test_event.py
+tests/test_apigateway.py
+tests/test_integration.py
 tests/test_plugin.py
-tests/test_response.py
-tests/examples/test_handler.py
+tests/test_response.py
```

### Comparing `pytest_aws_apigateway-0.3.0/tasks/release.py` & `pytest_aws_apigateway-0.4.0/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.3.0/tests/test_event.py` & `pytest_aws_apigateway-0.4.0/tests/test_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from httpx import Client
 
-from pytest_aws_apigateway.event import request_to_event
+from pytest_aws_apigateway.integration import build_integration_request
 
 
 def test_request():
     client = Client()
     url = "https://some-path/my/path?a=True"
     req = client.build_request(url=url, method="GET")
     print(req)
@@ -17,10 +17,10 @@
 
 def test_parse_path_parameters():
     client = Client()
 
     url = "https://some-path/my/path?a=True"
     resource = "/{id}/{id2}"
     req = client.build_request(url=url, method="GET")
-    event = request_to_event(req, resource=resource)
+    event = build_integration_request(req, resource=resource)
     assert event["pathParameters"]
     assert event["pathParameters"] == {"id": "my", "id2": "path"}
```


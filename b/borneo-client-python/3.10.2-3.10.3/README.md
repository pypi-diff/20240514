# Comparing `tmp/borneo_client_python-3.10.2.tar.gz` & `tmp/borneo_client_python-3.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borneo_client_python-3.10.2.tar", last modified: Mon May 13 13:28:45 2024, max compression
+gzip compressed data, was "borneo_client_python-3.10.3.tar", last modified: Mon May 13 13:56:01 2024, max compression
```

## Comparing `borneo_client_python-3.10.2.tar` & `borneo_client_python-3.10.3.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.222302 borneo_client_python-3.10.2/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:28:45.222302 borneo_client_python-3.10.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.210302 borneo_client_python-3.10.2/borneo_client_python/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   125040 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   310639 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   181979 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)   138321 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/borneo_client_python/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.222302 borneo_client_python-3.10.2/borneo_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:28:44.000000 borneo_client_python-3.10.2/borneo_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-13 13:28:45.000000 borneo_client_python-3.10.2/borneo_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:28:44.000000 borneo_client_python-3.10.2/borneo_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:28:44.000000 borneo_client_python-3.10.2/borneo_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 13:28:44.000000 borneo_client_python-3.10.2/borneo_client_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:28:45.222302 borneo_client_python-3.10.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.210302 borneo_client_python-3.10.2/smithy_aws_core/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_aws_core/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_aws_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_aws_core/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.214302 borneo_client_python-3.10.2/smithy_aws_core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_aws_core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_aws_core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.214302 borneo_client_python-3.10.2/smithy_core/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.214302 borneo_client_python-3.10.2/smithy_core/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.214302 borneo_client_python-3.10.2/smithy_core/aio/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/aio/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/aio/interfaces/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/aio/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/aio/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    28327 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/interceptors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/interfaces/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/interfaces/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/interfaces/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/rfc3986.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/aio/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/aio/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/auth/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/crt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/aio/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/identity/apikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/aio/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/interfaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/aio/restjson.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/smithy_http/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/restjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-13 13:21:14.000000 borneo_client_python-3.10.2/smithy_http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:28:45.218302 borneo_client_python-3.10.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-13 13:28:40.000000 borneo_client_python-3.10.2/tests/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.846844 borneo_client_python-3.10.3/borneo_auth_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/borneo_auth_provider/borneo_auth_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/borneo_client_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125040 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   310639 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181979 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138321 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/borneo_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/smithy_aws_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/smithy_aws_core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/aio/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/interfaces/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28327 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interceptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/rfc3986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/auth/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/crt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/identity/apikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/interfaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/restjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/restjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/tests/test_protocol.py
```

### Comparing `borneo_client_python-3.10.2/LICENSE` & `borneo_client_python-3.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/PKG-INFO` & `borneo_client_python-3.10.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo_client_python
-Version: 3.10.2
+Version: 3.10.3
 Summary: borneo_client_python client
 License: Apache-2.0
 Keywords: smithy,borneo_client_python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
```

### Comparing `borneo_client_python-3.10.2/README.md` & `borneo_client_python-3.10.3/README.md`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/auth.py` & `borneo_client_python-3.10.3/borneo_client_python/auth.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/client.py` & `borneo_client_python-3.10.3/borneo_client_python/client.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/config.py` & `borneo_client_python-3.10.3/borneo_client_python/config.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/deserialize.py` & `borneo_client_python-3.10.3/borneo_client_python/deserialize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -830,55 +830,55 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
+    if "accountId" not in output:
+        raise ServiceError(
+            'Expected to find "accountId" in the operation output, but it was not present.'
         )
+    kwargs["account_id"] = expect_type(str, output["accountId"])
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+    if (_deleted_at := output.get("deletedAt")) is not None:
+        kwargs["deleted_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _deleted_at)
+        )
 
     if (_cloud_account_id := output.get("cloudAccountId")) is not None:
         kwargs["cloud_account_id"] = expect_type(str, _cloud_account_id)
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+
     if (_permissions := output.get("permissions")) is not None:
         kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
 
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
+        )
+
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
-    if "accountId" not in output:
-        raise ServiceError(
-            'Expected to find "accountId" in the operation output, but it was not present.'
-        )
-    kwargs["account_id"] = expect_type(str, output["accountId"])
-
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
     if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
         kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
 
-    if (_deleted_at := output.get("deletedAt")) is not None:
-        kwargs["deleted_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _deleted_at)
-        )
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
 
     return DescribeAccountOutput(**kwargs)
 
 
 async def _deserialize_error_describe_account(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -917,38 +917,38 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
-    if (_toms := output.get("toms")) is not None:
-        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
-
     if (_tom_ids := output.get("tomIds")) is not None:
         kwargs["tom_ids"] = _deserialize_uuid_collection(_tom_ids, config)
 
-    if (_location_id := output.get("locationId")) is not None:
-        kwargs["location_id"] = expect_type(str, _location_id)
-
     if (_location := output.get("location")) is not None:
         kwargs["location"] = _deserialize_headquarter_record(_location, config)
 
+    if (_location_id := output.get("locationId")) is not None:
+        kwargs["location_id"] = expect_type(str, _location_id)
+
     if (_location_type := output.get("locationType")) is not None:
         kwargs["location_type"] = expect_type(str, _location_type)
 
+    if (_toms := output.get("toms")) is not None:
+        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
+
     if "assetId" not in output:
         raise ServiceError(
             'Expected to find "assetId" in the operation output, but it was not present.'
         )
     kwargs["asset_id"] = expect_type(str, output["assetId"])
 
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
     return DescribeAssetOutput(**kwargs)
 
 
 async def _deserialize_error_describe_asset(
@@ -989,55 +989,55 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+
+    if (_sample_tokens := output.get("sampleTokens")) is not None:
+        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
+
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
     if (_last_scanned := output.get("lastScanned")) is not None:
         kwargs["last_scanned"] = epoch_seconds_to_datetime(
             expect_type(int | float, _last_scanned)
         )
 
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
-
-    if (_sample_tokens := output.get("sampleTokens")) is not None:
-        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
-
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_source := output.get("source")) is not None:
-        kwargs["source"] = expect_type(str, _source)
-
     if (_snapshot := output.get("snapshot")) is not None:
         kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
 
     if (_parent_id := output.get("parentId")) is not None:
         kwargs["parent_id"] = expect_type(str, _parent_id)
 
-    if (_compliance := output.get("compliance")) is not None:
-        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
-
-    if (_owner := output.get("owner")) is not None:
-        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+    if (_source := output.get("source")) is not None:
+        kwargs["source"] = expect_type(str, _source)
 
     if "resourceId" not in output:
         raise ServiceError(
             'Expected to find "resourceId" in the operation output, but it was not present.'
         )
     kwargs["resource_id"] = expect_type(str, output["resourceId"])
 
+    if (_compliance := output.get("compliance")) is not None:
+        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
+
+    if (_owner := output.get("owner")) is not None:
+        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+
     return DescribeCatalogResourceOutput(**kwargs)
 
 
 async def _deserialize_error_describe_catalog_resource(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1075,30 +1075,30 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if "description" not in output:
+        raise ServiceError(
+            'Expected to find "description" in the operation output, but it was not present.'
+        )
+    kwargs["description"] = expect_type(str, output["description"])
+
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if "description" not in output:
-        raise ServiceError(
-            'Expected to find "description" in the operation output, but it was not present.'
-        )
-    kwargs["description"] = expect_type(str, output["description"])
-
     if "categoryLabel" not in output:
         raise ServiceError(
             'Expected to find "categoryLabel" in the operation output, but it was not present.'
         )
     kwargs["category_label"] = expect_type(str, output["categoryLabel"])
 
     return DescribeCategoryOutput(**kwargs)
@@ -1142,56 +1142,56 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_cloud_account_id := output.get("cloudAccountId")) is not None:
+        kwargs["cloud_account_id"] = expect_type(str, _cloud_account_id)
+
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_permissions := output.get("permissions")) is not None:
-        kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
-
-    if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
-        kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
-
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
-    if "accountId" not in output:
-        raise ServiceError(
-            'Expected to find "accountId" in the operation output, but it was not present.'
-        )
-    kwargs["account_id"] = expect_type(str, output["accountId"])
+    if (_permissions := output.get("permissions")) is not None:
+        kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
 
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
+    if "accountId" not in output:
+        raise ServiceError(
+            'Expected to find "accountId" in the operation output, but it was not present.'
+        )
+    kwargs["account_id"] = expect_type(str, output["accountId"])
+
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+
+    if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
+        kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
+
     if (_deleted_at := output.get("deletedAt")) is not None:
         kwargs["deleted_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _deleted_at)
         )
 
-    if (_cloud_account_id := output.get("cloudAccountId")) is not None:
-        kwargs["cloud_account_id"] = expect_type(str, _cloud_account_id)
-
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
-
     return DescribeCloudAccountOutput(**kwargs)
 
 
 async def _deserialize_error_describe_cloud_account(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1232,68 +1232,68 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_state := output.get("state")) is not None:
         kwargs["state"] = expect_type(str, _state)
 
-    if (_data_plane_id := output.get("dataPlaneId")) is not None:
-        kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
-
     if (_connector_type := output.get("connectorType")) is not None:
         kwargs["connector_type"] = expect_type(str, _connector_type)
 
-    if (_region := output.get("region")) is not None:
-        kwargs["region"] = expect_type(str, _region)
-
-    if (_resource_id := output.get("resourceId")) is not None:
-        kwargs["resource_id"] = expect_type(str, _resource_id)
+    if (_data_plane_id := output.get("dataPlaneId")) is not None:
+        kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
 
-    if (_params := output.get("params")) is not None:
-        kwargs["params"] = _deserialize_open_properties(_params, config)
+    if (_meta_data_sync_interval := output.get("metaDataSyncInterval")) is not None:
+        kwargs["meta_data_sync_interval"] = expect_type(str, _meta_data_sync_interval)
 
-    if "connectorId" not in output:
-        raise ServiceError(
-            'Expected to find "connectorId" in the operation output, but it was not present.'
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
         )
-    kwargs["connector_id"] = expect_type(str, output["connectorId"])
-
-    if (_resource_type := output.get("resourceType")) is not None:
-        kwargs["resource_type"] = expect_type(str, _resource_type)
-
-    if (_resource_account_id := output.get("resourceAccountId")) is not None:
-        kwargs["resource_account_id"] = expect_type(str, _resource_account_id)
-
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
 
     if (
         _next_meta_data_sync_schedule := output.get("nextMetaDataSyncSchedule")
     ) is not None:
         kwargs["next_meta_data_sync_schedule"] = epoch_seconds_to_datetime(
             expect_type(int | float, _next_meta_data_sync_schedule)
         )
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
         )
 
-    if (_meta_data_sync_interval := output.get("metaDataSyncInterval")) is not None:
-        kwargs["meta_data_sync_interval"] = expect_type(str, _meta_data_sync_interval)
-
     if (_is_meta_data_sync_running := output.get("isMetaDataSyncRunning")) is not None:
         kwargs["is_meta_data_sync_running"] = expect_type(
             bool, _is_meta_data_sync_running
         )
 
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_resource_type := output.get("resourceType")) is not None:
+        kwargs["resource_type"] = expect_type(str, _resource_type)
+
+    if (_region := output.get("region")) is not None:
+        kwargs["region"] = expect_type(str, _region)
+
+    if (_params := output.get("params")) is not None:
+        kwargs["params"] = _deserialize_open_properties(_params, config)
+
+    if (_resource_id := output.get("resourceId")) is not None:
+        kwargs["resource_id"] = expect_type(str, _resource_id)
+
+    if (_resource_account_id := output.get("resourceAccountId")) is not None:
+        kwargs["resource_account_id"] = expect_type(str, _resource_account_id)
+
+    if "connectorId" not in output:
+        raise ServiceError(
+            'Expected to find "connectorId" in the operation output, but it was not present.'
         )
+    kwargs["connector_id"] = expect_type(str, output["connectorId"])
 
     return DescribeConnectorOutput(**kwargs)
 
 
 async def _deserialize_error_describe_connector(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1391,44 +1391,44 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "createdAt" not in output:
+    if "discoverySource" not in output:
         raise ServiceError(
-            'Expected to find "createdAt" in the operation output, but it was not present.'
+            'Expected to find "discoverySource" in the operation output, but it was not present.'
         )
-    kwargs["created_at"] = epoch_seconds_to_datetime(
-        expect_type(int | float, output["createdAt"])
+    kwargs["discovery_source"] = _deserialize_discovery_source_list(
+        output["discoverySource"], config
     )
 
+    if "recipientModelId" not in output:
+        raise ServiceError(
+            'Expected to find "recipientModelId" in the operation output, but it was not present.'
+        )
+    kwargs["recipient_model_id"] = expect_type(str, output["recipientModelId"])
+
     if "discoveredRecipientId" not in output:
         raise ServiceError(
             'Expected to find "discoveredRecipientId" in the operation output, but it was not present.'
         )
     kwargs["discovered_recipient_id"] = expect_type(
         str, output["discoveredRecipientId"]
     )
 
-    if "discoverySource" not in output:
+    if "createdAt" not in output:
         raise ServiceError(
-            'Expected to find "discoverySource" in the operation output, but it was not present.'
+            'Expected to find "createdAt" in the operation output, but it was not present.'
         )
-    kwargs["discovery_source"] = _deserialize_discovery_source_list(
-        output["discoverySource"], config
+    kwargs["created_at"] = epoch_seconds_to_datetime(
+        expect_type(int | float, output["createdAt"])
     )
 
-    if "recipientModelId" not in output:
-        raise ServiceError(
-            'Expected to find "recipientModelId" in the operation output, but it was not present.'
-        )
-    kwargs["recipient_model_id"] = expect_type(str, output["recipientModelId"])
-
     return DescribeDiscoveredRecipientOutput(**kwargs)
 
 
 async def _deserialize_error_describe_discovered_recipient(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1466,44 +1466,44 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
-
-    if (_recipients := output.get("recipients")) is not None:
-        kwargs["recipients"] = _deserialize_recipients_discovered_of_domain_list(
-            _recipients, config
-        )
-
     if "domainId" not in output:
         raise ServiceError(
             'Expected to find "domainId" in the operation output, but it was not present.'
         )
     kwargs["domain_id"] = expect_type(str, output["domainId"])
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (_frequency := output.get("frequency")) is not None:
         kwargs["frequency"] = expect_type(str, _frequency)
 
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
+    if (_recipients := output.get("recipients")) is not None:
+        kwargs["recipients"] = _deserialize_recipients_discovered_of_domain_list(
+            _recipients, config
+        )
+
     return DescribeDomainOutput(**kwargs)
 
 
 async def _deserialize_error_describe_domain(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1541,36 +1541,36 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_additional_information := output.get("additionalInformation")) is not None:
-        kwargs["additional_information"] = expect_type(str, _additional_information)
-
     if (
         _additional_information_files := output.get("additionalInformationFiles")
     ) is not None:
         kwargs["additional_information_files"] = _deserialize_uuid_collection(
             _additional_information_files, config
         )
 
+    if (_integrity := output.get("integrity")) is not None:
+        kwargs["integrity"] = _deserialize_dpia_integrity_risk(_integrity, config)
+
     if (_confidentiality := output.get("confidentiality")) is not None:
         kwargs["confidentiality"] = _deserialize_dpia_confidentiality_risk(
             _confidentiality, config
         )
 
     if (_availability := output.get("availability")) is not None:
         kwargs["availability"] = _deserialize_dpia_availability_risk(
             _availability, config
         )
 
-    if (_integrity := output.get("integrity")) is not None:
-        kwargs["integrity"] = _deserialize_dpia_integrity_risk(_integrity, config)
+    if (_additional_information := output.get("additionalInformation")) is not None:
+        kwargs["additional_information"] = expect_type(str, _additional_information)
 
     if (_privacy_framework := output.get("privacyFramework")) is not None:
         kwargs["privacy_framework"] = _deserialize_dpia_privacy_framework(
             _privacy_framework, config
         )
 
     if (_status := output.get("status")) is not None:
@@ -1622,69 +1622,69 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "name" not in output:
+    if (_nif := output.get("nif")) is not None:
+        kwargs["nif"] = expect_type(str, _nif)
+
+    if "employeeId" not in output:
         raise ServiceError(
-            'Expected to find "name" in the operation output, but it was not present.'
+            'Expected to find "employeeId" in the operation output, but it was not present.'
         )
-    kwargs["name"] = expect_type(str, output["name"])
-
-    if (_end_date := output.get("endDate")) is not None:
-        kwargs["end_date"] = expect_type(str, _end_date)
-
-    if (_email := output.get("email")) is not None:
-        kwargs["email"] = expect_type(str, _email)
+    kwargs["employee_id"] = expect_type(str, output["employeeId"])
 
-    if (_position := output.get("position")) is not None:
-        kwargs["position"] = expect_type(str, _position)
+    if "surname" not in output:
+        raise ServiceError(
+            'Expected to find "surname" in the operation output, but it was not present.'
+        )
+    kwargs["surname"] = expect_type(str, output["surname"])
 
-    if (_department := output.get("department")) is not None:
-        kwargs["department"] = expect_type(str, _department)
+    if (_reference_id := output.get("referenceId")) is not None:
+        kwargs["reference_id"] = expect_type(str, _reference_id)
 
-    if "employeeId" not in output:
+    if "createdBy" not in output:
         raise ServiceError(
-            'Expected to find "employeeId" in the operation output, but it was not present.'
+            'Expected to find "createdBy" in the operation output, but it was not present.'
         )
-    kwargs["employee_id"] = expect_type(str, output["employeeId"])
+    kwargs["created_by"] = expect_type(str, output["createdBy"])
+
+    if (_manager_object := output.get("managerObject")) is not None:
+        kwargs["manager_object"] = _deserialize_manager_object(_manager_object, config)
 
     if (_start_date := output.get("startDate")) is not None:
         kwargs["start_date"] = expect_type(str, _start_date)
 
-    if (_manager := output.get("manager")) is not None:
-        kwargs["manager"] = expect_type(str, _manager)
+    if (_department := output.get("department")) is not None:
+        kwargs["department"] = expect_type(str, _department)
 
-    if (_nif := output.get("nif")) is not None:
-        kwargs["nif"] = expect_type(str, _nif)
+    if (_end_date := output.get("endDate")) is not None:
+        kwargs["end_date"] = expect_type(str, _end_date)
 
-    if (_reference_id := output.get("referenceId")) is not None:
-        kwargs["reference_id"] = expect_type(str, _reference_id)
+    if (_manager := output.get("manager")) is not None:
+        kwargs["manager"] = expect_type(str, _manager)
 
     if (_department_object := output.get("departmentObject")) is not None:
         kwargs["department_object"] = _deserialize_department_object(
             _department_object, config
         )
 
-    if "surname" not in output:
-        raise ServiceError(
-            'Expected to find "surname" in the operation output, but it was not present.'
-        )
-    kwargs["surname"] = expect_type(str, output["surname"])
+    if (_email := output.get("email")) is not None:
+        kwargs["email"] = expect_type(str, _email)
 
-    if "createdBy" not in output:
+    if "name" not in output:
         raise ServiceError(
-            'Expected to find "createdBy" in the operation output, but it was not present.'
+            'Expected to find "name" in the operation output, but it was not present.'
         )
-    kwargs["created_by"] = expect_type(str, output["createdBy"])
+    kwargs["name"] = expect_type(str, output["name"])
 
-    if (_manager_object := output.get("managerObject")) is not None:
-        kwargs["manager_object"] = _deserialize_manager_object(_manager_object, config)
+    if (_position := output.get("position")) is not None:
+        kwargs["position"] = expect_type(str, _position)
 
     return DescribeEmployeeOutput(**kwargs)
 
 
 async def _deserialize_error_describe_employee(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1723,38 +1723,38 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_city := output.get("city")) is not None:
-        kwargs["city"] = expect_type(str, _city)
-
-    if (_address := output.get("address")) is not None:
-        kwargs["address"] = expect_type(str, _address)
-
-    if (_country := output.get("country")) is not None:
-        kwargs["country"] = expect_type(str, _country)
+    if (_toms := output.get("toms")) is not None:
+        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
 
     if "headquarterId" not in output:
         raise ServiceError(
             'Expected to find "headquarterId" in the operation output, but it was not present.'
         )
     kwargs["headquarter_id"] = expect_type(str, output["headquarterId"])
 
-    if (_zipcode := output.get("zipcode")) is not None:
-        kwargs["zipcode"] = expect_type(str, _zipcode)
-
-    if (_toms := output.get("toms")) is not None:
-        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
-
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
+    if (_country := output.get("country")) is not None:
+        kwargs["country"] = expect_type(str, _country)
+
+    if (_city := output.get("city")) is not None:
+        kwargs["city"] = expect_type(str, _city)
+
+    if (_address := output.get("address")) is not None:
+        kwargs["address"] = expect_type(str, _address)
+
+    if (_zipcode := output.get("zipcode")) is not None:
+        kwargs["zipcode"] = expect_type(str, _zipcode)
+
     return DescribeHeadquarterOutput(**kwargs)
 
 
 async def _deserialize_error_describe_headquarter(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1792,43 +1792,49 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_snapshot := output.get("snapshot")) is not None:
+        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+
     if (_compliance := output.get("compliance")) is not None:
         kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
 
-    if (_snapshot := output.get("snapshot")) is not None:
-        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+    if (_has_finding := output.get("hasFinding")) is not None:
+        kwargs["has_finding"] = expect_type(bool, _has_finding)
 
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+    if (_stats := output.get("stats")) is not None:
+        kwargs["stats"] = _deserialize_record_type(_stats, config)
 
-    if (_has_finding := output.get("hasFinding")) is not None:
-        kwargs["has_finding"] = expect_type(bool, _has_finding)
+    if (_sample_tokens := output.get("sampleTokens")) is not None:
+        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
 
-    if (_resource_type := output.get("resourceType")) is not None:
-        kwargs["resource_type"] = expect_type(str, _resource_type)
+    if (_resource_name := output.get("resourceName")) is not None:
+        kwargs["resource_name"] = expect_type(str, _resource_name)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_file_name := output.get("fileName")) is not None:
+        kwargs["file_name"] = expect_type(str, _file_name)
+
+    if (_scan_id := output.get("scanId")) is not None:
+        kwargs["scan_id"] = expect_type(str, _scan_id)
+
+    if (_parent_id := output.get("parentId")) is not None:
+        kwargs["parent_id"] = expect_type(str, _parent_id)
 
     if (_tokens := output.get("tokens")) is not None:
         kwargs["tokens"] = _deserialize_tokens(_tokens, config)
 
-    if (_user_email := output.get("userEmail")) is not None:
-        kwargs["user_email"] = expect_type(str, _user_email)
-
     if "id" not in output:
         raise ServiceError(
             'Expected to find "id" in the operation output, but it was not present.'
         )
     kwargs["id"] = expect_type(str, output["id"])
 
     if (_scan_parameters := output.get("scanParameters")) is not None:
@@ -1838,39 +1844,33 @@
 
     if (_scan_iteration_id := output.get("scanIterationId")) is not None:
         kwargs["scan_iteration_id"] = expect_type(str, _scan_iteration_id)
 
     if (_user_name := output.get("userName")) is not None:
         kwargs["user_name"] = expect_type(str, _user_name)
 
-    if (_scan_id := output.get("scanId")) is not None:
-        kwargs["scan_id"] = expect_type(str, _scan_id)
-
-    if (_parent_id := output.get("parentId")) is not None:
-        kwargs["parent_id"] = expect_type(str, _parent_id)
-
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
-
     if (_resource_id := output.get("resourceId")) is not None:
         kwargs["resource_id"] = expect_type(str, _resource_id)
 
-    if (_resource_name := output.get("resourceName")) is not None:
-        kwargs["resource_name"] = expect_type(str, _resource_name)
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
 
-    if (_stats := output.get("stats")) is not None:
-        kwargs["stats"] = _deserialize_record_type(_stats, config)
+    if (_resource_type := output.get("resourceType")) is not None:
+        kwargs["resource_type"] = expect_type(str, _resource_type)
 
-    if (_sample_tokens := output.get("sampleTokens")) is not None:
-        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
 
-    if (_file_name := output.get("fileName")) is not None:
-        kwargs["file_name"] = expect_type(str, _file_name)
+    if (_user_email := output.get("userEmail")) is not None:
+        kwargs["user_email"] = expect_type(str, _user_email)
+
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
 
     return DescribeInspectionResultOutput(**kwargs)
 
 
 async def _deserialize_error_describe_inspection_result(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1911,74 +1911,74 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+
     if (_aka := output.get("aka")) is not None:
         kwargs["aka"] = expect_type(str, _aka)
 
+    if (_first_seen := output.get("firstSeen")) is not None:
+        kwargs["first_seen"] = expect_type(str, _first_seen)
+
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_parent_id := output.get("parentId")) is not None:
-        kwargs["parent_id"] = expect_type(str, _parent_id)
-
-    if (_data_categories := output.get("dataCategories")) is not None:
-        kwargs["data_categories"] = _deserialize_unique_string_list(
-            _data_categories, config
-        )
-
-    if (_severity_score := output.get("severityScore")) is not None:
-        kwargs["severity_score"] = expect_type(int, _severity_score)
-
-    if (_owner := output.get("owner")) is not None:
-        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
-
-    if (_source := output.get("source")) is not None:
-        kwargs["source"] = expect_type(str, _source)
-
-    if (_issue_id := output.get("issueId")) is not None:
-        kwargs["issue_id"] = expect_type(str, _issue_id)
-
-    if (_properties := output.get("properties")) is not None:
-        kwargs["properties"] = _deserialize_open_properties(_properties, config)
+    if (_last_updated := output.get("lastUpdated")) is not None:
+        kwargs["last_updated"] = expect_type(str, _last_updated)
 
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
     if (_failed_rules := output.get("failedRules")) is not None:
         kwargs["failed_rules"] = _deserialize_unique_string_list(_failed_rules, config)
 
-    if (_data_classification := output.get("dataClassification")) is not None:
-        kwargs["data_classification"] = _deserialize_unique_string_list(
-            _data_classification, config
-        )
+    if (_properties := output.get("properties")) is not None:
+        kwargs["properties"] = _deserialize_open_properties(_properties, config)
 
     if (_scan := output.get("scan")) is not None:
         kwargs["scan"] = _deserialize_scan_information(_scan, config)
 
+    if (_owner := output.get("owner")) is not None:
+        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+
     if "resourceId" not in output:
         raise ServiceError(
             'Expected to find "resourceId" in the operation output, but it was not present.'
         )
     kwargs["resource_id"] = expect_type(str, output["resourceId"])
 
-    if (_first_seen := output.get("firstSeen")) is not None:
-        kwargs["first_seen"] = expect_type(str, _first_seen)
+    if (_data_classification := output.get("dataClassification")) is not None:
+        kwargs["data_classification"] = _deserialize_unique_string_list(
+            _data_classification, config
+        )
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+    if (_source := output.get("source")) is not None:
+        kwargs["source"] = expect_type(str, _source)
 
-    if (_last_updated := output.get("lastUpdated")) is not None:
-        kwargs["last_updated"] = expect_type(str, _last_updated)
+    if (_issue_id := output.get("issueId")) is not None:
+        kwargs["issue_id"] = expect_type(str, _issue_id)
+
+    if (_parent_id := output.get("parentId")) is not None:
+        kwargs["parent_id"] = expect_type(str, _parent_id)
+
+    if (_data_categories := output.get("dataCategories")) is not None:
+        kwargs["data_categories"] = _deserialize_unique_string_list(
+            _data_categories, config
+        )
+
+    if (_severity_score := output.get("severityScore")) is not None:
+        kwargs["severity_score"] = expect_type(int, _severity_score)
 
     return DescribeInventoryResourceOutput(**kwargs)
 
 
 async def _deserialize_error_describe_inventory_resource(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2017,58 +2017,58 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
-
-    if (_resource_id := output.get("resourceId")) is not None:
-        kwargs["resource_id"] = expect_type(str, _resource_id)
+    if (_state := output.get("state")) is not None:
+        kwargs["state"] = expect_type(str, _state)
 
     if (_compliance_risk := output.get("complianceRisk")) is not None:
         kwargs["compliance_risk"] = _deserialize_compliance_risk(
             _compliance_risk, config
         )
 
-    if (_severity := output.get("severity")) is not None:
-        kwargs["severity"] = expect_type(str, _severity)
-
-    if (_events := output.get("events")) is not None:
-        kwargs["events"] = _deserialize_data_security_event_list(_events, config)
-
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_notifications := output.get("notifications")) is not None:
-        kwargs["notifications"] = _deserialize_issue_notification_list(
-            _notifications, config
-        )
-
-    if (_state := output.get("state")) is not None:
-        kwargs["state"] = expect_type(str, _state)
-
-    if (_resource := output.get("resource")) is not None:
-        kwargs["resource"] = _deserialize_issue_resource_details(_resource, config)
+    if (_resource_id := output.get("resourceId")) is not None:
+        kwargs["resource_id"] = expect_type(str, _resource_id)
 
     if "issueId" not in output:
         raise ServiceError(
             'Expected to find "issueId" in the operation output, but it was not present.'
         )
     kwargs["issue_id"] = expect_type(str, output["issueId"])
 
+    if (_severity := output.get("severity")) is not None:
+        kwargs["severity"] = expect_type(str, _severity)
+
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
+    if (_events := output.get("events")) is not None:
+        kwargs["events"] = _deserialize_data_security_event_list(_events, config)
+
+    if (_resource := output.get("resource")) is not None:
+        kwargs["resource"] = _deserialize_issue_resource_details(_resource, config)
+
     if (_security_risk := output.get("securityRisk")) is not None:
         kwargs["security_risk"] = _deserialize_security_risk(_security_risk, config)
 
+    if (_notifications := output.get("notifications")) is not None:
+        kwargs["notifications"] = _deserialize_issue_notification_list(
+            _notifications, config
+        )
+
     return DescribeIssueOutput(**kwargs)
 
 
 async def _deserialize_error_describe_issue(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -2113,137 +2113,137 @@
         output = json.loads(body)
 
     if (_data_subjects := output.get("dataSubjects")) is not None:
         kwargs["data_subjects"] = _deserialize_data_subject_collection(
             _data_subjects, config
         )
 
-    if (_active := output.get("active")) is not None:
-        kwargs["active"] = expect_type(bool, _active)
-
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_infotype_categories := output.get("infotypeCategories")) is not None:
-        kwargs["infotype_categories"] = _deserialize_infotype_category_list(
-            _infotype_categories, config
+    if "processingActivityId" not in output:
+        raise ServiceError(
+            'Expected to find "processingActivityId" in the operation output, but it was not present.'
         )
+    kwargs["processing_activity_id"] = expect_type(str, output["processingActivityId"])
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
 
-    if (_department_objects := output.get("departmentObjects")) is not None:
-        kwargs["department_objects"] = _deserialize_processing_activity_department_list(
-            _department_objects, config
+    if (_retention_period := output.get("retentionPeriod")) is not None:
+        kwargs["retention_period"] = _deserialize_retention_period(
+            _retention_period, config
         )
 
+    if (_additional_info := output.get("additionalInfo")) is not None:
+        kwargs["additional_info"] = expect_type(str, _additional_info)
+
     if (_model_id := output.get("modelId")) is not None:
         kwargs["model_id"] = expect_type(str, _model_id)
 
-    if (_company_role := output.get("companyRole")) is not None:
-        kwargs["company_role"] = expect_type(str, _company_role)
-
-    if (_purpose := output.get("purpose")) is not None:
-        kwargs["purpose"] = expect_type(str, _purpose)
-
     if (
         _processing_frequency_comment := output.get("processingFrequencyComment")
     ) is not None:
         kwargs["processing_frequency_comment"] = expect_type(
             str, _processing_frequency_comment
         )
 
-    if (_is_data_stored := output.get("isDataStored")) is not None:
-        kwargs["is_data_stored"] = expect_type(bool, _is_data_stored)
+    if (_company_role := output.get("companyRole")) is not None:
+        kwargs["company_role"] = expect_type(str, _company_role)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_infotype_volume := output.get("infotypeVolume")) is not None:
+        kwargs["infotype_volume"] = expect_type(str, _infotype_volume)
 
-    if (_recipient_objects := output.get("recipientObjects")) is not None:
-        kwargs["recipient_objects"] = _deserialize_processing_activity_recipient_list(
-            _recipient_objects, config
+    if (_management_methods := output.get("managementMethods")) is not None:
+        kwargs["management_methods"] = _deserialize_management_method_collection(
+            _management_methods, config
         )
 
-    if (_retention_period_comment := output.get("retentionPeriodComment")) is not None:
-        kwargs["retention_period_comment"] = expect_type(str, _retention_period_comment)
-
-    if (_created_by := output.get("createdBy")) is not None:
-        kwargs["created_by"] = expect_type(str, _created_by)
-
-    if (_processing_frequency := output.get("processingFrequency")) is not None:
-        kwargs["processing_frequency"] = expect_type(str, _processing_frequency)
-
-    if (
-        _are_access_requests_managed := output.get("areAccessRequestsManaged")
-    ) is not None:
-        kwargs["are_access_requests_managed"] = expect_type(
-            bool, _are_access_requests_managed
+    if (_additional_info_files := output.get("additionalInfoFiles")) is not None:
+        kwargs["additional_info_files"] = _deserialize_uuid_collection(
+            _additional_info_files, config
         )
 
-    if (_data_types := output.get("dataTypes")) is not None:
-        kwargs["data_types"] = _deserialize_data_type_collection(_data_types, config)
-
     if (_lawful_basis := output.get("lawfulBasis")) is not None:
         kwargs["lawful_basis"] = _deserialize_lawful_basis_collection(
             _lawful_basis, config
         )
 
     if (_contact_person_employee := output.get("contactPersonEmployee")) is not None:
         kwargs["contact_person_employee"] = _deserialize_processing_activity_employee(
             _contact_person_employee, config
         )
 
-    if (_additional_info_files := output.get("additionalInfoFiles")) is not None:
-        kwargs["additional_info_files"] = _deserialize_uuid_collection(
-            _additional_info_files, config
+    if (_data_types := output.get("dataTypes")) is not None:
+        kwargs["data_types"] = _deserialize_data_type_collection(_data_types, config)
+
+    if (_is_data_stored := output.get("isDataStored")) is not None:
+        kwargs["is_data_stored"] = expect_type(bool, _is_data_stored)
+
+    if (_processing_frequency := output.get("processingFrequency")) is not None:
+        kwargs["processing_frequency"] = expect_type(str, _processing_frequency)
+
+    if (
+        _are_access_requests_managed := output.get("areAccessRequestsManaged")
+    ) is not None:
+        kwargs["are_access_requests_managed"] = expect_type(
+            bool, _are_access_requests_managed
         )
 
-    if (_management_methods := output.get("managementMethods")) is not None:
-        kwargs["management_methods"] = _deserialize_management_method_collection(
-            _management_methods, config
+    if (_created_by := output.get("createdBy")) is not None:
+        kwargs["created_by"] = expect_type(str, _created_by)
+
+    if (_data_sources := output.get("dataSources")) is not None:
+        kwargs["data_sources"] = (
+            _deserialize_processing_activitiy_data_source_collection(
+                _data_sources, config
+            )
         )
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
-    if "processingActivityId" not in output:
-        raise ServiceError(
-            'Expected to find "processingActivityId" in the operation output, but it was not present.'
+    if (_recipient_objects := output.get("recipientObjects")) is not None:
+        kwargs["recipient_objects"] = _deserialize_processing_activity_recipient_list(
+            _recipient_objects, config
         )
-    kwargs["processing_activity_id"] = expect_type(str, output["processingActivityId"])
-
-    if (_additional_info := output.get("additionalInfo")) is not None:
-        kwargs["additional_info"] = expect_type(str, _additional_info)
 
     if (_infotypes := output.get("infotypes")) is not None:
         kwargs["infotypes"] = _deserialize_infotypes_list(_infotypes, config)
 
-    if (_retention_period := output.get("retentionPeriod")) is not None:
-        kwargs["retention_period"] = _deserialize_retention_period(
-            _retention_period, config
-        )
-
     if (_asset_objects := output.get("assetObjects")) is not None:
         kwargs["asset_objects"] = _deserialize_processing_activity_asset_list(
             _asset_objects, config
         )
 
-    if (_data_sources := output.get("dataSources")) is not None:
-        kwargs["data_sources"] = (
-            _deserialize_processing_activitiy_data_source_collection(
-                _data_sources, config
-            )
+    if (_purpose := output.get("purpose")) is not None:
+        kwargs["purpose"] = expect_type(str, _purpose)
+
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
+    if (_retention_period_comment := output.get("retentionPeriodComment")) is not None:
+        kwargs["retention_period_comment"] = expect_type(str, _retention_period_comment)
+
+    if (_department_objects := output.get("departmentObjects")) is not None:
+        kwargs["department_objects"] = _deserialize_processing_activity_department_list(
+            _department_objects, config
         )
 
-    if (_infotype_volume := output.get("infotypeVolume")) is not None:
-        kwargs["infotype_volume"] = expect_type(str, _infotype_volume)
+    if (_active := output.get("active")) is not None:
+        kwargs["active"] = expect_type(bool, _active)
+
+    if (_infotype_categories := output.get("infotypeCategories")) is not None:
+        kwargs["infotype_categories"] = _deserialize_infotype_category_list(
+            _infotype_categories, config
+        )
 
     return DescribeProcessingActivityOutput(**kwargs)
 
 
 async def _deserialize_error_describe_processing_activity(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2282,66 +2282,66 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_dpa_status := output.get("dpaStatus")) is not None:
+        kwargs["dpa_status"] = expect_type(str, _dpa_status)
 
     if (_dpa := output.get("dpa")) is not None:
         kwargs["dpa"] = expect_type(str, _dpa)
 
-    if (_dpa_status := output.get("dpaStatus")) is not None:
-        kwargs["dpa_status"] = expect_type(str, _dpa_status)
+    if (_category := output.get("category")) is not None:
+        kwargs["category"] = expect_type(str, _category)
 
-    if (_discovered_date := output.get("discoveredDate")) is not None:
-        kwargs["discovered_date"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _discovered_date)
+    if (_recipient_warranties := output.get("recipientWarranties")) is not None:
+        kwargs["recipient_warranties"] = _deserialize_warranty_list(
+            _recipient_warranties, config
         )
 
-    if (_role := output.get("role")) is not None:
-        kwargs["role"] = expect_type(str, _role)
-
-    if (_country := output.get("country")) is not None:
-        kwargs["country"] = expect_type(str, _country)
-
-    if (_state := output.get("state")) is not None:
-        kwargs["state"] = expect_type(str, _state)
+    if (_recipient_model_id := output.get("recipientModelId")) is not None:
+        kwargs["recipient_model_id"] = expect_type(str, _recipient_model_id)
 
-    if (_business_name := output.get("businessName")) is not None:
-        kwargs["business_name"] = expect_type(str, _business_name)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
 
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
+    if (_state := output.get("state")) is not None:
+        kwargs["state"] = expect_type(str, _state)
+
     if (_dpa_files := output.get("dpaFiles")) is not None:
         kwargs["dpa_files"] = _deserialize_uuid_collection(_dpa_files, config)
 
     if (_data_storage_location := output.get("dataStorageLocation")) is not None:
         kwargs["data_storage_location"] = _deserialize_country_list(
             _data_storage_location, config
         )
 
     if (_discovery_source := output.get("discoverySource")) is not None:
         kwargs["discovery_source"] = _deserialize_discovery_source_list(
             _discovery_source, config
         )
 
-    if (_category := output.get("category")) is not None:
-        kwargs["category"] = expect_type(str, _category)
-
-    if (_recipient_warranties := output.get("recipientWarranties")) is not None:
-        kwargs["recipient_warranties"] = _deserialize_warranty_list(
-            _recipient_warranties, config
+    if (_discovered_date := output.get("discoveredDate")) is not None:
+        kwargs["discovered_date"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _discovered_date)
         )
 
-    if (_recipient_model_id := output.get("recipientModelId")) is not None:
-        kwargs["recipient_model_id"] = expect_type(str, _recipient_model_id)
+    if (_role := output.get("role")) is not None:
+        kwargs["role"] = expect_type(str, _role)
+
+    if (_country := output.get("country")) is not None:
+        kwargs["country"] = expect_type(str, _country)
+
+    if (_business_name := output.get("businessName")) is not None:
+        kwargs["business_name"] = expect_type(str, _business_name)
 
     return DescribeRecipientOutput(**kwargs)
 
 
 async def _deserialize_error_describe_recipient(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2388,93 +2388,93 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_schedule_type := output.get("scheduleType")) is not None:
         kwargs["schedule_type"] = expect_type(str, _schedule_type)
 
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
-        )
+    if (_elapsed_time_ms := output.get("elapsedTimeMs")) is not None:
+        kwargs["elapsed_time_ms"] = expect_type(int, _elapsed_time_ms)
+
+    if (_snapshot := output.get("snapshot")) is not None:
+        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
 
     if (_schedule := output.get("schedule")) is not None:
         kwargs["schedule"] = _deserialize_scan_schedule(_schedule, config)
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_scan_meta(_meta, config)
-
-    if (_scan_filter := output.get("scanFilter")) is not None:
-        kwargs["scan_filter"] = _deserialize_scan_filter_list(_scan_filter, config)
-
-    if (_stats := output.get("stats")) is not None:
-        kwargs["stats"] = _deserialize_scan_stats(_stats, config)
-
     if (_inspection_policy := output.get("inspectionPolicy")) is not None:
         kwargs["inspection_policy"] = _deserialize_inspection_policy(
             _inspection_policy, config
         )
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_scan_meta(_meta, config)
 
-    if (_scan_type := output.get("scanType")) is not None:
-        kwargs["scan_type"] = expect_type(str, _scan_type)
+    if (_data_plane_name := output.get("dataPlaneName")) is not None:
+        kwargs["data_plane_name"] = expect_type(str, _data_plane_name)
 
-    if (_resource_type := output.get("resourceType")) is not None:
-        kwargs["resource_type"] = expect_type(str, _resource_type)
+    if (_scan_filter := output.get("scanFilter")) is not None:
+        kwargs["scan_filter"] = _deserialize_scan_filter_list(_scan_filter, config)
 
-    if (_snapshot := output.get("snapshot")) is not None:
-        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+    if (_resources := output.get("resources")) is not None:
+        kwargs["resources"] = _deserialize_scan_resources(_resources, config)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_scan_limits := output.get("scanLimits")) is not None:
+        kwargs["scan_limits"] = _deserialize_scan_limits(_scan_limits, config)
+
+    if (_data_plane_id := output.get("dataPlaneId")) is not None:
+        kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
     if (_next_execution := output.get("nextExecution")) is not None:
         kwargs["next_execution"] = epoch_seconds_to_datetime(
             expect_type(int | float, _next_execution)
         )
 
-    if (_cron := output.get("cron")) is not None:
-        kwargs["cron"] = expect_type(str, _cron)
-
     if "scanId" not in output:
         raise ServiceError(
             'Expected to find "scanId" in the operation output, but it was not present.'
         )
     kwargs["scan_id"] = expect_type(str, output["scanId"])
 
     if (_connector_id := output.get("connectorId")) is not None:
         kwargs["connector_id"] = expect_type(str, _connector_id)
 
-    if (_connector_type := output.get("connectorType")) is not None:
-        kwargs["connector_type"] = expect_type(str, _connector_type)
-
-    if (_data_plane_name := output.get("dataPlaneName")) is not None:
-        kwargs["data_plane_name"] = expect_type(str, _data_plane_name)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
 
     if (_data_plane_slug := output.get("dataPlaneSlug")) is not None:
         kwargs["data_plane_slug"] = expect_type(str, _data_plane_slug)
 
-    if (_scan_limits := output.get("scanLimits")) is not None:
-        kwargs["scan_limits"] = _deserialize_scan_limits(_scan_limits, config)
+    if (_cron := output.get("cron")) is not None:
+        kwargs["cron"] = expect_type(str, _cron)
 
-    if (_data_plane_id := output.get("dataPlaneId")) is not None:
-        kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
+    if (_connector_type := output.get("connectorType")) is not None:
+        kwargs["connector_type"] = expect_type(str, _connector_type)
 
-    if (_resources := output.get("resources")) is not None:
-        kwargs["resources"] = _deserialize_scan_resources(_resources, config)
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
 
-    if (_elapsed_time_ms := output.get("elapsedTimeMs")) is not None:
-        kwargs["elapsed_time_ms"] = expect_type(int, _elapsed_time_ms)
+    if (_stats := output.get("stats")) is not None:
+        kwargs["stats"] = _deserialize_scan_stats(_stats, config)
+
+    if (_resource_type := output.get("resourceType")) is not None:
+        kwargs["resource_type"] = expect_type(str, _resource_type)
+
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
+        )
+
+    if (_scan_type := output.get("scanType")) is not None:
+        kwargs["scan_type"] = expect_type(str, _scan_type)
 
     return DescribeScanOutput(**kwargs)
 
 
 async def _deserialize_error_describe_scan(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2525,110 +2525,110 @@
         kwargs["monitoring_publicly_accessible_areas"] = expect_type(
             bool, _monitoring_publicly_accessible_areas
         )
 
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
-    if (_blacklist := output.get("blacklist")) is not None:
-        kwargs["blacklist"] = expect_type(bool, _blacklist)
+    if (
+        _innovative_technologies_used := output.get("innovativeTechnologiesUsed")
+    ) is not None:
+        kwargs["innovative_technologies_used"] = expect_type(
+            bool, _innovative_technologies_used
+        )
 
     if (
         _extensive_automated_evaluation_characteristics := output.get(
             "extensiveAutomatedEvaluationCharacteristics"
         )
     ) is not None:
         kwargs["extensive_automated_evaluation_characteristics"] = expect_type(
             bool, _extensive_automated_evaluation_characteristics
         )
 
-    if (
-        _innovative_technologies_used := output.get("innovativeTechnologiesUsed")
-    ) is not None:
-        kwargs["innovative_technologies_used"] = expect_type(
-            bool, _innovative_technologies_used
-        )
-
-    if (_dpia_status := output.get("dpiaStatus")) is not None:
-        kwargs["dpia_status"] = expect_type(str, _dpia_status)
+    if (_blacklist := output.get("blacklist")) is not None:
+        kwargs["blacklist"] = expect_type(bool, _blacklist)
 
     if (
-        _processing_vulnerable_data_subject := output.get(
-            "processingVulnerableDataSubject"
-        )
+        _automated_decision_making := output.get("automatedDecisionMaking")
     ) is not None:
-        kwargs["processing_vulnerable_data_subject"] = expect_type(
-            bool, _processing_vulnerable_data_subject
+        kwargs["automated_decision_making"] = expect_type(
+            bool, _automated_decision_making
         )
 
     if (
-        _prevent_data_subjects_exercising_their_rights := output.get(
-            "preventDataSubjectsExercisingTheirRights"
+        _matching_merging_records_involved := output.get(
+            "matchingMergingRecordsInvolved"
         )
     ) is not None:
-        kwargs["prevent_data_subjects_exercising_their_rights"] = expect_type(
-            bool, _prevent_data_subjects_exercising_their_rights
+        kwargs["matching_merging_records_involved"] = expect_type(
+            bool, _matching_merging_records_involved
         )
 
-    if (_comment := output.get("comment")) is not None:
-        kwargs["comment"] = expect_type(str, _comment)
-
     if (_classifying_data_subject := output.get("classifyingDataSubject")) is not None:
         kwargs["classifying_data_subject"] = expect_type(
             bool, _classifying_data_subject
         )
 
     if (
-        _large_scale_data_processing := output.get("largeScaleDataProcessing")
+        _prevent_data_subjects_exercising_their_rights := output.get(
+            "preventDataSubjectsExercisingTheirRights"
+        )
     ) is not None:
-        kwargs["large_scale_data_processing"] = expect_type(
-            bool, _large_scale_data_processing
+        kwargs["prevent_data_subjects_exercising_their_rights"] = expect_type(
+            bool, _prevent_data_subjects_exercising_their_rights
         )
 
     if (
-        _automated_decision_making := output.get("automatedDecisionMaking")
+        _large_scale_processing_sensitive_data := output.get(
+            "largeScaleProcessingSensitiveData"
+        )
     ) is not None:
-        kwargs["automated_decision_making"] = expect_type(
-            bool, _automated_decision_making
+        kwargs["large_scale_processing_sensitive_data"] = expect_type(
+            bool, _large_scale_processing_sensitive_data
         )
 
     if (
         _processing_confidential_sensitive_data := output.get(
             "processingConfidentialSensitiveData"
         )
     ) is not None:
         kwargs["processing_confidential_sensitive_data"] = expect_type(
             bool, _processing_confidential_sensitive_data
         )
 
     if (
-        _large_scale_processing_sensitive_data := output.get(
-            "largeScaleProcessingSensitiveData"
-        )
-    ) is not None:
-        kwargs["large_scale_processing_sensitive_data"] = expect_type(
-            bool, _large_scale_processing_sensitive_data
-        )
-
-    if (
         _systematic_monitoring_data_subject := output.get(
             "systematicMonitoringDataSubject"
         )
     ) is not None:
         kwargs["systematic_monitoring_data_subject"] = expect_type(
             bool, _systematic_monitoring_data_subject
         )
 
     if (
-        _matching_merging_records_involved := output.get(
-            "matchingMergingRecordsInvolved"
+        _large_scale_data_processing := output.get("largeScaleDataProcessing")
+    ) is not None:
+        kwargs["large_scale_data_processing"] = expect_type(
+            bool, _large_scale_data_processing
+        )
+
+    if (_comment := output.get("comment")) is not None:
+        kwargs["comment"] = expect_type(str, _comment)
+
+    if (_dpia_status := output.get("dpiaStatus")) is not None:
+        kwargs["dpia_status"] = expect_type(str, _dpia_status)
+
+    if (
+        _processing_vulnerable_data_subject := output.get(
+            "processingVulnerableDataSubject"
         )
     ) is not None:
-        kwargs["matching_merging_records_involved"] = expect_type(
-            bool, _matching_merging_records_involved
+        kwargs["processing_vulnerable_data_subject"] = expect_type(
+            bool, _processing_vulnerable_data_subject
         )
 
     return DescribeThresholdOutput(**kwargs)
 
 
 async def _deserialize_error_describe_threshold(
     http_response: HTTPResponse, config: Config
@@ -2676,38 +2676,38 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_description := output.get("description")) is not None:
         kwargs["description"] = expect_type(str, _description)
 
+    if (_type := output.get("type")) is not None:
+        kwargs["type"] = expect_type(str, _type)
+
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_note := output.get("note")) is not None:
+        kwargs["note"] = expect_type(str, _note)
 
     if (_object_category := output.get("objectCategory")) is not None:
         kwargs["object_category"] = expect_type(str, _object_category)
 
     if (_list_ := output.get("list")) is not None:
         kwargs["list_"] = expect_type(str, _list_)
 
     if (_category := output.get("category")) is not None:
         kwargs["category"] = expect_type(str, _category)
 
-    if (_type := output.get("type")) is not None:
-        kwargs["type"] = expect_type(str, _type)
-
-    if (_note := output.get("note")) is not None:
-        kwargs["note"] = expect_type(str, _note)
-
     if (_document_files := output.get("documentFiles")) is not None:
         kwargs["document_files"] = _deserialize_uuid_collection(_document_files, config)
 
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
     if (_reference_code := output.get("referenceCode")) is not None:
         kwargs["reference_code"] = expect_type(str, _reference_code)
 
     return DescribeTomOutput(**kwargs)
 
 
 async def _deserialize_error_describe_tom(
@@ -2762,33 +2762,33 @@
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
     if (_email := output.get("email")) is not None:
         kwargs["email"] = expect_type(str, _email)
 
-    if (_deleted_at := output.get("deletedAt")) is not None:
-        kwargs["deleted_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _deleted_at)
-        )
-
     if "userId" not in output:
         raise ServiceError(
             'Expected to find "userId" in the operation output, but it was not present.'
         )
     kwargs["user_id"] = expect_type(str, output["userId"])
 
     if (_connector_source_type := output.get("connectorSourceType")) is not None:
         kwargs["connector_source_type"] = expect_type(str, _connector_source_type)
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
+    if (_deleted_at := output.get("deletedAt")) is not None:
+        kwargs["deleted_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _deleted_at)
+        )
+
     if (_external := output.get("external")) is not None:
         kwargs["external"] = expect_type(bool, _external)
 
     if (_connector_id := output.get("connectorId")) is not None:
         kwargs["connector_id"] = expect_type(str, _connector_id)
 
     if (_connector_user_id := output.get("connectorUserId")) is not None:
@@ -2840,20 +2840,20 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_accounts := output.get("accounts")) is not None:
-        kwargs["accounts"] = _deserialize_accounts_list(_accounts, config)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_accounts := output.get("accounts")) is not None:
+        kwargs["accounts"] = _deserialize_accounts_list(_accounts, config)
+
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
     return ListAccountsOutput(**kwargs)
 
 
 async def _deserialize_error_list_accounts(
@@ -2889,23 +2889,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     if "assets" not in output:
         raise ServiceError(
             'Expected to find "assets" in the operation output, but it was not present.'
         )
     kwargs["assets"] = _deserialize_asset_list(output["assets"], config)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if "total" not in output:
         raise ServiceError(
             'Expected to find "total" in the operation output, but it was not present.'
         )
     kwargs["total"] = expect_type(int, output["total"])
 
     return ListAssetsOutput(**kwargs)
@@ -2946,20 +2946,20 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_count := output.get("count")) is not None:
-        kwargs["count"] = expect_type(int, _count)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_count := output.get("count")) is not None:
+        kwargs["count"] = expect_type(int, _count)
+
     if (_resources := output.get("resources")) is not None:
         kwargs["resources"] = _deserialize_leaf_resources_data_list(_resources, config)
 
     return ListCatalogLeafResourcesOutput(**kwargs)
 
 
 async def _deserialize_error_list_catalog_leaf_resources(
@@ -3040,23 +3040,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_connectors := output.get("connectors")) is not None:
-        kwargs["connectors"] = _deserialize_connectors_list(_connectors, config)
-
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_connectors := output.get("connectors")) is not None:
+        kwargs["connectors"] = _deserialize_connectors_list(_connectors, config)
+
     return ListConnectorsOutput(**kwargs)
 
 
 async def _deserialize_error_list_connectors(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3089,28 +3089,28 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "total" not in output:
+    if "departments" not in output:
         raise ServiceError(
-            'Expected to find "total" in the operation output, but it was not present.'
+            'Expected to find "departments" in the operation output, but it was not present.'
         )
-    kwargs["total"] = expect_type(int, output["total"])
+    kwargs["departments"] = _deserialize_department_list(output["departments"], config)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    if "departments" not in output:
+    if "total" not in output:
         raise ServiceError(
-            'Expected to find "departments" in the operation output, but it was not present.'
+            'Expected to find "total" in the operation output, but it was not present.'
         )
-    kwargs["departments"] = _deserialize_department_list(output["departments"], config)
+    kwargs["total"] = expect_type(int, output["total"])
 
     return ListDepartmentsOutput(**kwargs)
 
 
 async def _deserialize_error_list_departments(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -3197,22 +3197,22 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_discovered_recipients := output.get("discoveredRecipients")) is not None:
         kwargs["discovered_recipients"] = _deserialize_discovered_recipient_list(
             _discovered_recipients, config
         )
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     return ListDiscoveredRecipientsOutput(**kwargs)
 
 
 async def _deserialize_error_list_discovered_recipients(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3292,23 +3292,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
     if (_domains := output.get("domains")) is not None:
         kwargs["domains"] = _deserialize_domain_list(_domains, config)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     return ListDomainsOutput(**kwargs)
 
 
 async def _deserialize_error_list_domains(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3341,28 +3341,28 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "total" not in output:
-        raise ServiceError(
-            'Expected to find "total" in the operation output, but it was not present.'
-        )
-    kwargs["total"] = expect_type(int, output["total"])
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
 
     if "employees" not in output:
         raise ServiceError(
             'Expected to find "employees" in the operation output, but it was not present.'
         )
     kwargs["employees"] = _deserialize_employee_list(output["employees"], config)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
+    if "total" not in output:
+        raise ServiceError(
+            'Expected to find "total" in the operation output, but it was not present.'
+        )
+    kwargs["total"] = expect_type(int, output["total"])
 
     return ListEmployeesOutput(**kwargs)
 
 
 async def _deserialize_error_list_employees(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -3447,20 +3447,20 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if (_events := output.get("events")) is not None:
         kwargs["events"] = _deserialize_events_list(_events, config)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     return ListEventsOutput(**kwargs)
 
 
 async def _deserialize_error_list_events(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3644,23 +3644,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_count := output.get("count")) is not None:
-        kwargs["count"] = expect_type(int, _count)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
     if (_resources := output.get("resources")) is not None:
         kwargs["resources"] = _deserialize_resource_inventory_list(_resources, config)
 
+    if (_count := output.get("count")) is not None:
+        kwargs["count"] = expect_type(int, _count)
+
     return ListInventoryResourcesOutput(**kwargs)
 
 
 async def _deserialize_error_list_inventory_resources(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3787,23 +3787,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_logs := output.get("logs")) is not None:
+        kwargs["logs"] = _deserialize_logs_results(_logs, config)
+
     if (_size := output.get("size")) is not None:
         kwargs["size"] = expect_type(int, _size)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    if (_logs := output.get("logs")) is not None:
-        kwargs["logs"] = _deserialize_logs_results(_logs, config)
-
     return ListLogsOutput(**kwargs)
 
 
 async def _deserialize_error_list_logs(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -4049,23 +4049,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
     if (_recipients := output.get("recipients")) is not None:
         kwargs["recipients"] = _deserialize_recipient_list(_recipients, config)
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     return ListRecipientsOutput(**kwargs)
 
 
 async def _deserialize_error_list_recipients(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -4238,20 +4238,20 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_toms := output.get("toms")) is not None:
         kwargs["toms"] = _deserialize_tom_collection(_toms, config)
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     return ListTomsOutput(**kwargs)
 
 
 async def _deserialize_error_list_toms(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -4287,20 +4287,20 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_user_profiles := output.get("userProfiles")) is not None:
         kwargs["user_profiles"] = _deserialize_user_profile_list(_user_profiles, config)
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     return ListUserProfilesOutput(**kwargs)
 
 
 async def _deserialize_error_list_user_profiles(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -5701,25 +5701,25 @@
     kwargs: dict[str, Any] = {"message": default_message}
 
     if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
     output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
-    if (_field_list := output.get("fieldList")) is not None:
-        kwargs["field_list"] = _deserialize_validation_exception_field_list(
-            _field_list, config
-        )
-
     if "message" not in output:
         raise ServiceError(
             'Expected to find "message" in the operation output, but it was not present.'
         )
     kwargs["message"] = expect_type(str, output["message"])
 
+    if (_field_list := output.get("fieldList")) is not None:
+        kwargs["field_list"] = _deserialize_validation_exception_field_list(
+            _field_list, config
+        )
+
     return ValidationException(**kwargs)
 
 
 def _deserialize_account_list_member(
     output: DocumentValue, config: Config
 ) -> AccountListMember:
     if not isinstance(output, dict):
```

### Comparing `borneo_client_python-3.10.2/borneo_client_python/errors.py` & `borneo_client_python-3.10.3/borneo_client_python/errors.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/models.py` & `borneo_client_python-3.10.3/borneo_client_python/models.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/borneo_client_python/serialize.py` & `borneo_client_python-3.10.3/borneo_client_python/serialize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -234,29 +234,29 @@
 ) -> HTTPRequest:
     path = "/assets"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.location_type is not None:
-        result["locationType"] = input.location_type
-
     if input.name is not None:
         result["name"] = input.name
 
+    if input.location_type is not None:
+        result["locationType"] = input.location_type
+
     if input.location_id is not None:
         result["locationId"] = input.location_id
 
-    if input.type is not None:
-        result["type"] = input.type
-
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
+    if input.type is not None:
+        result["type"] = input.type
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -282,22 +282,22 @@
 ) -> HTTPRequest:
     path = "/categories"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.category_label is not None:
-        result["categoryLabel"] = input.category_label
+    if input.description is not None:
+        result["description"] = input.description
 
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
-    if input.description is not None:
-        result["description"] = input.description
+    if input.category_label is not None:
+        result["categoryLabel"] = input.category_label
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -397,44 +397,44 @@
 async def _serialize_create_dpia(input: CreateDpiaInput, config: Config) -> HTTPRequest:
     path = "/dpias"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.additional_information_files is not None:
+        result["additionalInformationFiles"] = input.additional_information_files
+
     if input.additional_information is not None:
         result["additionalInformation"] = input.additional_information
 
     if input.confidentiality is not None:
         result["confidentiality"] = _serialize_dpia_confidentiality_risk(
             input.confidentiality, config
         )
 
-    if input.status is not None:
-        result["status"] = input.status
-
-    if input.additional_information_files is not None:
-        result["additionalInformationFiles"] = input.additional_information_files
-
     if input.privacy_framework is not None:
         result["privacyFramework"] = _serialize_dpia_privacy_framework(
             input.privacy_framework, config
         )
 
     if input.processing_activity_id is not None:
         result["processingActivityId"] = input.processing_activity_id
 
-    if input.integrity is not None:
-        result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
-
     if input.availability is not None:
         result["availability"] = _serialize_dpia_availability_risk(
             input.availability, config
         )
 
+    if input.status is not None:
+        result["status"] = input.status
+
+    if input.integrity is not None:
+        result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -460,47 +460,47 @@
 ) -> HTTPRequest:
     path = "/employees"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.department is not None:
+        result["department"] = input.department
+
     if input.created_by is not None:
         result["createdBy"] = input.created_by
 
+    if input.surname is not None:
+        result["surname"] = input.surname
+
+    if input.end_date is not None:
+        result["endDate"] = input.end_date
+
     if input.manager is not None:
         result["manager"] = input.manager
 
-    if input.department is not None:
-        result["department"] = input.department
+    if input.position is not None:
+        result["position"] = input.position
 
-    if input.end_date is not None:
-        result["endDate"] = input.end_date
+    if input.nif is not None:
+        result["nif"] = input.nif
 
     if input.reference_id is not None:
         result["referenceId"] = input.reference_id
 
-    if input.surname is not None:
-        result["surname"] = input.surname
-
     if input.name is not None:
         result["name"] = input.name
 
     if input.start_date is not None:
         result["startDate"] = input.start_date
 
     if input.email is not None:
         result["email"] = input.email
 
-    if input.position is not None:
-        result["position"] = input.position
-
-    if input.nif is not None:
-        result["nif"] = input.nif
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -526,32 +526,32 @@
 ) -> HTTPRequest:
     path = "/headquarters"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.address is not None:
-        result["address"] = input.address
+    if input.name is not None:
+        result["name"] = input.name
+
+    if input.city is not None:
+        result["city"] = input.city
 
     if input.country is not None:
         result["country"] = input.country
 
     if input.zipcode is not None:
         result["zipcode"] = input.zipcode
 
-    if input.city is not None:
-        result["city"] = input.city
+    if input.address is not None:
+        result["address"] = input.address
 
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
-    if input.name is not None:
-        result["name"] = input.name
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -582,91 +582,91 @@
     result: dict[str, DocumentValue] = {}
 
     if input.retention_period is not None:
         result["retentionPeriod"] = _serialize_retention_period(
             input.retention_period, config
         )
 
+    if input.active is not None:
+        result["active"] = input.active
+
     if input.company_role is not None:
         result["companyRole"] = input.company_role
 
-    if input.infotype_categories is not None:
-        result["infotypeCategories"] = input.infotype_categories
-
-    if input.data_subjects is not None:
-        result["dataSubjects"] = _serialize_data_subject_collection(
-            input.data_subjects, config
-        )
+    if input.infotype_volume is not None:
+        result["infotypeVolume"] = input.infotype_volume
 
-    if input.processing_frequency_comment is not None:
-        result["processingFrequencyComment"] = input.processing_frequency_comment
+    if input.name is not None:
+        result["name"] = input.name
 
-    if input.data_types is not None:
-        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
+    if input.departments is not None:
+        result["departments"] = input.departments
 
-    if input.is_data_stored is not None:
-        result["isDataStored"] = input.is_data_stored
+    if input.additional_info_files is not None:
+        result["additionalInfoFiles"] = input.additional_info_files
 
     if input.recipients is not None:
         result["recipients"] = _serialize_recipient_collection(input.recipients, config)
 
-    if input.active is not None:
-        result["active"] = input.active
+    if input.are_access_requests_managed is not None:
+        result["areAccessRequestsManaged"] = input.are_access_requests_managed
 
-    if input.name is not None:
-        result["name"] = input.name
+    if input.assets is not None:
+        result["assets"] = input.assets
 
-    if input.purpose is not None:
-        result["purpose"] = input.purpose
+    if input.processing_frequency_comment is not None:
+        result["processingFrequencyComment"] = input.processing_frequency_comment
 
-    if input.retention_period_comment is not None:
-        result["retentionPeriodComment"] = input.retention_period_comment
+    if input.lawful_basis is not None:
+        result["lawfulBasis"] = _serialize_lawful_basis_collection(
+            input.lawful_basis, config
+        )
 
-    if input.model_id is not None:
-        result["modelId"] = input.model_id
+    if input.data_subjects is not None:
+        result["dataSubjects"] = _serialize_data_subject_collection(
+            input.data_subjects, config
+        )
 
     if input.contact_person is not None:
         result["contactPerson"] = input.contact_person
 
     if input.data_sources is not None:
         result["dataSources"] = input.data_sources
 
-    if input.lawful_basis is not None:
-        result["lawfulBasis"] = _serialize_lawful_basis_collection(
-            input.lawful_basis, config
-        )
+    if input.model_id is not None:
+        result["modelId"] = input.model_id
 
-    if input.are_access_requests_managed is not None:
-        result["areAccessRequestsManaged"] = input.are_access_requests_managed
+    if input.purpose is not None:
+        result["purpose"] = input.purpose
 
-    if input.additional_info is not None:
-        result["additionalInfo"] = input.additional_info
+    if input.is_data_stored is not None:
+        result["isDataStored"] = input.is_data_stored
 
-    if input.assets is not None:
-        result["assets"] = input.assets
+    if input.retention_period_comment is not None:
+        result["retentionPeriodComment"] = input.retention_period_comment
 
-    if input.additional_info_files is not None:
-        result["additionalInfoFiles"] = input.additional_info_files
+    if input.infotypes is not None:
+        result["infotypes"] = input.infotypes
 
     if input.processing_frequency is not None:
         result["processingFrequency"] = input.processing_frequency
 
-    if input.infotype_volume is not None:
-        result["infotypeVolume"] = input.infotype_volume
-
-    if input.infotypes is not None:
-        result["infotypes"] = input.infotypes
-
     if input.management_methods is not None:
         result["managementMethods"] = _serialize_management_method_collection(
             input.management_methods, config
         )
 
-    if input.departments is not None:
-        result["departments"] = input.departments
+    if input.additional_info is not None:
+        result["additionalInfo"] = input.additional_info
+
+    if input.infotype_categories is not None:
+        result["infotypeCategories"] = input.infotype_categories
+
+    if input.data_types is not None:
+        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -693,55 +693,55 @@
 ) -> HTTPRequest:
     path = "/recipients"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.from_discovered_recipient_id is not None:
+        result["fromDiscoveredRecipientId"] = input.from_discovered_recipient_id
+
     if input.status is not None:
         result["status"] = input.status
 
-    if input.state is not None:
-        result["state"] = input.state
-
     if input.business_name is not None:
         result["businessName"] = input.business_name
 
-    if input.data_storage_location is not None:
-        result["dataStorageLocation"] = input.data_storage_location
+    if input.country is not None:
+        result["country"] = input.country
 
     if input.recipient_warranties is not None:
         result["recipientWarranties"] = input.recipient_warranties
 
     if input.role is not None:
         result["role"] = input.role
 
-    if input.dpa_files is not None:
-        result["dpaFiles"] = input.dpa_files
-
-    if input.category is not None:
-        result["category"] = input.category
-
-    if input.from_discovered_recipient_id is not None:
-        result["fromDiscoveredRecipientId"] = input.from_discovered_recipient_id
+    if input.state is not None:
+        result["state"] = input.state
 
-    if input.name is not None:
-        result["name"] = input.name
+    if input.dpa_status is not None:
+        result["dpaStatus"] = input.dpa_status
 
     if input.dpa is not None:
         result["dpa"] = input.dpa
 
-    if input.dpa_status is not None:
-        result["dpaStatus"] = input.dpa_status
+    if input.name is not None:
+        result["name"] = input.name
 
     if input.recipient_model_id is not None:
         result["recipientModelId"] = input.recipient_model_id
 
-    if input.country is not None:
-        result["country"] = input.country
+    if input.category is not None:
+        result["category"] = input.category
+
+    if input.data_storage_location is not None:
+        result["dataStorageLocation"] = input.data_storage_location
+
+    if input.dpa_files is not None:
+        result["dpaFiles"] = input.dpa_files
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -766,48 +766,48 @@
 async def _serialize_create_scan(input: CreateScanInput, config: Config) -> HTTPRequest:
     path = "/scan"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.resource_type is not None:
-        result["resourceType"] = input.resource_type
+    if input.cron is not None:
+        result["cron"] = input.cron
+
+    if input.schedule is not None:
+        result["schedule"] = _serialize_scan_schedule(input.schedule, config)
+
+    if input.scan_filter is not None:
+        result["scanFilter"] = _serialize_scan_filter_list(input.scan_filter, config)
 
     if input.inspection_policy is not None:
         result["inspectionPolicy"] = _serialize_inspection_policy(
             input.inspection_policy, config
         )
 
-    if input.scan_limits is not None:
-        result["scanLimits"] = _serialize_scan_limits(input.scan_limits, config)
-
-    if input.scan_filter is not None:
-        result["scanFilter"] = _serialize_scan_filter_list(input.scan_filter, config)
-
     if input.connector_id is not None:
         result["connectorId"] = input.connector_id
 
     if input.schedule_type is not None:
         result["scheduleType"] = input.schedule_type
 
-    if input.scan_type is not None:
-        result["scanType"] = input.scan_type
+    if input.name is not None:
+        result["name"] = input.name
 
     if input.resources is not None:
         result["resources"] = _serialize_scan_resources(input.resources, config)
 
-    if input.cron is not None:
-        result["cron"] = input.cron
+    if input.scan_limits is not None:
+        result["scanLimits"] = _serialize_scan_limits(input.scan_limits, config)
 
-    if input.name is not None:
-        result["name"] = input.name
+    if input.scan_type is not None:
+        result["scanType"] = input.scan_type
 
-    if input.schedule is not None:
-        result["schedule"] = _serialize_scan_schedule(input.schedule, config)
+    if input.resource_type is not None:
+        result["resourceType"] = input.resource_type
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -837,75 +837,75 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.automated_decision_making is not None:
         result["automatedDecisionMaking"] = input.automated_decision_making
 
+    if input.processing_confidential_sensitive_data is not None:
+        result["processingConfidentialSensitiveData"] = (
+            input.processing_confidential_sensitive_data
+        )
+
     if input.comment is not None:
         result["comment"] = input.comment
 
+    if input.matching_merging_records_involved is not None:
+        result["matchingMergingRecordsInvolved"] = (
+            input.matching_merging_records_involved
+        )
+
     if input.extensive_automated_evaluation_characteristics is not None:
         result["extensiveAutomatedEvaluationCharacteristics"] = (
             input.extensive_automated_evaluation_characteristics
         )
 
-    if input.innovative_technologies_used is not None:
-        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
-
-    if input.prevent_data_subjects_exercising_their_rights is not None:
-        result["preventDataSubjectsExercisingTheirRights"] = (
-            input.prevent_data_subjects_exercising_their_rights
+    if input.monitoring_publicly_accessible_areas is not None:
+        result["monitoringPubliclyAccessibleAreas"] = (
+            input.monitoring_publicly_accessible_areas
         )
 
-    if input.blacklist is not None:
-        result["blacklist"] = input.blacklist
+    if input.status is not None:
+        result["status"] = input.status
 
-    if input.matching_merging_records_involved is not None:
-        result["matchingMergingRecordsInvolved"] = (
-            input.matching_merging_records_involved
+    if input.large_scale_data_processing is not None:
+        result["largeScaleDataProcessing"] = input.large_scale_data_processing
+
+    if input.processing_activity_id is not None:
+        result["processingActivityId"] = input.processing_activity_id
+
+    if input.processing_vulnerable_data_subject is not None:
+        result["processingVulnerableDataSubject"] = (
+            input.processing_vulnerable_data_subject
         )
 
-    if input.classifying_data_subject is not None:
-        result["classifyingDataSubject"] = input.classifying_data_subject
+    if input.innovative_technologies_used is not None:
+        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
 
     if input.large_scale_processing_sensitive_data is not None:
         result["largeScaleProcessingSensitiveData"] = (
             input.large_scale_processing_sensitive_data
         )
 
-    if input.processing_confidential_sensitive_data is not None:
-        result["processingConfidentialSensitiveData"] = (
-            input.processing_confidential_sensitive_data
-        )
+    if input.blacklist is not None:
+        result["blacklist"] = input.blacklist
+
+    if input.classifying_data_subject is not None:
+        result["classifyingDataSubject"] = input.classifying_data_subject
 
     if input.systematic_monitoring_data_subject is not None:
         result["systematicMonitoringDataSubject"] = (
             input.systematic_monitoring_data_subject
         )
 
-    if input.processing_vulnerable_data_subject is not None:
-        result["processingVulnerableDataSubject"] = (
-            input.processing_vulnerable_data_subject
-        )
-
-    if input.large_scale_data_processing is not None:
-        result["largeScaleDataProcessing"] = input.large_scale_data_processing
-
-    if input.monitoring_publicly_accessible_areas is not None:
-        result["monitoringPubliclyAccessibleAreas"] = (
-            input.monitoring_publicly_accessible_areas
+    if input.prevent_data_subjects_exercising_their_rights is not None:
+        result["preventDataSubjectsExercisingTheirRights"] = (
+            input.prevent_data_subjects_exercising_their_rights
         )
 
-    if input.status is not None:
-        result["status"] = input.status
-
-    if input.processing_activity_id is not None:
-        result["processingActivityId"] = input.processing_activity_id
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1505,23 +1505,23 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.filter is not None:
         result["filter"] = _serialize_account_filter(input.filter, config)
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1589,20 +1589,20 @@
 ) -> HTTPRequest:
     path = "/resource/catalog/listLeafResources"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     if input.source_type is not None:
         result["sourceType"] = input.source_type
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.filter is not None:
@@ -1640,20 +1640,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.filter is not None:
         result["filter"] = _serialize_leaf_resource_filter(input.filter, config)
 
-    if input.source_type is not None:
-        result["sourceType"] = input.source_type
-
     if input.detailed is not None:
         result["detailed"] = input.detailed
 
+    if input.source_type is not None:
+        result["sourceType"] = input.source_type
+
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -1682,23 +1682,23 @@
 ) -> HTTPRequest:
     path = "/connector"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     if input.filter is not None:
         result["filter"] = _serialize_connector_filter(input.filter, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -1727,23 +1727,23 @@
 ) -> HTTPRequest:
     path = "/departments/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.filter is not None:
         result["filter"] = _serialize_department_select_filter(input.filter, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1794,20 +1794,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.filter is not None:
         result["filter"] = _serialize_discovered_recipient_filters(input.filter, config)
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -1863,20 +1863,20 @@
 ) -> HTTPRequest:
     path = "/domains/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -1969,29 +1969,29 @@
 async def _serialize_list_events(input: ListEventsInput, config: Config) -> HTTPRequest:
     path = "/events/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.select is not None:
         result["select"] = input.select
 
     if input.filter is not None:
         result["filter"] = _serialize_events_filter(input.filter, config)
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2092,29 +2092,29 @@
 ) -> HTTPRequest:
     path = "/insight/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.type is not None:
+        result["type"] = input.type
+
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
-    if input.type is not None:
-        result["type"] = input.type
-
     if input.filter is not None:
         result["filter"] = _serialize_inspection_result_filter(input.filter, config)
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2146,20 +2146,20 @@
 
     if input.select is not None:
         result["select"] = input.select
 
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.filter is not None:
         result["filter"] = _serialize_inventory_list_filter(input.filter, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -2188,29 +2188,29 @@
 ) -> HTTPRequest:
     path = "/resource/inventory/list/export"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.select is not None:
-        result["select"] = input.select
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.filter is not None:
         result["filter"] = _serialize_inventory_list_filter(input.filter, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
+    if input.select is not None:
+        result["select"] = input.select
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2234,32 +2234,32 @@
 async def _serialize_list_issues(input: ListIssuesInput, config: Config) -> HTTPRequest:
     path = "/issue/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.select is not None:
-        result["select"] = input.select
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.select is not None:
+        result["select"] = input.select
+
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.include is not None:
         result["include"] = input.include
 
     if input.filter is not None:
         result["filter"] = _serialize_issue_filter(input.filter, config)
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2283,22 +2283,22 @@
 async def _serialize_list_logs(input: ListLogsInput, config: Config) -> HTTPRequest:
     path = "/logs"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    if input.filter is not None:
+        result["filter"] = _serialize_list_logs_filter(input.filter, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.filter is not None:
-        result["filter"] = _serialize_list_logs_filter(input.filter, config)
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -2418,23 +2418,23 @@
         recipient_id=urlquote(input.recipient_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2496,26 +2496,26 @@
 ) -> HTTPRequest:
     path = "/recipients/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     if input.filter is not None:
         result["filter"] = _serialize_recipient_filters(input.filter, config)
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2597,20 +2597,20 @@
 async def _serialize_list_scans(input: ListScansInput, config: Config) -> HTTPRequest:
     path = "/scan/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.filter is not None:
         result["filter"] = _serialize_scan_select_filter(input.filter, config)
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.get_next_execution is not None:
         result["getNextExecution"] = input.get_next_execution
 
     if input.select is not None:
@@ -2646,26 +2646,26 @@
 async def _serialize_list_toms(input: ListTomsInput, config: Config) -> HTTPRequest:
     path = "/toms/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.filter is not None:
-        result["filter"] = _serialize_tom_select_filter(input.filter, config)
-
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.filter is not None:
+        result["filter"] = _serialize_tom_select_filter(input.filter, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2691,28 +2691,28 @@
 ) -> HTTPRequest:
     path = "/user/profile/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.select is not None:
-        result["select"] = input.select
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.filter is not None:
         result["filter"] = _serialize_user_profile_filter(input.filter, config)
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    if input.select is not None:
+        result["select"] = input.select
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3200,24 +3200,24 @@
 ) -> HTTPRequest:
     path = "/resource/tags"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.tag_value is not None:
-        result["tagValue"] = input.tag_value
+    if input.tag_key is not None:
+        result["tagKey"] = input.tag_key
 
     if input.tag_resources is not None:
         result["tagResources"] = _serialize_tag_resource_union(
             input.tag_resources, config
         )
 
-    if input.tag_key is not None:
-        result["tagKey"] = input.tag_key
+    if input.tag_value is not None:
+        result["tagValue"] = input.tag_value
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3249,26 +3249,26 @@
         asset_id=urlquote(input.asset_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.location_id is not None:
-        result["locationId"] = input.location_id
-
     if input.location_type is not None:
         result["locationType"] = input.location_type
 
-    if input.tom_ids is not None:
-        result["tomIds"] = input.tom_ids
-
     if input.name is not None:
         result["name"] = input.name
 
+    if input.location_id is not None:
+        result["locationId"] = input.location_id
+
+    if input.tom_ids is not None:
+        result["tomIds"] = input.tom_ids
+
     if input.type is not None:
         result["type"] = input.type
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -3429,41 +3429,41 @@
         dpia_id=urlquote(input.dpia_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.privacy_framework is not None:
-        result["privacyFramework"] = _serialize_dpia_privacy_framework(
-            input.privacy_framework, config
-        )
-
     if input.availability is not None:
         result["availability"] = _serialize_dpia_availability_risk(
             input.availability, config
         )
 
-    if input.additional_information_files is not None:
-        result["additionalInformationFiles"] = input.additional_information_files
+    if input.privacy_framework is not None:
+        result["privacyFramework"] = _serialize_dpia_privacy_framework(
+            input.privacy_framework, config
+        )
 
     if input.confidentiality is not None:
         result["confidentiality"] = _serialize_dpia_confidentiality_risk(
             input.confidentiality, config
         )
 
-    if input.status is not None:
-        result["status"] = input.status
+    if input.additional_information_files is not None:
+        result["additionalInformationFiles"] = input.additional_information_files
 
     if input.additional_information is not None:
         result["additionalInformation"] = input.additional_information
 
     if input.integrity is not None:
         result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
 
+    if input.status is not None:
+        result["status"] = input.status
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3500,35 +3500,35 @@
 
     if input.start_date is not None:
         result["startDate"] = input.start_date
 
     if input.manager is not None:
         result["manager"] = input.manager
 
-    if input.name is not None:
-        result["name"] = input.name
+    if input.end_date is not None:
+        result["endDate"] = input.end_date
 
     if input.department is not None:
         result["department"] = input.department
 
-    if input.email is not None:
-        result["email"] = input.email
-
     if input.nif is not None:
         result["nif"] = input.nif
 
-    if input.end_date is not None:
-        result["endDate"] = input.end_date
+    if input.name is not None:
+        result["name"] = input.name
 
-    if input.position is not None:
-        result["position"] = input.position
+    if input.email is not None:
+        result["email"] = input.email
 
     if input.surname is not None:
         result["surname"] = input.surname
 
+    if input.position is not None:
+        result["position"] = input.position
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3565,26 +3565,26 @@
 
     if input.name is not None:
         result["name"] = input.name
 
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
-    if input.zipcode is not None:
-        result["zipcode"] = input.zipcode
-
-    if input.country is not None:
-        result["country"] = input.country
-
     if input.city is not None:
         result["city"] = input.city
 
     if input.address is not None:
         result["address"] = input.address
 
+    if input.zipcode is not None:
+        result["zipcode"] = input.zipcode
+
+    if input.country is not None:
+        result["country"] = input.country
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3615,96 +3615,96 @@
         processing_activity_id=urlquote(input.processing_activity_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.processing_frequency is not None:
-        result["processingFrequency"] = input.processing_frequency
-
     if input.assets is not None:
         result["assets"] = input.assets
 
+    if input.processing_frequency is not None:
+        result["processingFrequency"] = input.processing_frequency
+
     if input.recipients is not None:
         result["recipients"] = _serialize_recipient_collection(input.recipients, config)
 
-    if input.contact_person is not None:
-        result["contactPerson"] = input.contact_person
-
-    if input.data_types is not None:
-        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
-
-    if input.lawful_basis is not None:
-        result["lawfulBasis"] = _serialize_lawful_basis_collection(
-            input.lawful_basis, config
-        )
-
-    if input.infotype_volume is not None:
-        result["infotypeVolume"] = input.infotype_volume
-
-    if input.departments is not None:
-        result["departments"] = input.departments
-
-    if input.additional_info is not None:
-        result["additionalInfo"] = input.additional_info
-
     if input.are_access_requests_managed is not None:
         result["areAccessRequestsManaged"] = input.are_access_requests_managed
 
-    if input.retention_period is not None:
-        result["retentionPeriod"] = _serialize_retention_period(
-            input.retention_period, config
-        )
-
     if input.data_sources is not None:
         result["dataSources"] = input.data_sources
 
-    if input.management_methods is not None:
-        result["managementMethods"] = _serialize_management_method_collection(
-            input.management_methods, config
-        )
-
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
     if input.additional_info_files is not None:
         result["additionalInfoFiles"] = input.additional_info_files
 
+    if input.is_data_stored is not None:
+        result["isDataStored"] = input.is_data_stored
+
+    if input.retention_period_comment is not None:
+        result["retentionPeriodComment"] = input.retention_period_comment
+
+    if input.infotype_volume is not None:
+        result["infotypeVolume"] = input.infotype_volume
+
+    if input.purpose is not None:
+        result["purpose"] = input.purpose
+
+    if input.data_types is not None:
+        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
+
+    if input.infotype_categories is not None:
+        result["infotypeCategories"] = input.infotype_categories
+
+    if input.contact_person is not None:
+        result["contactPerson"] = input.contact_person
+
     if input.data_subjects is not None:
         result["dataSubjects"] = _serialize_data_subject_collection(
             input.data_subjects, config
         )
 
-    if input.infotype_categories is not None:
-        result["infotypeCategories"] = input.infotype_categories
-
     if input.active is not None:
         result["active"] = input.active
 
+    if input.additional_info is not None:
+        result["additionalInfo"] = input.additional_info
+
+    if input.name is not None:
+        result["name"] = input.name
+
+    if input.retention_period is not None:
+        result["retentionPeriod"] = _serialize_retention_period(
+            input.retention_period, config
+        )
+
     if input.processing_frequency_comment is not None:
         result["processingFrequencyComment"] = input.processing_frequency_comment
 
-    if input.purpose is not None:
-        result["purpose"] = input.purpose
+    if input.model_id is not None:
+        result["modelId"] = input.model_id
 
     if input.company_role is not None:
         result["companyRole"] = input.company_role
 
-    if input.model_id is not None:
-        result["modelId"] = input.model_id
-
-    if input.name is not None:
-        result["name"] = input.name
+    if input.management_methods is not None:
+        result["managementMethods"] = _serialize_management_method_collection(
+            input.management_methods, config
+        )
 
-    if input.retention_period_comment is not None:
-        result["retentionPeriodComment"] = input.retention_period_comment
+    if input.departments is not None:
+        result["departments"] = input.departments
 
-    if input.is_data_stored is not None:
-        result["isDataStored"] = input.is_data_stored
+    if input.lawful_basis is not None:
+        result["lawfulBasis"] = _serialize_lawful_basis_collection(
+            input.lawful_basis, config
+        )
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3736,50 +3736,50 @@
         recipient_id=urlquote(input.recipient_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.category is not None:
-        result["category"] = input.category
-
-    if input.dpa_status is not None:
-        result["dpaStatus"] = input.dpa_status
-
     if input.name is not None:
         result["name"] = input.name
 
     if input.recipient_warranties is not None:
         result["recipientWarranties"] = input.recipient_warranties
 
     if input.business_name is not None:
         result["businessName"] = input.business_name
 
+    if input.category is not None:
+        result["category"] = input.category
+
+    if input.status is not None:
+        result["status"] = input.status
+
     if input.state is not None:
         result["state"] = input.state
 
     if input.country is not None:
         result["country"] = input.country
 
     if input.role is not None:
         result["role"] = input.role
 
-    if input.status is not None:
-        result["status"] = input.status
+    if input.dpa_files is not None:
+        result["dpaFiles"] = input.dpa_files
 
     if input.dpa is not None:
         result["dpa"] = input.dpa
 
+    if input.dpa_status is not None:
+        result["dpaStatus"] = input.dpa_status
+
     if input.data_storage_location is not None:
         result["dataStorageLocation"] = input.data_storage_location
 
-    if input.dpa_files is not None:
-        result["dpaFiles"] = input.dpa_files
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3810,74 +3810,74 @@
         threshold_id=urlquote(input.threshold_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.status is not None:
-        result["status"] = input.status
-
-    if input.innovative_technologies_used is not None:
-        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
-
     if input.extensive_automated_evaluation_characteristics is not None:
         result["extensiveAutomatedEvaluationCharacteristics"] = (
             input.extensive_automated_evaluation_characteristics
         )
 
-    if input.blacklist is not None:
-        result["blacklist"] = input.blacklist
-
-    if input.automated_decision_making is not None:
-        result["automatedDecisionMaking"] = input.automated_decision_making
+    if input.comment is not None:
+        result["comment"] = input.comment
 
-    if input.matching_merging_records_involved is not None:
-        result["matchingMergingRecordsInvolved"] = (
-            input.matching_merging_records_involved
+    if input.monitoring_publicly_accessible_areas is not None:
+        result["monitoringPubliclyAccessibleAreas"] = (
+            input.monitoring_publicly_accessible_areas
         )
 
-    if input.prevent_data_subjects_exercising_their_rights is not None:
-        result["preventDataSubjectsExercisingTheirRights"] = (
-            input.prevent_data_subjects_exercising_their_rights
+    if input.large_scale_data_processing is not None:
+        result["largeScaleDataProcessing"] = input.large_scale_data_processing
+
+    if input.processing_vulnerable_data_subject is not None:
+        result["processingVulnerableDataSubject"] = (
+            input.processing_vulnerable_data_subject
         )
 
-    if input.classifying_data_subject is not None:
-        result["classifyingDataSubject"] = input.classifying_data_subject
+    if input.status is not None:
+        result["status"] = input.status
+
+    if input.large_scale_processing_sensitive_data is not None:
+        result["largeScaleProcessingSensitiveData"] = (
+            input.large_scale_processing_sensitive_data
+        )
 
     if input.systematic_monitoring_data_subject is not None:
         result["systematicMonitoringDataSubject"] = (
             input.systematic_monitoring_data_subject
         )
 
+    if input.blacklist is not None:
+        result["blacklist"] = input.blacklist
+
+    if input.matching_merging_records_involved is not None:
+        result["matchingMergingRecordsInvolved"] = (
+            input.matching_merging_records_involved
+        )
+
     if input.processing_confidential_sensitive_data is not None:
         result["processingConfidentialSensitiveData"] = (
             input.processing_confidential_sensitive_data
         )
 
-    if input.large_scale_processing_sensitive_data is not None:
-        result["largeScaleProcessingSensitiveData"] = (
-            input.large_scale_processing_sensitive_data
-        )
-
-    if input.large_scale_data_processing is not None:
-        result["largeScaleDataProcessing"] = input.large_scale_data_processing
+    if input.automated_decision_making is not None:
+        result["automatedDecisionMaking"] = input.automated_decision_making
 
-    if input.comment is not None:
-        result["comment"] = input.comment
+    if input.innovative_technologies_used is not None:
+        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
 
-    if input.processing_vulnerable_data_subject is not None:
-        result["processingVulnerableDataSubject"] = (
-            input.processing_vulnerable_data_subject
+    if input.prevent_data_subjects_exercising_their_rights is not None:
+        result["preventDataSubjectsExercisingTheirRights"] = (
+            input.prevent_data_subjects_exercising_their_rights
         )
 
-    if input.monitoring_publicly_accessible_areas is not None:
-        result["monitoringPubliclyAccessibleAreas"] = (
-            input.monitoring_publicly_accessible_areas
-        )
+    if input.classifying_data_subject is not None:
+        result["classifyingDataSubject"] = input.classifying_data_subject
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3910,20 +3910,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.status is not None:
         result["status"] = input.status
 
-    if input.document_files is not None:
-        result["documentFiles"] = input.document_files
-
     if input.note is not None:
         result["note"] = input.note
 
+    if input.document_files is not None:
+        result["documentFiles"] = input.document_files
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
```

### Comparing `borneo_client_python-3.10.2/borneo_client_python.egg-info/PKG-INFO` & `borneo_client_python-3.10.3/borneo_client_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo_client_python
-Version: 3.10.2
+Version: 3.10.3
 Summary: borneo_client_python client
 License: Apache-2.0
 Keywords: smithy,borneo_client_python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
```

### Comparing `borneo_client_python-3.10.2/borneo_client_python.egg-info/SOURCES.txt` & `borneo_client_python-3.10.3/borneo_client_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+borneo_auth_provider/borneo_auth_provider.py
 borneo_client_python/__init__.py
 borneo_client_python/auth.py
 borneo_client_python/client.py
 borneo_client_python/config.py
 borneo_client_python/deserialize.py
 borneo_client_python/errors.py
 borneo_client_python/models.py
```

### Comparing `borneo_client_python-3.10.2/pyproject.toml` & `borneo_client_python-3.10.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "borneo_client_python"
-version = "3.10.2"
+version = "3.10.3"
 description = "borneo_client_python client"
 readme = "README.md"
 requires-python = ">=3.12"
 keywords = ["smithy", "borneo_client_python"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `borneo_client_python-3.10.2/smithy_aws_core/__init__.py` & `borneo_client_python-3.10.3/smithy_aws_core/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_aws_core/identity.py` & `borneo_client_python-3.10.3/smithy_aws_core/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/__init__.py` & `borneo_client_python-3.10.3/smithy_core/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/aio/interfaces/__init__.py` & `borneo_client_python-3.10.3/smithy_core/aio/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/aio/interfaces/identity.py` & `borneo_client_python-3.10.3/smithy_core/aio/interfaces/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/aio/types.py` & `borneo_client_python-3.10.3/smithy_core/aio/types.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/aio/utils.py` & `borneo_client_python-3.10.3/smithy_core/aio/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/documents.py` & `borneo_client_python-3.10.3/smithy_core/documents.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/exceptions.py` & `borneo_client_python-3.10.3/smithy_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/identity.py` & `borneo_client_python-3.10.3/smithy_core/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/interceptors.py` & `borneo_client_python-3.10.3/smithy_core/interceptors.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/interfaces/__init__.py` & `borneo_client_python-3.10.3/smithy_core/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/interfaces/identity.py` & `borneo_client_python-3.10.3/smithy_core/interfaces/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/interfaces/retries.py` & `borneo_client_python-3.10.3/smithy_core/interfaces/retries.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/retries.py` & `borneo_client_python-3.10.3/smithy_core/retries.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/rfc3986.py` & `borneo_client_python-3.10.3/smithy_core/rfc3986.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/schemas.py` & `borneo_client_python-3.10.3/smithy_core/schemas.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/shapes.py` & `borneo_client_python-3.10.3/smithy_core/shapes.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/types.py` & `borneo_client_python-3.10.3/smithy_core/types.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_core/utils.py` & `borneo_client_python-3.10.3/smithy_core/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/__init__.py` & `borneo_client_python-3.10.3/smithy_http/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/__init__.py` & `borneo_client_python-3.10.3/smithy_http/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/aiohttp.py` & `borneo_client_python-3.10.3/smithy_http/aio/aiohttp.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/auth/apikey.py` & `borneo_client_python-3.10.3/smithy_http/aio/auth/apikey.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/crt.py` & `borneo_client_python-3.10.3/smithy_http/aio/crt.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/endpoints.py` & `borneo_client_python-3.10.3/smithy_http/aio/endpoints.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/identity/apikey.py` & `borneo_client_python-3.10.3/smithy_http/aio/identity/apikey.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/interfaces/__init__.py` & `borneo_client_python-3.10.3/smithy_http/aio/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/interfaces/auth.py` & `borneo_client_python-3.10.3/smithy_http/aio/interfaces/auth.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/aio/restjson.py` & `borneo_client_python-3.10.3/smithy_http/aio/restjson.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/interfaces/__init__.py` & `borneo_client_python-3.10.3/smithy_http/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/restjson.py` & `borneo_client_python-3.10.3/smithy_http/restjson.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/smithy_http/utils.py` & `borneo_client_python-3.10.3/smithy_http/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.2/tests/test_protocol.py` & `borneo_client_python-3.10.3/tests/test_protocol.py`

 * *Files identical despite different names*


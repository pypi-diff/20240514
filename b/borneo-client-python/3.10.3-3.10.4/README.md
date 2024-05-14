# Comparing `tmp/borneo_client_python-3.10.3.tar.gz` & `tmp/borneo_client_python-3.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borneo_client_python-3.10.3.tar", last modified: Mon May 13 13:56:01 2024, max compression
+gzip compressed data, was "borneo_client_python-3.10.4.tar", last modified: Tue May 14 04:01:43 2024, max compression
```

## Comparing `borneo_client_python-3.10.3.tar` & `borneo_client_python-3.10.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.846844 borneo_client_python-3.10.3/borneo_auth_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/borneo_auth_provider/borneo_auth_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/borneo_client_python/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   125040 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   310639 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   181979 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)   138321 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/borneo_client_python/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/borneo_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 13:56:01.000000 borneo_client_python-3.10.3/borneo_client_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/smithy_aws_core/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.850844 borneo_client_python-3.10.3/smithy_aws_core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_aws_core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/aio/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/interfaces/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/aio/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    28327 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interceptors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/interfaces/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/rfc3986.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.854844 borneo_client_python-3.10.3/smithy_http/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/auth/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/crt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/identity/apikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/aio/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/interfaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/aio/restjson.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/smithy_http/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/restjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-13 13:48:40.000000 borneo_client_python-3.10.3/smithy_http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:01.858844 borneo_client_python-3.10.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-13 13:55:56.000000 borneo_client_python-3.10.3/tests/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.512517 borneo_client_python-3.10.4/borneo_auth_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/borneo_auth_provider/borneo_auth_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.512517 borneo_client_python-3.10.4/borneo_client_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125040 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   310639 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181979 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138321 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/borneo_client_python/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/borneo_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-14 04:01:43.000000 borneo_client_python-3.10.4/borneo_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 04:01:43.000000 borneo_client_python-3.10.4/borneo_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:01:43.000000 borneo_client_python-3.10.4/borneo_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 04:01:43.000000 borneo_client_python-3.10.4/borneo_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 04:01:43.000000 borneo_client_python-3.10.4/borneo_client_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.516517 borneo_client_python-3.10.4/smithy_aws_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_aws_core/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_aws_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_aws_core/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.516517 borneo_client_python-3.10.4/smithy_aws_core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_aws_core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_aws_core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.516517 borneo_client_python-3.10.4/smithy_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_core/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_core/aio/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/aio/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/aio/interfaces/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/aio/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/aio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28327 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/interceptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/interfaces/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/interfaces/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/interfaces/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/rfc3986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_http/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.520517 borneo_client_python-3.10.4/smithy_http/aio/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/auth/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/crt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/smithy_http/aio/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/identity/apikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/smithy_http/aio/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/interfaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/aio/restjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/smithy_http/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/restjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-14 03:54:37.000000 borneo_client_python-3.10.4/smithy_http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:01:43.524517 borneo_client_python-3.10.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 04:01:36.000000 borneo_client_python-3.10.4/tests/test_protocol.py
```

### Comparing `borneo_client_python-3.10.3/LICENSE` & `borneo_client_python-3.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/README.md` & `borneo_client_python-3.10.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,35 +9,44 @@
 - `pip install borneo-python-client`
 
 ### Usage
 
 To send a request using `@borneodata/borneo-client` and an example command:
 
 ```python
-# import { BorneoClient, DescribeCatalogResourceCommand } from '@borneodata/borneo-client';
-# import { BorneoAuthProvider } from '@borneodata/borneo-client-auth-provider';
+import asyncio
+import aiohttp
+from borneo_client_python.client import Borneo
+from borneo_client_python.config import Config, IdentityResolver, ApiKeyIdentity, IdentityProperties, ApiKeyIdentity
+from borneo_client_python.models import ListLogsInput, ListLogsFilter
+from borneo_auth_provider import borneo_auth_provider
+
+# Replace the service account key file location
+auth_provider = borneo_auth_provider.BorneoAuthProviderConfig.fromConfigFile('../Borneo-Service-Account-Token.json')
+
+class ApiKeyIdentityResolver(IdentityResolver[ApiKeyIdentity, IdentityProperties]):
+    async def get_identity(self, identity_properties) -> ApiKeyIdentity:
+        token = auth_provider.get_api_key()
+        return ApiKeyIdentity(api_key=token)
+        
+async def main() -> None:
+    async with aiohttp.ClientSession() as session:
+        endpoint_uri = auth_provider.get_api_endpoint()
+        client = Borneo(Config(endpoint_uri=endpoint_uri, api_key_identity_resolver=ApiKeyIdentityResolver(), retry_strategy=None))
+
+        # Payload inputs
+        input = ListLogsInput(ListLogsFilter())
+        data = await client.list_logs(input)
+
+        # Data output here
+        print(data)
+        await session.close()
 
-# async function getData() {
-#   const authProvider = await BorneoAuthProvider.fromConfigFile(`./Borneo-Service-Account-Token.json`);
-#   const client = new BorneoClient({
-#     endpoint: authProvider.getApiEndpoint(),
-#     apiKey: authProvider.getApiKey()
-#   });
-#   const input = {
-#     resourceId: '1bea4d02-8ce7-11ee-942f-3c7d0a1cd55d'
-#   };
-#   const cmd = new DescribeCatalogResourceCommand(input)
-#   const data = await client.send(cmd)
-  
-#   // The data is returned here and can be further processed.
-#   console.log(data)
-#   return data
-# }
-
-# getData()
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
 ### Config
 ```
 const config = {
   clientId: 'STRING_VALUE', /* required */
   region: 'STRING_VALUE', /* required */
```

### Comparing `borneo_client_python-3.10.3/borneo_auth_provider/borneo_auth_provider.py` & `borneo_client_python-3.10.4/borneo_auth_provider/borneo_auth_provider.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/auth.py` & `borneo_client_python-3.10.4/borneo_client_python/auth.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/client.py` & `borneo_client_python-3.10.4/borneo_client_python/client.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/config.py` & `borneo_client_python-3.10.4/borneo_client_python/config.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/deserialize.py` & `borneo_client_python-3.10.4/borneo_client_python/deserialize.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/errors.py` & `borneo_client_python-3.10.4/borneo_client_python/errors.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/models.py` & `borneo_client_python-3.10.4/borneo_client_python/models.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/borneo_client_python/serialize.py` & `borneo_client_python-3.10.4/borneo_client_python/serialize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -285,20 +285,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.description is not None:
         result["description"] = input.description
 
-    if input.infotypes is not None:
-        result["infotypes"] = input.infotypes
-
     if input.category_label is not None:
         result["categoryLabel"] = input.category_label
 
+    if input.infotypes is not None:
+        result["infotypes"] = input.infotypes
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -413,25 +413,25 @@
         )
 
     if input.privacy_framework is not None:
         result["privacyFramework"] = _serialize_dpia_privacy_framework(
             input.privacy_framework, config
         )
 
+    if input.status is not None:
+        result["status"] = input.status
+
     if input.processing_activity_id is not None:
         result["processingActivityId"] = input.processing_activity_id
 
     if input.availability is not None:
         result["availability"] = _serialize_dpia_availability_risk(
             input.availability, config
         )
 
-    if input.status is not None:
-        result["status"] = input.status
-
     if input.integrity is not None:
         result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -772,28 +772,28 @@
 
     if input.cron is not None:
         result["cron"] = input.cron
 
     if input.schedule is not None:
         result["schedule"] = _serialize_scan_schedule(input.schedule, config)
 
+    if input.schedule_type is not None:
+        result["scheduleType"] = input.schedule_type
+
     if input.scan_filter is not None:
         result["scanFilter"] = _serialize_scan_filter_list(input.scan_filter, config)
 
     if input.inspection_policy is not None:
         result["inspectionPolicy"] = _serialize_inspection_policy(
             input.inspection_policy, config
         )
 
     if input.connector_id is not None:
         result["connectorId"] = input.connector_id
 
-    if input.schedule_type is not None:
-        result["scheduleType"] = input.schedule_type
-
     if input.name is not None:
         result["name"] = input.name
 
     if input.resources is not None:
         result["resources"] = _serialize_scan_resources(input.resources, config)
 
     if input.scan_limits is not None:
@@ -2234,20 +2234,20 @@
 async def _serialize_list_issues(input: ListIssuesInput, config: Config) -> HTTPRequest:
     path = "/issue/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
-
     if input.select is not None:
         result["select"] = input.select
 
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
+
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.include is not None:
         result["include"] = input.include
 
     if input.filter is not None:
@@ -3633,20 +3633,20 @@
 
     if input.data_sources is not None:
         result["dataSources"] = input.data_sources
 
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
-    if input.additional_info_files is not None:
-        result["additionalInfoFiles"] = input.additional_info_files
-
     if input.is_data_stored is not None:
         result["isDataStored"] = input.is_data_stored
 
+    if input.additional_info_files is not None:
+        result["additionalInfoFiles"] = input.additional_info_files
+
     if input.retention_period_comment is not None:
         result["retentionPeriodComment"] = input.retention_period_comment
 
     if input.infotype_volume is not None:
         result["infotypeVolume"] = input.infotype_volume
 
     if input.purpose is not None:
```

### Comparing `borneo_client_python-3.10.3/borneo_client_python.egg-info/SOURCES.txt` & `borneo_client_python-3.10.4/borneo_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/pyproject.toml` & `borneo_client_python-3.10.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Code generated by smithy-python-codegen DO NOT EDIT.
 
 [build-system]
-requires = ["setuptools", "setuptools-scm", "wheel"]
+requires = ["setuptools", "setuptools-scm", "wheel", "pyjwt==2.0.0", "boto3==1.34.103", "botocore==1.34.103"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "borneo_client_python"
-version = "3.10.3"
+version = "3.10.4"
 description = "borneo_client_python client"
 readme = "README.md"
 requires-python = ">=3.12"
 keywords = ["smithy", "borneo_client_python"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `borneo_client_python-3.10.3/smithy_aws_core/__init__.py` & `borneo_client_python-3.10.4/smithy_aws_core/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_aws_core/identity.py` & `borneo_client_python-3.10.4/smithy_aws_core/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/__init__.py` & `borneo_client_python-3.10.4/smithy_core/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/aio/interfaces/__init__.py` & `borneo_client_python-3.10.4/smithy_core/aio/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/aio/interfaces/identity.py` & `borneo_client_python-3.10.4/smithy_core/aio/interfaces/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/aio/types.py` & `borneo_client_python-3.10.4/smithy_core/aio/types.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/aio/utils.py` & `borneo_client_python-3.10.4/smithy_core/aio/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/documents.py` & `borneo_client_python-3.10.4/smithy_core/documents.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/exceptions.py` & `borneo_client_python-3.10.4/smithy_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/identity.py` & `borneo_client_python-3.10.4/smithy_core/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/interceptors.py` & `borneo_client_python-3.10.4/smithy_core/interceptors.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/interfaces/__init__.py` & `borneo_client_python-3.10.4/smithy_core/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/interfaces/identity.py` & `borneo_client_python-3.10.4/smithy_core/interfaces/identity.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/interfaces/retries.py` & `borneo_client_python-3.10.4/smithy_core/interfaces/retries.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/retries.py` & `borneo_client_python-3.10.4/smithy_core/retries.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/rfc3986.py` & `borneo_client_python-3.10.4/smithy_core/rfc3986.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/schemas.py` & `borneo_client_python-3.10.4/smithy_core/schemas.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/shapes.py` & `borneo_client_python-3.10.4/smithy_core/shapes.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/types.py` & `borneo_client_python-3.10.4/smithy_core/types.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_core/utils.py` & `borneo_client_python-3.10.4/smithy_core/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/__init__.py` & `borneo_client_python-3.10.4/smithy_http/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/__init__.py` & `borneo_client_python-3.10.4/smithy_http/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/aiohttp.py` & `borneo_client_python-3.10.4/smithy_http/aio/aiohttp.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/auth/apikey.py` & `borneo_client_python-3.10.4/smithy_http/aio/auth/apikey.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/crt.py` & `borneo_client_python-3.10.4/smithy_http/aio/crt.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/endpoints.py` & `borneo_client_python-3.10.4/smithy_http/aio/endpoints.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/identity/apikey.py` & `borneo_client_python-3.10.4/smithy_http/aio/identity/apikey.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/interfaces/__init__.py` & `borneo_client_python-3.10.4/smithy_http/aio/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/interfaces/auth.py` & `borneo_client_python-3.10.4/smithy_http/aio/interfaces/auth.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/aio/restjson.py` & `borneo_client_python-3.10.4/smithy_http/aio/restjson.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/interfaces/__init__.py` & `borneo_client_python-3.10.4/smithy_http/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/restjson.py` & `borneo_client_python-3.10.4/smithy_http/restjson.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/smithy_http/utils.py` & `borneo_client_python-3.10.4/smithy_http/utils.py`

 * *Files identical despite different names*

### Comparing `borneo_client_python-3.10.3/tests/test_protocol.py` & `borneo_client_python-3.10.4/tests/test_protocol.py`

 * *Files identical despite different names*


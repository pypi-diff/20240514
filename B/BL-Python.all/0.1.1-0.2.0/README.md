# Comparing `tmp/BL_Python.all-0.1.1.tar.gz` & `tmp/bl_python_all-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.all-0.1.1.tar", last modified: Fri Feb 16 20:12:57 2024, max compression
+gzip compressed data, was "bl_python_all-0.2.0.tar", last modified: Tue May 14 21:57:13 2024, max compression
```

## Comparing `BL_Python.all-0.1.1.tar` & `bl_python_all-0.2.0.tar`

### file list

```diff
@@ -1,200 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.495194 BL_Python.all-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.495194 BL_Python.all-0.1.1/BL_Python.all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-16 20:12:57.000000 BL_Python.all-0.1.1/BL_Python.all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-02-16 20:12:57.000000 BL_Python.all-0.1.1/BL_Python.all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 20:12:57.000000 BL_Python.all-0.1.1/BL_Python.all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-16 20:12:57.000000 BL_Python.all-0.1.1/BL_Python.all.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-16 20:12:57.000000 BL_Python.all-0.1.1/BL_Python.all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-16 20:12:57.495194 BL_Python.all-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 20:12:57.495194 BL_Python.all-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/AWS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.459190 BL_Python.all-0.1.1/src/AWS/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/AWS/BL_Python/AWS/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/AWS/BL_Python/AWS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/AWS/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/GitHub/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.459190 BL_Python.all-0.1.1/src/GitHub/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/GitHub/BL_Python/GitHub/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/GitHub/BL_Python/GitHub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/GitHub/BL_Python/GitHub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/GitHub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.467191 BL_Python.all-0.1.1/src/database/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.459190 BL_Python.all-0.1.1/src/database/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/database/BL_Python/database/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/database/BL_Python/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/database/BL_Python/database/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/database/BL_Python/database/dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/database/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/development/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.459190 BL_Python.all-0.1.1/src/development/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/development/BL_Python/development/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/development/BL_Python/development/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/development/BL_Python/development/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/development/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/platform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/src/platform/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/platform/BL_Python/platform/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/platform/BL_Python/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/platform/BL_Python/platform/db_feature_flag_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/platform/BL_Python/platform/feature_flag_router.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/programming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/src/programming/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/programming/BL_Python/programming/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/programming/BL_Python/programming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/programming/BL_Python/programming/dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/programming/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/testing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/src/testing/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/testing/BL_Python/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/testing/BL_Python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/testing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.471192 BL_Python.all-0.1.1/src/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/src/web/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.475192 BL_Python.all-0.1.1/src/web/BL_Python/web/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/BL_Python/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/BL_Python/web/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/BL_Python/web/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/src/web/typings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.479192 BL_Python.all-0.1.1/src/web/typings/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.479192 BL_Python.all-0.1.1/src/web/typings/connexion/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/apps/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/apps/asynchronous.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/apps/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/datastructures.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.479192 BL_Python.all-0.1.1/src/web/typings/connexion/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/decorators/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/decorators/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/decorators/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.479192 BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/starlette.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/http_facts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/json_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/jsonifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/lifecycle.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/lifespan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/request_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/response_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/routing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/middleware/swagger_ui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/mock.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/connexion/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/operations/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/operations/openapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/operations/swagger2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/problem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/spec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/uri_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/connexion/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/validators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/validators/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/validators/form_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/validators/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/connexion/validators/parameter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/json_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/connexion/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.483193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/fastapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/fastapi/implementation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/flask/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/quart/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/quart/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework/sanic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/framework_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/src/web/typings/json_logging/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.463191 BL_Python.all-0.1.1/typings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/typings/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/typings/alembic/autogenerate/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/autogenerate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/autogenerate/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/autogenerate/compare.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/autogenerate/render.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/autogenerate/rewriter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/command.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30441 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.487193 BL_Python.all-0.1.1/typings/alembic/ddl/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/impl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/mssql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/oracle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/postgresql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/ddl/sqlite.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/migration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47452 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/op.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.491194 BL_Python.all-0.1.1/typings/alembic/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    64169 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/ops.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/schemaobj.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/operations/toimpl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.491194 BL_Python.all-0.1.1/typings/alembic/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35766 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/runtime/environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/runtime/migration.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.491194 BL_Python.all-0.1.1/typings/alembic/script/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/script/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/script/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/script/revision.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/script/write_hooks.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.491194 BL_Python.all-0.1.1/typings/alembic/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/testing/assertions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/testing/env.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/testing/fixtures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/testing/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:12:57.495194 BL_Python.all-0.1.1/typings/alembic/util/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/editor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/langhelpers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/messaging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/pyfiles.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-16 20:12:49.000000 BL_Python.all-0.1.1/typings/alembic/util/sqla_compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/BL_Python.all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-14 21:57:13.000000 bl_python_all-0.2.0/BL_Python.all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-14 21:57:13.000000 bl_python_all-0.2.0/BL_Python.all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:57:13.000000 bl_python_all-0.2.0/BL_Python.all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 21:57:13.000000 bl_python_all-0.2.0/BL_Python.all.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 21:57:13.000000 bl_python_all-0.2.0/BL_Python.all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:57:13.386737 bl_python_all-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/AWS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/AWS/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/AWS/BL_Python/AWS/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/AWS/BL_Python/AWS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/AWS/BL_Python/AWS/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/AWS/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/GitHub/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/GitHub/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/GitHub/BL_Python/GitHub/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/GitHub/BL_Python/GitHub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/GitHub/BL_Python/GitHub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/GitHub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/database/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/database/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/database/BL_Python/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/database/BL_Python/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/database/BL_Python/database/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/database/BL_Python/database/dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/database/BL_Python/database/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/database/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/development/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/development/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/development/BL_Python/development/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/development/BL_Python/development/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/development/BL_Python/development/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/development/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.338737 bl_python_all-0.2.0/src/identity/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/identity/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/identity/BL_Python/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/identity/BL_Python/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/identity/BL_Python/identity/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/identity/BL_Python/identity/dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/identity/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.326737 bl_python_all-0.2.0/src/platform/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/platform/BL_Python/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/platform/BL_Python/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/platform/BL_Python/platform/dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/programming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.330736 bl_python_all-0.2.0/src/programming/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/programming/BL_Python/programming/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/programming/BL_Python/programming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/programming/BL_Python/programming/dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/programming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/testing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.330736 bl_python_all-0.2.0/src/testing/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/testing/BL_Python/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/testing/BL_Python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/testing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.330736 bl_python_all-0.2.0/src/web/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/src/web/BL_Python/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/web/BL_Python/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/web/BL_Python/web/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/web/BL_Python/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/src/web/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.334736 bl_python_all-0.2.0/typings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.342737 bl_python_all-0.2.0/typings/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.346737 bl_python_all-0.2.0/typings/alembic/autogenerate/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/autogenerate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/autogenerate/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/autogenerate/compare.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/autogenerate/render.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/autogenerate/rewriter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29823 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.346737 bl_python_all-0.2.0/typings/alembic/ddl/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/_autogen.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/mssql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/oracle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/postgresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/ddl/sqlite.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/migration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    48244 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/op.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.346737 bl_python_all-0.2.0/typings/alembic/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    64920 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    62676 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/schemaobj.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/operations/toimpl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.350736 bl_python_all-0.2.0/typings/alembic/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35932 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/runtime/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/runtime/migration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.350736 bl_python_all-0.2.0/typings/alembic/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/script/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/script/revision.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/script/write_hooks.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.350736 bl_python_all-0.2.0/typings/alembic/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/testing/assertions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/testing/env.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/testing/fixtures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/testing/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.350736 bl_python_all-0.2.0/typings/alembic/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/editor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/langhelpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/messaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/pyfiles.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/alembic/util/sqla_compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.354737 bl_python_all-0.2.0/typings/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.354737 bl_python_all-0.2.0/typings/connexion/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/apps/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/apps/asynchronous.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/apps/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/datastructures.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.358737 bl_python_all-0.2.0/typings/connexion/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/decorators/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/decorators/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/decorators/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.358737 bl_python_all-0.2.0/typings/connexion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/frameworks/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/frameworks/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/frameworks/starlette.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/http_facts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/json_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/jsonifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/lifecycle.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.358737 bl_python_all-0.2.0/typings/connexion/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/lifespan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/request_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/response_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/routing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/middleware/swagger_ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/mock.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/connexion/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/operations/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/operations/openapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/operations/swagger2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/problem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/uri_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/connexion/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/validators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/validators/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/validators/form_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/validators/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/connexion/validators/parameter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/flask_injector/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_injector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_injector/tests.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/flask_login/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/__about__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/login_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/test_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/flask_login/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/json_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/json_logging/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.362737 bl_python_all-0.2.0/typings/json_logging/framework/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/connexion/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.366737 bl_python_all-0.2.0/typings/json_logging/framework/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/fastapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.366737 bl_python_all-0.2.0/typings/json_logging/framework/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/flask/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.366737 bl_python_all-0.2.0/typings/json_logging/framework/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/quart/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.366737 bl_python_all-0.2.0/typings/json_logging/framework/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework/sanic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/framework_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/json_logging/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.374737 bl_python_all-0.2.0/typings/saml2/
+-rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/algsupport.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/argtree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/assertion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/attribute_converter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/attribute_resolver.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.374737 bl_python_all-0.2.0/typings/saml2/attributemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/attributemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.374737 bl_python_all-0.2.0/typings/saml2/authn_context/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38744 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/ippword.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38607 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/mobiletwofactor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38849 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/ppt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    37241 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/pword.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    37023 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/authn_context/sslcert.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cert.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/client_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/country_codes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cryptography/asymmetric.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cryptography/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cryptography/pki.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/cryptography/symmetric.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/data/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/data/schemas/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/data/templates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/ecp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/ecp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/entity.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/entity_category/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/entity_category/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/eptid.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/algsupport.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/idpdisc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/mdattr.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/mdrpi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/mdui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/pefim.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/requested_attributes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/shibmd.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/extension/sp_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/httpbase.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/httputil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/ident.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/mcache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26965 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/md.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/mdbcache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/mdie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17985 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/mdstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/mongo_store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/pack.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/population.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.378737 bl_python_all-0.2.0/typings/saml2/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/profile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/profile/ecp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/profile/paos.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/profile/samlec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/s2repoze/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/s2repoze/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/s_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/saml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24413 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/samlp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/schema/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/schema/soapenv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/sdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21647 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/sigver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/soap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/time_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/userinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/userinfo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/validate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/virtual_org.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/ws/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/xml/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/xml/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/xml/schema/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/xmldsig/
+-rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/xmldsig/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:57:13.382737 bl_python_all-0.2.0/typings/saml2/xmlenc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-14 21:57:08.000000 bl_python_all-0.2.0/typings/saml2/xmlenc/__init__.pyi
```

### Comparing `BL_Python.all-0.1.1/LICENSE.md` & `bl_python_all-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/pyproject.toml` & `bl_python_all-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "Natural Language :: English"
 ]
 dependencies = [
     "BL_Python.AWS",
     "BL_Python.database",
     "BL_Python.development",
     "BL_Python.GitHub",
+    "BL_Python.identity",
     "BL_Python.platform",
     "BL_Python.programming",
     "BL_Python.testing",
     "BL_Python.web"
 ]
 
 dynamic = ["version", "readme"]
@@ -51,49 +52,50 @@
 
 [tool.setuptools.package-dir]
 "BL_Python" = "src"
 "BL_Python.AWS" = "src/AWS/BL_Python/AWS"
 "BL_Python.database" = "src/database/BL_Python/database"
 "BL_Python.development" = "src/development/BL_Python/development"
 "BL_Python.GitHub" = "src/GitHub/BL_Python/GitHub"
+"BL_Python.identity" = "src/identity/BL_Python/identity"
 "BL_Python.platform" = "src/platform/BL_Python/platform"
 "BL_Python.programming" = "src/programming/BL_Python/programming"
 "BL_Python.testing" = "src/testing/BL_Python/testing"
 "BL_Python.web" = "src/web/BL_Python/web"
 
 [tool.setuptools]
 packages = [
     "BL_Python",
     "BL_Python.AWS",
     "BL_Python.database",
     "BL_Python.development",
     "BL_Python.GitHub",
+    "BL_Python.identity",
     "BL_Python.platform",
     "BL_Python.programming",
     "BL_Python.testing",
     "BL_Python.web"
 ]
 
 [tool.setuptools.package-data]
 "BL_Python" = ["py.typed"]
 
 #
 [project.optional-dependencies]
 dev-dependencies = [
-    "pytest",
+    "pytest ~= 8.0",
     "pytest-mock",
     "mock",
-    "pytest-cov",
-
-    # code quality. allow minor version updates.
-    # this can possibly change behavior of quality checks,
-    # which allows us to catch new types of problems.
-    "pyright",
-    "isort",
-    "black"
+    "pytest-cov ~= 4.1",
+    "coverage ~= 7.4",
+    "junit2html ~= 30.1",
+    "pyright ~= 1.1",
+    "isort ~= 5.13",
+    "ruff ~= 0.3",
+    "bandit[sarif,toml] ~= 1.7"
 ]
 
 [tool.pyright]
 pythonVersion = "3.10"
 
 include = [
     "*.py",
@@ -114,14 +116,15 @@
 ]
 
 extraPaths = [
     "src/AWS",
     "src/database",
     "src/development",
     "src/GitHub",
+    "src/identity",
     "src/platform",
     "src/programming",
     "src/testing",
     "src/web"
 ]
 
 stubPath = "./typings"
@@ -137,34 +140,37 @@
 reportMissingSuperCall = "information"
 reportPropertyTypeMismatch = "error"
 reportShadowedImports = "information"
 reportUninitializedInstanceVariable = "information"
 reportUnnecessaryTypeIgnoreComment = "information"
 reportUnusedCallResult = "information"
 reportMissingTypeStubs = "information"
+reportWildcardImportFromLibrary = "warning"
 
 [tool.pytest.ini_options]
 pythonpath = [
     ".",
     "src/AWS",
     "src/database",
     "src/development",
     "src/GitHub",
+    "src/identity",
     "src/platform",
     "src/programming",
     "src/testing",
     "src/web",
 ]
 
 testpaths = [
     "test",
     "src/AWS/test",
     "src/database/test",
     "src/development/test",
     "src/GitHub/test",
+    "src/identity/test",
     "src/platform/test",
     "src/programming/test",
     "src/testing/test",
     "src/web/test"
 ]
 
 addopts = [
@@ -172,31 +178,33 @@
     # to debug tests without altering these options see
     # https://pytest-cov.readthedocs.io/en/latest/debuggers.html
     # For more information regarding doing this with VSCode see
     # https://github.com/microsoft/vscode-python/issues/21255
     # and
     # https://github.com/microsoft/vscode-python/issues/21845
     "--cov=.",
-    "--junitxml=pytest.xml",
+    "--junitxml=reports/pytest/pytest.xml",
     "-o=junit_family=xunit2",
-    "--cov-report=xml:cov.xml",
+    "--cov-report=xml:reports/pytest/cov.xml",
     "--cov-report=term-missing",
 ]
 
 python_files = "test_*.py"
 
 norecursedirs = "__pycache__ build .pytest_cache *.egg-info .venv .github-venv"
 
 [tool.coverage.report]
 include_namespace_packages = true
 
 [tool.coverage.html]
+directory = "reports/pytest/coverage"
 show_contexts = true
 
 [tool.coverage.run]
+data_file = "reports/pytest/.coverage"
 dynamic_context = "test_function"
 relative_files = true
 omit = [
     ".venv/*",
     "*/.venv/*",
     ".github-venv/*",
     "*/test/*",
@@ -210,14 +218,50 @@
     "*/typings/*",
     "node_modules/*",
     "__pycache__/*",
     "*/__pycache__/*"
 ]
 branch = true
 
-[tool.black]
-exclude = "src/.+/(typings|build)"
+[tool.bandit]
+exclude_dirs = [
+    "./build/*",
+    "./.github-venv/*",
+    "./.pytest_cache/*",
+    "./typings/*",
+    "./node_modules/*",
+    "./__pycache__/*",
+    "./.github/*",
+    "./.venv/*",
+    "./.git/*",
+    "./test/*/test*.py",
+    "./src/*/test/*/test*.py"
+]
+
+[tool.ruff]
+include = [
+    "pyproject.toml",
+    "src/**/*.py",
+    "src/**/*.pyi",
+    "test/**/*.py",
+    "test/**.*.pyi",
+]
+[tool.ruff.format]
+exclude = [
+    "typings/**/*.py",
+    "typings/**/*.pyi",
+    "src/**/typings/**/*.py",
+    "src/**/typings/**/*.pyi",
+    "src/**/build/**/*.py",
+    "src/**/build/**/*.pyi",
+]
+quote-style = "double"
+indent-style = "space"
+skip-magic-trailing-comma = false
+line-ending = "auto"
+docstring-code-format = false
+docstring-code-line-length = "dynamic"
 
 [tool.isort]
 profile = "black"
 src_paths = ["src"]
 skip_glob = ["src/*/typings", "src/*/build"]
```

### Comparing `BL_Python.all-0.1.1/src/GitHub/BL_Python/GitHub/api.py` & `bl_python_all-0.2.0/src/GitHub/BL_Python/GitHub/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,15 @@
     ):
         ## repo = organization.get_repo(repository_name)
         ## can't use repo.organization because of this
         ## https://github.com/PyGithub/PyGithub/issues/1598
         repository = self._client.get_repo(f"{organization_name}/{repository_name}")
         organization: Organization = self._client.get_organization(organization_name)
         # fixes the PyGithub API URLs for working with the organiztion owning the repository
-        cast(
-            Any, repository._organization  # pyright: ignore[reportPrivateUsage]
-        )._value = organization
+        cast(Any, repository._organization)._value = organization  # pyright: ignore[reportPrivateUsage]
         return repository
 
     def create_repository(
         self,
         name: str,
         description: str,
         organization_name: str | None = None,
```

### Comparing `BL_Python.all-0.1.1/src/database/BL_Python/database/dependency_injection.py` & `bl_python_all-0.2.0/src/database/BL_Python/database/dependency_injection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from BL_Python.database.config import Config, DatabaseConfig
 from BL_Python.database.engine import DatabaseEngine
-from injector import Binder, CallableProvider, Module, inject, singleton
+from BL_Python.database.types import MetaBase
+from BL_Python.programming.dependency_injection import ConfigModule
+from injector import Binder, CallableProvider, Injector, Module, inject, singleton
 from sqlalchemy.orm.scoping import ScopedSession
 from sqlalchemy.orm.session import Session
 from typing_extensions import override
 
 from .config import DatabaseConfig
 
 
 class ScopedSessionModule(Module):
     """
     Configure SQLAlchemy Session depedencies for Injector.
     """
 
+    _bases: list[MetaBase | type[MetaBase]] | None = None
+
     @override
-    def configure(
-        self, binder: Binder, database_config: DatabaseConfig | None = None
-    ) -> None:
+    def configure(self, binder: Binder) -> None:
         # Any ScopedSession dependency should be the same for the lifetime of the application.
         # ScopeSession is a factory that creates a Session per thread.
         # The Session returned is the same for the lifetime of the thread.
         binder.bind(
             ScopedSession,
             to=CallableProvider(self._get_scoped_session),
             scope=singleton,
@@ -28,30 +31,48 @@
         # Injecting a Session means calling the ScopedSession factory.
         # This is largely a convenience dependency, because the same
         # instance can be obtained by executing the factory that is
         # ScopedSession. ScopedSession handles all thread local concerns.
         # It is safe for this method to be called multiple times.
         binder.bind(Session, to=CallableProvider(self._get_session))
 
-        # it is possible for DatabaseConfig to have been registered
-        # in another module for the IoC container.
-        if database_config:
-            binder.bind(DatabaseConfig, database_config)
+    def __init__(self, bases: list[MetaBase | type[MetaBase]] | None = None) -> None:
+        super().__init__()
+        self._bases = bases
 
     @inject
     def _get_scoped_session(self, database_config: DatabaseConfig) -> ScopedSession:
         """
         Returns a ScopedSession instance configured with
         the correct engine and connection string.
         Defaults to using the `sessionmaker` Session factory.
         """
         return DatabaseEngine.get_session_from_connection_string(
-            database_config.connection_string, database_config.sqlalchemy_echo
+            database_config.connection_string,
+            database_config.sqlalchemy_echo,
+            {},
+            database_config.connect_args,
+            bases=self._bases,
         )
 
     @inject
     def _get_session(self, session_factory: ScopedSession) -> Session:
         """
         Returns a Session instance from the injected ScopedSession instance.
         """
         session: Session = session_factory()
         return session
+
+
+def get_database_config_container(config: Config):
+    config_module = ConfigModule(config, Config)
+    database_config_module = ConfigModule(config.database, DatabaseConfig)
+
+    return Injector([config_module, database_config_module])
+
+
+def get_database_ioc_container(
+    config: Config, bases: list[MetaBase | type[MetaBase]] | None = None
+):
+    container = get_database_config_container(config)
+    container.binder.install(ScopedSessionModule(bases=bases))
+    return container
```

### Comparing `BL_Python.all-0.1.1/src/development/BL_Python/development/profiling.py` & `bl_python_all-0.2.0/src/development/BL_Python/development/profiling.py`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/BL_Python/web/application.py` & `bl_python_all-0.2.0/src/web/BL_Python/web/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,53 +6,55 @@
 
 import logging
 from dataclasses import dataclass
 from os import environ, path
 from typing import Generic, Optional, TypeVar, cast
 
 import json_logging
+from BL_Python.AWS.ssm import SSMParameters
 from BL_Python.programming.config import AbstractConfig, ConfigBuilder, load_config
 from BL_Python.programming.dependency_injection import ConfigModule
 from connexion import FlaskApp
 from flask import Blueprint, Flask
 from flask_injector import FlaskInjector
 from injector import Module
 from lib_programname import get_path_executed_script
 
 from .config import Config
 from .middleware import (
     register_api_request_handlers,
     register_api_response_handlers,
+    register_context_middleware,
     register_error_handlers,
 )
 from .middleware.dependency_injection import configure_dependencies
 
 _get_program_dir = lambda: path.dirname(get_path_executed_script())
 _get_exec_dir = lambda: path.abspath(".")
 
 TApp = Flask | FlaskApp
-T_app = TypeVar("T_app", bound=TApp, covariant=True)
+T_app = TypeVar("T_app", bound=TApp)
 
 
 @dataclass
 class AppInjector(Generic[T_app]):
     app: T_app
     flask_injector: FlaskInjector
 
 
-FlaskAppInjector = AppInjector[Flask]
-OpenAPIAppInjector = AppInjector[FlaskApp]
-
-
 @dataclass
 class CreateAppResult(Generic[T_app]):
     flask_app: Flask
     app_injector: AppInjector[T_app]
 
 
+FlaskAppResult = CreateAppResult[Flask]
+OpenAPIAppResult = CreateAppResult[FlaskApp]
+
+
 # In Python 3.12 we can use generics in functions,
 # but we target >= Python 3.10. This is one way
 # around that limitation.
 class App(Generic[T_app]):
     """
     Create a new generic type for the application instance.
 
@@ -61,15 +63,15 @@
     """
 
     @staticmethod
     def create(
         config_filename: str = "config.toml",
         # FIXME should be a list of PydanticDataclass
         application_configs: list[type[AbstractConfig]] | None = None,
-        application_modules: list[Module] | None = None,
+        application_modules: list[Module | type[Module]] | None = None,
     ) -> CreateAppResult[T_app]:
         """
         Bootstrap the Flask applcation.
 
         Args:
             config_filename: The name of the TOML file to load configuration information from.
             application_config: A list of Pydantic objects to store configuration information from the TOML file.
@@ -81,15 +83,15 @@
         )
 
 
 def create_app(
     config_filename: str = "config.toml",
     # FIXME should be a list of PydanticDataclass
     application_configs: list[type[AbstractConfig]] | None = None,
-    application_modules: list[Module] | None = None,
+    application_modules: list[Module | type[Module]] | None = None,
     # FIXME eventually should replace with builders
     # and configurators so this list of params doesn't
     # just grow and grow.
     # startup_builder: IStartupBuilder,
     # config: Config,
 ) -> CreateAppResult[TApp]:
     """
@@ -110,21 +112,30 @@
     if application_configs is not None:
         # fmt: off
         config_type = ConfigBuilder[Config]()\
             .with_root_config(Config)\
             .with_configs(application_configs)\
             .build()
         # fmt: on
-    full_config: Config
-    if config_overrides:
-        full_config = load_config(
-            config_type, config_filename, {"flask": config_overrides}
-        )
-    else:
-        full_config = load_config(config_type, config_filename)
+
+    full_config: Config | None = None
+    try:
+        # requires that aws-ssm.ini exists and is correctly configured
+        ssm_parameters = SSMParameters()
+        full_config = ssm_parameters.load_config(config_type)
+    except Exception as e:
+        logging.getLogger().warn(f"SSM parameter load failed: {e}")
+
+    if full_config is None:
+        if config_overrides:
+            full_config = load_config(
+                config_type, config_filename, {"flask": config_overrides}
+            )
+        else:
+            full_config = load_config(config_type, config_filename)
 
     full_config.prepare_env_for_flask()
 
     if full_config.flask is None:
         raise Exception("You must set [flask] in the application configuration.")
 
     if not full_config.flask.app_name:
@@ -139,14 +150,15 @@
         app = openapi
     else:
         app = configure_blueprint_routes(full_config)
 
     register_error_handlers(app)
     _ = register_api_request_handlers(app)
     _ = register_api_response_handlers(app)
+    _ = register_context_middleware(app)
     # register_app_teardown_handlers(app)
 
     # Register every subconfig as a ConfigModule.
     # This will allow subpackages to resolve their own config types,
     # allow for type safety against objects of those types.
     # Otherwise, they can resolve `AbstractConfig`, but then type
     # safety is lost.
@@ -154,15 +166,15 @@
     # those will override the automatically generated `ConfigModule`s.
     application_modules = [
         ConfigModule(config, type(config)) for (_, config) in full_config
     ] + (application_modules if application_modules else [])
     # The `full_config` module cannot be overridden unless the application
     # IoC container is fiddled with. `full_config` is the instance registered
     # to `AbstractConfig`.
-    modules = application_modules + [ConfigModule(full_config, type(full_config))]
+    modules = application_modules + [ConfigModule(full_config, Config)]
     flask_injector = configure_dependencies(app, application_modules=modules)
 
     flask_app = app.app if isinstance(app, FlaskApp) else app
     return CreateAppResult(flask_app, AppInjector(app, flask_injector))
 
 
 def configure_openapi(config: Config, name: Optional[str] = None):
```

### Comparing `BL_Python.all-0.1.1/src/web/BL_Python/web/config.py` & `bl_python_all-0.2.0/src/web/BL_Python/web/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import field
 from os import environ
-from typing import Any, Literal
+from typing import Literal
 
 from flask.config import Config as FlaskAppConfig
 from pydantic import BaseModel
 
 
 class LoggingConfig(BaseModel):
     log_level: str = "INFO"
@@ -55,23 +55,21 @@
     secure: bool = True
     samesite: str = "none"
 
     def _prepare_env_for_flask(self):
         if not self.secret_key:
             raise Exception("`flask.session.cookie.secret_key` must be set in config.")
 
-        environ.update(
-            {
-                "SECRET_KEY": self.secret_key,
-                "SESSION_COOKIE_NAME": self.name,
-                "SESSION_COOKIE_HTTPONLY": str(1 if self.httponly else 0),
-                "SESSION_COOKIE_SECURE": str(1 if self.secure else 0),
-                "SESSION_COOKIE_SAMESITE": self.samesite,
-            }
-        )
+        environ.update({
+            "SECRET_KEY": self.secret_key,
+            "SESSION_COOKIE_NAME": self.name,
+            "SESSION_COOKIE_HTTPONLY": str(1 if self.httponly else 0),
+            "SESSION_COOKIE_SECURE": str(1 if self.secure else 0),
+            "SESSION_COOKIE_SAMESITE": self.samesite,
+        })
 
     def _update_flask_config(self, flask_app_config: FlaskAppConfig):
         class ConfigObject:
             SECRET_KEY = self.secret_key
             SESSION_COOKIE_NAME = self.name
             SESSION_COOKIE_HTTPONLY = self.httponly
             SESSION_COOKIE_SECURE = self.secure
@@ -83,25 +81,19 @@
 class FlaskSessionConfig(BaseModel):
     cookie: FlaskSessionCookieConfig
     permanent: bool = True
     lifetime: int | None = 86400
     refresh_each_request: bool = True
 
     def _prepare_env_for_flask(self):
-        environ.update(
-            {
-                "PERMANENT_SESSION": str(1 if self.permanent else 0),
-                "PERMANENT_SESSION_LIFETIME": (
-                    str(self.lifetime) if self.lifetime else ""
-                ),
-                "SESSION_REFRESH_EACH_REQUEST": str(
-                    1 if self.refresh_each_request else 0
-                ),
-            }
-        )
+        environ.update({
+            "PERMANENT_SESSION": str(1 if self.permanent else 0),
+            "PERMANENT_SESSION_LIFETIME": (str(self.lifetime) if self.lifetime else ""),
+            "SESSION_REFRESH_EACH_REQUEST": str(1 if self.refresh_each_request else 0),
+        })
         self.cookie._prepare_env_for_flask()  # pyright: ignore[reportPrivateUsage]
 
     def _update_flask_config(self, flask_app_config: FlaskAppConfig):
         self.cookie._update_flask_config(  # pyright: ignore[reportPrivateUsage]
             flask_app_config
         )
 
@@ -144,23 +136,14 @@
             FLASK_RUN_PORT = self.port
             FLASK_RUN_HOST = self.host
             TESTING = self.env == "Testing"
 
         flask_app_config.from_object(ConfigObject)
 
 
-class SAML2Config(BaseModel):
-    metadata: str | None = None
-    metadata_url: str | None = None
-    relay_state: str | None = None
-    # TODO is there a more specific type than `Any`
-    # that fits logging configurations?
-    logging: dict[str, Any] | None = None
-
-
 from BL_Python.programming.config import AbstractConfig
 
 
 class Config(BaseModel, AbstractConfig):
     logging: LoggingConfig = LoggingConfig()
     web: WebConfig = WebConfig()
     flask: FlaskConfig | None = None
```

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/__init__.pyi` & `bl_python_all-0.2.0/typings/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/apps/abstract.pyi` & `bl_python_all-0.2.0/typings/connexion/apps/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/apps/asynchronous.pyi` & `bl_python_all-0.2.0/typings/connexion/apps/asynchronous.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/apps/flask.pyi` & `bl_python_all-0.2.0/typings/connexion/apps/flask.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/cli.pyi` & `bl_python_all-0.2.0/typings/connexion/cli.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/datastructures.pyi` & `bl_python_all-0.2.0/typings/connexion/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/decorators/main.pyi` & `bl_python_all-0.2.0/typings/connexion/decorators/main.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/decorators/parameter.pyi` & `bl_python_all-0.2.0/typings/connexion/decorators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/decorators/response.pyi` & `bl_python_all-0.2.0/typings/connexion/decorators/response.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/exceptions.pyi` & `bl_python_all-0.2.0/typings/connexion/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/abstract.pyi` & `bl_python_all-0.2.0/typings/connexion/frameworks/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/flask.pyi` & `bl_python_all-0.2.0/typings/connexion/frameworks/flask.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/frameworks/starlette.pyi` & `bl_python_all-0.2.0/typings/connexion/frameworks/starlette.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/handlers.pyi` & `bl_python_all-0.2.0/typings/connexion/handlers.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/json_schema.pyi` & `bl_python_all-0.2.0/typings/connexion/json_schema.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/jsonifier.pyi` & `bl_python_all-0.2.0/typings/connexion/jsonifier.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/lifecycle.pyi` & `bl_python_all-0.2.0/typings/connexion/lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/abstract.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/context.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/context.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/exceptions.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/lifespan.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/lifespan.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/main.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/main.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/request_validation.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/request_validation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/response_validation.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/response_validation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/routing.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/routing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/security.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/server_error.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/server_error.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/middleware/swagger_ui.pyi` & `bl_python_all-0.2.0/typings/connexion/middleware/swagger_ui.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/mock.pyi` & `bl_python_all-0.2.0/typings/connexion/mock.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/operations/__init__.pyi` & `bl_python_all-0.2.0/typings/connexion/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/operations/abstract.pyi` & `bl_python_all-0.2.0/typings/connexion/operations/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/operations/openapi.pyi` & `bl_python_all-0.2.0/typings/connexion/operations/openapi.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/operations/swagger2.pyi` & `bl_python_all-0.2.0/typings/connexion/operations/swagger2.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/options.pyi` & `bl_python_all-0.2.0/typings/connexion/options.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/problem.pyi` & `bl_python_all-0.2.0/typings/connexion/problem.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/resolver.pyi` & `bl_python_all-0.2.0/typings/connexion/resolver.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/security.pyi` & `bl_python_all-0.2.0/typings/connexion/security.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/spec.pyi` & `bl_python_all-0.2.0/typings/connexion/spec.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/testing.pyi` & `bl_python_all-0.2.0/typings/connexion/testing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/types.pyi` & `bl_python_all-0.2.0/typings/connexion/types.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/uri_parsing.pyi` & `bl_python_all-0.2.0/typings/connexion/uri_parsing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/utils.pyi` & `bl_python_all-0.2.0/typings/connexion/utils.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/validators/__init__.pyi` & `bl_python_all-0.2.0/typings/connexion/validators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/validators/abstract.pyi` & `bl_python_all-0.2.0/typings/connexion/validators/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/validators/form_data.pyi` & `bl_python_all-0.2.0/typings/connexion/validators/form_data.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/validators/json.pyi` & `bl_python_all-0.2.0/typings/connexion/validators/json.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/connexion/validators/parameter.pyi` & `bl_python_all-0.2.0/typings/connexion/validators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/__init__.pyi` & `bl_python_all-0.2.0/typings/json_logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework/connexion/__init__.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework/fastapi/implementation.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework/flask/__init__.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework/flask/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework/quart/__init__.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework/quart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework/sanic/__init__.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework/sanic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/framework_base.pyi` & `bl_python_all-0.2.0/typings/json_logging/framework_base.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/src/web/typings/json_logging/util.pyi` & `bl_python_all-0.2.0/typings/json_logging/util.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/autogenerate/api.pyi` & `bl_python_all-0.2.0/typings/alembic/autogenerate/api.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Any, Callable, Dict, Iterator, Optional, Sequence, Set, TYPE_CHECKING, Union
+from typing import Any, Dict, Iterator, List, Optional, Sequence, Set, TYPE_CHECKING, Union
 from .. import util
+from ..util import sqla_compat
 from sqlalchemy.engine import Connection, Dialect, Inspector
-from sqlalchemy.sql.schema import MetaData, SchemaItem
+from sqlalchemy.sql.schema import MetaData, SchemaItem, Table
 from ..config import Config
 from ..operations.ops import DowngradeOps, MigrationScript, UpgradeOps
-from ..runtime.environment import NameFilterParentNames, NameFilterType, RenderItemFn
+from ..runtime.environment import NameFilterParentNames, NameFilterType, ProcessRevisionDirectiveFn, RenderItemFn
 from ..runtime.migration import MigrationContext
 from ..script.base import Script, ScriptDirectory
+from ..script.revision import _GetRevArg
 
 if TYPE_CHECKING:
     ...
 def compare_metadata(context: MigrationContext, metadata: MetaData) -> Any:
     """Compare a database schema to that given in a
     :class:`~sqlalchemy.schema.MetaData` instance.
 
@@ -178,15 +180,15 @@
     """Maintains configuration and state that's specific to an
     autogenerate operation."""
     metadata: Optional[MetaData] = ...
     connection: Optional[Connection] = ...
     dialect: Optional[Dialect] = ...
     imports: Set[str] = ...
     migration_context: MigrationContext = ...
-    def __init__(self, migration_context: MigrationContext, metadata: Optional[MetaData] = ..., opts: Optional[dict] = ..., autogenerate: bool = ...) -> None:
+    def __init__(self, migration_context: MigrationContext, metadata: Optional[MetaData] = ..., opts: Optional[Dict[str, Any]] = ..., autogenerate: bool = ...) -> None:
         ...
     
     @util.memoized_property
     def inspector(self) -> Inspector:
         ...
     
     def run_name_filters(self, name: Optional[str], type_: NameFilterType, parent_names: NameFilterParentNames) -> bool:
@@ -198,43 +200,43 @@
         the chance to filter what names should be reflected as database
         objects.  The filters here are produced directly via the
         :paramref:`.EnvironmentContext.configure.include_name` parameter.
 
         """
         ...
     
-    def run_object_filters(self, object_: SchemaItem, name: Optional[str], type_: NameFilterType, reflected: bool, compare_to: Optional[SchemaItem]) -> bool:
+    def run_object_filters(self, object_: SchemaItem, name: sqla_compat._ConstraintName, type_: NameFilterType, reflected: bool, compare_to: Optional[SchemaItem]) -> bool:
         """Run the context's object filters and return True if the targets
         should be part of the autogenerate operation.
 
         This method should be run for every kind of object encountered within
         an autogenerate operation, giving the environment the chance
         to filter what objects should be included in the comparison.
         The filters here are produced directly via the
         :paramref:`.EnvironmentContext.configure.include_object` parameter.
 
         """
         ...
     
     run_filters = ...
     @util.memoized_property
-    def sorted_tables(self): # -> list[Unknown]:
+    def sorted_tables(self) -> List[Table]:
         """Return an aggregate of the :attr:`.MetaData.sorted_tables`
         collection(s).
 
         For a sequence of :class:`.MetaData` objects, this
         concatenates the :attr:`.MetaData.sorted_tables` collection
         for each individual :class:`.MetaData`  in the order of the
         sequence.  It does **not** collate the sorted tables collections.
 
         """
         ...
     
     @util.memoized_property
-    def table_key_to_table(self): # -> dict[Unknown, Unknown]:
+    def table_key_to_table(self) -> Dict[str, Table]:
         """Return an aggregate  of the :attr:`.MetaData.tables` dictionaries.
 
         The :attr:`.MetaData.tables` collection is a dictionary of table key
         to :class:`.Table`; this method aggregates the dictionary across
         multiple :class:`.MetaData` objects into one dictionary.
 
         Duplicate table keys are **not** supported; if two :class:`.MetaData`
@@ -244,21 +246,23 @@
         ...
     
 
 
 class RevisionContext:
     """Maintains configuration and state that's specific to a revision
     file generation operation."""
-    def __init__(self, config: Config, script_directory: ScriptDirectory, command_args: Dict[str, Any], process_revision_directives: Optional[Callable] = ...) -> None:
+    generated_revisions: List[MigrationScript]
+    process_revision_directives: Optional[ProcessRevisionDirectiveFn]
+    def __init__(self, config: Config, script_directory: ScriptDirectory, command_args: Dict[str, Any], process_revision_directives: Optional[ProcessRevisionDirectiveFn] = ...) -> None:
         ...
     
-    def run_autogenerate(self, rev: tuple, migration_context: MigrationContext) -> None:
+    def run_autogenerate(self, rev: _GetRevArg, migration_context: MigrationContext) -> None:
         ...
     
-    def run_no_autogenerate(self, rev: tuple, migration_context: MigrationContext) -> None:
+    def run_no_autogenerate(self, rev: _GetRevArg, migration_context: MigrationContext) -> None:
         ...
     
     def generate_scripts(self) -> Iterator[Optional[Script]]:
         ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/autogenerate/render.pyi` & `bl_python_all-0.2.0/typings/alembic/autogenerate/render.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/autogenerate/rewriter.pyi` & `bl_python_all-0.2.0/typings/alembic/autogenerate/rewriter.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Callable, List, Optional, TYPE_CHECKING, Type, Union
-from alembic.operations.ops import AddColumnOp, AlterColumnOp, CreateTableOp, MigrateOperation, MigrationScript, ModifyTableOps
-from alembic.runtime.migration import MigrationContext
-from alembic.script.revision import Revision
+from typing import Any, Callable, List, TYPE_CHECKING, Tuple, Type, Union
+from ..operations.ops import AddColumnOp, AlterColumnOp, CreateTableOp, MigrateOperation, MigrationScript, ModifyTableOps
+from ..runtime.migration import MigrationContext
+from ..script.revision import _GetRevArg
 
 if TYPE_CHECKING:
     ...
+ProcessRevisionDirectiveFn = Callable[["MigrationContext", "_GetRevArg", List["MigrationScript"]], None]
 class Rewriter:
     """A helper object that allows easy 'rewriting' of ops streams.
 
     The :class:`.Rewriter` object is intended to be passed along
     to the
     :paramref:`.EnvironmentContext.configure.process_revision_directives`
     parameter in an ``env.py`` script.    Once constructed, any number
@@ -31,22 +32,22 @@
 
     .. seealso::
 
         :ref:`autogen_rewriter` - usage example
 
     """
     _traverse = ...
-    _chained: Optional[Rewriter] = ...
+    _chained: Tuple[Union[ProcessRevisionDirectiveFn, Rewriter], ...] = ...
     def __init__(self) -> None:
         ...
     
-    def chain(self, other: Rewriter) -> Rewriter:
+    def chain(self, other: Union[ProcessRevisionDirectiveFn, Rewriter,]) -> Rewriter:
         """Produce a "chain" of this :class:`.Rewriter` to another.
 
-        This allows two rewriters to operate serially on a stream,
+        This allows two or more rewriters to operate serially on a stream,
         e.g.::
 
             writer1 = autogenerate.Rewriter()
             writer2 = autogenerate.Rewriter()
 
 
             @writer1.rewrites(ops.AddColumnOp)
@@ -67,30 +68,30 @@
         :param other: a :class:`.Rewriter` instance
         :return: a new :class:`.Rewriter` that will run the operations
          of this writer, then the "other" writer, in succession.
 
         """
         ...
     
-    def rewrites(self, operator: Union[Type[AddColumnOp], Type[MigrateOperation], Type[AlterColumnOp], Type[CreateTableOp], Type[ModifyTableOps],]) -> Callable:
+    def rewrites(self, operator: Union[Type[AddColumnOp], Type[MigrateOperation], Type[AlterColumnOp], Type[CreateTableOp], Type[ModifyTableOps],]) -> Callable[..., Any]:
         """Register a function as rewriter for a given type.
 
         The function should receive three arguments, which are
         the :class:`.MigrationContext`, a ``revision`` tuple, and
         an op directive of the type indicated.  E.g.::
 
             @writer1.rewrites(ops.AddColumnOp)
             def add_column_nullable(context, revision, op):
                 op.column.nullable = True
                 return op
 
         """
         ...
     
-    def __call__(self, context: MigrationContext, revision: Revision, directives: List[MigrationScript]) -> None:
+    def __call__(self, context: MigrationContext, revision: _GetRevArg, directives: List[MigrationScript]) -> None:
         ...
     
-    def process_revision_directives(self, context: MigrationContext, revision: Revision, directives: List[MigrationScript]) -> None:
+    def process_revision_directives(self, context: MigrationContext, revision: _GetRevArg, directives: List[MigrationScript]) -> None:
         ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/command.pyi` & `bl_python_all-0.2.0/typings/alembic/command.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 This type stub file was generated by pyright.
 """
 
 from typing import List, Optional, TYPE_CHECKING, Union
 from .runtime.environment import ProcessRevisionDirectiveFn
 from alembic.config import Config
 from alembic.script.base import Script
+from alembic.script.revision import _RevIdType
 
 if TYPE_CHECKING:
     ...
-def list_templates(config: Config): # -> None:
+def list_templates(config: Config) -> None:
     """List available templates.
 
     :param config: a :class:`.Config` object.
 
     """
     ...
 
@@ -26,21 +27,18 @@
 
     :param template: string name of the migration environment template to
      use.
 
     :param package: when True, write ``__init__.py`` files into the
      environment location as well as the versions/ location.
 
-     .. versionadded:: 1.2
-
-
     """
     ...
 
-def revision(config: Config, message: Optional[str] = ..., autogenerate: bool = ..., sql: bool = ..., head: str = ..., splice: bool = ..., branch_label: Optional[str] = ..., version_path: Optional[str] = ..., rev_id: Optional[str] = ..., depends_on: Optional[str] = ..., process_revision_directives: Optional[ProcessRevisionDirectiveFn] = ...) -> Union[Optional[Script], List[Optional[Script]]]:
+def revision(config: Config, message: Optional[str] = ..., autogenerate: bool = ..., sql: bool = ..., head: str = ..., splice: bool = ..., branch_label: Optional[_RevIdType] = ..., version_path: Optional[str] = ..., rev_id: Optional[str] = ..., depends_on: Optional[str] = ..., process_revision_directives: Optional[ProcessRevisionDirectiveFn] = ...) -> Union[Optional[Script], List[Optional[Script]]]:
     """Create a new revision file.
 
     :param config: a :class:`.Config` object.
 
     :param message: string message to apply to the revision; this is the
      ``-m`` option to ``alembic revision``.
 
@@ -89,15 +87,15 @@
     :param config: a :class:`.Config` object.
 
     .. versionadded:: 1.9.0
 
     """
     ...
 
-def merge(config: Config, revisions: str, message: Optional[str] = ..., branch_label: Optional[str] = ..., rev_id: Optional[str] = ...) -> Optional[Script]:
+def merge(config: Config, revisions: _RevIdType, message: Optional[str] = ..., branch_label: Optional[_RevIdType] = ..., rev_id: Optional[str] = ...) -> Optional[Script]:
     """Merge two revisions together.  Creates a new migration file.
 
     :param config: a :class:`.Config` instance
 
     :param message: string message to apply to the revision
 
     :param branch_label: string label name to apply to the new revision
@@ -196,39 +194,34 @@
     :param config: a :class:`.Config` instance.
 
     :param verbose: output in verbose mode.
 
     """
     ...
 
-def stamp(config: Config, revision: str, sql: bool = ..., tag: Optional[str] = ..., purge: bool = ...) -> None:
+def stamp(config: Config, revision: _RevIdType, sql: bool = ..., tag: Optional[str] = ..., purge: bool = ...) -> None:
     """'stamp' the revision table with the given revision; don't
     run any migrations.
 
     :param config: a :class:`.Config` instance.
 
     :param revision: target revision or list of revisions.   May be a list
      to indicate stamping of multiple branch heads.
 
      .. note:: this parameter is called "revisions" in the command line
         interface.
 
-     .. versionchanged:: 1.2  The revision may be a single revision or
-        list of revisions when stamping multiple branch heads.
-
     :param sql: use ``--sql`` mode
 
     :param tag: an arbitrary "tag" that can be intercepted by custom
      ``env.py`` scripts via the :class:`.EnvironmentContext.get_tag_argument`
      method.
 
     :param purge: delete all entries in the version table before stamping.
 
-     .. versionadded:: 1.2
-
     """
     ...
 
 def edit(config: Config, rev: str) -> None:
     """Edit revision script(s) using $EDITOR.
 
     :param config: a :class:`.Config` instance.
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/config.pyi` & `bl_python_all-0.2.0/typings/alembic/config.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 This type stub file was generated by pyright.
 """
 
-from configparser import ConfigParser
 import os
-from argparse import Namespace
-from typing import Any, Dict, Mapping, Optional, TextIO, Union, overload
+from argparse import ArgumentParser, Namespace
+from configparser import ConfigParser
+from typing import Any, Dict, Mapping, Optional, Sequence, TextIO, Union, overload
+
 from typing_extensions import TypedDict
+
 from . import util
 
 class Config:
     r"""Represent an Alembic configuration.
 
     Within an ``env.py`` script, this is available
     via the :attr:`.EnvironmentContext.config` attribute,
     which in turn is available at ``alembic.context``::
 
         from alembic import context
 
         some_param = context.config.get_main_option("my option")
 
-    When invoking Alembic programatically, a new
+    When invoking Alembic programmatically, a new
     :class:`.Config` can be created by passing
     the name of an .ini file to the constructor::
 
         from alembic.config import Config
         alembic_cfg = Config("/path/to/yourapp/alembic.ini")
 
     With a :class:`.Config` object, you can then
@@ -77,23 +79,23 @@
      which will be populated into the :attr:`.Config.attributes` dictionary.
 
      .. seealso::
 
         :ref:`connection_sharing`
 
     """
-    def __init__(self, file_: Union[str, os.PathLike[str], None] = ..., ini_section: str = ..., output_buffer: Optional[TextIO] = ..., stdout: TextIO = ..., cmd_opts: Optional[Namespace] = ..., config_args: Mapping[str, Any] = ..., attributes: Optional[dict] = ...) -> None:
+    def __init__(self, file_: Union[str, os.PathLike[str], None] = ..., ini_section: str = ..., output_buffer: Optional[TextIO] = ..., stdout: TextIO = ..., cmd_opts: Optional[Namespace] = ..., config_args: Mapping[str, Any] = ..., attributes: Optional[Dict[str, Any]] = ...) -> None:
         """Construct a new :class:`.Config`"""
         ...
     
     cmd_opts: Optional[Namespace] = ...
     config_file_name: Union[str, os.PathLike[str], None] = ...
     config_ini_section: str = ...
     @util.memoized_property
-    def attributes(self): -> dict[Any, Any]:
+    def attributes(self) -> Dict[str, Any]:
         """A Python dictionary for storage of additional state.
 
 
         This is a utility dictionary which can include not just strings but
         engines, connections, schema objects, or anything else.
         Use this to pass objects into an env.py script, such as passing
         a :class:`sqlalchemy.engine.base.Connection` when calling
@@ -104,15 +106,15 @@
             :ref:`connection_sharing`
 
             :paramref:`.Config.attributes`
 
         """
         ...
     
-    def print_stdout(self, text: str, *arg) -> None:
+    def print_stdout(self, text: str, *arg: Any) -> None:
         """Render a message to standard out.
 
         When :meth:`.Config.print_stdout` is called with additional args
         those arguments will formatted against the provided text,
         otherwise we simply output the provided text verbatim.
 
         This is a no-op when the``quiet`` messaging option is enabled.
@@ -217,15 +219,15 @@
     def get_main_option(self, name: str, default: str) -> str:
         ...
     
     @overload
     def get_main_option(self, name: str, default: Optional[str] = ...) -> Optional[str]:
         ...
     
-    def get_main_option(self, name, default=...): # -> str | None:
+    def get_main_option(self, name: str, default: Optional[str] = ...) -> Optional[str]:
         """Return an option from the 'main' section of the .ini file.
 
         This defaults to being a key from the ``[alembic]``
         section, unless the ``-n/--name`` flag were used to
         indicate a different section.
 
         """
@@ -240,24 +242,26 @@
 
 class MessagingOptions(TypedDict, total=False):
     quiet: bool
     ...
 
 
 class CommandLine:
+    parser: ArgumentParser
+
     def __init__(self, prog: Optional[str] = ...) -> None:
         ...
     
     def run_cmd(self, config: Config, options: Namespace) -> None:
         ...
     
-    def main(self, argv=...): # -> None:
+    def main(self, argv: Optional[Sequence[str]] = ...) -> None:
         ...
     
 
 
-def main(argv=..., prog=..., **kwargs): # -> None:
+def main(argv: Optional[Sequence[str]] = ..., prog: Optional[str] = ..., **kwargs: Any) -> None:
     """The console runner function for Alembic."""
     ...
 
 if __name__ == "__main__":
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/context.pyi` & `bl_python_all-0.2.0/typings/alembic/context.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Collection,
-    ContextManager,
-    Dict,
-    List,
-    Literal,
-    Mapping,
-    MutableMapping,
-    Optional,
-    TextIO,
-    Tuple,
-    Union,
-    overload,
-)
-
-from sqlalchemy import Table
+from typing import Any, Callable, Collection, ContextManager, Dict, Iterable, List, Literal, Mapping, MutableMapping, Optional, Sequence, TYPE_CHECKING, TextIO, Tuple, Union, overload
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.engine.url import URL
-from sqlalchemy.sql.elements import ClauseElement
+from sqlalchemy.sql import Executable
 from sqlalchemy.sql.schema import Column, FetchedValue, MetaData, SchemaItem
-
+from sqlalchemy.sql.type_api import TypeEngine
 from .autogenerate.api import AutogenContext
 from .config import Config
-from .operations.ops import MigrateOperation
+from .operations.ops import MigrationScript
 from .runtime.migration import MigrationContext, MigrationInfo, _ProxyTransaction
 from .script import ScriptDirectory
 
-if TYPE_CHECKING: ...
-
+if TYPE_CHECKING:
+    ...
 def begin_transaction() -> Union[_ProxyTransaction, ContextManager[None]]:
     """Return a context manager that will
     enclose an operation within a "transaction",
     as defined by the environment's offline
     and transactional DDL settings.
 
     e.g.::
@@ -76,110 +58,15 @@
     directly to produce transactional state in "online"
     mode.
 
     """
     ...
 
 config: Config
-
-def configure(
-    connection: Optional[Connection] = ...,
-    url: Union[str, URL, None] = ...,
-    dialect_name: Optional[str] = ...,
-    dialect_opts: Optional[Dict[str, Any]] = ...,
-    transactional_ddl: Optional[bool] = ...,
-    transaction_per_migration: bool = ...,
-    output_buffer: Optional[TextIO] = ...,
-    starting_rev: Optional[str] = ...,
-    tag: Optional[str] = ...,
-    template_args: Optional[Dict[str, Any]] = ...,
-    render_as_batch: bool = ...,
-    # Alembic documents and supports list[MetaData]
-    # despite the typehint not including it in the
-    # library
-    target_metadata: Optional[MetaData | list[MetaData]] = ...,
-    include_name: Optional[
-        Callable[
-            [
-                Optional[str],
-                Literal[
-                    "schema",
-                    "table",
-                    "column",
-                    "index",
-                    "unique_constraint",
-                    "foreign_key_constraint",
-                ],
-                MutableMapping[
-                    Literal[
-                        "schema_name",
-                        "table_name",
-                        "schema_qualified_table_name",
-                    ],
-                    Optional[str],
-                ],
-            ],
-            bool,
-        ]
-    ] = ...,
-    include_object: Optional[
-        Callable[
-            [
-                Table,
-                str,
-                Literal[
-                    "schema",
-                    "table",
-                    "column",
-                    "index",
-                    "unique_constraint",
-                    "foreign_key_constraint",
-                ],
-                bool,
-                Optional[SchemaItem],
-            ],
-            bool,
-        ]
-    ] = ...,
-    include_schemas: bool = ...,
-    process_revision_directives: Optional[
-        Callable[[MigrationContext, Tuple[str, str], List[MigrateOperation]], None]
-    ] = ...,
-    compare_type: bool = ...,
-    compare_server_default: Union[
-        bool,
-        Callable[
-            [
-                MigrationContext,
-                Column[Any],
-                Column[Any],
-                Optional[str],
-                Optional[FetchedValue],
-                Optional[str],
-            ],
-            Optional[bool],
-        ],
-    ] = ...,
-    render_item: Optional[
-        Callable[[str, Any, AutogenContext], Union[str, Literal[False]]]
-    ] = ...,
-    literal_binds: bool = ...,
-    upgrade_token: str = ...,
-    downgrade_token: str = ...,
-    alembic_module_prefix: str = ...,
-    sqlalchemy_module_prefix: str = ...,
-    user_module_prefix: Optional[str] = ...,
-    on_version_apply: Optional[
-        Callable[
-            [MigrationContext, MigrationInfo, Collection[Any], Mapping[str, Any]],
-            None,
-        ]
-    ] = ...,
-    **kw: Any
-) -> None:
+def configure(connection: Optional[Connection] = ..., url: Union[str, URL, None] = ..., dialect_name: Optional[str] = ..., dialect_opts: Optional[Dict[str, Any]] = ..., transactional_ddl: Optional[bool] = ..., transaction_per_migration: bool = ..., output_buffer: Optional[TextIO] = ..., starting_rev: Optional[str] = ..., tag: Optional[str] = ..., template_args: Optional[Dict[str, Any]] = ..., render_as_batch: bool = ..., target_metadata: Union[MetaData, Sequence[MetaData], None] = ..., include_name: Optional[Callable[[Optional[str], Literal["schema", "table", "column", "index", "unique_constraint", "foreign_key_constraint",], MutableMapping[Literal["schema_name", "table_name", "schema_qualified_table_name",], Optional[str],]], bool,]] = ..., include_object: Optional[Callable[[SchemaItem, Optional[str], Literal["schema", "table", "column", "index", "unique_constraint", "foreign_key_constraint",], bool, Optional[SchemaItem]], bool,]] = ..., include_schemas: bool = ..., process_revision_directives: Optional[Callable[[MigrationContext, Union[str, Iterable[Optional[str]], Iterable[str]], List[MigrationScript]], None,]] = ..., compare_type: Union[bool, Callable[[MigrationContext, Column[Any], Column[Any], TypeEngine[Any], TypeEngine[Any]], Optional[bool],],] = ..., compare_server_default: Union[bool, Callable[[MigrationContext, Column[Any], Column[Any], Optional[str], Optional[FetchedValue], Optional[str]], Optional[bool],],] = ..., render_item: Optional[Callable[[str, Any, AutogenContext], Union[str, Literal[False]]]] = ..., literal_binds: bool = ..., upgrade_token: str = ..., downgrade_token: str = ..., alembic_module_prefix: str = ..., sqlalchemy_module_prefix: str = ..., user_module_prefix: Optional[str] = ..., on_version_apply: Optional[Callable[[MigrationContext, MigrationInfo, Collection[Any], Mapping[str, Any]], None,]] = ..., **kw: Any) -> None:
     """Configure a :class:`.MigrationContext` within this
     :class:`.EnvironmentContext` which will provide database
     connectivity and other configuration to a series of
     migration scripts.
 
     Many methods on :class:`.EnvironmentContext` require that
     this method has been called in order to function, as they
@@ -216,17 +103,14 @@
      ``connection`` is not passed.
     :param dialect_name: string name of a dialect, such as
      "postgresql", "mssql", etc.
      The type of dialect to be used will be derived from this if
      ``connection`` and ``url`` are not passed.
     :param dialect_opts: dictionary of options to be passed to dialect
      constructor.
-
-     .. versionadded:: 1.0.12
-
     :param transactional_ddl: Force the usage of "transactional"
      DDL on or off;
      this otherwise defaults to whether or not the dialect in
      use supports it.
     :param transaction_per_migration: if True, nest each migration script
      in a transaction rather than the full series of migrations to
      run.
@@ -301,20 +185,24 @@
      The tables present in each :class:`~sqlalchemy.schema.MetaData`
      will be compared against
      what is locally available on the target
      :class:`~sqlalchemy.engine.Connection`
      to produce candidate upgrade/downgrade operations.
     :param compare_type: Indicates type comparison behavior during
      an autogenerate
-     operation.  Defaults to ``False`` which disables type
-     comparison.  Set to
-     ``True`` to turn on default type comparison, which has varied
-     accuracy depending on backend.   See :ref:`compare_types`
+     operation.  Defaults to ``True`` turning on type comparison, which
+     has good accuracy on most backends.   See :ref:`compare_types`
      for an example as well as information on other type
-     comparison options.
+     comparison options. Set to ``False`` which disables type
+     comparison. A callable can also be passed to provide custom type
+     comparison, see :ref:`compare_types` for additional details.
+
+     .. versionchanged:: 1.12.0 The default value of
+        :paramref:`.EnvironmentContext.configure.compare_type` has been
+        changed to ``True``.
 
      .. seealso::
 
         :ref:`compare_types`
 
         :paramref:`.EnvironmentContext.configure.compare_server_default`
 
@@ -390,16 +278,14 @@
 
         context.configure(
             # ...
             include_schemas = True,
             include_name = include_name
         )
 
-     .. versionadded:: 1.5
-
      .. seealso::
 
         :ref:`autogenerate_include_hooks`
 
         :paramref:`.EnvironmentContext.configure.include_object`
 
         :paramref:`.EnvironmentContext.configure.include_schemas`
@@ -607,17 +493,15 @@
      be placed between each statement when generating offline
      Oracle migrations.  Defaults to ``/``.  Oracle doesn't add a
      semicolon between statements like most other backends.
 
     """
     ...
 
-def execute(
-    sql: Union[ClauseElement, str], execution_options: Optional[dict] = ...
-) -> None:
+def execute(sql: Union[Executable, str], execution_options: Optional[Dict[str, Any]] = ...) -> None:
     """Execute the given SQL using the current change context.
 
     The behavior of :meth:`.execute` is the same
     as that of :meth:`.Operations.execute`.  Please see that
     function's documentation for full detail including
     caveats and limitations.
 
@@ -723,29 +607,37 @@
         open ended system of extending ``env.py`` scripts via the command
         line.
 
     """
     ...
 
 @overload
-def get_x_argument(as_dictionary: Literal[False]) -> List[str]: ...
+def get_x_argument(as_dictionary: Literal[False]) -> List[str]:
+    ...
+
 @overload
-def get_x_argument(as_dictionary: Literal[True]) -> Dict[str, str]: ...
+def get_x_argument(as_dictionary: Literal[True]) -> Dict[str, str]:
+    ...
+
 @overload
 def get_x_argument(as_dictionary: bool = ...) -> Union[List[str], Dict[str, str]]:
     """Return the value(s) passed for the ``-x`` argument, if any.
 
     The ``-x`` argument is an open ended flag that allows any user-defined
     value or values to be passed on the command line, then available
     here for consumption by a custom ``env.py`` script.
 
     The return value is a list, returned directly from the ``argparse``
     structure.  If ``as_dictionary=True`` is passed, the ``x`` arguments
     are parsed using ``key=value`` format into a dictionary that is
-    then returned.
+    then returned. If there is no ``=`` in the argument, value is an empty
+    string.
+
+    .. versionchanged:: 1.13.1 Support ``as_dictionary=True`` when
+       arguments are passed without the ``=`` symbol.
 
     For example, to support passing a database URL on the command line,
     the standard ``env.py`` script can be modified like this::
 
         cmd_line_url = context.get_x_argument(
             as_dictionary=True).get('dbname')
         if cmd_line_url:
@@ -781,15 +673,15 @@
 
     This function does not require that the :class:`.MigrationContext`
     has been configured.
 
     """
     ...
 
-def is_transactional_ddl():
+def is_transactional_ddl() -> bool:
     """Return True if the context is configured to expect a
     transactional DDL capable backend.
 
     This defaults to the type of database in use, and
     can be overridden by the ``transactional_ddl`` argument
     to :meth:`.configure`
 
@@ -818,18 +710,18 @@
     This function requires that a :class:`.MigrationContext` has
     first been made available via :meth:`.configure`.
 
     """
     ...
 
 script: ScriptDirectory
-
 def static_output(text: str) -> None:
     """Emit text directly to the "offline" SQL stream.
 
     Typically this is for emitting comments that
     start with --.  The statement is not treated
     as a SQL execution, no ; or batch separator
     is added, etc.
 
     """
     ...
+
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/base.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/base.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/impl.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/impl.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Any, Dict, List, Literal, Optional, Sequence, Set, TYPE_CHECKING, TextIO, Tuple, Type, Union
+from typing import Any, Dict, List, Literal, NamedTuple, Optional, Sequence, Set, TYPE_CHECKING, TextIO, Tuple, Type, Union
+from ._autogen import ComparisonResult as ComparisonResult
 from sqlalchemy.engine import Connection, Dialect
-from sqlalchemy.sql.elements import ClauseElement, ColumnElement, quoted_name
+from sqlalchemy.sql import ClauseElement, Executable
+from sqlalchemy.sql.elements import ColumnElement, quoted_name
 from sqlalchemy.sql.schema import Column, Constraint, ForeignKeyConstraint, Index, Table, UniqueConstraint
 from sqlalchemy.sql.selectable import TableClause
 from sqlalchemy.sql.type_api import TypeEngine
 from .base import _ServerDefault
 from ..autogenerate.api import AutogenContext
 from ..operations.batch import ApplyBatchImpl, BatchOperationsImpl
 
 if TYPE_CHECKING:
     ...
+log = ...
 class ImplMeta(type):
     def __init__(cls, classname: str, bases: Tuple[Type[DefaultImpl]], dict_: Dict[str, Any]) -> None:
         ...
     
 
 
 _impls: Dict[str, Type[DefaultImpl]] = ...
-Params = ...
 class DefaultImpl(metaclass=ImplMeta):
     """Provide the entrypoint for major migration operations,
     including database-specific behavioral variances.
 
     While individual SQL/DDL constructs already provide
     for database-specific implementations, variances here
     allow for entirely different sequences of operations
@@ -71,15 +73,15 @@
         """
         ...
     
     @property
     def bind(self) -> Optional[Connection]:
         ...
     
-    def execute(self, sql: Union[ClauseElement, str], execution_options: Optional[dict[str, Any]] = ...) -> None:
+    def execute(self, sql: Union[Executable, str], execution_options: Optional[dict[str, Any]] = ...) -> None:
         ...
     
     def alter_column(self, table_name: str, column_name: str, nullable: Optional[bool] = ..., server_default: Union[_ServerDefault, Literal[False]] = ..., name: Optional[str] = ..., type_: Optional[TypeEngine] = ..., schema: Optional[str] = ..., autoincrement: Optional[bool] = ..., comment: Optional[Union[str, Literal[False]]] = ..., existing_comment: Optional[str] = ..., existing_type: Optional[TypeEngine] = ..., existing_server_default: Optional[_ServerDefault] = ..., existing_nullable: Optional[bool] = ..., existing_autoincrement: Optional[bool] = ..., **kw: Any) -> None:
         ...
     
     def add_column(self, table_name: str, column: Column[Any], schema: Optional[Union[str, quoted_name]] = ...) -> None:
         ...
@@ -98,27 +100,27 @@
     
     def create_table(self, table: Table) -> None:
         ...
     
     def drop_table(self, table: Table) -> None:
         ...
     
-    def create_index(self, index: Index) -> None:
+    def create_index(self, index: Index, **kw: Any) -> None:
         ...
     
     def create_table_comment(self, table: Table) -> None:
         ...
     
     def drop_table_comment(self, table: Table) -> None:
         ...
     
     def create_column_comment(self, column: ColumnElement[Any]) -> None:
         ...
     
-    def drop_index(self, index: Index) -> None:
+    def drop_index(self, index: Index, **kw: Any) -> None:
         ...
     
     def bulk_insert(self, table: Union[TableClause, Table], rows: List[dict], multiinsert: bool = ...) -> None:
         ...
     
     def compare_type(self, inspector_column: Column[Any], metadata_column: Column) -> bool:
         """Returns True if there ARE differences between the types of the two
@@ -136,16 +138,14 @@
     def cast_for_batch_migrate(self, existing, existing_transfer, new_type): # -> None:
         ...
     
     def render_ddl_sql_expr(self, expr: ClauseElement, is_server_default: bool = ..., **kw: Any) -> str:
         """Render a SQL expression that is typically a server default,
         index expression, etc.
 
-        .. versionadded:: 1.0.11
-
         """
         ...
     
     def correct_for_autogen_foreignkeys(self, conn_fks: Set[ForeignKeyConstraint], metadata_fks: Set[ForeignKeyConstraint]) -> None:
         ...
     
     def autogen_column_reflect(self, inspector, table, column_info): # -> None:
@@ -186,12 +186,38 @@
 
         """
         ...
     
     def render_type(self, type_obj: TypeEngine, autogen_context: AutogenContext) -> Union[str, Literal[False]]:
         ...
     
-    def create_index_sig(self, index: Index) -> Tuple[Any, ...]:
+    def compare_indexes(self, metadata_index: Index, reflected_index: Index) -> ComparisonResult:
+        """Compare two indexes by comparing the signature generated by
+        ``create_index_sig``.
+
+        This method returns a ``ComparisonResult``.
+        """
         ...
     
+    def compare_unique_constraint(self, metadata_constraint: UniqueConstraint, reflected_constraint: UniqueConstraint) -> ComparisonResult:
+        """Compare two unique constraints by comparing the two signatures.
+
+        The arguments are two tuples that contain the unique constraint and
+        the signatures generated by ``create_unique_constraint_sig``.
+
+        This method returns a ``ComparisonResult``.
+        """
+        ...
+    
+    def adjust_reflected_dialect_options(self, reflected_object: Dict[str, Any], kind: str) -> Dict[str, Any]:
+        ...
+    
+
+
+class Params(NamedTuple):
+    token0: str
+    tokens: List[str]
+    args: List[str]
+    kwargs: Dict[str, str]
+    ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/mssql.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/mssql.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Any, List, Literal, Optional, TYPE_CHECKING, Union
-from sqlalchemy.ext.compiler import compiles
+from typing import Any, Dict, List, Literal, Optional, TYPE_CHECKING, Union
 from sqlalchemy.schema import Column
 from sqlalchemy.sql.base import Executable
 from sqlalchemy.sql.elements import ClauseElement
 from .base import AddColumn, ColumnDefault, ColumnName, ColumnNullable, ColumnType, RenameTable, _ServerDefault
 from .impl import DefaultImpl
+from ..util.sqla_compat import compiles
 from sqlalchemy.dialects.mssql.base import MSDDLCompiler
 from sqlalchemy.sql.schema import Index, Table
 from sqlalchemy.sql.selectable import TableClause
 from sqlalchemy.sql.type_api import TypeEngine
 
 if TYPE_CHECKING:
     ...
@@ -30,26 +30,29 @@
     
     def emit_commit(self) -> None:
         ...
     
     def alter_column(self, table_name: str, column_name: str, nullable: Optional[bool] = ..., server_default: Optional[Union[_ServerDefault, Literal[False]]] = ..., name: Optional[str] = ..., type_: Optional[TypeEngine] = ..., schema: Optional[str] = ..., existing_type: Optional[TypeEngine] = ..., existing_server_default: Optional[_ServerDefault] = ..., existing_nullable: Optional[bool] = ..., **kw: Any) -> None:
         ...
     
-    def create_index(self, index: Index) -> None:
+    def create_index(self, index: Index, **kw: Any) -> None:
         ...
     
     def bulk_insert(self, table: Union[TableClause, Table], rows: List[dict], **kw: Any) -> None:
         ...
     
     def drop_column(self, table_name: str, column: Column[Any], schema: Optional[str] = ..., **kw) -> None:
         ...
     
     def compare_server_default(self, inspector_column, metadata_column, rendered_metadata_default, rendered_inspector_default): # -> bool:
         ...
     
+    def adjust_reflected_dialect_options(self, reflected_object: Dict[str, Any], kind: str) -> Dict[str, Any]:
+        ...
+    
 
 
 class _ExecDropConstraint(Executable, ClauseElement):
     inherit_cache = ...
     def __init__(self, tname: str, colname: Union[Column[Any], str], type_: str, schema: Optional[str]) -> None:
         ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/mysql.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/mysql.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/oracle.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/oracle.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This type stub file was generated by pyright.
 """
 
 from typing import Any, TYPE_CHECKING
-from sqlalchemy.ext.compiler import compiles
 from .base import AddColumn, ColumnComment, ColumnDefault, ColumnName, ColumnNullable, ColumnType, IdentityColumnDefault, RenameTable
 from .impl import DefaultImpl
+from ..util.sqla_compat import compiles
 from sqlalchemy.dialects.oracle.base import OracleDDLCompiler
 from sqlalchemy.sql.schema import Column
 
 if TYPE_CHECKING:
     ...
 class OracleImpl(DefaultImpl):
     __dialect__ = ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/postgresql.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/postgresql.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Any, Literal, Optional, Sequence, TYPE_CHECKING, Tuple, Union
-from sqlalchemy import Index
+from typing import Any, Dict, Literal, Optional, Sequence, TYPE_CHECKING, Tuple, Union
+from sqlalchemy import Index, UniqueConstraint
 from sqlalchemy.dialects.postgresql import ExcludeConstraint
-from sqlalchemy.sql.elements import BinaryExpression, ColumnClause, quoted_name
-from .base import AlterColumn, ColumnComment, IdentityColumnDefault, RenameTable, _ServerDefault, compiles
-from .impl import DefaultImpl
+from sqlalchemy.sql.elements import ClauseElement, ColumnClause, ColumnElement, quoted_name
+from .base import AlterColumn, ColumnComment, IdentityColumnDefault, RenameTable, _ServerDefault
+from .impl import ComparisonResult, DefaultImpl
 from ..operations import ops
 from ..operations.base import BatchOperations, Operations
 from ..util import sqla_compat
+from ..util.sqla_compat import compiles
 from sqlalchemy.dialects.postgresql.base import PGDDLCompiler
 from sqlalchemy.sql.schema import Table
 from sqlalchemy.sql.type_api import TypeEngine
 from ..autogenerate.api import AutogenContext
 from ..runtime.migration import MigrationContext
 
 if TYPE_CHECKING:
     ...
 log = ...
 class PostgresqlImpl(DefaultImpl):
     __dialect__ = ...
     transactional_ddl = ...
     type_synonyms = ...
-    identity_attrs_ignore = ...
-    def create_index(self, index): # -> None:
+    def create_index(self, index: Index, **kw: Any) -> None:
         ...
     
     def prep_table_for_batch(self, batch_impl, table): # -> None:
         ...
     
     def compare_server_default(self, inspector_column, metadata_column, rendered_metadata_default, rendered_inspector_default): # -> bool:
         ...
@@ -39,15 +39,29 @@
     
     def autogen_column_reflect(self, inspector, table, column_info): # -> None:
         ...
     
     def correct_for_autogen_constraints(self, conn_unique_constraints, conn_indexes, metadata_unique_constraints, metadata_indexes): # -> None:
         ...
     
-    def create_index_sig(self, index: Index) -> Tuple[Any, ...]:
+    _default_modifiers_re = ...
+    def compare_indexes(self, metadata_index: Index, reflected_index: Index) -> ComparisonResult:
+        ...
+    
+    def compare_unique_constraint(self, metadata_constraint: UniqueConstraint, reflected_constraint: UniqueConstraint) -> ComparisonResult:
+        ...
+    
+    def adjust_reflected_dialect_options(self, reflected_options: Dict[str, Any], kind: str) -> Dict[str, Any]:
+        ...
+    
+    def render_ddl_sql_expr(self, expr: ClauseElement, is_server_default: bool = ..., is_index: bool = ..., **kw: Any) -> str:
+        """Render a SQL expression that is typically a server default,
+        index expression, etc.
+
+        """
         ...
     
     def render_type(self, type_: TypeEngine, autogen_context: AutogenContext) -> Union[str, Literal[False]]:
         ...
     
 
 
@@ -75,15 +89,15 @@
 
 @Operations.register_operation("create_exclude_constraint")
 @BatchOperations.register_operation("create_exclude_constraint", "batch_create_exclude_constraint")
 @ops.AddConstraintOp.register_add_constraint("exclude_constraint")
 class CreateExcludeConstraintOp(ops.AddConstraintOp):
     """Represent a create exclude constraint operation."""
     constraint_type = ...
-    def __init__(self, constraint_name: sqla_compat._ConstraintName, table_name: Union[str, quoted_name], elements: Union[Sequence[Tuple[str, str]], Sequence[Tuple[ColumnClause[Any], str]],], where: Optional[Union[BinaryExpression, str]] = ..., schema: Optional[str] = ..., _orig_constraint: Optional[ExcludeConstraint] = ..., **kw) -> None:
+    def __init__(self, constraint_name: sqla_compat._ConstraintName, table_name: Union[str, quoted_name], elements: Union[Sequence[Tuple[str, str]], Sequence[Tuple[ColumnClause[Any], str]],], where: Optional[Union[ColumnElement[bool], str]] = ..., schema: Optional[str] = ..., _orig_constraint: Optional[ExcludeConstraint] = ..., **kw) -> None:
         ...
     
     @classmethod
     def from_constraint(cls, constraint: ExcludeConstraint) -> CreateExcludeConstraintOp:
         ...
     
     def to_constraint(self, migration_context: Optional[MigrationContext] = ...) -> ExcludeConstraint:
@@ -124,15 +138,15 @@
          when issuing DDL for this constraint.
         :param schema: Optional schema name to operate within.
 
         """
         ...
     
     @classmethod
-    def batch_create_exclude_constraint(cls, operations: BatchOperations, constraint_name: str, *elements: Any, **kw: Any): # -> Any:
+    def batch_create_exclude_constraint(cls, operations: BatchOperations, constraint_name: str, *elements: Any, **kw: Any) -> Optional[Table]:
         """Issue a "create exclude constraint" instruction using the
         current batch migration context.
 
         .. note::  This method is Postgresql specific, and additionally
            requires at least SQLAlchemy 1.0.
 
         .. seealso::
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/ddl/sqlite.pyi` & `bl_python_all-0.2.0/typings/alembic/ddl/sqlite.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This type stub file was generated by pyright.
 """
 
 from typing import Any, Dict, Optional, TYPE_CHECKING, Union
-from sqlalchemy.ext.compiler import compiles
 from .base import RenameTable
 from .impl import DefaultImpl
+from ..util.sqla_compat import compiles
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.sql.compiler import DDLCompiler
 from sqlalchemy.sql.elements import Cast, ClauseElement
 from sqlalchemy.sql.schema import Column, Constraint, Table
 from sqlalchemy.sql.type_api import TypeEngine
 from ..operations.batch import BatchOperationsImpl
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/op.pyi` & `bl_python_all-0.2.0/typings/alembic/op.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 This type stub file was generated by pyright.
 """
 
 from contextlib import contextmanager
-from typing import Any, Awaitable, Callable, Dict, Iterator, List, Literal, Mapping, Optional, Sequence, TYPE_CHECKING, Tuple, Type, TypeVar, Union
-from sqlalchemy.sql.expression import TableClause, Update
+from typing import Any, Awaitable, Callable, Dict, Iterator, List, Literal, Mapping, Optional, Sequence, TYPE_CHECKING, Tuple, Type, TypeVar, Union, overload
 from sqlalchemy.engine import Connection
-from sqlalchemy.sql.elements import BinaryExpression, TextClause, conv
+from sqlalchemy.sql import Executable
+from sqlalchemy.sql.elements import ColumnElement, TextClause, conv
+from sqlalchemy.sql.expression import TableClause
 from sqlalchemy.sql.functions import Function
 from sqlalchemy.sql.schema import Column, Computed, Identity, SchemaItem, Table
 from sqlalchemy.sql.type_api import TypeEngine
-from .operations.ops import BatchOperations, MigrateOperation
+from .operations.base import BatchOperations
+from .operations.ops import AddColumnOp, AddConstraintOp, AlterColumnOp, AlterTableOp, BulkInsertOp, CreateIndexOp, CreateTableCommentOp, CreateTableOp, DropColumnOp, DropConstraintOp, DropIndexOp, DropTableCommentOp, DropTableOp, ExecuteSQLOp, MigrateOperation
 from .runtime.migration import MigrationContext
 from .util.sqla_compat import _literal_bindparam
 
 if TYPE_CHECKING:
     ...
 _T = TypeVar("_T")
+_C = TypeVar("_C", bound=Callable[..., Any])
 def add_column(table_name: str, column: Column[Any], *, schema: Optional[str] = ...) -> None:
     """Issue an "add column" instruction using the current
     migration context.
 
     e.g.::
 
         from alembic import op
@@ -93,15 +96,15 @@
      quoting of the schema outside of the default behavior, use
      the SQLAlchemy construct
      :class:`~sqlalchemy.sql.elements.quoted_name`.
 
     """
     ...
 
-def alter_column(table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_type: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
+def alter_column(table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_type: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
     r"""Issue an "alter column" instruction using the
     current migration context.
 
     Generally, only that aspect of the column which
     is being changed, i.e. name, type, nullability,
     default, needs to be specified.  Multiple changes
     can also be specified at once and the backend should
@@ -132,17 +135,14 @@
     :param server_default: Optional; specify a string
      SQL expression, :func:`~sqlalchemy.sql.expression.text`,
      or :class:`~sqlalchemy.schema.DefaultClause` to indicate
      an alteration to the column's default value.
      Set to ``None`` to have the default removed.
     :param comment: optional string text of a new comment to add to the
      column.
-
-     .. versionadded:: 1.0.6
-
     :param new_column_name: Optional; specify a string name here to
      indicate the new name within a column rename operation.
     :param type\_: Optional; a :class:`~sqlalchemy.types.TypeEngine`
      type object to specify a change to the column's type.
      For SQLAlchemy types that also indicate a constraint (i.e.
      :class:`~sqlalchemy.types.Boolean`, :class:`~sqlalchemy.types.Enum`),
      the constraint is also generated.
@@ -151,15 +151,15 @@
     :param existing_type: Optional; a
      :class:`~sqlalchemy.types.TypeEngine`
      type object to specify the previous type.   This
      is required for all MySQL column alter operations that
      don't otherwise specify a new type, as well as for
      when nullability is being changed on a SQL Server
      column.  It is also used if the type is a so-called
-     SQLlchemy "schema" type which may define a constraint (i.e.
+     SQLAlchemy "schema" type which may define a constraint (i.e.
      :class:`~sqlalchemy.types.Boolean`,
      :class:`~sqlalchemy.types.Enum`),
      so that the constraint can be dropped.
     :param existing_server_default: Optional; The existing
      default value of the column.   Required on MySQL if
      an existing default is not being changed; else MySQL
      removes the default.
@@ -168,32 +168,29 @@
      is not being changed; else MySQL sets this to NULL.
     :param existing_autoincrement: Optional; the existing autoincrement
      of the column.  Used for MySQL's system of altering a column
      that specifies ``AUTO_INCREMENT``.
     :param existing_comment: string text of the existing comment on the
      column to be maintained.  Required on MySQL if the existing comment
      on the column is not being changed.
-
-     .. versionadded:: 1.0.6
-
     :param schema: Optional schema name to operate within.  To control
      quoting of the schema outside of the default behavior, use
      the SQLAlchemy construct
      :class:`~sqlalchemy.sql.elements.quoted_name`.
     :param postgresql_using: String argument which will indicate a
      SQL expression to render within the Postgresql-specific USING clause
      within ALTER COLUMN.    This string is taken directly as raw SQL which
      must explicitly include any necessary quoting or escaping of tokens
      within the expression.
 
     """
     ...
 
 @contextmanager
-def batch_alter_table(table_name: str, schema: Optional[str] = ..., recreate: Literal["auto", "always", "never"] = ..., partial_reordering: Optional[tuple] = ..., copy_from: Optional[Table] = ..., table_args: Tuple[Any, ...] = ..., table_kwargs: Mapping[str, Any] = ..., reflect_args: Tuple[Any, ...] = ..., reflect_kwargs: Mapping[str, Any] = ..., naming_convention: Optional[Dict[str, str]] = ...) -> Iterator[BatchOperations]:
+def batch_alter_table(table_name: str, schema: Optional[str] = ..., recreate: Literal["auto", "always", "never"] = ..., partial_reordering: Optional[Tuple[Any, ...]] = ..., copy_from: Optional[Table] = ..., table_args: Tuple[Any, ...] = ..., table_kwargs: Mapping[str, Any] = ..., reflect_args: Tuple[Any, ...] = ..., reflect_kwargs: Mapping[str, Any] = ..., naming_convention: Optional[Dict[str, str]] = ...) -> Iterator[BatchOperations]:
     """Invoke a series of per-table migrations in batch.
 
     Batch mode allows a series of operations specific to a table
     to be syntactically grouped together, and allows for alternate
     modes of table migration, in particular the "recreate" style of
     migration required by SQLite.
 
@@ -315,26 +312,24 @@
         ) as batch_op:
             pass
 
      The ordering of columns not included in the partial_reordering
      set is undefined.   Therefore it is best to specify the complete
      ordering of all columns for best results.
 
-     .. versionadded:: 1.4.0
-
     .. note:: batch mode requires SQLAlchemy 0.8 or above.
 
     .. seealso::
 
         :ref:`batch_migrations`
 
     """
     ...
 
-def bulk_insert(table: Union[Table, TableClause], rows: List[dict], *, multiinsert: bool = ...) -> None:
+def bulk_insert(table: Union[Table, TableClause], rows: List[Dict[str, Any]], *, multiinsert: bool = ...) -> None:
     """Issue a "bulk insert" operation using the current
     migration context.
 
     This provides a means of representing an INSERT of multiple rows
     which works equally well in the context of executing on a live
     connection as well as that of generating a SQL script.   In the
     case of a SQL script, the values are rendered inline into the
@@ -424,15 +419,15 @@
        statements being emitted per parameter set, and is needed
        in those cases where non-literal values are present in the
        parameter sets.
 
     """
     ...
 
-def create_check_constraint(constraint_name: Optional[str], table_name: str, condition: Union[str, BinaryExpression, TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
+def create_check_constraint(constraint_name: Optional[str], table_name: str, condition: Union[str, ColumnElement[bool], TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
     """Issue a "create check constraint" instruction using the
     current migration context.
 
     e.g.::
 
         from alembic import op
         from sqlalchemy.sql import column, func
@@ -556,15 +551,15 @@
      DEFERRABLE when issuing DDL for this constraint.
     :param source_schema: Optional schema name of the source table.
     :param referent_schema: Optional schema name of the destination table.
 
     """
     ...
 
-def create_index(index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., **kw: Any) -> None:
+def create_index(index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., if_not_exists: Optional[bool] = ..., **kw: Any) -> None:
     r"""Issue a "create index" instruction using the current
     migration context.
 
     e.g.::
 
         from alembic import op
 
@@ -584,28 +579,32 @@
      :func:`~sqlalchemy.sql.expression.text` constructs.
     :param schema: Optional schema name to operate within.  To control
      quoting of the schema outside of the default behavior, use
      the SQLAlchemy construct
      :class:`~sqlalchemy.sql.elements.quoted_name`.
     :param unique: If True, create a unique index.
 
-    :param quote:
-        Force quoting of this column's name on or off, corresponding
-        to ``True`` or ``False``. When left at its default
-        of ``None``, the column identifier will be quoted according to
-        whether the name is case sensitive (identifiers with at least one
-        upper case character are treated as case sensitive), or if it's a
-        reserved word. This flag is only needed to force quoting of a
-        reserved word which is not known by the SQLAlchemy dialect.
+    :param quote: Force quoting of this column's name on or off,
+     corresponding to ``True`` or ``False``. When left at its default
+     of ``None``, the column identifier will be quoted according to
+     whether the name is case sensitive (identifiers with at least one
+     upper case character are treated as case sensitive), or if it's a
+     reserved word. This flag is only needed to force quoting of a
+     reserved word which is not known by the SQLAlchemy dialect.
+
+    :param if_not_exists: If True, adds IF NOT EXISTS operator when
+     creating the new index.
+
+     .. versionadded:: 1.12.0
 
     :param \**kw: Additional keyword arguments not mentioned above are
-        dialect specific, and passed in the form
-        ``<dialectname>_<argname>``.
-        See the documentation regarding an individual dialect at
-        :ref:`dialect_toplevel` for detail on documented arguments.
+     dialect specific, and passed in the form
+     ``<dialectname>_<argname>``.
+     See the documentation regarding an individual dialect at
+     :ref:`dialect_toplevel` for detail on documented arguments.
 
     """
     ...
 
 def create_primary_key(constraint_name: Optional[str], table_name: str, columns: List[str], *, schema: Optional[str] = ...) -> None:
     """Issue a "create primary key" instruction using the current
     migration context.
@@ -722,16 +721,14 @@
 
     """
     ...
 
 def create_table_comment(table_name: str, comment: Optional[str], *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
     """Emit a COMMENT ON operation to set the comment for a table.
 
-    .. versionadded:: 1.0.6
-
     :param table_name: string name of the target table.
     :param comment: string value of the comment being registered against
      the specified table.
     :param existing_comment: String value of a comment
      already registered on the specified table, used within autogenerate
      so that the operation is reversible, but not required for direct
      use.
@@ -835,34 +832,40 @@
      quoting of the schema outside of the default behavior, use
      the SQLAlchemy construct
      :class:`~sqlalchemy.sql.elements.quoted_name`.
 
     """
     ...
 
-def drop_index(index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., **kw: Any) -> None:
+def drop_index(index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., if_exists: Optional[bool] = ..., **kw: Any) -> None:
     r"""Issue a "drop index" instruction using the current
     migration context.
 
     e.g.::
 
         drop_index("accounts")
 
     :param index_name: name of the index.
     :param table_name: name of the owning table.  Some
      backends such as Microsoft SQL Server require this.
     :param schema: Optional schema name to operate within.  To control
      quoting of the schema outside of the default behavior, use
      the SQLAlchemy construct
      :class:`~sqlalchemy.sql.elements.quoted_name`.
+
+    :param if_exists: If True, adds IF EXISTS operator when
+     dropping the index.
+
+     .. versionadded:: 1.12.0
+
     :param \**kw: Additional keyword arguments not mentioned above are
-        dialect specific, and passed in the form
-        ``<dialectname>_<argname>``.
-        See the documentation regarding an individual dialect at
-        :ref:`dialect_toplevel` for detail on documented arguments.
+     dialect specific, and passed in the form
+     ``<dialectname>_<argname>``.
+     See the documentation regarding an individual dialect at
+     :ref:`dialect_toplevel` for detail on documented arguments.
 
     """
     ...
 
 def drop_table(table_name: str, *, schema: Optional[str] = ..., **kw: Any) -> None:
     r"""Issue a "drop table" instruction using the current
     migration context.
@@ -883,30 +886,28 @@
     """
     ...
 
 def drop_table_comment(table_name: str, *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
     """Issue a "drop table comment" operation to
     remove an existing comment set on a table.
 
-    .. versionadded:: 1.0.6
-
     :param table_name: string name of the target table.
     :param existing_comment: An optional string value of a comment already
      registered on the specified table.
 
     .. seealso::
 
         :meth:`.Operations.create_table_comment`
 
         :paramref:`.Operations.alter_column.comment`
 
     """
     ...
 
-def execute(sqltext: Union[str, TextClause, Update], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+def execute(sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
     r"""Execute the given SQL using the current migration context.
 
     The given SQL can be a plain string, e.g.::
 
         op.execute("INSERT INTO table (foo) VALUES ('some value')")
 
     Or it can be any kind of Core SQL Expression construct, such as
@@ -951,30 +952,29 @@
         connection.execute(
             account.update()
             .where(account.c.name == "account 1")
             .values({"name": "account 2"})
         )
 
     Additionally, when passing the statement as a plain string, it is first
-    coerceed into a :func:`sqlalchemy.sql.expression.text` construct
+    coerced into a :func:`sqlalchemy.sql.expression.text` construct
     before being passed along.  In the less likely case that the
     literal SQL string contains a colon, it must be escaped with a
     backslash, as::
 
        op.execute(r"INSERT INTO table (foo) VALUES ('\:colon_value')")
 
 
     :param sqltext: Any legal SQLAlchemy expression, including:
 
     * a string
     * a :func:`sqlalchemy.sql.expression.text` construct.
     * a :func:`sqlalchemy.sql.expression.insert` construct.
-    * a :func:`sqlalchemy.sql.expression.update`,
-      :func:`sqlalchemy.sql.expression.insert`,
-      or :func:`sqlalchemy.sql.expression.delete`  construct.
+    * a :func:`sqlalchemy.sql.expression.update` construct.
+    * a :func:`sqlalchemy.sql.expression.delete` construct.
     * Any "executable" described in SQLAlchemy Core documentation,
       noting that no result set is returned.
 
     .. note::  when passing a plain string, the statement is coerced into
        a :func:`sqlalchemy.sql.expression.text` construct. This construct
        considers symbols with colons, e.g. ``:foo`` to be bound parameters.
        To avoid this, ensure that colon symbols are escaped, e.g.
@@ -1039,27 +1039,27 @@
 def get_context() -> MigrationContext:
     """Return the :class:`.MigrationContext` object that's
     currently in use.
 
     """
     ...
 
-def implementation_for(op_cls: Any) -> Callable[..., Any]:
+def implementation_for(op_cls: Any) -> Callable[[_C], _C]:
     """Register an implementation for a given :class:`.MigrateOperation`.
 
     This is part of the operation extensibility API.
 
     .. seealso::
 
         :ref:`operation_plugins` - example of use
 
     """
     ...
 
-def inline_literal(value: Union[str, int], type_: Optional[TypeEngine] = ...) -> _literal_bindparam:
+def inline_literal(value: Union[str, int], type_: Optional[TypeEngine[Any]] = ...) -> _literal_bindparam:
     r"""Produce an 'inline literal' expression, suitable for
     using in an INSERT, UPDATE, or DELETE statement.
 
     When using Alembic in "offline" mode, CRUD operations
     aren't compatible with SQLAlchemy's default behavior surrounding
     literal values,
     which is that they are converted into bound values and passed
@@ -1095,22 +1095,31 @@
     .. seealso::
 
         :paramref:`.EnvironmentContext.configure.literal_binds`
 
     """
     ...
 
+@overload
+def invoke(operation: CreateTableOp) -> Table:
+    ...
+
+@overload
+def invoke(operation: Union[AddConstraintOp, DropConstraintOp, CreateIndexOp, DropIndexOp, AddColumnOp, AlterColumnOp, AlterTableOp, CreateTableCommentOp, DropTableCommentOp, DropColumnOp, BulkInsertOp, DropTableOp, ExecuteSQLOp,]) -> None:
+    ...
+
+@overload
 def invoke(operation: MigrateOperation) -> Any:
     """Given a :class:`.MigrateOperation`, invoke it in terms of
     this :class:`.Operations` instance.
 
     """
     ...
 
-def register_operation(name: str, sourcename: Optional[str] = ...) -> Callable[..., Any]:
+def register_operation(name: str, sourcename: Optional[str] = ...) -> Callable[[Type[_T]], Type[_T]]:
     """Register a new operation for this class.
 
     This method is normally used to add new operations
     to the :class:`.Operations` class, and possibly the
     :class:`.BatchOperations` class as well.   All Alembic migration
     operations are implemented via this system, however the system
     is also available as a public API to facilitate adding custom
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/operations/base.pyi` & `bl_python_all-0.2.0/typings/alembic/operations/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """
 This type stub file was generated by pyright.
 """
 
 from contextlib import contextmanager
-from typing import Any, Awaitable, Callable, Dict, Iterator, List, Literal, Mapping, Optional, Sequence, TYPE_CHECKING, Tuple, Type, TypeVar, Union
+from typing import Any, Awaitable, Callable, Dict, Iterator, List, Literal, Mapping, Optional, Sequence, TYPE_CHECKING, Tuple, Type, TypeVar, Union, overload
 from sqlalchemy.sql.elements import conv
 from .. import util
 from ..util.sqla_compat import _literal_bindparam
 from sqlalchemy import Table
 from sqlalchemy.engine import Connection
-from sqlalchemy.sql.expression import BinaryExpression, TableClause, TextClause, Update
+from sqlalchemy.sql import Executable
+from sqlalchemy.sql.expression import ColumnElement, TableClause, TextClause
 from sqlalchemy.sql.functions import Function
 from sqlalchemy.sql.schema import Column, Computed, Identity, SchemaItem
 from sqlalchemy.types import TypeEngine
 from .batch import BatchOperationsImpl
-from .ops import MigrateOperation
+from .ops import AddColumnOp, AddConstraintOp, AlterColumnOp, AlterTableOp, BulkInsertOp, CreateIndexOp, CreateTableCommentOp, CreateTableOp, DropColumnOp, DropConstraintOp, DropIndexOp, DropTableCommentOp, DropTableOp, ExecuteSQLOp, MigrateOperation
 from ..ddl import DefaultImpl
 from ..runtime.migration import MigrationContext
 
 if TYPE_CHECKING:
     ...
 __all__ = ("Operations", "BatchOperations")
 _T = TypeVar("_T")
+_C = TypeVar("_C", bound=Callable[..., Any])
 class AbstractOperations(util.ModuleClsProxy):
     """Base class for Operations and BatchOperations.
 
     .. versionadded:: 1.11.0
 
     """
     impl: Union[DefaultImpl, BatchOperationsImpl]
@@ -36,15 +38,15 @@
         :param migration_context: a :class:`.MigrationContext`
          instance.
 
         """
         ...
     
     @classmethod
-    def register_operation(cls, name: str, sourcename: Optional[str] = ...) -> Callable[..., Any]:
+    def register_operation(cls, name: str, sourcename: Optional[str] = ...) -> Callable[[Type[_T]], Type[_T]]:
         """Register a new operation for this class.
 
         This method is normally used to add new operations
         to the :class:`.Operations` class, and possibly the
         :class:`.BatchOperations` class as well.   All Alembic migration
         operations are implemented via this system, however the system
         is also available as a public API to facilitate adding custom
@@ -55,15 +57,15 @@
             :ref:`operation_plugins`
 
 
         """
         ...
     
     @classmethod
-    def implementation_for(cls, op_cls: Any) -> Callable[..., Any]:
+    def implementation_for(cls, op_cls: Any) -> Callable[[_C], _C]:
         """Register an implementation for a given :class:`.MigrateOperation`.
 
         This is part of the operation extensibility API.
 
         .. seealso::
 
             :ref:`operation_plugins` - example of use
@@ -73,15 +75,15 @@
     
     @classmethod
     @contextmanager
     def context(cls, migration_context: MigrationContext) -> Iterator[Operations]:
         ...
     
     @contextmanager
-    def batch_alter_table(self, table_name: str, schema: Optional[str] = ..., recreate: Literal["auto", "always", "never"] = ..., partial_reordering: Optional[tuple] = ..., copy_from: Optional[Table] = ..., table_args: Tuple[Any, ...] = ..., table_kwargs: Mapping[str, Any] = ..., reflect_args: Tuple[Any, ...] = ..., reflect_kwargs: Mapping[str, Any] = ..., naming_convention: Optional[Dict[str, str]] = ...) -> Iterator[BatchOperations]:
+    def batch_alter_table(self, table_name: str, schema: Optional[str] = ..., recreate: Literal["auto", "always", "never"] = ..., partial_reordering: Optional[Tuple[Any, ...]] = ..., copy_from: Optional[Table] = ..., table_args: Tuple[Any, ...] = ..., table_kwargs: Mapping[str, Any] = ..., reflect_args: Tuple[Any, ...] = ..., reflect_kwargs: Mapping[str, Any] = ..., naming_convention: Optional[Dict[str, str]] = ...) -> Iterator[BatchOperations]:
         """Invoke a series of per-table migrations in batch.
 
         Batch mode allows a series of operations specific to a table
         to be syntactically grouped together, and allows for alternate
         modes of table migration, in particular the "recreate" style of
         migration required by SQLite.
 
@@ -203,16 +205,14 @@
             ) as batch_op:
                 pass
 
          The ordering of columns not included in the partial_reordering
          set is undefined.   Therefore it is best to specify the complete
          ordering of all columns for best results.
 
-         .. versionadded:: 1.4.0
-
         .. note:: batch mode requires SQLAlchemy 0.8 or above.
 
         .. seealso::
 
             :ref:`batch_migrations`
 
         """
@@ -221,14 +221,26 @@
     def get_context(self) -> MigrationContext:
         """Return the :class:`.MigrationContext` object that's
         currently in use.
 
         """
         ...
     
+    @overload
+    def invoke(self, operation: CreateTableOp) -> Table:
+        ...
+    
+    @overload
+    def invoke(self, operation: Union[AddConstraintOp, DropConstraintOp, CreateIndexOp, DropIndexOp, AddColumnOp, AlterColumnOp, AlterTableOp, CreateTableCommentOp, DropTableCommentOp, DropColumnOp, BulkInsertOp, DropTableOp, ExecuteSQLOp,]) -> None:
+        ...
+    
+    @overload
+    def invoke(self, operation: MigrateOperation) -> Any:
+        ...
+    
     def invoke(self, operation: MigrateOperation) -> Any:
         """Given a :class:`.MigrateOperation`, invoke it in terms of
         this :class:`.Operations` instance.
 
         """
         ...
     
@@ -458,15 +470,15 @@
              quoting of the schema outside of the default behavior, use
              the SQLAlchemy construct
              :class:`~sqlalchemy.sql.elements.quoted_name`.
 
             """
             ...
         
-        def alter_column(self, table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_type: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
+        def alter_column(self, table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_type: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
             r"""Issue an "alter column" instruction using the
             current migration context.
 
             Generally, only that aspect of the column which
             is being changed, i.e. name, type, nullability,
             default, needs to be specified.  Multiple changes
             can also be specified at once and the backend should
@@ -497,17 +509,14 @@
             :param server_default: Optional; specify a string
              SQL expression, :func:`~sqlalchemy.sql.expression.text`,
              or :class:`~sqlalchemy.schema.DefaultClause` to indicate
              an alteration to the column's default value.
              Set to ``None`` to have the default removed.
             :param comment: optional string text of a new comment to add to the
              column.
-
-             .. versionadded:: 1.0.6
-
             :param new_column_name: Optional; specify a string name here to
              indicate the new name within a column rename operation.
             :param type\_: Optional; a :class:`~sqlalchemy.types.TypeEngine`
              type object to specify a change to the column's type.
              For SQLAlchemy types that also indicate a constraint (i.e.
              :class:`~sqlalchemy.types.Boolean`, :class:`~sqlalchemy.types.Enum`),
              the constraint is also generated.
@@ -516,15 +525,15 @@
             :param existing_type: Optional; a
              :class:`~sqlalchemy.types.TypeEngine`
              type object to specify the previous type.   This
              is required for all MySQL column alter operations that
              don't otherwise specify a new type, as well as for
              when nullability is being changed on a SQL Server
              column.  It is also used if the type is a so-called
-             SQLlchemy "schema" type which may define a constraint (i.e.
+             SQLAlchemy "schema" type which may define a constraint (i.e.
              :class:`~sqlalchemy.types.Boolean`,
              :class:`~sqlalchemy.types.Enum`),
              so that the constraint can be dropped.
             :param existing_server_default: Optional; The existing
              default value of the column.   Required on MySQL if
              an existing default is not being changed; else MySQL
              removes the default.
@@ -533,31 +542,28 @@
              is not being changed; else MySQL sets this to NULL.
             :param existing_autoincrement: Optional; the existing autoincrement
              of the column.  Used for MySQL's system of altering a column
              that specifies ``AUTO_INCREMENT``.
             :param existing_comment: string text of the existing comment on the
              column to be maintained.  Required on MySQL if the existing comment
              on the column is not being changed.
-
-             .. versionadded:: 1.0.6
-
             :param schema: Optional schema name to operate within.  To control
              quoting of the schema outside of the default behavior, use
              the SQLAlchemy construct
              :class:`~sqlalchemy.sql.elements.quoted_name`.
             :param postgresql_using: String argument which will indicate a
              SQL expression to render within the Postgresql-specific USING clause
              within ALTER COLUMN.    This string is taken directly as raw SQL which
              must explicitly include any necessary quoting or escaping of tokens
              within the expression.
 
             """
             ...
         
-        def bulk_insert(self, table: Union[Table, TableClause], rows: List[dict], *, multiinsert: bool = ...) -> None:
+        def bulk_insert(self, table: Union[Table, TableClause], rows: List[Dict[str, Any]], *, multiinsert: bool = ...) -> None:
             """Issue a "bulk insert" operation using the current
             migration context.
 
             This provides a means of representing an INSERT of multiple rows
             which works equally well in the context of executing on a live
             connection as well as that of generating a SQL script.   In the
             case of a SQL script, the values are rendered inline into the
@@ -647,15 +653,15 @@
                statements being emitted per parameter set, and is needed
                in those cases where non-literal values are present in the
                parameter sets.
 
             """
             ...
         
-        def create_check_constraint(self, constraint_name: Optional[str], table_name: str, condition: Union[str, BinaryExpression, TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
+        def create_check_constraint(self, constraint_name: Optional[str], table_name: str, condition: Union[str, ColumnElement[bool], TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
             """Issue a "create check constraint" instruction using the
             current migration context.
 
             e.g.::
 
                 from alembic import op
                 from sqlalchemy.sql import column, func
@@ -779,15 +785,15 @@
              DEFERRABLE when issuing DDL for this constraint.
             :param source_schema: Optional schema name of the source table.
             :param referent_schema: Optional schema name of the destination table.
 
             """
             ...
         
-        def create_index(self, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., **kw: Any) -> None:
+        def create_index(self, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., if_not_exists: Optional[bool] = ..., **kw: Any) -> None:
             r"""Issue a "create index" instruction using the current
             migration context.
 
             e.g.::
 
                 from alembic import op
 
@@ -807,28 +813,32 @@
              :func:`~sqlalchemy.sql.expression.text` constructs.
             :param schema: Optional schema name to operate within.  To control
              quoting of the schema outside of the default behavior, use
              the SQLAlchemy construct
              :class:`~sqlalchemy.sql.elements.quoted_name`.
             :param unique: If True, create a unique index.
 
-            :param quote:
-                Force quoting of this column's name on or off, corresponding
-                to ``True`` or ``False``. When left at its default
-                of ``None``, the column identifier will be quoted according to
-                whether the name is case sensitive (identifiers with at least one
-                upper case character are treated as case sensitive), or if it's a
-                reserved word. This flag is only needed to force quoting of a
-                reserved word which is not known by the SQLAlchemy dialect.
+            :param quote: Force quoting of this column's name on or off,
+             corresponding to ``True`` or ``False``. When left at its default
+             of ``None``, the column identifier will be quoted according to
+             whether the name is case sensitive (identifiers with at least one
+             upper case character are treated as case sensitive), or if it's a
+             reserved word. This flag is only needed to force quoting of a
+             reserved word which is not known by the SQLAlchemy dialect.
+
+            :param if_not_exists: If True, adds IF NOT EXISTS operator when
+             creating the new index.
+
+             .. versionadded:: 1.12.0
 
             :param \**kw: Additional keyword arguments not mentioned above are
-                dialect specific, and passed in the form
-                ``<dialectname>_<argname>``.
-                See the documentation regarding an individual dialect at
-                :ref:`dialect_toplevel` for detail on documented arguments.
+             dialect specific, and passed in the form
+             ``<dialectname>_<argname>``.
+             See the documentation regarding an individual dialect at
+             :ref:`dialect_toplevel` for detail on documented arguments.
 
             """
             ...
         
         def create_primary_key(self, constraint_name: Optional[str], table_name: str, columns: List[str], *, schema: Optional[str] = ...) -> None:
             """Issue a "create primary key" instruction using the current
             migration context.
@@ -945,16 +955,14 @@
 
             """
             ...
         
         def create_table_comment(self, table_name: str, comment: Optional[str], *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
             """Emit a COMMENT ON operation to set the comment for a table.
 
-            .. versionadded:: 1.0.6
-
             :param table_name: string name of the target table.
             :param comment: string value of the comment being registered against
              the specified table.
             :param existing_comment: String value of a comment
              already registered on the specified table, used within autogenerate
              so that the operation is reversible, but not required for direct
              use.
@@ -1058,34 +1066,40 @@
              quoting of the schema outside of the default behavior, use
              the SQLAlchemy construct
              :class:`~sqlalchemy.sql.elements.quoted_name`.
 
             """
             ...
         
-        def drop_index(self, index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., **kw: Any) -> None:
+        def drop_index(self, index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., if_exists: Optional[bool] = ..., **kw: Any) -> None:
             r"""Issue a "drop index" instruction using the current
             migration context.
 
             e.g.::
 
                 drop_index("accounts")
 
             :param index_name: name of the index.
             :param table_name: name of the owning table.  Some
              backends such as Microsoft SQL Server require this.
             :param schema: Optional schema name to operate within.  To control
              quoting of the schema outside of the default behavior, use
              the SQLAlchemy construct
              :class:`~sqlalchemy.sql.elements.quoted_name`.
+
+            :param if_exists: If True, adds IF EXISTS operator when
+             dropping the index.
+
+             .. versionadded:: 1.12.0
+
             :param \**kw: Additional keyword arguments not mentioned above are
-                dialect specific, and passed in the form
-                ``<dialectname>_<argname>``.
-                See the documentation regarding an individual dialect at
-                :ref:`dialect_toplevel` for detail on documented arguments.
+             dialect specific, and passed in the form
+             ``<dialectname>_<argname>``.
+             See the documentation regarding an individual dialect at
+             :ref:`dialect_toplevel` for detail on documented arguments.
 
             """
             ...
         
         def drop_table(self, table_name: str, *, schema: Optional[str] = ..., **kw: Any) -> None:
             r"""Issue a "drop table" instruction using the current
             migration context.
@@ -1106,30 +1120,28 @@
             """
             ...
         
         def drop_table_comment(self, table_name: str, *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
             """Issue a "drop table comment" operation to
             remove an existing comment set on a table.
 
-            .. versionadded:: 1.0.6
-
             :param table_name: string name of the target table.
             :param existing_comment: An optional string value of a comment already
              registered on the specified table.
 
             .. seealso::
 
                 :meth:`.Operations.create_table_comment`
 
                 :paramref:`.Operations.alter_column.comment`
 
             """
             ...
         
-        def execute(self, sqltext: Union[str, TextClause, Update], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+        def execute(self, sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
             r"""Execute the given SQL using the current migration context.
 
             The given SQL can be a plain string, e.g.::
 
                 op.execute("INSERT INTO table (foo) VALUES ('some value')")
 
             Or it can be any kind of Core SQL Expression construct, such as
@@ -1174,30 +1186,29 @@
                 connection.execute(
                     account.update()
                     .where(account.c.name == "account 1")
                     .values({"name": "account 2"})
                 )
 
             Additionally, when passing the statement as a plain string, it is first
-            coerceed into a :func:`sqlalchemy.sql.expression.text` construct
+            coerced into a :func:`sqlalchemy.sql.expression.text` construct
             before being passed along.  In the less likely case that the
             literal SQL string contains a colon, it must be escaped with a
             backslash, as::
 
                op.execute(r"INSERT INTO table (foo) VALUES ('\:colon_value')")
 
 
             :param sqltext: Any legal SQLAlchemy expression, including:
 
             * a string
             * a :func:`sqlalchemy.sql.expression.text` construct.
             * a :func:`sqlalchemy.sql.expression.insert` construct.
-            * a :func:`sqlalchemy.sql.expression.update`,
-              :func:`sqlalchemy.sql.expression.insert`,
-              or :func:`sqlalchemy.sql.expression.delete`  construct.
+            * a :func:`sqlalchemy.sql.expression.update` construct.
+            * a :func:`sqlalchemy.sql.expression.delete` construct.
             * Any "executable" described in SQLAlchemy Core documentation,
               noting that no result set is returned.
 
             .. note::  when passing a plain string, the statement is coerced into
                a :func:`sqlalchemy.sql.expression.text` construct. This construct
                considers symbols with colons, e.g. ``:foo`` to be bound parameters.
                To avoid this, ensure that colon symbols are escaped, e.g.
@@ -1249,58 +1260,54 @@
             .. seealso::
 
                 :meth:`.Operations.add_column`
 
             """
             ...
         
-        def alter_column(self, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_type: Union[TypeEngine, Type[TypeEngine], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., insert_before: Optional[str] = ..., insert_after: Optional[str] = ..., **kw: Any) -> None:
+        def alter_column(self, column_name: str, *, nullable: Optional[bool] = ..., comment: Union[str, Literal[False], None] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_type: Union[TypeEngine[Any], Type[TypeEngine[Any]], None] = ..., existing_server_default: Union[str, bool, Identity, Computed, None] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., insert_before: Optional[str] = ..., insert_after: Optional[str] = ..., **kw: Any) -> None:
             """Issue an "alter column" instruction using the current
             batch migration context.
 
             Parameters are the same as that of :meth:`.Operations.alter_column`,
             as well as the following option(s):
 
             :param insert_before: String name of an existing column which this
              column should be placed before, when creating the new table.
 
-             .. versionadded:: 1.4.0
-
             :param insert_after: String name of an existing column which this
              column should be placed after, when creating the new table.  If
              both :paramref:`.BatchOperations.alter_column.insert_before`
              and :paramref:`.BatchOperations.alter_column.insert_after` are
              omitted, the column is inserted after the last existing column
              in the table.
 
-             .. versionadded:: 1.4.0
-
             .. seealso::
 
                 :meth:`.Operations.alter_column`
 
 
             """
             ...
         
-        def create_check_constraint(self, constraint_name: str, condition: Union[str, BinaryExpression, TextClause], **kw: Any) -> None:
+        def create_check_constraint(self, constraint_name: str, condition: Union[str, ColumnElement[bool], TextClause], **kw: Any) -> None:
             """Issue a "create check constraint" instruction using the
             current batch migration context.
 
             The batch form of this call omits the ``source`` and ``schema``
             arguments from the call.
 
             .. seealso::
 
                 :meth:`.Operations.create_check_constraint`
 
             """
             ...
         
-        def create_exclude_constraint(self, constraint_name: str, *elements: Any, **kw: Any): # -> None:
+        def create_exclude_constraint(self, constraint_name: str, *elements: Any, **kw: Any) -> Optional[Table]:
             """Issue a "create exclude constraint" instruction using the
             current batch migration context.
 
             .. note::  This method is Postgresql specific, and additionally
                requires at least SQLAlchemy 1.0.
 
             .. seealso::
@@ -1359,16 +1366,14 @@
             """
             ...
         
         def create_table_comment(self, comment: Optional[str], *, existing_comment: Optional[str] = ...) -> None:
             """Emit a COMMENT ON operation to set the comment for a table
             using the current batch migration context.
 
-            .. versionadded:: 1.6.0
-
             :param comment: string value of the comment being registered against
              the specified table.
             :param existing_comment: String value of a comment
              already registered on the specified table, used within autogenerate
              so that the operation is reversible, but not required for direct
              use.
 
@@ -1426,23 +1431,21 @@
             ...
         
         def drop_table_comment(self, *, existing_comment: Optional[str] = ...) -> None:
             """Issue a "drop table comment" operation to
             remove an existing comment set on a table using the current
             batch operations context.
 
-            .. versionadded:: 1.6.0
-
             :param existing_comment: An optional string value of a comment already
              registered on the specified table.
 
             """
             ...
         
-        def execute(self, sqltext: Union[str, TextClause, Update], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+        def execute(self, sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
             """Execute the given SQL using the current migration context.
 
             .. seealso::
 
                 :meth:`.Operations.execute`
 
             """
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/operations/batch.pyi` & `bl_python_all-0.2.0/typings/alembic/operations/batch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 This type stub file was generated by pyright.
 """
 
 from typing import Any, Dict, Literal, Optional, TYPE_CHECKING, Union
 from sqlalchemy import Column, Index, Table
+from sqlalchemy.sql.schema import Constraint
 from sqlalchemy.engine import Dialect
 from sqlalchemy.sql.elements import ColumnClause
 from sqlalchemy.sql.functions import Function
-from sqlalchemy.sql.schema import Constraint
 from sqlalchemy.sql.type_api import TypeEngine
 from ..ddl.impl import DefaultImpl
 
 if TYPE_CHECKING:
     ...
 class BatchOperationsImpl:
     def __init__(self, operations, table_name, schema, recreate, copy_from, table_args, table_kwargs, reflect_args, reflect_kwargs, naming_convention, partial_reordering) -> None:
@@ -42,18 +42,18 @@
     
     def drop_constraint(self, const: Constraint) -> None:
         ...
     
     def rename_table(self, *arg, **kw): # -> None:
         ...
     
-    def create_index(self, idx: Index) -> None:
+    def create_index(self, idx: Index, **kw: Any) -> None:
         ...
     
-    def drop_index(self, idx: Index) -> None:
+    def drop_index(self, idx: Index, **kw: Any) -> None:
         ...
     
     def create_table_comment(self, table): # -> None:
         ...
     
     def drop_table_comment(self, table): # -> None:
         ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/operations/ops.pyi` & `bl_python_all-0.2.0/typings/alembic/operations/ops.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 This type stub file was generated by pyright.
 """
 
 from abc import abstractmethod
-from typing import Any, Callable, FrozenSet, List, Literal, MutableMapping, Optional, Sequence, Set, TYPE_CHECKING, Tuple, Type, Union
+from typing import Any, Callable, Dict, FrozenSet, List, Literal, MutableMapping, Optional, Sequence, Set, TYPE_CHECKING, Tuple, Type, TypeVar, Union
 from .base import BatchOperations, Operations
 from .. import util
 from ..util import sqla_compat
-from sqlalchemy.sql.dml import Insert, Update
-from sqlalchemy.sql.elements import BinaryExpression, ColumnElement, TextClause, conv, quoted_name
+from sqlalchemy.sql import Executable
+from sqlalchemy.sql.elements import ColumnElement, TextClause, conv, quoted_name
 from sqlalchemy.sql.functions import Function
 from sqlalchemy.sql.schema import CheckConstraint, Column, Computed, Constraint, ForeignKeyConstraint, Identity, Index, MetaData, PrimaryKeyConstraint, SchemaItem, Table, UniqueConstraint
 from sqlalchemy.sql.selectable import TableClause
 from sqlalchemy.sql.type_api import TypeEngine
 from ..autogenerate.rewriter import Rewriter
 from ..runtime.migration import MigrationContext
+from ..script.revision import _RevIdType
 
 if TYPE_CHECKING:
     ...
+_T = TypeVar("_T", bound=Any)
+_AC = TypeVar("_AC", bound="AddConstraintOp")
 class MigrateOperation:
     """base class for migration command and organization objects.
 
     This system is part of the operation extensibility API.
 
     .. seealso::
 
@@ -29,15 +32,15 @@
 
         :ref:`operation_plugins`
 
         :ref:`customizing_revision`
 
     """
     @util.memoized_property
-    def info(self): # -> dict[Unknown, Unknown]:
+    def info(self) -> Dict[Any, Any]:
         """A dictionary that may be used to store arbitrary information
         along with this :class:`.MigrateOperation` object.
 
         """
         ...
     
     _mutations: FrozenSet[Rewriter] = ...
@@ -49,19 +52,19 @@
     
 
 
 class AddConstraintOp(MigrateOperation):
     """Represent an add constraint operation."""
     add_constraint_ops = ...
     @property
-    def constraint_type(self):
+    def constraint_type(self) -> str:
         ...
     
     @classmethod
-    def register_add_constraint(cls, type_: str) -> Callable:
+    def register_add_constraint(cls, type_: str) -> Callable[[Type[_AC]], Type[_AC]]:
         ...
     
     @classmethod
     def from_constraint(cls, constraint: Constraint) -> AddConstraintOp:
         ...
     
     @abstractmethod
@@ -388,15 +391,15 @@
     def from_constraint(cls, constraint: Constraint) -> CreateCheckConstraintOp:
         ...
     
     def to_constraint(self, migration_context: Optional[MigrationContext] = ...) -> CheckConstraint:
         ...
     
     @classmethod
-    def create_check_constraint(cls, operations: Operations, constraint_name: Optional[str], table_name: str, condition: Union[str, BinaryExpression, TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
+    def create_check_constraint(cls, operations: Operations, constraint_name: Optional[str], table_name: str, condition: Union[str, ColumnElement[bool], TextClause], *, schema: Optional[str] = ..., **kw: Any) -> None:
         """Issue a "create check constraint" instruction using the
         current migration context.
 
         e.g.::
 
             from alembic import op
             from sqlalchemy.sql import column, func
@@ -432,15 +435,15 @@
          the SQLAlchemy construct
          :class:`~sqlalchemy.sql.elements.quoted_name`.
 
         """
         ...
     
     @classmethod
-    def batch_create_check_constraint(cls, operations: BatchOperations, constraint_name: str, condition: Union[str, BinaryExpression, TextClause], **kw: Any) -> None:
+    def batch_create_check_constraint(cls, operations: BatchOperations, constraint_name: str, condition: Union[str, ColumnElement[bool], TextClause], **kw: Any) -> None:
         """Issue a "create check constraint" instruction using the
         current batch migration context.
 
         The batch form of this call omits the ``source`` and ``schema``
         arguments from the call.
 
         .. seealso::
@@ -452,15 +455,15 @@
     
 
 
 @Operations.register_operation("create_index")
 @BatchOperations.register_operation("create_index", "batch_create_index")
 class CreateIndexOp(MigrateOperation):
     """Represent a create index operation."""
-    def __init__(self, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, ColumnElement[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., **kw: Any) -> None:
+    def __init__(self, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, ColumnElement[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., if_not_exists: Optional[bool] = ..., **kw: Any) -> None:
         ...
     
     def reverse(self) -> DropIndexOp:
         ...
     
     def to_diff_tuple(self) -> Tuple[str, Index]:
         ...
@@ -469,15 +472,15 @@
     def from_index(cls, index: Index) -> CreateIndexOp:
         ...
     
     def to_index(self, migration_context: Optional[MigrationContext] = ...) -> Index:
         ...
     
     @classmethod
-    def create_index(cls, operations: Operations, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., **kw: Any) -> None:
+    def create_index(cls, operations: Operations, index_name: Optional[str], table_name: str, columns: Sequence[Union[str, TextClause, Function[Any]]], *, schema: Optional[str] = ..., unique: bool = ..., if_not_exists: Optional[bool] = ..., **kw: Any) -> None:
         r"""Issue a "create index" instruction using the current
         migration context.
 
         e.g.::
 
             from alembic import op
 
@@ -497,28 +500,32 @@
          :func:`~sqlalchemy.sql.expression.text` constructs.
         :param schema: Optional schema name to operate within.  To control
          quoting of the schema outside of the default behavior, use
          the SQLAlchemy construct
          :class:`~sqlalchemy.sql.elements.quoted_name`.
         :param unique: If True, create a unique index.
 
-        :param quote:
-            Force quoting of this column's name on or off, corresponding
-            to ``True`` or ``False``. When left at its default
-            of ``None``, the column identifier will be quoted according to
-            whether the name is case sensitive (identifiers with at least one
-            upper case character are treated as case sensitive), or if it's a
-            reserved word. This flag is only needed to force quoting of a
-            reserved word which is not known by the SQLAlchemy dialect.
+        :param quote: Force quoting of this column's name on or off,
+         corresponding to ``True`` or ``False``. When left at its default
+         of ``None``, the column identifier will be quoted according to
+         whether the name is case sensitive (identifiers with at least one
+         upper case character are treated as case sensitive), or if it's a
+         reserved word. This flag is only needed to force quoting of a
+         reserved word which is not known by the SQLAlchemy dialect.
+
+        :param if_not_exists: If True, adds IF NOT EXISTS operator when
+         creating the new index.
+
+         .. versionadded:: 1.12.0
 
         :param \**kw: Additional keyword arguments not mentioned above are
-            dialect specific, and passed in the form
-            ``<dialectname>_<argname>``.
-            See the documentation regarding an individual dialect at
-            :ref:`dialect_toplevel` for detail on documented arguments.
+         dialect specific, and passed in the form
+         ``<dialectname>_<argname>``.
+         See the documentation regarding an individual dialect at
+         :ref:`dialect_toplevel` for detail on documented arguments.
 
         """
         ...
     
     @classmethod
     def batch_create_index(cls, operations: BatchOperations, index_name: str, columns: List[str], **kw: Any) -> None:
         """Issue a "create index" instruction using the
@@ -533,15 +540,15 @@
     
 
 
 @Operations.register_operation("drop_index")
 @BatchOperations.register_operation("drop_index", "batch_drop_index")
 class DropIndexOp(MigrateOperation):
     """Represent a drop index operation."""
-    def __init__(self, index_name: Union[quoted_name, str, conv], table_name: Optional[str] = ..., *, schema: Optional[str] = ..., _reverse: Optional[CreateIndexOp] = ..., **kw: Any) -> None:
+    def __init__(self, index_name: Union[quoted_name, str, conv], table_name: Optional[str] = ..., *, schema: Optional[str] = ..., if_exists: Optional[bool] = ..., _reverse: Optional[CreateIndexOp] = ..., **kw: Any) -> None:
         ...
     
     def to_diff_tuple(self) -> Tuple[str, Index]:
         ...
     
     def reverse(self) -> CreateIndexOp:
         ...
@@ -550,34 +557,40 @@
     def from_index(cls, index: Index) -> DropIndexOp:
         ...
     
     def to_index(self, migration_context: Optional[MigrationContext] = ...) -> Index:
         ...
     
     @classmethod
-    def drop_index(cls, operations: Operations, index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., **kw: Any) -> None:
+    def drop_index(cls, operations: Operations, index_name: str, table_name: Optional[str] = ..., *, schema: Optional[str] = ..., if_exists: Optional[bool] = ..., **kw: Any) -> None:
         r"""Issue a "drop index" instruction using the current
         migration context.
 
         e.g.::
 
             drop_index("accounts")
 
         :param index_name: name of the index.
         :param table_name: name of the owning table.  Some
          backends such as Microsoft SQL Server require this.
         :param schema: Optional schema name to operate within.  To control
          quoting of the schema outside of the default behavior, use
          the SQLAlchemy construct
          :class:`~sqlalchemy.sql.elements.quoted_name`.
+
+        :param if_exists: If True, adds IF EXISTS operator when
+         dropping the index.
+
+         .. versionadded:: 1.12.0
+
         :param \**kw: Additional keyword arguments not mentioned above are
-            dialect specific, and passed in the form
-            ``<dialectname>_<argname>``.
-            See the documentation regarding an individual dialect at
-            :ref:`dialect_toplevel` for detail on documented arguments.
+         dialect specific, and passed in the form
+         ``<dialectname>_<argname>``.
+         See the documentation regarding an individual dialect at
+         :ref:`dialect_toplevel` for detail on documented arguments.
 
         """
         ...
     
     @classmethod
     def batch_drop_index(cls, operations: BatchOperations, index_name: str, **kw: Any) -> None:
         """Issue a "drop index" instruction using the
@@ -772,16 +785,14 @@
     def __init__(self, table_name: str, comment: Optional[str], *, schema: Optional[str] = ..., existing_comment: Optional[str] = ...) -> None:
         ...
     
     @classmethod
     def create_table_comment(cls, operations: Operations, table_name: str, comment: Optional[str], *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
         """Emit a COMMENT ON operation to set the comment for a table.
 
-        .. versionadded:: 1.0.6
-
         :param table_name: string name of the target table.
         :param comment: string value of the comment being registered against
          the specified table.
         :param existing_comment: String value of a comment
          already registered on the specified table, used within autogenerate
          so that the operation is reversible, but not required for direct
          use.
@@ -796,34 +807,32 @@
         ...
     
     @classmethod
     def batch_create_table_comment(cls, operations: BatchOperations, comment: Optional[str], *, existing_comment: Optional[str] = ...) -> None:
         """Emit a COMMENT ON operation to set the comment for a table
         using the current batch migration context.
 
-        .. versionadded:: 1.6.0
-
         :param comment: string value of the comment being registered against
          the specified table.
         :param existing_comment: String value of a comment
          already registered on the specified table, used within autogenerate
          so that the operation is reversible, but not required for direct
          use.
 
         """
         ...
     
-    def reverse(self): # -> Any:
+    def reverse(self) -> Union[CreateTableCommentOp, DropTableCommentOp]:
         """Reverses the COMMENT ON operation against a table."""
         ...
     
-    def to_table(self, migration_context=...): # -> Table:
+    def to_table(self, migration_context: Optional[MigrationContext] = ...) -> Table:
         ...
     
-    def to_diff_tuple(self): # -> tuple[Literal['add_table_comment'], Table, str | None]:
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
         ...
     
 
 
 @Operations.register_operation("drop_table_comment")
 @BatchOperations.register_operation("drop_table_comment", "batch_drop_table_comment")
 class DropTableCommentOp(AlterTableOp):
@@ -832,16 +841,14 @@
         ...
     
     @classmethod
     def drop_table_comment(cls, operations: Operations, table_name: str, *, existing_comment: Optional[str] = ..., schema: Optional[str] = ...) -> None:
         """Issue a "drop table comment" operation to
         remove an existing comment set on a table.
 
-        .. versionadded:: 1.0.6
-
         :param table_name: string name of the target table.
         :param existing_comment: An optional string value of a comment already
          registered on the specified table.
 
         .. seealso::
 
             :meth:`.Operations.create_table_comment`
@@ -853,30 +860,28 @@
     
     @classmethod
     def batch_drop_table_comment(cls, operations: BatchOperations, *, existing_comment: Optional[str] = ...) -> None:
         """Issue a "drop table comment" operation to
         remove an existing comment set on a table using the current
         batch operations context.
 
-        .. versionadded:: 1.6.0
-
         :param existing_comment: An optional string value of a comment already
          registered on the specified table.
 
         """
         ...
     
-    def reverse(self): # -> Any:
+    def reverse(self) -> CreateTableCommentOp:
         """Reverses the COMMENT ON operation against a table."""
         ...
     
-    def to_table(self, migration_context=...): # -> Table:
+    def to_table(self, migration_context: Optional[MigrationContext] = ...) -> Table:
         ...
     
-    def to_diff_tuple(self): # -> tuple[Literal['remove_table_comment'], Table]:
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
         ...
     
 
 
 @Operations.register_operation("alter_column")
 @BatchOperations.register_operation("alter_column", "batch_alter_column")
 class AlterColumnOp(AlterTableOp):
@@ -890,15 +895,15 @@
     def has_changes(self) -> bool:
         ...
     
     def reverse(self) -> AlterColumnOp:
         ...
     
     @classmethod
-    def alter_column(cls, operations: Operations, table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Optional[Union[str, Literal[False]]] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Optional[Union[TypeEngine, Type[TypeEngine]]] = ..., existing_type: Optional[Union[TypeEngine, Type[TypeEngine]]] = ..., existing_server_default: Optional[Union[str, bool, Identity, Computed]] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
+    def alter_column(cls, operations: Operations, table_name: str, column_name: str, *, nullable: Optional[bool] = ..., comment: Optional[Union[str, Literal[False]]] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Optional[Union[TypeEngine[Any], Type[TypeEngine[Any]]]] = ..., existing_type: Optional[Union[TypeEngine[Any], Type[TypeEngine[Any]]]] = ..., existing_server_default: Optional[Union[str, bool, Identity, Computed]] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., schema: Optional[str] = ..., **kw: Any) -> None:
         r"""Issue an "alter column" instruction using the
         current migration context.
 
         Generally, only that aspect of the column which
         is being changed, i.e. name, type, nullability,
         default, needs to be specified.  Multiple changes
         can also be specified at once and the backend should
@@ -929,17 +934,14 @@
         :param server_default: Optional; specify a string
          SQL expression, :func:`~sqlalchemy.sql.expression.text`,
          or :class:`~sqlalchemy.schema.DefaultClause` to indicate
          an alteration to the column's default value.
          Set to ``None`` to have the default removed.
         :param comment: optional string text of a new comment to add to the
          column.
-
-         .. versionadded:: 1.0.6
-
         :param new_column_name: Optional; specify a string name here to
          indicate the new name within a column rename operation.
         :param type\_: Optional; a :class:`~sqlalchemy.types.TypeEngine`
          type object to specify a change to the column's type.
          For SQLAlchemy types that also indicate a constraint (i.e.
          :class:`~sqlalchemy.types.Boolean`, :class:`~sqlalchemy.types.Enum`),
          the constraint is also generated.
@@ -948,15 +950,15 @@
         :param existing_type: Optional; a
          :class:`~sqlalchemy.types.TypeEngine`
          type object to specify the previous type.   This
          is required for all MySQL column alter operations that
          don't otherwise specify a new type, as well as for
          when nullability is being changed on a SQL Server
          column.  It is also used if the type is a so-called
-         SQLlchemy "schema" type which may define a constraint (i.e.
+         SQLAlchemy "schema" type which may define a constraint (i.e.
          :class:`~sqlalchemy.types.Boolean`,
          :class:`~sqlalchemy.types.Enum`),
          so that the constraint can be dropped.
         :param existing_server_default: Optional; The existing
          default value of the column.   Required on MySQL if
          an existing default is not being changed; else MySQL
          removes the default.
@@ -965,52 +967,45 @@
          is not being changed; else MySQL sets this to NULL.
         :param existing_autoincrement: Optional; the existing autoincrement
          of the column.  Used for MySQL's system of altering a column
          that specifies ``AUTO_INCREMENT``.
         :param existing_comment: string text of the existing comment on the
          column to be maintained.  Required on MySQL if the existing comment
          on the column is not being changed.
-
-         .. versionadded:: 1.0.6
-
         :param schema: Optional schema name to operate within.  To control
          quoting of the schema outside of the default behavior, use
          the SQLAlchemy construct
          :class:`~sqlalchemy.sql.elements.quoted_name`.
         :param postgresql_using: String argument which will indicate a
          SQL expression to render within the Postgresql-specific USING clause
          within ALTER COLUMN.    This string is taken directly as raw SQL which
          must explicitly include any necessary quoting or escaping of tokens
          within the expression.
 
         """
         ...
     
     @classmethod
-    def batch_alter_column(cls, operations: BatchOperations, column_name: str, *, nullable: Optional[bool] = ..., comment: Optional[Union[str, Literal[False]]] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Optional[Union[TypeEngine, Type[TypeEngine]]] = ..., existing_type: Optional[Union[TypeEngine, Type[TypeEngine]]] = ..., existing_server_default: Optional[Union[str, bool, Identity, Computed]] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., insert_before: Optional[str] = ..., insert_after: Optional[str] = ..., **kw: Any) -> None:
+    def batch_alter_column(cls, operations: BatchOperations, column_name: str, *, nullable: Optional[bool] = ..., comment: Optional[Union[str, Literal[False]]] = ..., server_default: Any = ..., new_column_name: Optional[str] = ..., type_: Optional[Union[TypeEngine[Any], Type[TypeEngine[Any]]]] = ..., existing_type: Optional[Union[TypeEngine[Any], Type[TypeEngine[Any]]]] = ..., existing_server_default: Optional[Union[str, bool, Identity, Computed]] = ..., existing_nullable: Optional[bool] = ..., existing_comment: Optional[str] = ..., insert_before: Optional[str] = ..., insert_after: Optional[str] = ..., **kw: Any) -> None:
         """Issue an "alter column" instruction using the current
         batch migration context.
 
         Parameters are the same as that of :meth:`.Operations.alter_column`,
         as well as the following option(s):
 
         :param insert_before: String name of an existing column which this
          column should be placed before, when creating the new table.
 
-         .. versionadded:: 1.4.0
-
         :param insert_after: String name of an existing column which this
          column should be placed after, when creating the new table.  If
          both :paramref:`.BatchOperations.alter_column.insert_before`
          and :paramref:`.BatchOperations.alter_column.insert_after` are
          omitted, the column is inserted after the last existing column
          in the table.
 
-         .. versionadded:: 1.4.0
-
         .. seealso::
 
             :meth:`.Operations.alter_column`
 
 
         """
         ...
@@ -1026,19 +1021,19 @@
     
     def reverse(self) -> DropColumnOp:
         ...
     
     def to_diff_tuple(self) -> Tuple[str, Optional[str], str, Column[Any]]:
         ...
     
-    def to_column(self) -> Column:
+    def to_column(self) -> Column[Any]:
         ...
     
     @classmethod
-    def from_column(cls, col: Column) -> AddColumnOp:
+    def from_column(cls, col: Column[Any]) -> AddColumnOp:
         ...
     
     @classmethod
     def from_column_and_tablename(cls, schema: Optional[str], tname: str, col: Column[Any]) -> AddColumnOp:
         ...
     
     @classmethod
@@ -1149,15 +1144,15 @@
     def reverse(self) -> AddColumnOp:
         ...
     
     @classmethod
     def from_column_and_tablename(cls, schema: Optional[str], tname: str, col: Column[Any]) -> DropColumnOp:
         ...
     
-    def to_column(self, migration_context: Optional[MigrationContext] = ...) -> Column:
+    def to_column(self, migration_context: Optional[MigrationContext] = ...) -> Column[Any]:
         ...
     
     @classmethod
     def drop_column(cls, operations: Operations, table_name: str, column_name: str, *, schema: Optional[str] = ..., **kw: Any) -> None:
         """Issue a "drop column" instruction using the current
         migration context.
 
@@ -1209,19 +1204,19 @@
         ...
     
 
 
 @Operations.register_operation("bulk_insert")
 class BulkInsertOp(MigrateOperation):
     """Represent a bulk insert operation."""
-    def __init__(self, table: Union[Table, TableClause], rows: List[dict], *, multiinsert: bool = ...) -> None:
+    def __init__(self, table: Union[Table, TableClause], rows: List[Dict[str, Any]], *, multiinsert: bool = ...) -> None:
         ...
     
     @classmethod
-    def bulk_insert(cls, operations: Operations, table: Union[Table, TableClause], rows: List[dict], *, multiinsert: bool = ...) -> None:
+    def bulk_insert(cls, operations: Operations, table: Union[Table, TableClause], rows: List[Dict[str, Any]], *, multiinsert: bool = ...) -> None:
         """Issue a "bulk insert" operation using the current
         migration context.
 
         This provides a means of representing an INSERT of multiple rows
         which works equally well in the context of executing on a live
         connection as well as that of generating a SQL script.   In the
         case of a SQL script, the values are rendered inline into the
@@ -1317,19 +1312,19 @@
     
 
 
 @Operations.register_operation("execute")
 @BatchOperations.register_operation("execute", "batch_execute")
 class ExecuteSQLOp(MigrateOperation):
     """Represent an execute SQL operation."""
-    def __init__(self, sqltext: Union[Update, str, Insert, TextClause], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+    def __init__(self, sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
         ...
     
     @classmethod
-    def execute(cls, operations: Operations, sqltext: Union[str, TextClause, Update], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+    def execute(cls, operations: Operations, sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
         r"""Execute the given SQL using the current migration context.
 
         The given SQL can be a plain string, e.g.::
 
             op.execute("INSERT INTO table (foo) VALUES ('some value')")
 
         Or it can be any kind of Core SQL Expression construct, such as
@@ -1374,30 +1369,29 @@
             connection.execute(
                 account.update()
                 .where(account.c.name == "account 1")
                 .values({"name": "account 2"})
             )
 
         Additionally, when passing the statement as a plain string, it is first
-        coerceed into a :func:`sqlalchemy.sql.expression.text` construct
+        coerced into a :func:`sqlalchemy.sql.expression.text` construct
         before being passed along.  In the less likely case that the
         literal SQL string contains a colon, it must be escaped with a
         backslash, as::
 
            op.execute(r"INSERT INTO table (foo) VALUES ('\:colon_value')")
 
 
         :param sqltext: Any legal SQLAlchemy expression, including:
 
         * a string
         * a :func:`sqlalchemy.sql.expression.text` construct.
         * a :func:`sqlalchemy.sql.expression.insert` construct.
-        * a :func:`sqlalchemy.sql.expression.update`,
-          :func:`sqlalchemy.sql.expression.insert`,
-          or :func:`sqlalchemy.sql.expression.delete`  construct.
+        * a :func:`sqlalchemy.sql.expression.update` construct.
+        * a :func:`sqlalchemy.sql.expression.delete` construct.
         * Any "executable" described in SQLAlchemy Core documentation,
           noting that no result set is returned.
 
         .. note::  when passing a plain string, the statement is coerced into
            a :func:`sqlalchemy.sql.expression.text` construct. This construct
            considers symbols with colons, e.g. ``:foo`` to be bound parameters.
            To avoid this, ensure that colon symbols are escaped, e.g.
@@ -1406,24 +1400,27 @@
         :param execution_options: Optional dictionary of
          execution options, will be passed to
          :meth:`sqlalchemy.engine.Connection.execution_options`.
         """
         ...
     
     @classmethod
-    def batch_execute(cls, operations: Operations, sqltext: Union[str, TextClause, Update], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
+    def batch_execute(cls, operations: Operations, sqltext: Union[Executable, str], *, execution_options: Optional[dict[str, Any]] = ...) -> None:
         """Execute the given SQL using the current migration context.
 
         .. seealso::
 
             :meth:`.Operations.execute`
 
         """
         ...
     
+    def to_diff_tuple(self) -> Tuple[str, Union[Executable, str]]:
+        ...
+    
 
 
 class OpContainer(MigrateOperation):
     """Represent a sequence of operations operation."""
     def __init__(self, ops: Sequence[MigrateOperation] = ...) -> None:
         ...
     
@@ -1473,15 +1470,15 @@
 
         :ref:`customizing_revision`
 
     """
     def __init__(self, ops: Sequence[MigrateOperation] = ..., downgrade_token: str = ...) -> None:
         ...
     
-    def reverse(self): # -> UpgradeOps:
+    def reverse(self) -> UpgradeOps:
         ...
     
 
 
 class MigrationScript(MigrateOperation):
     """represents a migration script.
 
@@ -1502,43 +1499,45 @@
 
     .. seealso::
 
         :ref:`customizing_revision`
 
     """
     _needs_render: Optional[bool]
-    def __init__(self, rev_id: Optional[str], upgrade_ops: UpgradeOps, downgrade_ops: DowngradeOps, *, message: Optional[str] = ..., imports: Set[str] = ..., head: Optional[str] = ..., splice: Optional[bool] = ..., branch_label: Optional[str] = ..., version_path: Optional[str] = ..., depends_on: Optional[Union[str, Sequence[str]]] = ...) -> None:
+    _upgrade_ops: List[UpgradeOps]
+    _downgrade_ops: List[DowngradeOps]
+    def __init__(self, rev_id: Optional[str], upgrade_ops: UpgradeOps, downgrade_ops: DowngradeOps, *, message: Optional[str] = ..., imports: Set[str] = ..., head: Optional[str] = ..., splice: Optional[bool] = ..., branch_label: Optional[_RevIdType] = ..., version_path: Optional[str] = ..., depends_on: Optional[_RevIdType] = ...) -> None:
         ...
     
     @property
-    def upgrade_ops(self): # -> Any | None:
+    def upgrade_ops(self) -> Optional[UpgradeOps]:
         """An instance of :class:`.UpgradeOps`.
 
         .. seealso::
 
             :attr:`.MigrationScript.upgrade_ops_list`
         """
         ...
     
     @upgrade_ops.setter
-    def upgrade_ops(self, upgrade_ops): # -> None:
+    def upgrade_ops(self, upgrade_ops: Union[UpgradeOps, List[UpgradeOps]]) -> None:
         ...
     
     @property
-    def downgrade_ops(self): # -> Any | None:
+    def downgrade_ops(self) -> Optional[DowngradeOps]:
         """An instance of :class:`.DowngradeOps`.
 
         .. seealso::
 
             :attr:`.MigrationScript.downgrade_ops_list`
         """
         ...
     
     @downgrade_ops.setter
-    def downgrade_ops(self, downgrade_ops): # -> None:
+    def downgrade_ops(self, downgrade_ops: Union[DowngradeOps, List[DowngradeOps]]) -> None:
         ...
     
     @property
     def upgrade_ops_list(self) -> List[UpgradeOps]:
         """A list of :class:`.UpgradeOps` instances.
 
         This is used in place of the :attr:`.MigrationScript.upgrade_ops`
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/operations/schemaobj.pyi` & `bl_python_all-0.2.0/typings/alembic/operations/schemaobj.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/operations/toimpl.pyi` & `bl_python_all-0.2.0/typings/alembic/operations/toimpl.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/runtime/environment.pyi` & `bl_python_all-0.2.0/typings/alembic/runtime/environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,36 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Collection,
-    ContextManager,
-    Dict,
-    List,
-    Mapping,
-    MutableMapping,
-    Optional,
-    TextIO,
-    Tuple,
-    Union,
-    overload,
-)
-
-from sqlalchemy.engine import URL
-from sqlalchemy.engine.base import Connection
-from sqlalchemy.sql.elements import ClauseElement
+from typing import Any, Callable, Collection, ContextManager, Dict, List, Mapping, MutableMapping, Optional, Sequence, TYPE_CHECKING, TextIO, Tuple, Union, overload
 from sqlalchemy.sql.schema import FetchedValue, MetaData
 from typing_extensions import Literal
-
+from .migration import MigrationContext, _ProxyTransaction
 from .. import util
+from ..script.revision import _GetRevArg
+from sqlalchemy.engine import URL
+from sqlalchemy.engine.base import Connection
+from sqlalchemy.sql import Executable
 from ..config import Config
 from ..ddl import DefaultImpl
 from ..script.base import ScriptDirectory
-from .migration import MigrationContext, _ProxyTransaction
 
-if TYPE_CHECKING: ...
+if TYPE_CHECKING:
+    ...
 _RevNumber = Optional[Union[str, Tuple[str, ...]]]
-ProcessRevisionDirectiveFn = Callable[
-    [MigrationContext, Tuple[str, str], List["MigrateOperation"]], None
-]
+ProcessRevisionDirectiveFn = Callable[[MigrationContext, _GetRevArg, List["MigrationScript"]], None]
 RenderItemFn = Callable[[str, Any, "AutogenContext"], Union[str, Literal[False]]]
-NameFilterType = Literal[
-    "schema",
-    "table",
-    "column",
-    "index",
-    "unique_constraint",
-    "foreign_key_constraint",
-]
-NameFilterParentNames = MutableMapping[
-    Literal["schema_name", "table_name", "schema_qualified_table_name"],
-    Optional[str],
-]
+NameFilterType = Literal["schema", "table", "column", "index", "unique_constraint", "foreign_key_constraint",]
+NameFilterParentNames = MutableMapping[Literal["schema_name", "table_name", "schema_qualified_table_name"], Optional[str],]
 IncludeNameFn = Callable[[Optional[str], NameFilterType, NameFilterParentNames], bool]
-IncludeObjectFn = Callable[
-    ["SchemaItem", Optional[str], NameFilterType, bool, Optional["SchemaItem"]],
-    bool,
-]
-OnVersionApplyFn = Callable[
-    [MigrationContext, "MigrationInfo", Collection[Any], Mapping[str, Any]],
-    None,
-]
-CompareServerDefault = Callable[
-    [
-        MigrationContext,
-        "Column[Any]",
-        "Column[Any]",
-        Optional[str],
-        Optional[FetchedValue],
-        Optional[str],
-    ],
-    Optional[bool],
-]
-
+IncludeObjectFn = Callable[["SchemaItem", Optional[str], NameFilterType, bool, Optional["SchemaItem"]], bool,]
+OnVersionApplyFn = Callable[[MigrationContext, "MigrationInfo", Collection[Any], Mapping[str, Any]], None,]
+CompareServerDefault = Callable[[MigrationContext, "Column[Any]", "Column[Any]", Optional[str], Optional[FetchedValue], Optional[str]], Optional[bool],]
+CompareType = Callable[[MigrationContext, "Column[Any]", "Column[Any]", "TypeEngine[Any]", "TypeEngine[Any]"], Optional[bool],]
 class EnvironmentContext(util.ModuleClsProxy):
     """A configurational facade made available in an ``env.py`` script.
 
     The :class:`.EnvironmentContext` acts as a *facade* to the more
     nuts-and-bolts objects of :class:`.MigrationContext` as well as certain
     aspects of :class:`.Config`,
     within the context of the ``env.py`` script that is invoked by
@@ -129,104 +86,114 @@
         invocation of migration scripts, the :class:`.MigrationContext`
         and :class:`.ScriptDirectory` objects can be created and
         used directly.  The :class:`.EnvironmentContext` object
         is *only* needed when you need to actually invoke the
         ``env.py`` module present in the migration environment.
 
     """
-
     _migration_context: Optional[MigrationContext] = ...
     config: Config = ...
     script: ScriptDirectory = ...
     def __init__(self, config: Config, script: ScriptDirectory, **kw: Any) -> None:
         r"""Construct a new :class:`.EnvironmentContext`.
 
         :param config: a :class:`.Config` instance.
         :param script: a :class:`.ScriptDirectory` instance.
         :param \**kw: keyword options that will be ultimately
          passed along to the :class:`.MigrationContext` when
          :meth:`.EnvironmentContext.configure` is called.
 
         """
         ...
+    
     def __enter__(self) -> EnvironmentContext:
         """Establish a context which provides a
         :class:`.EnvironmentContext` object to
         env.py scripts.
 
         The :class:`.EnvironmentContext` will
         be made available as ``from alembic import context``.
 
         """
         ...
-    def __exit__(self, *arg: Any, **kw: Any) -> None: ...
+    
+    def __exit__(self, *arg: Any, **kw: Any) -> None:
+        ...
+    
     def is_offline_mode(self) -> bool:
         """Return True if the current migrations environment
         is running in "offline mode".
 
         This is ``True`` or ``False`` depending
         on the ``--sql`` flag passed.
 
         This function does not require that the :class:`.MigrationContext`
         has been configured.
 
         """
         ...
-    def is_transactional_ddl(self):  # -> bool:
+    
+    def is_transactional_ddl(self) -> bool:
         """Return True if the context is configured to expect a
         transactional DDL capable backend.
 
         This defaults to the type of database in use, and
         can be overridden by the ``transactional_ddl`` argument
         to :meth:`.configure`
 
         This function requires that a :class:`.MigrationContext`
         has first been made available via :meth:`.configure`.
 
         """
         ...
-    def requires_connection(self) -> bool: ...
+    
+    def requires_connection(self) -> bool:
+        ...
+    
     def get_head_revision(self) -> _RevNumber:
         """Return the hex identifier of the 'head' script revision.
 
         If the script directory has multiple heads, this
         method raises a :class:`.CommandError`;
         :meth:`.EnvironmentContext.get_head_revisions` should be preferred.
 
         This function does not require that the :class:`.MigrationContext`
         has been configured.
 
         .. seealso:: :meth:`.EnvironmentContext.get_head_revisions`
 
         """
         ...
+    
     def get_head_revisions(self) -> _RevNumber:
         """Return the hex identifier of the 'heads' script revision(s).
 
         This returns a tuple containing the version number of all
         heads in the script directory.
 
         This function does not require that the :class:`.MigrationContext`
         has been configured.
 
         """
         ...
+    
     def get_starting_revision_argument(self) -> _RevNumber:
         """Return the 'starting revision' argument,
         if the revision was passed using ``start:end``.
 
         This is only meaningful in "offline" mode.
         Returns ``None`` if no value is available
         or was configured.
 
         This function does not require that the :class:`.MigrationContext`
         has been configured.
 
         """
         ...
+    
     def get_revision_argument(self) -> _RevNumber:
         """Get the 'destination' revision argument.
 
         This is typically the argument passed to the
         ``upgrade`` or ``downgrade`` command.
 
         If it was specified as ``head``, the actual
@@ -234,14 +201,15 @@
         as ``base``, ``None`` is returned.
 
         This function does not require that the :class:`.MigrationContext`
         has been configured.
 
         """
         ...
+    
     def get_tag_argument(self) -> Optional[str]:
         """Return the value passed for the ``--tag`` argument, if any.
 
         The ``--tag`` argument is not used directly by Alembic,
         but is available for custom ``env.py`` configurations that
         wish to use it; particularly for offline generation scripts
         that wish to generate tagged filenames.
@@ -253,35 +221,42 @@
 
             :meth:`.EnvironmentContext.get_x_argument` - a newer and more
             open ended system of extending ``env.py`` scripts via the command
             line.
 
         """
         ...
+    
     @overload
-    def get_x_argument(self, as_dictionary: Literal[False]) -> List[str]: ...
+    def get_x_argument(self, as_dictionary: Literal[False]) -> List[str]:
+        ...
+    
     @overload
-    def get_x_argument(self, as_dictionary: Literal[True]) -> Dict[str, str]: ...
+    def get_x_argument(self, as_dictionary: Literal[True]) -> Dict[str, str]:
+        ...
+    
     @overload
-    def get_x_argument(
-        self, as_dictionary: bool = ...
-    ) -> Union[List[str], Dict[str, str]]: ...
-    def get_x_argument(
-        self, as_dictionary: bool = ...
-    ) -> Union[List[str], Dict[str, str]]:
+    def get_x_argument(self, as_dictionary: bool = ...) -> Union[List[str], Dict[str, str]]:
+        ...
+    
+    def get_x_argument(self, as_dictionary: bool = ...) -> Union[List[str], Dict[str, str]]:
         """Return the value(s) passed for the ``-x`` argument, if any.
 
         The ``-x`` argument is an open ended flag that allows any user-defined
         value or values to be passed on the command line, then available
         here for consumption by a custom ``env.py`` script.
 
         The return value is a list, returned directly from the ``argparse``
         structure.  If ``as_dictionary=True`` is passed, the ``x`` arguments
         are parsed using ``key=value`` format into a dictionary that is
-        then returned.
+        then returned. If there is no ``=`` in the argument, value is an empty
+        string.
+
+        .. versionchanged:: 1.13.1 Support ``as_dictionary=True`` when
+           arguments are passed without the ``=`` symbol.
 
         For example, to support passing a database URL on the command line,
         the standard ``env.py`` script can be modified like this::
 
             cmd_line_url = context.get_x_argument(
                 as_dictionary=True).get('dbname')
             if cmd_line_url:
@@ -303,47 +278,16 @@
 
             :meth:`.EnvironmentContext.get_tag_argument`
 
             :attr:`.Config.cmd_opts`
 
         """
         ...
-    def configure(
-        self,
-        connection: Optional[Connection] = ...,
-        url: Optional[Union[str, URL]] = ...,
-        dialect_name: Optional[str] = ...,
-        dialect_opts: Optional[Dict[str, Any]] = ...,
-        transactional_ddl: Optional[bool] = ...,
-        transaction_per_migration: bool = ...,
-        output_buffer: Optional[TextIO] = ...,
-        starting_rev: Optional[str] = ...,
-        tag: Optional[str] = ...,
-        template_args: Optional[Dict[str, Any]] = ...,
-        render_as_batch: bool = ...,
-        # Alembic documents and supports list[MetaData]
-        # despite the typehint not including it in the
-        # library
-        target_metadata: Optional[MetaData | list[MetaData]] = ...,
-        include_name: Optional[IncludeNameFn] = ...,
-        include_object: Optional[IncludeObjectFn] = ...,
-        include_schemas: bool = ...,
-        process_revision_directives: Optional[ProcessRevisionDirectiveFn] = ...,
-        compare_type: bool = ...,
-        compare_server_default: Union[bool, CompareServerDefault] = ...,
-        render_item: Optional[RenderItemFn] = ...,
-        literal_binds: bool = ...,
-        upgrade_token: str = ...,
-        downgrade_token: str = ...,
-        alembic_module_prefix: str = ...,
-        sqlalchemy_module_prefix: str = ...,
-        user_module_prefix: Optional[str] = ...,
-        on_version_apply: Optional[OnVersionApplyFn] = ...,
-        **kw: Any
-    ) -> None:
+    
+    def configure(self, connection: Optional[Connection] = ..., url: Optional[Union[str, URL]] = ..., dialect_name: Optional[str] = ..., dialect_opts: Optional[Dict[str, Any]] = ..., transactional_ddl: Optional[bool] = ..., transaction_per_migration: bool = ..., output_buffer: Optional[TextIO] = ..., starting_rev: Optional[str] = ..., tag: Optional[str] = ..., template_args: Optional[Dict[str, Any]] = ..., render_as_batch: bool = ..., target_metadata: Union[MetaData, Sequence[MetaData], None] = ..., include_name: Optional[IncludeNameFn] = ..., include_object: Optional[IncludeObjectFn] = ..., include_schemas: bool = ..., process_revision_directives: Optional[ProcessRevisionDirectiveFn] = ..., compare_type: Union[bool, CompareType] = ..., compare_server_default: Union[bool, CompareServerDefault] = ..., render_item: Optional[RenderItemFn] = ..., literal_binds: bool = ..., upgrade_token: str = ..., downgrade_token: str = ..., alembic_module_prefix: str = ..., sqlalchemy_module_prefix: str = ..., user_module_prefix: Optional[str] = ..., on_version_apply: Optional[OnVersionApplyFn] = ..., **kw: Any) -> None:
         """Configure a :class:`.MigrationContext` within this
         :class:`.EnvironmentContext` which will provide database
         connectivity and other configuration to a series of
         migration scripts.
 
         Many methods on :class:`.EnvironmentContext` require that
         this method has been called in order to function, as they
@@ -380,17 +324,14 @@
          ``connection`` is not passed.
         :param dialect_name: string name of a dialect, such as
          "postgresql", "mssql", etc.
          The type of dialect to be used will be derived from this if
          ``connection`` and ``url`` are not passed.
         :param dialect_opts: dictionary of options to be passed to dialect
          constructor.
-
-         .. versionadded:: 1.0.12
-
         :param transactional_ddl: Force the usage of "transactional"
          DDL on or off;
          this otherwise defaults to whether or not the dialect in
          use supports it.
         :param transaction_per_migration: if True, nest each migration script
          in a transaction rather than the full series of migrations to
          run.
@@ -465,20 +406,24 @@
          The tables present in each :class:`~sqlalchemy.schema.MetaData`
          will be compared against
          what is locally available on the target
          :class:`~sqlalchemy.engine.Connection`
          to produce candidate upgrade/downgrade operations.
         :param compare_type: Indicates type comparison behavior during
          an autogenerate
-         operation.  Defaults to ``False`` which disables type
-         comparison.  Set to
-         ``True`` to turn on default type comparison, which has varied
-         accuracy depending on backend.   See :ref:`compare_types`
+         operation.  Defaults to ``True`` turning on type comparison, which
+         has good accuracy on most backends.   See :ref:`compare_types`
          for an example as well as information on other type
-         comparison options.
+         comparison options. Set to ``False`` which disables type
+         comparison. A callable can also be passed to provide custom type
+         comparison, see :ref:`compare_types` for additional details.
+
+         .. versionchanged:: 1.12.0 The default value of
+            :paramref:`.EnvironmentContext.configure.compare_type` has been
+            changed to ``True``.
 
          .. seealso::
 
             :ref:`compare_types`
 
             :paramref:`.EnvironmentContext.configure.compare_server_default`
 
@@ -554,16 +499,14 @@
 
             context.configure(
                 # ...
                 include_schemas = True,
                 include_name = include_name
             )
 
-         .. versionadded:: 1.5
-
          .. seealso::
 
             :ref:`autogenerate_include_hooks`
 
             :paramref:`.EnvironmentContext.configure.include_object`
 
             :paramref:`.EnvironmentContext.configure.include_schemas`
@@ -770,14 +713,15 @@
         :param oracle_batch_separator: The "batch separator" which will
          be placed between each statement when generating offline
          Oracle migrations.  Defaults to ``/``.  Oracle doesn't add a
          semicolon between statements like most other backends.
 
         """
         ...
+    
     def run_migrations(self, **kw: Any) -> None:
         """Run migrations as determined by the current command line
         configuration
         as well as versioning information present (or not) in the current
         database connection (if one is present).
 
         The function accepts optional ``**kw`` arguments.   If these are
@@ -791,39 +735,40 @@
         to the migration functions.
 
         This function requires that a :class:`.MigrationContext` has
         first been made available via :meth:`.configure`.
 
         """
         ...
-    def execute(
-        self, sql: Union[ClauseElement, str], execution_options: Optional[dict] = ...
-    ) -> None:
+    
+    def execute(self, sql: Union[Executable, str], execution_options: Optional[Dict[str, Any]] = ...) -> None:
         """Execute the given SQL using the current change context.
 
         The behavior of :meth:`.execute` is the same
         as that of :meth:`.Operations.execute`.  Please see that
         function's documentation for full detail including
         caveats and limitations.
 
         This function requires that a :class:`.MigrationContext` has
         first been made available via :meth:`.configure`.
 
         """
         ...
+    
     def static_output(self, text: str) -> None:
         """Emit text directly to the "offline" SQL stream.
 
         Typically this is for emitting comments that
         start with --.  The statement is not treated
         as a SQL execution, no ; or batch separator
         is added, etc.
 
         """
         ...
+    
     def begin_transaction(self) -> Union[_ProxyTransaction, ContextManager[None]]:
         """Return a context manager that will
         enclose an operation within a "transaction",
         as defined by the environment's offline
         and transactional DDL settings.
 
         e.g.::
@@ -860,28 +805,35 @@
         has more specific transactional needs can of course
         manipulate the :class:`~sqlalchemy.engine.Connection`
         directly to produce transactional state in "online"
         mode.
 
         """
         ...
+    
     def get_context(self) -> MigrationContext:
         """Return the current :class:`.MigrationContext` object.
 
         If :meth:`.EnvironmentContext.configure` has not been
         called yet, raises an exception.
 
         """
         ...
+    
     def get_bind(self) -> Connection:
         """Return the current 'bind'.
 
         In "online" mode, this is the
         :class:`sqlalchemy.engine.Connection` currently being used
         to emit SQL to the database.
 
         This function requires that a :class:`.MigrationContext`
         has first been made available via :meth:`.configure`.
 
         """
         ...
-    def get_impl(self) -> DefaultImpl: ...
+    
+    def get_impl(self) -> DefaultImpl:
+        ...
+    
+
+
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/runtime/migration.pyi` & `bl_python_all-0.2.0/typings/alembic/runtime/migration.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This type stub file was generated by pyright.
 """
 
 from contextlib import contextmanager
 from typing import Any, Collection, ContextManager, Dict, Iterator, List, Optional, Set, TYPE_CHECKING, Tuple, Union
 from sqlalchemy.engine import Dialect, URL
 from sqlalchemy.engine.base import Connection
-from sqlalchemy.sql.elements import ClauseElement
+from sqlalchemy.sql import Executable
 from .environment import EnvironmentContext
 from ..config import Config
 from ..script.base import Script, ScriptDirectory
 from ..script.revision import Revision, RevisionMap, _RevisionOrBase
 
 if TYPE_CHECKING:
     ...
@@ -147,16 +147,14 @@
             It is recommended that when an application includes migrations with
             "autocommit" blocks, that
             :paramref:`.EnvironmentContext.transaction_per_migration` be used
             so that the calling environment is tuned to expect short per-file
             migrations whether or not one of them has an autocommit block.
 
 
-        .. versionadded:: 1.2.0
-
         """
         ...
     
     def begin_transaction(self, _per_migration: bool = ...) -> Union[_ProxyTransaction, ContextManager[None]]:
         """Begin a logical transaction for migration operations.
 
         This method is used within an ``env.py`` script to demarcate where
@@ -267,15 +265,15 @@
         :param \**kw: keyword arguments here will be passed to each
          migration callable, that is the ``upgrade()`` or ``downgrade()``
          method within revision scripts.
 
         """
         ...
     
-    def execute(self, sql: Union[ClauseElement, str], execution_options: Optional[dict] = ...) -> None:
+    def execute(self, sql: Union[Executable, str], execution_options: Optional[Dict[str, Any]] = ...) -> None:
         """Execute a SQL construct or string statement.
 
         The underlying execution mechanics are used, that is
         if this is "offline mode" the SQL is written to the
         output buffer, otherwise the SQL is emitted on
         the current SQLAlchemy connection.
 
@@ -392,14 +390,19 @@
 
 
 class MigrationStep:
     from_revisions_no_deps: Tuple[str, ...]
     to_revisions_no_deps: Tuple[str, ...]
     is_upgrade: bool
     migration_fn: Any
+    if TYPE_CHECKING:
+        @property
+        def doc(self) -> Optional[str]:
+            ...
+        
     @property
     def name(self) -> str:
         ...
     
     @classmethod
     def upgrade_from_script(cls, revision_map: RevisionMap, script: Script) -> RevisionStep:
         ...
@@ -428,15 +431,15 @@
     def __repr__(self): # -> str:
         ...
     
     def __eq__(self, other: object) -> bool:
         ...
     
     @property
-    def doc(self) -> str:
+    def doc(self) -> Optional[str]:
         ...
     
     @property
     def from_revisions(self) -> Tuple[str, ...]:
         ...
     
     @property
@@ -458,15 +461,15 @@
 
         """
         ...
     
     def merge_branch_idents(self, heads: Set[str]) -> Tuple[List[str], str, str]:
         ...
     
-    def unmerge_branch_idents(self, heads: Collection[str]) -> Tuple[str, str, Tuple[str, ...]]:
+    def unmerge_branch_idents(self, heads: Set[str]) -> Tuple[str, str, Tuple[str, ...]]:
         ...
     
     def should_create_branch(self, heads: Set[str]) -> bool:
         ...
     
     def should_merge_branches(self, heads: Set[str]) -> bool:
         ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/script/base.pyi` & `bl_python_all-0.2.0/typings/alembic/script/base.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 This type stub file was generated by pyright.
 """
 
 from types import ModuleType
-from typing import Any, Iterator, List, Mapping, Optional, Sequence, Set, TYPE_CHECKING, Tuple, Union
+from typing import Any, Iterator, List, Mapping, Optional, Set, TYPE_CHECKING, Tuple, Union
 from . import revision
+from ..util import compat
+from .revision import Revision, _GetRevArg, _RevIdType
 from ..config import Config, MessagingOptions
-from ..script.revision import Revision
 
 if TYPE_CHECKING:
     ...
-_RevIdType = Union[str, Sequence[str]]
+if compat.py39:
+    ...
+else:
+    ...
 _sourceless_rev_file = ...
 _only_source_rev_file = ...
 _legacy_rev = ...
-_mod_def_re = ...
 _slug_re = ...
 _default_file_template = ...
 _split_on_space_comma = ...
 _split_on_space_comma_colon = ...
 class ScriptDirectory:
     """Provides operations upon an Alembic script directory.
 
@@ -65,25 +68,25 @@
         :param head: the head revision; defaults to "heads" to indicate
          all head revisions.  May also be "head" to indicate a single
          head revision.
 
         """
         ...
     
-    def get_revisions(self, id_: _RevIdType) -> Tuple[Optional[Script], ...]:
+    def get_revisions(self, id_: _GetRevArg) -> Tuple[Script, ...]:
         """Return the :class:`.Script` instance with the given rev identifier,
         symbolic name, or sequence of identifiers.
 
         """
         ...
     
-    def get_all_current(self, id_: Tuple[str, ...]) -> Set[Optional[Script]]:
+    def get_all_current(self, id_: Tuple[str, ...]) -> Set[Script]:
         ...
     
-    def get_revision(self, id_: str) -> Optional[Script]:
+    def get_revision(self, id_: str) -> Script:
         """Return the :class:`.Script` instance with the given rev id.
 
         .. seealso::
 
             :meth:`.ScriptDirectory.get_revisions`
 
         """
@@ -172,18 +175,18 @@
         by the command functions in :mod:`alembic.command`.
 
 
         """
         ...
     
     @property
-    def env_py_location(self): # -> str:
+    def env_py_location(self) -> str:
         ...
     
-    def generate_revision(self, revid: str, message: Optional[str], head: Optional[str] = ..., refresh: bool = ..., splice: Optional[bool] = ..., branch_labels: Optional[str] = ..., version_path: Optional[str] = ..., depends_on: Optional[_RevIdType] = ..., **kw: Any) -> Optional[Script]:
+    def generate_revision(self, revid: str, message: Optional[str], head: Optional[_RevIdType] = ..., splice: Optional[bool] = ..., branch_labels: Optional[_RevIdType] = ..., version_path: Optional[str] = ..., depends_on: Optional[_RevIdType] = ..., **kw: Any) -> Optional[Script]:
         """Generate a new revision file.
 
         This runs the ``script.py.mako`` template, given
         template arguments, and creates a new file.
 
         :param revid: String revision id.  Typically this
          comes from ``alembic.util.rev_id()``.
@@ -191,15 +194,14 @@
          by the -m argument to the ``revision`` command.
         :param head: the head revision to generate against.  Defaults
          to the current "head" if no branches are present, else raises
          an exception.
         :param splice: if True, allow the "head" version to not be an
          actual head; otherwise, the selected head must be a head
          (e.g. endpoint) revision.
-        :param refresh: deprecated.
 
         """
         ...
     
 
 
 class Script(revision.Revision):
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/script/revision.pyi` & `bl_python_all-0.2.0/typings/alembic/script/revision.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Any, Callable, Collection, Dict, FrozenSet, Iterable, Iterator, Optional, Sequence, Set, TYPE_CHECKING, Tuple, TypeVar, Union, overload
+from typing import Any, Callable, Dict, FrozenSet, Iterable, Iterator, List, Optional, Protocol, Sequence, Set, TYPE_CHECKING, Tuple, TypeVar, Union, overload
 from .. import util
 
 if TYPE_CHECKING:
     ...
-_RevIdType = Union[str, Sequence[str]]
+_RevIdType = Union[str, List[str], Tuple[str, ...]]
+_GetRevArg = Union[str, Iterable[Optional[str]], Iterable[str],]
 _RevisionIdentifierType = Union[str, Tuple[str, ...], None]
 _RevisionOrStr = Union["Revision", str]
 _RevisionOrBase = Union["Revision", "Literal['base']"]
 _InterimRevisionMapType = Dict[str, "Revision"]
 _RevisionMapType = Dict[Union[None, str, Tuple[()]], Optional["Revision"]]
-_T = TypeVar("_T", bound=Union[str, "Revision"])
+_T = TypeVar("_T")
+_TR = TypeVar("_TR", bound=Optional[_RevisionOrStr])
 _relative_destination = ...
 _revision_illegal_chars = ...
+class _CollectRevisionsProtocol(Protocol):
+    def __call__(self, upper: _RevisionIdentifierType, lower: _RevisionIdentifierType, inclusive: bool, implicit_base: bool, assert_relative_length: bool) -> Tuple[Set[Revision], Tuple[Optional[_RevisionOrBase], ...]]:
+        ...
+    
+
+
 class RevisionError(Exception):
     ...
 
 
 class RangeNotAncestorError(RevisionError):
     def __init__(self, lower: _RevisionIdentifierType, upper: _RevisionIdentifierType) -> None:
         ...
@@ -133,15 +141,15 @@
         .. seealso::
 
             :meth:`.ScriptDirectory.get_heads`
 
         """
         ...
     
-    def get_revisions(self, id_: Union[str, Collection[Optional[str]], None]) -> Tuple[Optional[_RevisionOrBase], ...]:
+    def get_revisions(self, id_: Optional[_GetRevArg]) -> Tuple[Optional[_RevisionOrBase], ...]:
         """Return the :class:`.Revision` instances with the given rev id
         or identifiers.
 
         May be given a single identifier, a sequence of identifiers, or the
         special symbols "head" or "base".  The result is a tuple of one
         or more identifiers, or an empty tuple in the case of "base".
 
@@ -167,15 +175,15 @@
         is matched against all identifiers that start with the given
         characters; if there is exactly one match, that determines the
         full revision.
 
         """
         ...
     
-    def filter_for_lineage(self, targets: Iterable[_T], check_against: Optional[str], include_dependencies: bool = ...) -> Tuple[_T, ...]:
+    def filter_for_lineage(self, targets: Iterable[_TR], check_against: Optional[str], include_dependencies: bool = ...) -> Tuple[_TR, ...]:
         ...
     
     def iterate_revisions(self, upper: _RevisionIdentifierType, lower: _RevisionIdentifierType, implicit_base: bool = ..., inclusive: bool = ..., assert_relative_length: bool = ..., select_for_downgrade: bool = ...) -> Iterator[Revision]:
         """Iterate through script revisions, starting at the given
         upper revision identifier and ending at the lower.
 
         The traversal uses strictly the `down_revision`
@@ -253,20 +261,20 @@
     def is_merge_point(self) -> bool:
         """Return True if this :class:`.Script` is a merge point."""
         ...
     
 
 
 @overload
-def tuple_rev_as_scalar(rev: Optional[Sequence[str]]) -> Optional[Union[str, Sequence[str]]]:
+def tuple_rev_as_scalar(rev: None) -> None:
     ...
 
 @overload
-def tuple_rev_as_scalar(rev: Optional[Sequence[Optional[str]]]) -> Optional[Union[Optional[str], Sequence[Optional[str]]]]:
+def tuple_rev_as_scalar(rev: Union[Tuple[_T, ...], List[_T]]) -> Union[_T, Tuple[_T, ...], List[_T]]:
     ...
 
-def tuple_rev_as_scalar(rev): # -> None:
+def tuple_rev_as_scalar(rev: Optional[Sequence[_T]]) -> Union[_T, Sequence[_T], None]:
     ...
 
 def is_revision(rev: Any) -> Revision:
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/script/write_hooks.pyi` & `bl_python_all-0.2.0/typings/alembic/script/write_hooks.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 REVISION_SCRIPT_TOKEN = ...
 _registry: dict = ...
 def register(name: str) -> Callable:
     """A function decorator that will register that function as a write hook.
 
     See the documentation linked below for an example.
 
-    .. versionadded:: 1.2.0
-
     .. seealso::
 
         :ref:`post_write_hooks_custom`
 
 
     """
     ...
 
 @register("console_scripts")
 def console_scripts(path: str, options: dict, ignore_output: bool = ...) -> None:
     ...
 
+@register("exec")
+def exec_(path: str, options: dict, ignore_output: bool = ...) -> None:
+    ...
+
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/testing/__init__.pyi` & `bl_python_all-0.2.0/typings/alembic/testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/testing/assertions.pyi` & `bl_python_all-0.2.0/typings/alembic/testing/assertions.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     The expect version **asserts** that the warnings were in fact seen.
 
     Note that the test suite sets SAWarning warnings to raise exceptions.
 
     """
     ...
 
-def emits_python_deprecation_warning(*messages): # -> (_Fn@decorator) -> _Fn@decorator:
+def emits_python_deprecation_warning(*messages): # -> Any:
     """Decorator form of expect_warnings().
 
     Note that emits_warning does **not** assert that the warnings
     were in fact seen.
 
     """
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/testing/env.pyi` & `bl_python_all-0.2.0/typings/alembic/testing/env.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/testing/fixtures.pyi` & `bl_python_all-0.2.0/typings/alembic/testing/fixtures.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         ...
     
     @testing.fixture
     def migration_context(self, connection): # -> MigrationContext:
         ...
     
     @testing.fixture
-    def connection(self): # -> Generator[db, Any, None]:
+    def connection(self): # -> Generator[Any, Any, None]:
         ...
     
 
 
 class TablesTest(TestBase, SQLAlchemyTablesTest):
     ...
 
@@ -33,15 +33,15 @@
 if sqla_14:
     ...
 else:
     class FutureEngineMixin:
         __requires__ = ...
     
     
-def capture_db(dialect=...): # -> tuple[Engine, list[Unknown]]:
+def capture_db(dialect=...): # -> tuple[Engine, list[Any]]:
     ...
 
 _engs: Dict[Any, Any] = ...
 @contextmanager
 def capture_context_buffer(**kw): # -> Generator[BytesIO | StringIO, Any, None]:
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/testing/util.pyi` & `bl_python_all-0.2.0/typings/alembic/testing/util.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This type stub file was generated by pyright.
 """
 
-def flag_combinations(*combinations): # -> (_FN@combinations) -> _FN@combinations:
+def flag_combinations(*combinations):
     """A facade around @testing.combinations() oriented towards boolean
     keyword-based arguments.
 
     Basically generates a nice looking identifier based on the keywords
     and also sets up the argument names.
 
     E.g.::
@@ -39,14 +39,14 @@
 
     This is used so that we can have module-level fixtures that
     refer to instance-level variables using lambdas.
 
     """
     ...
 
-def metadata_fixture(ddl=...): # -> (fn: Unknown) -> Unknown:
+def metadata_fixture(ddl=...): # -> Callable[..., Any]:
     """Provide MetaData for a pytest fixture."""
     ...
 
 def testing_engine(url=..., options=..., future=...):
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/util/editor.pyi` & `bl_python_all-0.2.0/typings/alembic/util/editor.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.all-0.1.1/typings/alembic/util/langhelpers.pyi` & `bl_python_all-0.2.0/typings/saml2/authn_context/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,93 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import (Any, Callable, Dict, Mapping, Optional, Tuple, TypeVar,
-                    overload)
+from saml2 import extension_elements_to_elements
+from saml2.authn_context import ippword, mobiletwofactor, ppt, pword, sslcert
+from saml2.saml import AuthnContext, AuthnContextClassRef
+from saml2.samlp import RequestedAuthnContext
 
-EMPTY_DICT: Mapping[Any, Any] = ...
-_T = TypeVar("_T")
-class _ModuleClsMeta(type):
-    def __setattr__(cls, key: str, value: Callable) -> None:
+UNSPECIFIED = ...
+INTERNETPROTOCOLPASSWORD = ...
+MOBILETWOFACTORCONTRACT = ...
+PASSWORDPROTECTEDTRANSPORT = ...
+PASSWORD = ...
+TLSCLIENT = ...
+TIMESYNCTOKEN = ...
+AL1 = ...
+AL2 = ...
+AL3 = ...
+AL4 = ...
+CMP_TYPE = ...
+class AuthnBroker:
+    def __init__(self) -> None:
         ...
     
-
-
-class ModuleClsProxy(metaclass=_ModuleClsMeta):
-    """Create module level proxy functions for the
-    methods on a given class.
-
-    The functions will have a compatible signature
-    as the methods.
-
-    """
-    _setups: Dict[type, Tuple[set, list]] = ...
-    @classmethod
-    def create_module_class_proxy(cls, globals_, locals_): # -> None:
+    @staticmethod
+    def exact(a, b):
         ...
     
+    @staticmethod
+    def minimum(a, b):
+        ...
+    
+    @staticmethod
+    def maximum(a, b):
+        ...
+    
+    @staticmethod
+    def better(a, b):
+        ...
+    
+    def add(self, spec, method, level=..., authn_authority=..., reference=...): # -> None:
+        """
+        Adds a new authentication method.
+        Assumes not more than one authentication method per AuthnContext
+        specification.
 
+        :param spec: What the authentication endpoint offers in the form
+            of an AuthnContext
+        :param method: A identifier of the authentication method.
+        :param level: security level, positive integers, 0 is lowest
+        :param reference: Desired unique reference to this `spec'
+        :return:
+        """
+        ...
+    
+    def remove(self, spec, method=..., level=..., authn_authority=...): # -> None:
+        ...
+    
+    def pick(self, req_authn_context=...): # -> list[tuple[Any, Any]] | list[Any] | None:
+        """
+        Given the authentication context find zero or more places where
+        the user could be sent next. Ordered according to security level.
 
-def rev_id() -> str:
-    ...
-
-@overload
-def to_tuple(x: Any, default: tuple) -> tuple:
-    ...
-
-@overload
-def to_tuple(x: None, default: Optional[_T] = ...) -> _T:
-    ...
-
-@overload
-def to_tuple(x: Any, default: Optional[tuple] = ...) -> tuple:
-    ...
-
-def to_tuple(x, default=...): # -> tuple[str] | tuple[Unknown, ...] | tuple[Unknown] | None:
-    ...
-
-def dedupe_tuple(tup: Tuple[str, ...]) -> Tuple[str, ...]:
-    ...
-
-class Dispatcher:
-    def __init__(self, uselist: bool = ...) -> None:
+        :param req_authn_context: The requested context as an
+            RequestedAuthnContext instance
+        :return: An URL
+        """
         ...
     
-    def dispatch_for(self, target: Any, qualifier: str = ...) -> Callable:
+    def match(self, requested, provided): # -> bool:
         ...
     
-    def dispatch(self, obj: Any, qualifier: str = ...) -> Any:
+    def __getitem__(self, ref):
         ...
     
-    def branch(self) -> Dispatcher:
-        """Return a copy of this dispatcher that is independently
-        writable."""
+    def get_authn_by_accr(self, accr):
         ...
     
 
 
-def not_none(value: Optional[_T]) -> _T:
+def authn_context_factory(text): # -> None:
+    ...
+
+def authn_context_decl_from_extension_elements(extelems): # -> None:
+    ...
+
+def authn_context_class_ref(ref): # -> AuthnContext:
+    ...
+
+def requested_authn_context(class_ref, comparison=...): # -> RequestedAuthnContext:
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/util/messaging.pyi` & `bl_python_all-0.2.0/typings/alembic/util/messaging.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 This type stub file was generated by pyright.
 """
 
 from collections.abc import Iterable
 from contextlib import contextmanager
-from typing import Optional, TextIO, Union
+from typing import Iterator, Optional, TextIO, Union
 
 log = ...
 ioctl = ...
 if TERMWIDTH <= 0:
     TERMWIDTH = ...
 def write_outstream(stream: TextIO, *text: Union[str, bytes], quiet: bool = ...) -> None:
     ...
 
 @contextmanager
-def status(status_msg: str, newline: bool = ..., quiet: bool = ...): # -> Generator[None, Any, None]:
+def status(status_msg: str, newline: bool = ..., quiet: bool = ...) -> Iterator[None]:
     ...
 
-def err(message: str, quiet: bool = ...):
+def err(message: str, quiet: bool = ...) -> None:
     ...
 
 def obfuscate_url_pw(input_url: str) -> str:
     ...
 
 def warn(msg: str, stacklevel: int = ...) -> None:
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/util/pyfiles.pyi` & `bl_python_all-0.2.0/typings/alembic/util/pyfiles.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Optional
+from types import ModuleType
+from typing import Any, Optional
 
-def template_to_file(template_file: str, dest: str, output_encoding: str, **kw) -> None:
+def template_to_file(template_file: str, dest: str, output_encoding: str, **kw: Any) -> None:
     ...
 
 def coerce_resource_to_filename(fname: str) -> str:
     """Interpret a filename as either a filesystem location or as a package
     resource.
 
     Names that are non absolute paths and contain a colon
@@ -17,14 +18,14 @@
     """
     ...
 
 def pyc_file_from_path(path: str) -> Optional[str]:
     """Given a python source path, locate the .pyc."""
     ...
 
-def load_python_file(dir_: str, filename: str): # -> ModuleType:
+def load_python_file(dir_: str, filename: str) -> ModuleType:
     """Load a file from the given path as a Python module."""
     ...
 
-def load_module_py(module_id: str, path: str): # -> ModuleType:
+def load_module_py(module_id: str, path: str) -> ModuleType:
     ...
```

### Comparing `BL_Python.all-0.1.1/typings/alembic/util/sqla_compat.pyi` & `bl_python_all-0.2.0/typings/alembic/util/sqla_compat.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 """
 This type stub file was generated by pyright.
 """
 
-from typing import Optional, TYPE_CHECKING, TypeVar, Union
-from sqlalchemy import Index, Table, __version__, sql, types as sqltypes
+from typing import Any, Callable, Optional, Protocol, TYPE_CHECKING, Type, TypeVar, Union
+from sqlalchemy import ClauseElement, Index, Table, sql, types as sqltypes
+from sqlalchemy.sql.base import _NoneName
 from sqlalchemy.sql.elements import BindParameter, ColumnElement, TextClause
 from typing_extensions import TypeGuard
-from sqlalchemy.sql.base import _NoneName
 from sqlalchemy.util import symbol as _NoneName
 
 if TYPE_CHECKING:
     ...
 _CE = TypeVar("_CE", bound=Union["ColumnElement[Any]", "SchemaItem"])
+class _CompilerProtocol(Protocol):
+    def __call__(self, element: Any, compiler: Any, **kw: Any) -> str:
+        ...
+    
+
+
 _vers = ...
 sqla_13 = ...
 sqla_14 = ...
 sqla_14_18 = ...
 sqla_14_26 = ...
 sqla_2 = ...
-sqlalchemy_version = __version__
+sqlalchemy_version = ...
 class _Unsupported:
     "Placeholder for unsupported SQLAlchemy classes"
     ...
 
 
+if TYPE_CHECKING:
+    def compiles(element: Type[ClauseElement], *dialects: str) -> Callable[[_CompilerProtocol], _CompilerProtocol]:
+        ...
+    
+else:
+    ...
 if sqla_2:
     ...
 else:
     ...
 _ConstraintName = Union[None, str, _NoneName]
 _ConstraintNameDefined = Union[str, _NoneName]
 def constraint_name_defined(name: _ConstraintName) -> TypeGuard[_ConstraintNameDefined]:
@@ -62,25 +74,28 @@
     See SQLAlchemy issue 3174.
 
     """
     __visit_name__ = ...
     def __init__(self, table: Table, text: TextClause) -> None:
         ...
     
-    def get_children(self): # -> list[Unknown]:
+    def get_children(self): # -> list[Column[NullType]]:
         ...
     
 
 
 class _literal_bindparam(BindParameter):
     ...
 
 
 if sqla_14:
-    ...
+    _select = ...
 else:
     def create_mock_engine(url, executor, **kw): # -> Engine:
         ...
     
 def is_expression_index(index: Index) -> bool:
     ...
 
+def is_expression(expr: Any) -> bool:
+    ...
+
```


# Comparing `tmp/BL_Python.web-0.1.1.tar.gz` & `tmp/bl_python_web-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.web-0.1.1.tar", last modified: Fri Feb 16 20:11:19 2024, max compression
+gzip compressed data, was "bl_python_web-0.2.0.tar", last modified: Tue May 14 21:50:45 2024, max compression
```

## Comparing `BL_Python.web-0.1.1.tar` & `bl_python_web-0.2.0.tar`

### file list

```diff
@@ -1,164 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.992047 BL_Python.web-0.1.1/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/encryption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/middleware/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/middleware/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/middleware/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/middleware/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/middleware/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/middleware/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.000047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21276 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/scaffolder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.992047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.992047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.992047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.992047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.996047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.996047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/BL_Python.web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-16 20:11:18.000000 BL_Python.web-0.1.1/BL_Python.web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.996047 BL_Python.web-0.1.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.004047 BL_Python.web-0.1.1/test/unit/application/
--rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/application/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    19626 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/create_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.008047 BL_Python.web-0.1.1/test/unit/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.008047 BL_Python.web-0.1.1/test/unit/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_api_request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_api_response_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_flask_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/middleware/test_openapi_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.008047 BL_Python.web-0.1.1/test/unit/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/scaffolding/test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/test/unit/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:18.996047 BL_Python.web-0.1.1/typings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.012047 BL_Python.web-0.1.1/typings/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.012047 BL_Python.web-0.1.1/typings/connexion/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/apps/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/apps/asynchronous.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/apps/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/datastructures.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.012047 BL_Python.web-0.1.1/typings/connexion/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/decorators/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/decorators/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/decorators/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.012047 BL_Python.web-0.1.1/typings/connexion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/frameworks/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/frameworks/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/frameworks/starlette.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/http_facts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/json_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/jsonifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/lifecycle.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.016047 BL_Python.web-0.1.1/typings/connexion/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/lifespan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/request_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/response_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/routing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/middleware/swagger_ui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/mock.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.016047 BL_Python.web-0.1.1/typings/connexion/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/operations/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/operations/openapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/operations/swagger2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/problem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/spec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/uri_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.016047 BL_Python.web-0.1.1/typings/connexion/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/validators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/validators/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/validators/form_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/validators/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/connexion/validators/parameter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/connexion/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/fastapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/fastapi/implementation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/flask/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/quart/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/quart/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 20:11:19.020047 BL_Python.web-0.1.1/typings/json_logging/framework/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework/sanic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/framework_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-16 20:11:10.000000 BL_Python.web-0.1.1/typings/json_logging/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.931189 bl_python_web-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.939189 bl_python_web-0.2.0/BL_Python/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/encryption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    19522 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24782 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/scaffolder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__meta__.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/conftest.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/BL_Python.web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/test/unit/application/
+-rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/application/test_create_flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/application/test_create_openapi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_api_request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_api_response_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_flask_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_openapi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/scaffolding/test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.939189 bl_python_web-0.2.0/typings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/asynchronous.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/datastructures.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/starlette.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/http_facts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/json_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/jsonifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/lifecycle.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/lifespan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/request_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/response_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/routing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/swagger_ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/mock.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/openapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/swagger2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/problem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/uri_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/form_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/parameter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/flask_injector/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_injector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_injector/tests.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/flask_login/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/__about__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/login_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/test_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/connexion/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/flask/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/quart/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/sanic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/util.pyi
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/application.py` & `bl_python_web-0.2.0/BL_Python/web/application.py`

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

### Comparing `BL_Python.web-0.1.1/BL_Python/web/config.py` & `bl_python_web-0.2.0/BL_Python/web/config.py`

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

### Comparing `BL_Python.web-0.1.1/BL_Python/web/encryption/__init__.py` & `bl_python_web-0.2.0/BL_Python/web/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/middleware/__init__.py` & `bl_python_web-0.2.0/BL_Python/web/middleware/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from BL_Python.web.middleware.flask import (
     register_flask_api_request_handlers,
     register_flask_api_response_handlers,
 )
 from BL_Python.web.middleware.openapi import (
     register_openapi_api_request_handlers,
     register_openapi_api_response_handlers,
+    register_openapi_context_middleware,
 )
 from connexion import FlaskApp
 from flask import Flask, Response
 from flask.typing import (
     AfterRequestCallable,
     BeforeRequestCallable,
     ResponseReturnValue,
@@ -41,14 +42,16 @@
     Callable[..., ResponseReturnValue] | Callable[..., Awaitable[ResponseReturnValue]]
 )
 T_error_handler = TypeVar("T_error_handler", bound=ErrorHandlerCallable)
 
 TFlaskApp = Flask | FlaskApp
 T_flask_app = TypeVar("T_flask_app", bound=TFlaskApp)
 
+RegisterMiddlewareCallback = Callable[[FlaskApp], None]
+
 
 def bind_errorhandler(
     app: TFlaskApp,
     code_or_exception: type[Exception] | int,
 ) -> Callable[[T_error_handler], T_error_handler | None]:
     if isinstance(app, Flask):
         return app.errorhandler(code_or_exception)
@@ -68,14 +71,20 @@
         # TODO consider moving request/response logging to the WSGI app
         # apparently Flask may not call this if unhandled exceptions occur
         return register_flask_api_response_handlers(app)
     else:
         return register_openapi_api_response_handlers(app)
 
 
+def register_context_middleware(app: TFlaskApp):
+    if not isinstance(app, FlaskApp):
+        return
+    return register_openapi_context_middleware(app)
+
+
 def register_error_handlers(app: TFlaskApp):
     @bind_errorhandler(app, Exception)
     # @inject
     def catch_all_catastrophic(error: Exception, log: Logger):
         # error: connexion.lifecycle.ConnexionRequest, log: ZeroDivisionError
         log.exception(error)
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/middleware/consts.py` & `bl_python_web-0.2.0/BL_Python/web/middleware/consts.py`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/middleware/dependency_injection.py` & `bl_python_web-0.2.0/BL_Python/web/middleware/dependency_injection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from functools import partial
-from typing import Any, Protocol, Tuple, cast
+from typing import Any, Callable, Protocol, Tuple, Type, cast
 
 from BL_Python.programming.patterns.dependency_injection import LoggerModule
 from connexion import ConnexionMiddleware, FlaskApp
 from connexion.apps.flask import FlaskASGIApp, FlaskOperation
+from connexion.middleware.main import MiddlewarePosition
 from flask import Config as Config
 from flask import Flask
-from flask_injector import wrap_function  # pyright: ignore[reportUnknownVariableType]
-from flask_injector import FlaskInjector
+from flask_injector import FlaskInjector, wrap_function
 from injector import Binder, Injector, Module
 from starlette.types import ASGIApp, Receive, Scope, Send
 from typing_extensions import override
 
-from . import TFlaskApp
+from . import RegisterMiddlewareCallback, TFlaskApp
 
 
 class MiddlewareRoutine(Protocol):
     def __call__(
         self, scope: Scope, receive: Receive, send: Send, *args: Any
     ) -> None: ...
 
 
 class AppModule(Module):
     def __init__(self, app: TFlaskApp, *args: Tuple[Any, Any]) -> None:
         super().__init__()
         if isinstance(app, Flask):
             self._flask_app = app
-        elif isinstance(
-            app, FlaskApp
-        ):  # pyright: ignore[reportUnnecessaryIsInstance] guard against things like not using `MagicMock(spec=...)`
+        elif isinstance(app, FlaskApp):  # pyright: ignore[reportUnnecessaryIsInstance] guard against things like not using `MagicMock(spec=...)`
             self._flask_app = app.app
         else:
             raise ValueError(
                 f"Wrong type provided for Flask instance. Provided type is `{type(app)}` but excepted `{TFlaskApp}`."
             )
 
         self._other_dependencies = args
@@ -45,35 +43,57 @@
 
         for dependency in self._other_dependencies:
             binder.bind(dependency[0], to=dependency[1])
 
 
 def configure_dependencies(
     app: TFlaskApp,
-    application_modules: list[Module] | None = None,
+    application_modules: list[Module | type[Module]] | None = None,
 ) -> FlaskInjector:
     """
     Configures dependency injection and registers all Flask
     application dependencies. The FlaskInjector instance
     can be used to bootstrap and start the Flask application.
     """
     if isinstance(app, FlaskApp):
         flask_app = app.app
     else:
         flask_app = app
 
-    modules = [AppModule(app)] + (application_modules if application_modules else [])
+    modules = [
+        (module if isinstance(module, Module) else module())
+        for module in [AppModule(app)]
+        + (application_modules if application_modules else [])
+    ]
 
     # bootstrap the flask application and its dependencies
     flask_injector = FlaskInjector(flask_app, modules)
 
     flask_injector.injector.binder.bind(Injector, flask_injector.injector)
 
     if isinstance(app, FlaskApp):
         app.add_middleware(OpenAPIEndpointDependencyInjectionMiddleware(flask_injector))
+
+        # For every module registered, check if any are "middleware" type modules.
+        # if they are, they need to be registered with the application.
+        # In the event the application is a Connexion application,
+        # this needs to happen after _configure_openapi_middleware_dependencies
+        # because the middleware is a "FILO" stack - the items are the end
+        # of the stack are executed first. By ensuring this happens before
+        # OpenAPIEndpointDependencyInjectionMiddleware, other Middlewares
+        # can alter routing information.
+        # TODO this needs to happen in some form for plain Flask applications too.
+        for module in modules:
+            register_callback: RegisterMiddlewareCallback | None = getattr(
+                module, "register_middleware", None
+            )
+            if register_callback is not None and callable(register_callback):
+                register_callback(app)
+
+        # this binds all BL_Python middlewares with Injector
         _configure_openapi_middleware_dependencies(app, flask_injector)
 
     return flask_injector
 
 
 class OpenAPIEndpointDependencyInjectionMiddleware:
     """
@@ -132,40 +152,87 @@
                         None,
                     )
 
                     if not flask_asgi_app:
                         return await send(message)
 
                     endpoints = cast(
-                        dict[str, FlaskOperation], flask_asgi_app.app.view_functions
+                        dict[str, FlaskOperation | Callable[..., Any]],
+                        flask_asgi_app.app.view_functions,
                     )
 
                     for endpoint_name, endpoint in endpoints.items():
                         # Skip anything that does not have `@inject` applied
                         if not hasattr(endpoint, "__bindings__"):
                             continue
 
-                        # _fn is the original function that ends up being called.
-                        # we wrap it with Injector, then replace it
-                        endpoints[endpoint_name]._fn = wrap_function(
-                            endpoint._fn,
-                            self._flask_injector.injector,
-                        )
+                        if hasattr(endpoint, "_fn") and isinstance(
+                            endpoint, FlaskOperation
+                        ):
+                            # _fn is the original function that ends up being called.
+                            # we wrap it with Injector, then replace it
+                            endpoints[endpoint_name]._fn = wrap_function(  # pyright: ignore[reportFunctionMemberAccess]
+                                endpoint._fn,
+                                self._flask_injector.injector,
+                            )
+                        # If a blueprint is added through anything other than
+                        # by Connexion, `_fn` is not set. This happens with, e.g.,
+                        # the SSO blueprint.
+                        else:
+                            if callable(endpoint):
+                                endpoints[endpoint_name] = wrap_function(
+                                    endpoint,
+                                    self._flask_injector.injector,
+                                )
 
                     return await send(message)
 
                 await self._app(scope, receive, wrapped_send)
 
         return type(
             "_DependencyInjectionMiddleware",
             (_InternalDependencyInjectionMiddleware,),
             {},
         )
 
 
+def bind_middleware(
+    app: TFlaskApp,
+    flask_injector: FlaskInjector,
+    middleware: Type[ASGIApp],
+    position: MiddlewarePosition = MiddlewarePosition.BEFORE_CONTEXT,
+):
+    middleware_class: Callable[..., Any] = middleware
+
+    # hasn't been registered with the application yet
+    if not isinstance(middleware, partial):
+        if not isinstance(app, FlaskApp):
+            return
+
+        app.add_middleware(middleware_class, position)
+    else:
+        middleware_class = middleware.func
+
+    # Connexion/Starlette middleware are classes w/ a __call__ method
+    middleware_routine = cast(
+        MiddlewareRoutine | None, getattr(middleware_class, "__call__", None)
+    )
+    if not middleware_routine:
+        return
+
+    # Skip any __call__ methods without `@inject` applied
+    if not hasattr(middleware_routine, "__bindings__"):
+        return
+
+    # Wrap the __call__ method and replace the original with the now-wrapped method
+    middleware_class.__call__ = (  # pyright: ignore[reportFunctionMemberAccess]
+        wrap_function(middleware_routine, flask_injector.injector)
+    )
+
+
 def _configure_openapi_middleware_dependencies(
     app: TFlaskApp, flask_injector: FlaskInjector
 ):
     """
     Bind any Connexion middleware classes whose __call__ member has a __bindings__ attribute.
     This attribute signals that @inject was used on it.
     """
@@ -175,26 +242,13 @@
         return
 
     app_middlewares = getattr(app_middleware, "middlewares", None)
     if not app_middlewares:
         return
 
     for middleware in cast(list[type], app_middlewares):
+        # these are all middlewares that are registered by Connexion
+        # so we can skip them
         if not isinstance(middleware, partial):
             continue
 
-        # Connexion/Starlette middleware are classes w/ a __call__ method
-        middleware_class = middleware.func
-        middleware_routine = cast(
-            MiddlewareRoutine | None, getattr(middleware_class, "__call__", None)
-        )
-        if not middleware_routine:
-            continue
-
-        # Skip any __call__ methods without `@inject` applied
-        if not hasattr(middleware_routine, "__bindings__"):
-            continue
-
-        # Wrap the __call__ method and replace the original with the now-wrapped method
-        middleware_class.__call__ = (  # pyright: ignore[reportFunctionMemberAccess]
-            wrap_function(middleware_routine, flask_injector.injector)
-        )
+        bind_middleware(app, flask_injector, middleware)
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/middleware/flask/__init__.py` & `bl_python_web-0.2.0/BL_Python/web/middleware/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/middleware/openapi/__init__.py` & `bl_python_web-0.2.0/BL_Python/web/middleware/openapi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import re
 import uuid
+from contextlib import ExitStack
+from contextvars import Token
 from logging import Logger
 from typing import Any, Awaitable, Callable, Literal, TypeVar, cast
 from uuid import uuid4
 
 import json_logging
-from BL_Python.programming.collections.dict import AnyDict
-from connexion import ConnexionMiddleware, FlaskApp, utils
-from flask import Flask, Response
+from BL_Python.programming.collections.dict import AnyDict, merge
+from connexion import ConnexionMiddleware, FlaskApp, context, utils
+from connexion.middleware import MiddlewarePosition
+from flask import Flask, Request, Response, request
+from flask.ctx import AppContext
+from flask.globals import _cv_app  # pyright: ignore[reportPrivateUsage]
+from flask.globals import current_app
 from flask.typing import (
     AfterRequestCallable,
     BeforeRequestCallable,
     ResponseReturnValue,
 )
 from injector import inject
 from starlette.types import ASGIApp, Receive, Scope, Send
-from typing_extensions import TypedDict
+from typing_extensions import TypedDict, final
 
 from ...config import Config
 from ..consts import (
     CONTENT_SECURITY_POLICY_HEADER,
     CORRELATION_ID_HEADER,
     CORS_ACCESS_CONTROL_ALLOW_CREDENTIALS_HEADER,
     CORS_ACCESS_CONTROL_ALLOW_METHODS_HEADER,
@@ -162,17 +168,15 @@
         )
 
 
 def _headers_as_dict(
     request_response: MiddlewareRequestDict | MiddlewareResponseDict,
 ):
     if (
-        isinstance(
-            request_response, dict
-        )  # pyright: ignore[reportUnnecessaryIsInstance]
+        isinstance(request_response, dict)  # pyright: ignore[reportUnnecessaryIsInstance]
         and "headers" in request_response.keys()
     ):
         # FIXME does this work for a middleware _response_ as well?
         return {
             key: value for (key, value) in decode_headers(request_response["headers"])
         }
     else:
@@ -426,35 +430,130 @@
                 )
 
                 if request_correlation_id:
                     # validate format
                     _ = uuid.UUID(request_correlation_id.decode(encoding))
                 else:
                     request_correlation_id = str(uuid4()).encode(encoding)
-                    request_headers.append(
-                        (correlation_id_header_encoded, request_correlation_id)
-                    )
+                    request_headers.append((
+                        correlation_id_header_encoded,
+                        request_correlation_id,
+                    ))
                     log.info(
                         f'Generated new UUID "{request_correlation_id}" for {CORRELATION_ID_HEADER} request header.'
                     )
 
-                response_headers.append(
-                    (correlation_id_header_encoded, request_correlation_id)
-                )
+                response_headers.append((
+                    correlation_id_header_encoded,
+                    request_correlation_id,
+                ))
 
                 return await send(message)
             except ValueError as e:
                 log.warning(
                     f"Badly formatted {CORRELATION_ID_HEADER} received in request."
                 )
                 raise e
 
         await self._app(scope, receive, wrapped_send)
 
 
+@final
+class FlaskContextMiddleware:
+    """
+    Connexion does not set Flask contexts in all cases they may be needed, like
+    in middlewares that execute before ContextMiddleware. This middleware creates
+    the Flask application, request, and session contexts if they are not currently set.
+    """
+
+    def __init__(
+        self,
+        app: ASGIApp,
+    ) -> None:
+        self.app = app
+
+    @inject
+    async def __call__(
+        self, scope: Scope, receive: Receive, send: Send, app: Flask
+    ) -> None:
+        receive_token: Token[Receive] | None = None
+        scope_token: Token[Scope] | None = None
+        app_ctx_token: Token[AppContext] | None = None
+
+        try:
+            receive_token = context._receive.set(receive)  # pyright: ignore[reportPrivateUsage]
+            scope_token = context._scope.set(scope)  # pyright: ignore[reportPrivateUsage]
+
+            if scope["type"] not in ["http", "websocket"]:
+                await self.app(scope, receive, send)
+                return
+
+            with ExitStack() as exit_stack:
+                if not isinstance(current_app, Flask):  # pyright: ignore[reportUnnecessaryIsInstance] it is not a Flask if it is not set
+                    app_ctx = exit_stack.enter_context(app.app_context())
+
+                    app_ctx_token = _cv_app.set(app_ctx)
+
+                if not isinstance(request, Request):  # pyright: ignore[reportUnnecessaryIsInstance] it is not a Request if it is not set
+                    request_environ = merge(
+                        {
+                            "PATH_INFO": scope.get("path")
+                            or context.request._starlette_request.url.path,
+                            "wsgi.url_scheme": scope.get("scheme")
+                            or context.request._starlette_request.url.scheme,
+                            "REQUEST_METHOD": scope.get("method")
+                            or context.request._starlette_request.method,
+                            # there is the possibility this value in scope is "127.0.0.1" when using "localhost"
+                            # which is not consistent with the _starlette_request value.
+                            "SERVER_NAME": (
+                                scope["server"][0]
+                                if scope.get("server")
+                                else context.request._starlette_request.base_url.hostname
+                            ),
+                            "SERVER_PORT": (
+                                scope["server"][1]
+                                if scope.get("server")
+                                else context.request._starlette_request.base_url.port
+                            ),
+                            "QUERY_STRING": scope.get("query_string")
+                            or context.request._starlette_request.url.query,
+                            "REMOTE_ADDR": ":".join([
+                                str(value) for value in scope["client"]
+                            ])
+                            or f"{context.request._starlette_request.client.host}:{context.request._starlette_request.client.port}",
+                        },
+                        dict({
+                            (
+                                f"{'HTTP_' if header.upper() not in ['CONTENT_TYPE', 'CONTENT_LENGTH'] else ''}{header.upper().replace('-', '_')}",
+                                value,
+                            )
+                            for header, value in context.request.headers.items()
+                        }),
+                    )
+
+                    request_ctx = exit_stack.enter_context(
+                        app.request_context(request_environ)
+                    )
+                    request_ctx.push()
+
+                await self.app(scope, receive, send)
+
+        finally:
+            if app_ctx_token is not None:
+                _cv_app.reset(app_ctx_token)
+            if receive_token is not None:
+                context._receive.reset(receive_token)  # pyright: ignore[reportPrivateUsage]
+            if scope_token is not None:
+                context._scope.reset(scope_token)  # pyright: ignore[reportPrivateUsage]
+
+
 def register_openapi_api_request_handlers(app: FlaskApp):
     app.add_middleware(RequestLoggerMiddleware)
 
 
 def register_openapi_api_response_handlers(app: FlaskApp):
     app.add_middleware(CorrelationIDMiddleware)
     app.add_middleware(ResponseLoggerMiddleware)
+
+
+def register_openapi_context_middleware(app: FlaskApp):
+    app.add_middleware(FlaskContextMiddleware, MiddlewarePosition.BEFORE_EXCEPTION)
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/__main__.py` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,49 +2,44 @@
 import sys
 from argparse import ArgumentParser, Namespace
 from functools import partial
 from os import environ
 from pathlib import Path
 from typing import Callable, Literal, NamedTuple
 
-from BL_Python.programming.cli.argparse import (
-    associate_disallow_duplicate_values,
-    disallow,
-)
+from BL_Python.programming.cli.argparse import DisallowDuplicateValues, disallow
 from BL_Python.web.scaffolding import (
     Operation,
     ScaffoldConfig,
     ScaffoldEndpoint,
     Scaffolder,
     ScaffoldModule,
 )
 from typing_extensions import final
 
 APPLICATION_ENDPOINT_PATH_NAME = "application"
 
 
 class ScaffoldInputArgs(Namespace):
-    mode: Literal[  # pyright: ignore[reportUninitializedInstanceVariable]
-        "create", "modify"
-    ]
+    mode: Literal["create", "modify"]  # pyright: ignore[reportUninitializedInstanceVariable]
     mode_executor: "Callable[[ScaffoldParsedArgs], None]"  # pyright: ignore[reportUninitializedInstanceVariable]
     name: Operation  # pyright: ignore[reportUninitializedInstanceVariable]
     endpoints: list[Operation] | None = None
     template_type: Literal["basic", "openapi"] = "basic"
-    modules: list[Literal["database"]] | None = None
+    modules: list[Literal["database", "test"]] | None = None
     output_directory: str | None = None
 
 
 class ScaffoldParsedArgs(NamedTuple):
     mode: Literal["create", "modify"]
     mode_executor: "Callable[[ScaffoldParsedArgs], None]"
     name: Operation
     endpoints: list[Operation]
     template_type: Literal["basic", "openapi"]
-    modules: list[Literal["database"]] | None
+    modules: list[Literal["database", "test"]] | None
     output_directory: str
 
 
 @final
 class ScaffolderCli:
     _log: logging.Logger
 
@@ -84,27 +79,27 @@
             help="The name of the application.",
         )
         _ = create_parser.add_argument(
             "-e",
             metavar="endpoint",
             dest="endpoints",
             type=disallow([APPLICATION_ENDPOINT_PATH_NAME], "endpoint", Operation),
-            action=associate_disallow_duplicate_values("name"),
+            action=DisallowDuplicateValues,
             help="The name of an endpoint to scaffold. Can be specified more than once. If not specified, an endpoint sharing the name of the application will be scaffolded.",
         )
         template_types = ["basic", "openapi"]
         _ = create_parser.add_argument(
             "-t",
             choices=template_types,
             dest="template_type",
             type=str.lower,
             default="basic",
             help="The type of template to scaffold.",
         )
-        modules = ["database"]
+        modules = ["database", "test"]
         _ = create_parser.add_argument(
             "-m",
             choices=modules,
             action="append",
             dest="modules",
             type=str,
             help="An optional module to include in the application. Can be specified more than once.",
@@ -132,15 +127,15 @@
             help="The name of the application.",
         )
         _ = modify_parser.add_argument(
             "-e",
             metavar="endpoint",
             dest="endpoints",
             type=disallow([APPLICATION_ENDPOINT_PATH_NAME], "endpoint", Operation),
-            action=associate_disallow_duplicate_values("name"),
+            action=DisallowDuplicateValues,
             help="The name of an endpoint to scaffold. Can be specified more than once. If not specified, an endpoint sharing the name of the application will be scaffolded.",
         )
         _ = modify_parser.add_argument(
             "-o",
             metavar="output directory",
             dest="output_directory",
             type=str,
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/scaffolder.py` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/scaffolder.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 import sys
 import types
 from dataclasses import asdict, dataclass, field
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_file_location
 from os import sep as path_separator
 from pathlib import Path
-from typing import Any, final
+from typing import Any, Literal, final
 
 from BL_Python.programming.collections.dict import merge
 from jinja2 import BaseLoader, Environment, PackageLoader, Template
 
 # fmt: off
-from pkg_resources import (
-    ResourceManager,  # pyright: ignore[reportUnknownVariableType,reportAttributeAccessIssue]
-)
-from pkg_resources import get_provider
-from typing_extensions import final, override
+from pkg_resources import IResourceProvider, ResourceManager, get_provider
+from typing_extensions import override
 
 # fmt: on
 
 
 @dataclass
 class Operation:
     url_path_name: str
@@ -38,55 +35,62 @@
 
     @override
     def __str__(self) -> str:
         return self.url_path_name
 
     @override
     def __eq__(self, __value: object) -> bool:
-
         return isinstance(__value, Operation) and (
             self.url_path_name == __value.url_path_name
             or self.module_name == __value.module_name
         )
 
 
 @dataclass
 class ScaffoldEndpoint:
     operation: Operation
     # This is Flask's default hostname.
-    hostname: str = "http://127.0.0.1:5000"
+    hostname: str = "http://localhost:5000"
 
 
 @dataclass
 class ScaffoldModule:
     module_name: str
 
 
 @dataclass
 class ScaffoldConfig:
     output_directory: str
     application: Operation
-    template_type: str | None = None
+    template_type: Literal["basic", "openapi"] | None = None
     modules: list[ScaffoldModule] | None = None
     module: dict[str, Any] = field(default_factory=dict)
     endpoints: list[ScaffoldEndpoint] | None = None
     mode: str = "create"
 
 
 @final
 class Scaffolder:
+    # These are used to aid in discovering files that are
+    # part of the BL_Python.web module. Relative path lookups
+    # do not work, so they are done using _provider.
+    _manager: Any
+    _provider: IResourceProvider
+
     def __init__(self, config: ScaffoldConfig, log: logging.Logger) -> None:
         self._config = config
         self._config_dict = asdict(config)
         self._log = log
         self._checked_directories: set[Path] = set()
         # BaseLoader is used for rendering strings only. It does not need additional functionality.
         self._base_env = Environment(
             loader=BaseLoader  # pyright: ignore[reportArgumentType]
         )
+        self._manager = ResourceManager()
+        self._provider = get_provider("BL_Python.web")
 
     def _create_directory(self, directory: Path, overwrite_existing_files: bool = True):
         """Create the directories that the rendered templates will be stored in."""
         if directory in self._checked_directories:
             return
 
         self._checked_directories.add(directory)
@@ -123,14 +127,15 @@
         self,
         template_name: str,
         template_environment: Environment,
         template_directory_prefix: str = "",
         template_config: dict[str, Any] | None = None,
         template: Template | None = None,
         overwrite_existing_files: bool = True,
+        write_rendered_template: bool = True,
     ):
         """
         Render a template that can either be found by name in
         the provided `template_environment`, or render the provided `template`.
 
         :param template_name: The name of the template that might be discoverable in the `template_environment`.
         :param template_environment: The jinja2 template environment used for rendering the template.
@@ -143,14 +148,16 @@
             file `./__init__.py` is discovered at the template environment root,
             the file will instead be stored at `<output directory>/{{application.module_name}}/modules/database/__init__.py`.
         :param template_config: A dictionary of values that the template can reference.
         :param template: If provided, this template will be rendered instead of trying to discover the template with the name `template_name`
             in the template environment.
         :param overwrite_existing_files: If True, any existing files will be overwritten. If False, the template will not be rendered, and
             the file at the output location will not be overwritten.
+        :param write_rendered_template: If True, the template will be written to the filesystem. If False, the template will be rendered, but
+            not output anywhere.
         """
         if template_config is None:
             template_config = self._config_dict
 
         rendered_template_path = Path(
             # This causes paths with jinja2 directives to be rendered.
             # For example, if `self._config_dict['application'].module_name` is `foo`,
@@ -184,44 +191,60 @@
             f"Rendering template `{template_output_path}` with config `{template_config}`"
         )
 
         # if a template is not provided, find the template in the environment
         if not template:
             template = template_environment.get_template(template_name)
 
-        template.stream(  # pyright: ignore[reportUnknownMemberType]
-            **template_config
-        ).dump(str(template_output_path))
+        if write_rendered_template:
+            template.stream(  # pyright: ignore[reportUnknownMemberType]
+                **template_config
+            ).dump(str(template_output_path))
+        else:
+            template_stream = template.stream(**template_config)
+            while next(template_stream, None):
+                pass
 
     def _scaffold_directory(
         self,
         env: Environment,
         template_directory_prefix: str = "",
         overwrite_existing_files: bool = True,
     ):
         """
         Render all templates discovered under the root directory of the provided template environment.
         Rendered templates are output relative to their location in the template directory, prefixed
         with `<output directory>/template_directory_prefix`.
         Only files ending with `.j2` are rendered.
         """
+        META_TEMPLATE_NAME = "__meta__.j2"
         # render the base templates
-        for template_name in env.list_templates(extensions=["j2"]):
+        templates = env.list_templates(extensions=["j2"])
+        # if a module have a `__meta__.j2` file, then
+        # that module is responsible for rendering its
+        # own templates.
+        # the template name will be without its parent directory
+        # because the module renderer uses the module
+        # template directory as the root directory.
+        if META_TEMPLATE_NAME in templates:
             self._render_template(
-                template_name,
+                META_TEMPLATE_NAME,
                 env,
                 template_directory_prefix=template_directory_prefix,
                 overwrite_existing_files=overwrite_existing_files,
+                write_rendered_template=False,
             )
-
-    # These are used to aid in discovering files that are
-    # part of the BL_Python.web module. Relative path lookups
-    # do not work, so they are done using _provider.
-    _manager: Any = ResourceManager()
-    _provider = get_provider("BL_Python.web")
+        else:
+            for template_name in templates:
+                self._render_template(
+                    template_name,
+                    env,
+                    template_directory_prefix=template_directory_prefix,
+                    overwrite_existing_files=overwrite_existing_files,
+                )
 
     def _execute_module_hooks(self, module_template_directory: str):
         """
         Modules may have a file named `__hook__.py`. If it exists, it
         is executed as part of the scaffolding process.
 
         Hooks that can be configured in a module are:
@@ -255,38 +278,97 @@
                 # only called when an application is being created,
                 # any such method is only called when an application
                 # is being created. Although the only documented
                 # method allowed is `on_create`, any such prefixed
                 # method will be called.
                 module_var(self._config_dict, self._log)
 
+    def render_module_template(
+        self,
+        module: ScaffoldModule,
+        module_template_directory: Path,
+        overwrite_existing_files: bool = True,
+    ):
+        def _render_module_template(
+            template_name: str,
+            config: dict[Any, Any],
+        ):
+            meta_module_env = Environment(
+                trim_blocks=True,
+                lstrip_blocks=True,
+                loader=PackageLoader(
+                    "BL_Python.web",
+                    str(Path(module_template_directory, "templates")),
+                ),
+            )
+            # set a test module-specific "meta" config for
+            # use by whatever templates this loop will render
+            self._config_dict["meta"] = config
+
+            self._render_template(
+                template_name,
+                meta_module_env,
+                template_directory_prefix=f"{self._config.application.module_name}/modules/{module.module_name}",
+                overwrite_existing_files=overwrite_existing_files,
+            )
+
+        return _render_module_template
+
     def _scaffold_modules(self, overwrite_existing_files: bool = True):
         """
         Render any modules configured to render.
         """
         if self._config.modules is None:
             self._log.debug("No optional modules to scaffold.")
             return
 
         # each module's configuration currently only includes
         # the module's name. This name also matches the filesystem
         # directory for the module's templates.
         for module in self._config.modules:
             # module templates are stored under `optional/`
             # because we don't always want to render any given module.
-            module_template_directory = f"scaffolding/templates/optional/{{{{application.module_name}}}}/modules/{module.module_name}"
+            module_template_directory = Path(
+                f"scaffolding/templates/optional/{{{{application.module_name}}}}/modules/{module.module_name}"
+            )
             # executed module hooks before any rendering is done
             # so the hooks can modify the config or do other
             # work if it's needed.
-            self._execute_module_hooks(module_template_directory)
+            self._execute_module_hooks(str(module_template_directory))
 
-            module_env = Environment(
-                trim_blocks=True,
-                lstrip_blocks=True,
-                loader=PackageLoader("BL_Python.web", str(module_template_directory)),
+            # all modules contain templates under templates/
+            # but only modules with __meta__.j2 control how
+            # their own templates are rendered.
+            if self._provider.has_resource(  # pyright: ignore[reportUnknownMemberType]
+                str(Path(module_template_directory, "__meta__.j2"))
+            ):
+                module_env = Environment(
+                    trim_blocks=True,
+                    lstrip_blocks=True,
+                    loader=PackageLoader(
+                        "BL_Python.web", str(Path(module_template_directory))
+                    ),
+                )
+            else:
+                module_env = Environment(
+                    trim_blocks=True,
+                    lstrip_blocks=True,
+                    loader=PackageLoader(
+                        "BL_Python.web",
+                        str(Path(module_template_directory, "templates")),
+                    ),
+                )
+
+            # this is necessary to overwrite for every module
+            # because the directory and module config are
+            # unique for each one.
+            module_env.globals["render_module_template"] = self.render_module_template(  # pyright: ignore[reportArgumentType]
+                module=module,
+                module_template_directory=module_template_directory,
+                overwrite_existing_files=overwrite_existing_files,
             )
 
             self._scaffold_directory(
                 module_env,
                 # prefix the directory so that rendered templates
                 # are output _not_ relative to the template environment
                 # root, which would store the rendered templates in `./`.
@@ -423,15 +505,15 @@
             )
             return
 
         # modify can only run from an existing application's
         # parent directory.
         if self._config.mode == "modify" and not in_parent_directory:
             self._log.critical(
-                f"Attempted to modify an existing application from a directory that is not the existing application's parent directory. This is not supported. Change your working directory to the application's parent directory."
+                "Attempted to modify an existing application from a directory that is not the existing application's parent directory. This is not supported. Change your working directory to the application's parent directory."
             )
             return
 
         if (
             # Only in create mode do we make absolutely certain that
             # the user is intentionally using a directory that
             # already exists, if it indeed does.
@@ -450,30 +532,30 @@
             self._log.debug(f"User's input is `{response}`. Continuing.")
 
         # used for the primary set of templates that a
         # scaffolded application is made up of.
         base_env = Environment(
             trim_blocks=True,
             lstrip_blocks=True,
-            loader=PackageLoader("BL_Python.web", f"scaffolding/templates/base"),
+            loader=PackageLoader("BL_Python.web", "scaffolding/templates/base"),
         )
         # used for the selected template type templates
         # that can replace files from the base templates.
         template_type_env = Environment(
             trim_blocks=True,
             lstrip_blocks=True,
             loader=PackageLoader(
                 "BL_Python.web", f"scaffolding/templates/{self._config.template_type}"
             ),
         )
         # used for templates under `optional/`
         optional_env = Environment(
             trim_blocks=True,
             lstrip_blocks=True,
-            loader=PackageLoader("BL_Python.web", f"scaffolding/templates/optional"),
+            loader=PackageLoader("BL_Python.web", "scaffolding/templates/optional"),
         )
 
         if self._config.mode == "create":
             # scaffold modules first so they can alter the config if necessary.
             # a template environment is not passed in because `scaffold_modules`
             # creates a new environment for each module.
             self._scaffold_modules()
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/README.md.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/README.md.j2`

 * *Files 7% similar despite different names*

```diff
@@ -44,7 +44,11 @@
 
 Existing endpoints can be freely changed provided the methods comply with the configuration in [openapi.yaml]({{application.module_name}}/openapi.yaml). Added methods must have a corresponding `operationId` added to [openapi.yaml]({{application.module_name}}/openapi.yaml).
 {% endif %}
 
 ## Configuration
 
 Read more about configuring this application in [CONFIGURATION](docs/CONFIGURATION.md).
+
+## Further information
+
+For detailed information on, or assistance with, `BL_Python` please visit [uclahs-cds/BL_Python](https://github.com/uclahs-cds/BL_Python).
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 connection_string = '{{module.database.connection_string}}'
 sqlalchemy_echo = false
 
 {% endif %}
 [flask]
 app_name = '{{application.module_name}}'
 env = 'development'
-host = "127.0.0.1"
+host = "localhost"
 # FIXME this should be an int
 port = "5000"
 
 [flask.session]
 permanent = true
 lifetime = 86400
 refresh_each_request = true
```

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py` & `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from logging import Logger
 from typing import Any
 
 
 def on_create(config: dict[str, Any], log: Logger):
     """Called when an application is created."""
+    log.debug(f"Database module hook executed")
 
     config["module"]["database"] = {}
 
     connection_string = input(
         "\nEnter a database connection string.\nBy default this is `sqlite:///:memory:?check_same_thread=False`.\nRetain this default by pressing enter, or type something else.\n> "
     )
```

### Comparing `BL_Python.web-0.1.1/LICENSE.md` & `bl_python_web-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/pyproject.toml` & `bl_python_web-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,21 @@
     "Intended Audience :: Developers",
     "Development Status :: 4 - Beta",
     "Natural Language :: English"
 ]
 
 dependencies = [
     "BL_Python.programming",
+    "BL_Python.platform",
+    "BL_Python.identity",
+    "BL_Python.database",
 
     "Flask == 3.0.2",
     "flask-injector",
+    "flask-login",
     "connexion == 3.0.6",
     "connexion[uvicorn]",
     "swagger_ui_bundle",
     "python-dotenv",
     "json-logging",
     "lib_programname",
     "toml",
```

### Comparing `BL_Python.web-0.1.1/test/unit/application/test_create_app.py` & `bl_python_web-0.2.0/test/unit/application/test_create_flask_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 from os import environ
 from pathlib import Path
 from typing import cast
 
 import pytest
 from BL_Python.programming.config import AbstractConfig
 from BL_Python.programming.str import get_random_str
-from BL_Python.web.application import App, configure_blueprint_routes, configure_openapi
-from BL_Python.web.config import Config, FlaskConfig, FlaskOpenApiConfig
+from BL_Python.web.application import App, configure_blueprint_routes
+from BL_Python.web.config import Config, FlaskConfig
+from BL_Python.web.testing.create_app import (
+    CreateFlaskApp,
+    FlaskClientInjectorConfigurable,
+)
 from flask import Blueprint, Flask
 from mock import MagicMock
 from pydantic import BaseModel
 from pytest_mock import MockerFixture
 
-from ..create_app import CreateApp, FlaskClientInjectorConfigurable
 
-
-class TestCreateApp(CreateApp):
-    # TODO extend blueprint and openapi tests to cover each relevant config attribute
-    def test__configure_blueprint_routes__requires_flask_config(self):
+class TestCreateFlaskApp(CreateFlaskApp):
+    def test__CreateFlaskApp__configure_blueprint_routes__requires_flask_config(self):
         with pytest.raises(
             Exception,
             match=r"^Flask configuration is empty\. Review the `flask` section of your application's `config\.toml`\.$",
         ):
             _ = configure_blueprint_routes(Config())
 
-    def test__configure_blueprint_routes__creates_flask_app_using_config(
+    def test__CreateFlaskApp__configure_blueprint_routes__creates_flask_app_using_config(
         self, mocker: MockerFixture
     ):
+        _ = mocker.patch("BL_Python.web.application.json_logging")
         flask_mock = mocker.patch("BL_Python.web.application.Flask")
 
-        app_name = f"{TestCreateApp.test__configure_blueprint_routes__creates_flask_app_using_config.__name__}-app_name"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__configure_blueprint_routes__creates_flask_app_using_config.__name__}-app_name"
 
-        with pytest.raises(
-            RuntimeError, match=r"^app is not a valid flask.app.Flask app instance$"
-        ):
-            _ = configure_blueprint_routes(Config(flask=FlaskConfig(app_name=app_name)))
+        _ = configure_blueprint_routes(Config(flask=FlaskConfig(app_name=app_name)))
 
         flask_mock.assert_called_with(app_name)
 
     @pytest.mark.parametrize("filename", ["foo", "foo.py", "__main__.py"])
-    def test__configure_blueprint_routes__when_discovering_blueprints_ignores_directories_in_path(
+    def test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_ignores_directories_in_path(
         self, filename: str, mocker: MockerFixture
     ):
         mocker.stop(
             self._automatic_mocks["BL_Python.web.application._import_blueprint_modules"]
         )
 
         spec_lookup_mock = mocker.patch("importlib.util.spec_from_file_location")
@@ -52,15 +51,15 @@
             is_file=MagicMock(
                 # fakes a directory
                 return_value=False
             )
         )
         type(glob_item_mock).name = filename
 
-        app_name = f"{TestCreateApp.test__configure_blueprint_routes__when_discovering_blueprints_ignores_directories_in_path.__name__}-app_name"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_ignores_directories_in_path.__name__}-app_name"
 
         _path = Path
         _ = mocker.patch(
             "pathlib.Path",
             return_value=MagicMock(
                 glob=MagicMock(return_value=[glob_item_mock]),
             ),
@@ -88,15 +87,15 @@
             (True, "foo"),
             (True, "foo.py"),
             (True, "__main__.py"),
             (True, "__init__.py"),
             (False, "__init__.py"),
         ],
     )
-    def test__configure_blueprint_routes__when_discovering_blueprints_registers_python_files_and_modules(
+    def test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_registers_python_files_and_modules(
         self, is_file: bool, filename: str, mocker: MockerFixture
     ):
         mocker.stop(
             self._automatic_mocks["BL_Python.web.application._import_blueprint_modules"]
         )
 
         glob_item_mock = MagicMock(
@@ -106,15 +105,15 @@
             )
         )
         type(glob_item_mock).name = filename
 
         spec_lookup_mock = mocker.patch("importlib.util.spec_from_file_location")
         _ = mocker.patch("importlib.util.module_from_spec")
 
-        app_name = f"{TestCreateApp.test__configure_blueprint_routes__when_discovering_blueprints_registers_python_files_and_modules.__name__}-app_name"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_registers_python_files_and_modules.__name__}-app_name"
 
         _ = mocker.patch(
             "pathlib.Path",
             return_value=MagicMock(
                 glob=MagicMock(return_value=[glob_item_mock]),
             ),
         )
@@ -142,15 +141,15 @@
             (True, "foo"),
             (True, "foo.py"),
             (True, "__main__.py"),
             (True, "__init__.py"),
             (False, "__init__.py"),
         ],
     )
-    def test__configure_blueprint_routes__when_discovering_blueprints_registers_blueprint_modules(
+    def test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_registers_blueprint_modules(
         self, is_file: bool, filename: str, mocker: MockerFixture
     ):
         mocker.stop(
             self._automatic_mocks["BL_Python.web.application._import_blueprint_modules"]
         )
         _ = mocker.patch("importlib.util.spec_from_file_location")
         _ = mocker.patch("flask.app.Flask.register_blueprint")
@@ -165,15 +164,15 @@
 
         blueprint = Blueprint("foo_blueprint", "")
         _ = mocker.patch(
             "importlib.util.module_from_spec",
             return_value=MagicMock(foo_blueprint=blueprint),
         )
 
-        app_name = f"{TestCreateApp.test__configure_blueprint_routes__when_discovering_blueprints_registers_blueprint_modules.__name__}-app_name"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_registers_blueprint_modules.__name__}-app_name"
 
         _path = Path
         _ = mocker.patch(
             "pathlib.Path",
             return_value=MagicMock(
                 glob=MagicMock(return_value=[glob_item_mock, glob_item_mock]),
             ),
@@ -191,15 +190,15 @@
             # either through automatic cleanup, `with` statements,
             # or `mocker.stop`.
             pathlib.Path = _path
 
         assert cast(MagicMock, flask_app.register_blueprint).call_count == 2
         cast(MagicMock, flask_app.register_blueprint).assert_called_with(blueprint)
 
-    def test__configure_blueprint_routes__when_discovering_blueprints_stops_when_module_load_fails(
+    def test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_stops_when_module_load_fails(
         self, mocker: MockerFixture
     ):
         mocker.stop(
             self._automatic_mocks["BL_Python.web.application._import_blueprint_modules"]
         )
 
         glob_item_mock = MagicMock(
@@ -215,15 +214,15 @@
         _path = Path
         _ = mocker.patch(
             "pathlib.Path",
             return_value=MagicMock(
                 glob=MagicMock(return_value=[glob_item_mock]),
             ),
         )
-        app_name = f"{TestCreateApp.test__configure_blueprint_routes__when_discovering_blueprints_stops_when_module_load_fails.__name__}-app_name"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__configure_blueprint_routes__when_discovering_blueprints_stops_when_module_load_fails.__name__}-app_name"
 
         with pytest.raises(
             Exception,
             match=rf"^Module cannot be created from path {glob_item_mock}$",
         ):
             try:
                 _ = configure_blueprint_routes(
@@ -234,71 +233,51 @@
                 )
             finally:
                 # mocker doesn't appear to restore pathlib.Path correctly
                 # either through automatic cleanup, `with` statements,
                 # or `mocker.stop`.
                 pathlib.Path = _path
 
-    def test__configure_openapi__requires_flask_config(self):
-        with pytest.raises(
-            Exception,
-            match=r"^OpenAPI configuration is empty\. Review the `openapi` section of your application's `config\.toml`\.$",
-        ):
-            _ = configure_openapi(Config())
-
-    def test__configure_openapi__creates_flask_app_using_config(
-        self, mocker: MockerFixture
-    ):
-        connexion_mock = mocker.patch("BL_Python.web.application.FlaskApp")
-
-        app_name = f"{TestCreateApp.test__configure_openapi__creates_flask_app_using_config.__name__}-app_name"
-        spec_path = "."
-
-        with pytest.raises(
-            RuntimeError,
-            match=r"^app is not a valid connexion.app.Connexion app instance$",
-        ):
-            _ = configure_openapi(
-                Config(
-                    flask=FlaskConfig(
-                        app_name=app_name,
-                        openapi=FlaskOpenApiConfig(spec_path=spec_path),
-                    )
-                )
-            )
-
-        connexion_mock.assert_called_with(app_name, specification_dir=spec_path)
-
-    def test__create_app__requires_flask_config(
+    def test__CreateFlaskApp__create_app__requires_flask_config(
         self, flask_client_configurable: FlaskClientInjectorConfigurable
     ):
         with pytest.raises(
             Exception,
             match=r"^You must set \[flask\] in the application configuration\.$",
         ):
-            _ = flask_client_configurable(Config())
+            _ = next(flask_client_configurable(Config()))
 
-    def test__create_app__loads_config_from_toml(
+    def test__CreateFlaskApp__create_app__loads_config_from_toml(
         self, basic_config: Config, mocker: MockerFixture
     ):
+        _ = mocker.patch(
+            "BL_Python.web.application.SSMParameters",
+            return_value=MagicMock(load_config=MagicMock(return_value=None)),
+        )
         load_config_mock = mocker.patch(
             "BL_Python.web.application.load_config", return_value=basic_config
         )
 
-        toml_filename = f"{TestCreateApp.test__create_app__loads_config_from_toml.__name__}-config.toml"
+        toml_filename = f"{TestCreateFlaskApp.test__CreateFlaskApp__create_app__loads_config_from_toml.__name__}-config.toml"
         _ = App[Flask].create(config_filename=toml_filename)
         assert load_config_mock.called
         assert load_config_mock.call_args and load_config_mock.call_args[0]
         assert load_config_mock.call_args[0][1] == toml_filename
 
-    def test__create_app__uses_custom_config_types(self, mocker: MockerFixture):
-        toml_filename = f"{TestCreateApp.test__create_app__uses_custom_config_types.__name__}-config.toml"
+    def test__CreateFlaskApp__create_app__uses_custom_config_types(
+        self, mocker: MockerFixture
+    ):
+        _ = mocker.patch(
+            "BL_Python.web.application.SSMParameters",
+            return_value=MagicMock(load_config=MagicMock(return_value=None)),
+        )
+        toml_filename = f"{TestCreateFlaskApp.test__CreateFlaskApp__create_app__uses_custom_config_types.__name__}-config.toml"
         toml_load_result = {
             "flask": {
-                "app_name": f"{TestCreateApp.test__create_app__uses_custom_config_types.__name__}-app_name"
+                "app_name": f"{TestCreateFlaskApp.test__CreateFlaskApp__create_app__uses_custom_config_types.__name__}-app_name"
             },
             "custom": {"foo": get_random_str(k=26)},
         }
 
         _ = mocker.patch("toml.load", return_value=toml_load_result)
 
         class CustomConfig(BaseModel, AbstractConfig):
@@ -316,22 +295,26 @@
     @pytest.mark.parametrize(
         "envvar_name,config_var_name,var_value",
         [
             ("FLASK_APP", "app_name", "foobar"),
             ("FLASK_ENV", "env", "barfoo"),
         ],
     )
-    def test__create_app__updates_flask_config_from_envvars(
+    def test__CreateFlaskApp__create_app__updates_flask_config_from_envvars(
         self,
         envvar_name: str,
         config_var_name: str,
         var_value: str,
         basic_config: Config,
         mocker: MockerFixture,
     ):
+        _ = mocker.patch(
+            "BL_Python.web.application.SSMParameters",
+            return_value=MagicMock(load_config=MagicMock(return_value=None)),
+        )
         object.__setattr__(basic_config.flask, config_var_name, var_value)
 
         environ.update({envvar_name: var_value})
         _ = mocker.patch(
             "BL_Python.web.application.load_config", return_value=basic_config
         )
         _ = App[Flask].create()
@@ -344,22 +327,26 @@
             ("FLASK_APP", None, "foobar", False),
             ("FLASK_ENV", None, "barfoo", False),
             (None, "app_name", "foobar", False),
             (None, "app_name", "", True),
             (None, "env", "barfoo", False),
         ],
     )
-    def test__create_app__requires_application_name(
+    def test__CreateFlaskApp__create_app__requires_application_name(
         self,
         envvar_name: str | None,
         config_var_name: str | None,
         var_value: str,
         should_fail: bool,
         mocker: MockerFixture,
     ):
+        _ = mocker.patch(
+            "BL_Python.web.application.SSMParameters",
+            return_value=MagicMock(load_config=MagicMock(return_value=None)),
+        )
         environ.update({"FLASK_APP": "", "FLASK_ENV": ""})
 
         if envvar_name is not None:
             environ.update({envvar_name: var_value})
 
         toml_load_result = {}
         if config_var_name is not None:
@@ -369,42 +356,29 @@
 
         if should_fail:
             with pytest.raises(Exception):
                 _ = App[Flask].create()
         else:
             _ = App[Flask].create()
 
-    @pytest.mark.parametrize("type", ["basic", "openapi"])
-    def test__create_app__configures_appropriate_app_type_based_on_config(
-        self, type: str, mocker: MockerFixture
+    def test__CreateFlaskApp__create_app__configures_appropriate_app_type_based_on_config(
+        self, mocker: MockerFixture
     ):
-        toml_filename = f"{TestCreateApp.test__create_app__configures_appropriate_app_type_based_on_config.__name__}-config.toml"
-        app_name = f"{TestCreateApp.test__create_app__configures_appropriate_app_type_based_on_config.__name__}-app_name"
+        toml_filename = f"{TestCreateFlaskApp.test__CreateFlaskApp__create_app__configures_appropriate_app_type_based_on_config.__name__}-config.toml"
+        app_name = f"{TestCreateFlaskApp.test__CreateFlaskApp__create_app__configures_appropriate_app_type_based_on_config.__name__}-app_name"
+        _ = mocker.patch(
+            "BL_Python.web.application.SSMParameters",
+            return_value=MagicMock(load_config=MagicMock(return_value=None)),
+        )
         _ = mocker.patch("BL_Python.web.application.register_error_handlers")
         _ = mocker.patch("BL_Python.web.application.register_api_request_handlers")
         _ = mocker.patch("BL_Python.web.application.register_api_response_handlers")
         _ = mocker.patch("BL_Python.web.application.configure_dependencies")
 
-        if type == "basic":
-            configure_method_mock = mocker.patch(
-                "BL_Python.web.application.configure_blueprint_routes"
-            )
-            config = Config(flask=FlaskConfig(app_name=app_name))
-            _ = mocker.patch(
-                "BL_Python.web.application.load_config", return_value=config
-            )
-            _ = App[Flask].create(config_filename=toml_filename)
-        elif type == "openapi":
-            configure_method_mock = mocker.patch(
-                "BL_Python.web.application.configure_openapi"
-            )
-            config = Config(
-                flask=FlaskConfig(app_name=app_name, openapi=FlaskOpenApiConfig())
-            )
-            _ = mocker.patch(
-                "BL_Python.web.application.load_config", return_value=config
-            )
-            _ = App[Flask].create(config_filename=toml_filename)
-        else:
-            raise Exception(f"Invalid test parameter value '{type}'.")
+        configure_method_mock = mocker.patch(
+            "BL_Python.web.application.configure_blueprint_routes"
+        )
+        config = Config(flask=FlaskConfig(app_name=app_name))
+        _ = mocker.patch("BL_Python.web.application.load_config", return_value=config)
+        _ = App[Flask].create(config_filename=toml_filename)
 
         configure_method_mock.assert_called_once_with(config)
```

### Comparing `BL_Python.web-0.1.1/test/unit/encryption/test_encryption.py` & `bl_python_web-0.2.0/test/unit/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_api_request_handlers.py` & `bl_python_web-0.2.0/test/unit/middleware/test_api_request_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from typing import Any, cast
 
 import pytest
 from BL_Python.web.middleware import register_api_request_handlers
 from BL_Python.web.middleware.consts import INCOMING_REQUEST_MESSAGE
+from BL_Python.web.testing.create_app import CreateFlaskApp, FlaskClientInjector
 from pytest import LogCaptureFixture
 from pytest_mock import MockerFixture
 
-from ..create_app import CreateApp, FlaskClientInjector
 
-
-class TestApiRequestHandlers(CreateApp):
+class TestApiRequestHandlers(CreateFlaskApp):
     def test__register_api_request_handlers__binds_flask_before_request(
         self, flask_client: FlaskClientInjector, mocker: MockerFixture
     ):
         flask_before_request_mock = mocker.patch(
             "flask.sansio.scaffold.Scaffold.before_request"
         )
```

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_api_response_handlers.py` & `bl_python_web-0.2.0/test/unit/middleware/test_api_response_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,25 @@
     CONTENT_SECURITY_POLICY_HEADER,
     CORS_ACCESS_CONTROL_ALLOW_CREDENTIALS_HEADER,
     CORS_ACCESS_CONTROL_ALLOW_METHODS_HEADER,
     CORS_ACCESS_CONTROL_ALLOW_ORIGIN_HEADER,
     OUTGOING_RESPONSE_MESSAGE,
 )
 from BL_Python.web.middleware.flask import bind_requesthandler
+from BL_Python.web.testing.create_app import (
+    CreateFlaskApp,
+    FlaskClientInjector,
+    FlaskClientInjectorConfigurable,
+)
 from flask import Flask, Response
 from pytest import LogCaptureFixture
 from pytest_mock import MockerFixture
 
-from ..create_app import CreateApp, FlaskClientInjector, FlaskClientInjectorConfigurable
-
 
-class TestApiResponseHandlers(CreateApp):
+class TestApiResponseHandlers(CreateFlaskApp):
     def test__register_api_response_handlers__binds_flask_before_request(
         self, flask_client: FlaskClientInjector, mocker: MockerFixture
     ):
         flask_before_request_mock = mocker.patch(
             "flask.sansio.scaffold.Scaffold.before_request"
         )
 
@@ -34,15 +37,15 @@
     def test__wrap_all_api_responses__sets_CSP_header(
         self,
         flask_client_configurable: FlaskClientInjectorConfigurable,
         basic_config: Config,
     ):
         csp_value = "default-src 'self' cdn.example.com;"
         basic_config.web.security.csp = csp_value
-        flask_client = flask_client_configurable(basic_config)
+        flask_client = next(flask_client_configurable(basic_config))
         response = flask_client.client.get("/")
         header_value = response.headers.get(CONTENT_SECURITY_POLICY_HEADER)
         assert header_value == csp_value
 
     @pytest.mark.parametrize(
         "header,value,config_attribute_name",
         [
@@ -70,15 +73,15 @@
         header: str,
         value: str,
         config_attribute_name: str,
         flask_client_configurable: FlaskClientInjectorConfigurable,
         basic_config: Config,
     ):
         setattr(basic_config.web.security.cors, config_attribute_name, value)
-        flask_client = flask_client_configurable(basic_config)
+        flask_client = next(flask_client_configurable(basic_config))
         response = flask_client.client.get("/")
         header_value = response.headers.get(header)
         assert header_value == ",".join(value) if isinstance(value, list) else value
 
     def test__log_all_api_responses__logs_response_information(
         self,
         flask_client: FlaskClientInjector,
```

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_dependency_injection.py` & `bl_python_web-0.2.0/test/unit/middleware/test_dependency_injection.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from mock import MagicMock
 
 
 def test__AppModule__binds_extra_dependencies():
     flask_mock = MagicMock(spec=Flask)
     flask_mock.name = f"{test__AppModule__binds_extra_dependencies.__name__}-app_name"
     flask_mock.config = {}
-    flask_mock.configure_mock()
     extra_dependency_mock = MagicMock()
 
     class TestDependencyType: ...
 
     app_module = AppModule(flask_mock, (TestDependencyType, extra_dependency_mock))
 
     injector = Injector(app_module)
```

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_error_handlers.py` & `bl_python_web-0.2.0/test/unit/middleware/test_error_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from json.decoder import JSONDecoder
 from typing import Callable
 
 import pytest
+from BL_Python.web.testing.create_app import CreateFlaskApp, FlaskClientInjector
 from flask import Response, abort
 from werkzeug.exceptions import Unauthorized
 
-from ..create_app import CreateApp, FlaskClientInjector
-
 
 def _raise_custom_unauthorized_exception():
     response = Response("Unauthorized.", 401)
     raise Unauthorized(response.data, response)
 
 
-class TestErrorHandlers(CreateApp):
+class TestErrorHandlers(CreateFlaskApp):
     @pytest.mark.parametrize(
         "expected_status_code,expected_status_msg,failure_lambda",
         [
             (
                 500,
                 "Internal Server Error",
                 lambda: 1 / 0,  # 1/0 to raise an exception (any exception)
```

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_flask_middleware.py` & `bl_python_web-0.2.0/test/unit/middleware/test_flask_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,51 +6,50 @@
 from BL_Python.web.config import Config
 from BL_Python.web.middleware import bind_errorhandler
 from BL_Python.web.middleware.consts import CORRELATION_ID_HEADER
 from BL_Python.web.middleware.flask import (
     _get_correlation_id,  # pyright: ignore[reportPrivateUsage]
 )
 from BL_Python.web.middleware.flask import bind_requesthandler
-from flask import Flask, Response, abort
-from mock import MagicMock
-from pytest_mock import MockerFixture
-from werkzeug.exceptions import BadRequest, HTTPException, Unauthorized
-
-from ..create_app import (
-    CreateApp,
+from BL_Python.web.testing.create_app import (
+    CreateFlaskApp,
     FlaskClientInjector,
     FlaskClientInjectorConfigurable,
     RequestConfigurable,
 )
+from flask import Flask, Response, abort
+from mock import MagicMock
+from pytest_mock import MockerFixture
+from werkzeug.exceptions import BadRequest, HTTPException, Unauthorized
 
 
-class TestFlaskMiddleware(CreateApp):
+class TestFlaskMiddleware(CreateFlaskApp):
     @pytest.mark.parametrize("format", ["plaintext", "JSON"])
     def test___register_api_response_handlers__sets_correlation_id_response_header_when_not_set_in_request_header(
         self,
         format: Literal["plaintext", "JSON"],
         flask_client_configurable: FlaskClientInjectorConfigurable,
         basic_config: Config,
     ):
         basic_config.logging.format = format
-        flask_client = flask_client_configurable(basic_config)
+        flask_client = next(flask_client_configurable(basic_config))
         response = flask_client.client.get("/")
 
         assert response.headers[CORRELATION_ID_HEADER]
         _ = uuid.UUID(response.headers[CORRELATION_ID_HEADER])
 
     @pytest.mark.parametrize("format", ["plaintext", "JSON"])
     def test___register_api_response_handlers__sets_correlation_id_response_header_when_set_in_request_header(
         self,
         format: Literal["plaintext", "JSON"],
         flask_client_configurable: FlaskClientInjectorConfigurable,
         basic_config: Config,
     ):
         basic_config.logging.format = format
-        flask_client = flask_client_configurable(basic_config)
+        flask_client = next(flask_client_configurable(basic_config))
         correlation_id = str(uuid4())
         response = flask_client.client.get(
             "/", headers={CORRELATION_ID_HEADER: correlation_id}
         )
 
         assert response.headers[CORRELATION_ID_HEADER] == correlation_id
 
@@ -159,15 +158,15 @@
         failure_lambda: Callable[[], Response],
     ):
         application_errorhandler_mock = MagicMock()
         with Flask("foo").test_client() as test_client:
             _ = bind_errorhandler(test_client.application, code_or_exception_type)(
                 application_errorhandler_mock
             )
-            # this probably doesn't need to be done w/ connexion
+
             _ = test_client.application.route("/")(failure_lambda)
 
             _ = test_client.get("/")
 
         assert application_errorhandler_mock.called
         assert isinstance(
             application_errorhandler_mock.call_args[0][0], expected_exception_type
```

### Comparing `BL_Python.web-0.1.1/test/unit/middleware/test_openapi_middleware.py` & `bl_python_web-0.2.0/test/unit/middleware/test_openapi_middleware.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import uuid
 from typing import Literal
 
 import pytest
-from BL_Python.web.application import OpenAPIAppInjector
+from BL_Python.identity.config import Config as RootSSOConfig
+from BL_Python.identity.config import SSOConfig
+from BL_Python.platform.dependency_injection import UserLoaderModule
+from BL_Python.platform.identity import Role, User
+from BL_Python.programming.config import AbstractConfig
+from BL_Python.web.application import OpenAPIAppResult
 from BL_Python.web.config import Config
 from BL_Python.web.middleware import bind_errorhandler
 from BL_Python.web.middleware.consts import CORRELATION_ID_HEADER
 from BL_Python.web.middleware.flask import (
     _get_correlation_id,  # pyright: ignore[reportPrivateUsage]
 )
 from BL_Python.web.middleware.flask import bind_requesthandler
+from BL_Python.web.testing.create_app import (
+    CreateOpenAPIApp,
+    OpenAPIClientInjectorConfigurable,
+    OpenAPIMockController,
+    RequestConfigurable,
+)
 from connexion import FlaskApp
 from flask import Flask, abort
+from injector import Module
 from mock import MagicMock
 from pytest_mock import MockerFixture
 from werkzeug.exceptions import BadRequest, HTTPException, Unauthorized
 
-from ..create_app import (
-    CreateApp,
-    OpenAPIClientInjectorConfigurable,
-    OpenAPIMockController,
-    RequestConfigurable,
-)
-
 
-class TestOpenAPIMiddleware(CreateApp):
+class TestOpenAPIMiddleware(CreateOpenAPIApp):
     @pytest.mark.parametrize("format", ["plaintext", "JSON"])
     def test___register_api_response_handlers__sets_correlation_id_response_header_when_not_set_in_request_header(
         self,
         format: Literal["plaintext", "JSON"],
         openapi_client_configurable: OpenAPIClientInjectorConfigurable,
         openapi_config: Config,
         openapi_mock_controller: OpenAPIMockController,
     ):
         openapi_config.logging.format = format
         openapi_mock_controller.begin()
-        flask_client = openapi_client_configurable(openapi_config)
+        flask_client = next(openapi_client_configurable(openapi_config))
 
         response = flask_client.client.get("/")
 
         assert response.headers[CORRELATION_ID_HEADER]
         _ = uuid.UUID(response.headers[CORRELATION_ID_HEADER])
 
     @pytest.mark.parametrize("format", ["plaintext", "JSON"])
@@ -48,15 +53,15 @@
         format: Literal["plaintext", "JSON"],
         openapi_client_configurable: OpenAPIClientInjectorConfigurable,
         openapi_config: Config,
         openapi_mock_controller: OpenAPIMockController,
     ):
         openapi_config.logging.format = format
         openapi_mock_controller.begin()
-        flask_client = openapi_client_configurable(openapi_config)
+        flask_client = next(openapi_client_configurable(openapi_config))
         correlation_id = str(uuid.uuid4())
         response = flask_client.client.get(
             "/", headers={CORRELATION_ID_HEADER: correlation_id}
         )
 
         assert response.headers[CORRELATION_ID_HEADER] == correlation_id
 
@@ -67,15 +72,15 @@
         openapi_client_configurable: OpenAPIClientInjectorConfigurable,
         openapi_config: Config,
         openapi_mock_controller: OpenAPIMockController,
     ):
         openapi_config.logging.format = format
         correlation_id = "abc123"
         openapi_mock_controller.begin()
-        flask_client = openapi_client_configurable(openapi_config)
+        flask_client = next(openapi_client_configurable(openapi_config))
 
         response = flask_client.client.get(
             "/", headers={CORRELATION_ID_HEADER: correlation_id}
         )
 
         assert response.status_code == 500
 
@@ -165,27 +170,26 @@
         "code_or_exception,openapi_mock_controller",
         [(Exception, lambda: 1), (HTTPException, lambda: 1), (401, lambda: 1)],
         indirect=["openapi_mock_controller"],
     )
     def test__bind_errorhandler__binds_flask_errorhandler(
         self,
         code_or_exception: type[Exception] | int,
-        # openapi_client: OpenAPIClientInjector,
         openapi_config: Config,
         openapi_client_configurable: OpenAPIClientInjectorConfigurable,
         openapi_mock_controller: OpenAPIMockController,
         mocker: MockerFixture,
     ):
         flask_errorhandler_mock = mocker.patch("flask.Flask.errorhandler")
 
-        def app_init_hook(app: OpenAPIAppInjector):
-            _ = bind_errorhandler(app.app, code_or_exception)
+        def client_init_hook(app: OpenAPIAppResult):
+            _ = bind_errorhandler(app.app_injector.app, code_or_exception)
 
         openapi_mock_controller.begin()
-        _ = openapi_client_configurable(openapi_config, app_init_hook)
+        _ = next(openapi_client_configurable(openapi_config, client_init_hook))
 
         flask_errorhandler_mock.assert_called_with(code_or_exception)
 
     @pytest.mark.parametrize(
         "code_or_exception_type,expected_exception_type,openapi_mock_controller",
         [
             (
@@ -217,7 +221,55 @@
 
         _ = flask_client.get("/", headers={"Host": "localhost:5000"})
 
         assert application_errorhandler_mock.called
         assert isinstance(
             application_errorhandler_mock.call_args[0][0], expected_exception_type
         )
+
+    # FIXME just a temporary test as an example set up for testing SAML2
+    def test__SAML2Middleware__something(
+        self,
+        openapi_config: Config,
+        openapi_client_configurable: OpenAPIClientInjectorConfigurable,
+        openapi_mock_controller: OpenAPIMockController,
+        mocker: MockerFixture,
+    ):
+        def app_init_hook(
+            application_configs: list[type[AbstractConfig]],
+            application_modules: list[Module | type[Module]],
+        ):
+            application_modules.append(
+                UserLoaderModule(
+                    loader=User,  # pyright: ignore[reportArgumentType]
+                    roles=Role,  # pyright: ignore[reportArgumentType]
+                    user_table=MagicMock(),  # pyright: ignore[reportArgumentType]
+                    role_table=MagicMock(),  # pyright: ignore[reportArgumentType]
+                    bases=[],
+                )
+            )
+
+        def client_init_hook(app: OpenAPIAppResult):
+            app.app_injector.flask_injector.injector.binder.bind(
+                RootSSOConfig,
+                to=RootSSOConfig(
+                    sso=SSOConfig(
+                        protocol="SAML2",
+                        settings={
+                            "relay_state": "http://localhost:5000/sso/redir",
+                            "metadata_url": "http://example.org",
+                            "metadata": "<xml />",
+                        },
+                    )
+                ),
+            )
+
+        openapi_mock_controller.begin()
+        app = next(
+            openapi_client_configurable(openapi_config, client_init_hook, app_init_hook)
+        )
+
+        response = app.client.get("/saml/logout")
+
+        # 401 for now because no real auth is configured.
+        # if SSO was broken, 500 would return
+        assert response.status_code == 401
```

### Comparing `BL_Python.web-0.1.1/test/unit/scaffolding/test_scaffolding.py` & `bl_python_web-0.2.0/test/unit/scaffolding/test_scaffolding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
+import re
 from dataclasses import asdict
 from typing import Any, cast
 
 import pytest
 from BL_Python.web.scaffolding.__main__ import ScaffolderCli, scaffold
 from BL_Python.web.scaffolding.scaffolder import (
     Operation,
+    ScaffoldConfig,
     ScaffoldEndpoint,
+    Scaffolder,
     ScaffoldModule,
 )
 from pytest import CaptureFixture
 from pytest_mock import MockerFixture
 
 # pyright: reportPrivateUsage=false
 
@@ -184,40 +187,30 @@
 @pytest.mark.parametrize("mode", ["create", "modify"])
 def test__parse_args__disallows_duplicated_endpoint_names(
     mode: str, capsys: CaptureFixture[str]
 ):
     with pytest.raises(SystemExit) as e:
         # foo-bar and foo_bar are normalized and are equivalent.
         # no need to duplicate the name normalization tests; just use the exact values here
-        _ = ScaffolderCli()._parse_args(
-            [mode, "-n", "test", "-e", "foo", "-e", "foo_bar", "-e", "foo-bar"]
-        )
-        # T
+        # fmt: off
+        _ = ScaffolderCli()._parse_args([mode, "-n", "test", "-e", "foo", "-e", "foo_bar", "-e", "foo-bar"])
+        # fmt: on
     captured = capsys.readouterr()
     assert e.value.code == 2
     assert (
         f"{mode}: error: argument -e: The ['-e'] argument does not allow duplicate values. The value `foo-bar` duplicates the value `foo_bar`."
         in captured.err
     )
 
 
 @pytest.mark.parametrize("mode", ["create", "modify"])
-def test__parse_args__disallows_endpoints_with_same_name_as_application(
-    mode: str, capsys: CaptureFixture[str]
-):
-    with pytest.raises(SystemExit) as e:
-        # foo-bar and foo_bar are normalized and are equivalent.
-        # no need to duplicate the name normalization tests; just use the exact values here
-        _ = ScaffolderCli()._parse_args([mode, "-n", "foo-bar", "-e", "foo_bar"])
-    captured = capsys.readouterr()
-    assert e.value.code == 2
-    assert (
-        f"{mode}: error: argument -e: The ['-e'] argument cannot be equivalent to the `name` argument. The value `foo_bar` is equivalent to the value `foo-bar`."
-        in captured.err
-    )
+def test__parse_args__allows_endpoints_with_same_name_as_application(mode: str):
+    # foo-bar and foo_bar are normalized and are equivalent.
+    # no need to duplicate the name normalization tests; just use the exact values here
+    _ = ScaffolderCli()._parse_args([mode, "-n", "foo-bar", "-e", "foo_bar"])
 
 
 @pytest.mark.parametrize("mode", ["create", "modify"])
 def test__parse_args__uses_application_name_for_endpoint_if_no_endpoints_given(
     mode: str,
 ):
     args = ScaffolderCli()._parse_args([mode, "-n", "test"])
@@ -284,26 +277,31 @@
 ):
     args = ScaffolderCli()._parse_args([mode, "-n", "test", "-m", module_name])
 
     assert args.modules is not None
     assert module_name in args.modules
 
 
-@pytest.mark.parametrize("mode,module_name", [("create", "DATABASE")])
+@pytest.mark.parametrize(
+    "mode,module_name", [("create", "DATABASE"), ("create", "TEST")]
+)
 def test__parse_args__does_not_lowercase_modules(
     mode: str, module_name: str, capsys: CaptureFixture[str]
 ):
     with pytest.raises(SystemExit) as e:
         _ = ScaffolderCli()._parse_args([mode, "-n", "test", "-m", module_name])
 
     captured = capsys.readouterr()
     assert e.value.code == 2
     assert (
-        f"{mode}: error: argument -m: invalid choice: 'DATABASE' (choose from 'database')"
-        in captured.err
+        re.search(
+            rf"{mode}: error: argument -m: invalid choice: '{module_name}' \(choose from.+'{module_name.lower()}'",
+            captured.err,
+        )
+        is not None
     )
 
 
 @pytest.mark.parametrize("mode", ["create", "modify"])
 def test__parse_args__supports_setting_explicit_output_directory(mode: str):
     args = ScaffolderCli()._parse_args([mode, "-n", "test", "-o", "output_dir"])
 
@@ -471,7 +469,91 @@
         module.module_name
         for module in cast(
             list[ScaffoldModule], config_mock.call_args.kwargs["modules"]
         )
     ]
 
     assert "database" in module_names
+
+
+def test__scaffold__create_mode_database_module_configures_database(
+    mocker: MockerFixture,
+):
+    # TODO refactor Scaffolder so all these mocks don't need to happen
+    _ = mocker.patch("builtins.input", return_value="Y")
+    _ = mocker.patch("BL_Python.web.scaffolding.scaffolder.BaseLoader")
+    _ = mocker.patch("BL_Python.web.scaffolding.scaffolder.Environment")
+    _ = mocker.patch("BL_Python.web.scaffolding.scaffolder.PackageLoader")
+    _ = mocker.patch("BL_Python.web.scaffolding.scaffolder.Template")
+    _ = mocker.patch(
+        "BL_Python.web.scaffolding.scaffolder.Scaffolder._create_directory"
+    )
+    _ = mocker.patch(
+        "BL_Python.web.scaffolding.scaffolder.Scaffolder._scaffold_directory"
+    )
+    _ = mocker.patch(
+        "BL_Python.web.scaffolding.scaffolder.Scaffolder._scaffold_endpoints"
+    )
+    _ = mocker.patch(
+        "BL_Python.web.scaffolding.scaffolder.Scaffolder._check_scaffolded_application_exists",
+        return_value=False,
+    )
+    module_hook_mock = mocker.patch(
+        "BL_Python.web.scaffolding.scaffolder.Scaffolder._execute_module_hooks"
+    )
+
+    argv_values = ["create", "-n", "test", "-m", "database", "-o", "/dev/null"]
+
+    scaffold(argv_values)
+
+    pass
+    module_hook_mock.assert_called_once_with(
+        "scaffolding/templates/optional/{{application.module_name}}/modules/database"
+    )
+
+
+@pytest.fixture
+def scaffold_config():
+    return ScaffoldConfig(
+        output_directory="/dev/null",
+        application=Operation(name="foo"),
+        template_type="basic",
+        modules=[ScaffoldModule(module_name="database")],
+    )
+
+
+def test__database_module__on_create__asks_for_connection_string(
+    scaffold_config: ScaffoldConfig,
+    mocker: MockerFixture,
+):
+    input_mock = mocker.patch("builtins.input", return_value="")
+
+    mock_log = mocker.patch("logging.Logger", spec=logging.Logger)
+    scaffolder = Scaffolder(config=scaffold_config, log=mock_log)
+    scaffolder._execute_module_hooks(
+        "scaffolding/templates/optional/{{application.module_name}}/modules/database",
+    )
+
+    input_mock.assert_called()
+    assert [
+        arg
+        for arg in input_mock.call_args.args
+        if "Enter a database connection string" in arg
+    ]
+
+
+def test__database_module__on_create__uses_user_input_connection_string(
+    scaffold_config: ScaffoldConfig,
+    mocker: MockerFixture,
+):
+    _ = mocker.patch("builtins.input", return_value="sqlite:///dev/null")
+
+    mock_log = mocker.patch("logging.Logger", spec=logging.Logger)
+    scaffolder = Scaffolder(config=scaffold_config, log=mock_log)
+    scaffolder._execute_module_hooks(
+        "scaffolding/templates/optional/{{application.module_name}}/modules/database",
+    )
+
+    assert (
+        scaffolder._config_dict["module"]["database"]["connection_string"]
+        == "sqlite:///dev/null"
+    )
```

### Comparing `BL_Python.web-0.1.1/test/unit/test_config.py` & `bl_python_web-0.2.0/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/__init__.pyi` & `bl_python_web-0.2.0/typings/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/apps/abstract.pyi` & `bl_python_web-0.2.0/typings/connexion/apps/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/apps/asynchronous.pyi` & `bl_python_web-0.2.0/typings/connexion/apps/asynchronous.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/apps/flask.pyi` & `bl_python_web-0.2.0/typings/connexion/apps/flask.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/cli.pyi` & `bl_python_web-0.2.0/typings/connexion/cli.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/datastructures.pyi` & `bl_python_web-0.2.0/typings/connexion/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/decorators/main.pyi` & `bl_python_web-0.2.0/typings/connexion/decorators/main.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/decorators/parameter.pyi` & `bl_python_web-0.2.0/typings/connexion/decorators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/decorators/response.pyi` & `bl_python_web-0.2.0/typings/connexion/decorators/response.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/exceptions.pyi` & `bl_python_web-0.2.0/typings/connexion/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/frameworks/abstract.pyi` & `bl_python_web-0.2.0/typings/connexion/frameworks/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/frameworks/flask.pyi` & `bl_python_web-0.2.0/typings/connexion/frameworks/flask.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/frameworks/starlette.pyi` & `bl_python_web-0.2.0/typings/connexion/frameworks/starlette.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/handlers.pyi` & `bl_python_web-0.2.0/typings/connexion/handlers.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/json_schema.pyi` & `bl_python_web-0.2.0/typings/connexion/json_schema.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/jsonifier.pyi` & `bl_python_web-0.2.0/typings/connexion/jsonifier.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/lifecycle.pyi` & `bl_python_web-0.2.0/typings/connexion/lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/abstract.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/context.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/context.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/exceptions.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/lifespan.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/lifespan.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/main.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/main.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/request_validation.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/request_validation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/response_validation.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/response_validation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/routing.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/routing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/security.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/server_error.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/server_error.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/middleware/swagger_ui.pyi` & `bl_python_web-0.2.0/typings/connexion/middleware/swagger_ui.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/mock.pyi` & `bl_python_web-0.2.0/typings/connexion/mock.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/operations/__init__.pyi` & `bl_python_web-0.2.0/typings/connexion/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/operations/abstract.pyi` & `bl_python_web-0.2.0/typings/connexion/operations/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/operations/openapi.pyi` & `bl_python_web-0.2.0/typings/connexion/operations/openapi.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/operations/swagger2.pyi` & `bl_python_web-0.2.0/typings/connexion/operations/swagger2.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/options.pyi` & `bl_python_web-0.2.0/typings/connexion/options.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/problem.pyi` & `bl_python_web-0.2.0/typings/connexion/problem.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/resolver.pyi` & `bl_python_web-0.2.0/typings/connexion/resolver.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/security.pyi` & `bl_python_web-0.2.0/typings/connexion/security.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/spec.pyi` & `bl_python_web-0.2.0/typings/connexion/spec.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/testing.pyi` & `bl_python_web-0.2.0/typings/connexion/testing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/types.pyi` & `bl_python_web-0.2.0/typings/connexion/types.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/uri_parsing.pyi` & `bl_python_web-0.2.0/typings/connexion/uri_parsing.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/utils.pyi` & `bl_python_web-0.2.0/typings/connexion/utils.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/validators/__init__.pyi` & `bl_python_web-0.2.0/typings/connexion/validators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/validators/abstract.pyi` & `bl_python_web-0.2.0/typings/connexion/validators/abstract.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/validators/form_data.pyi` & `bl_python_web-0.2.0/typings/connexion/validators/form_data.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/validators/json.pyi` & `bl_python_web-0.2.0/typings/connexion/validators/json.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/connexion/validators/parameter.pyi` & `bl_python_web-0.2.0/typings/connexion/validators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/__init__.pyi` & `bl_python_web-0.2.0/typings/json_logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework/connexion/__init__.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework/fastapi/implementation.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework/flask/__init__.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework/flask/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework/quart/__init__.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework/quart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework/sanic/__init__.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework/sanic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/framework_base.pyi` & `bl_python_web-0.2.0/typings/json_logging/framework_base.pyi`

 * *Files identical despite different names*

### Comparing `BL_Python.web-0.1.1/typings/json_logging/util.pyi` & `bl_python_web-0.2.0/typings/json_logging/util.pyi`

 * *Files identical despite different names*


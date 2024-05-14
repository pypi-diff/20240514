# Comparing `tmp/ansys_templates-2.0.0.tar.gz` & `tmp/ansys_templates-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-2.0.0.tar` & `ansys_templates-2.1.0.tar`

### file list

```diff
@@ -1,217 +1,229 @@
--rw-r--r--   0        0        0     1091 2024-03-05 16:27:19.268418 ansys_templates-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9568 2024-03-05 16:27:19.268418 ansys_templates-2.0.0/README.rst
--rw-r--r--   0        0        0     3174 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2266 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     4550 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3558 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      545 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3589 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2781 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      379 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
--rw-r--r--   0        0        0       11 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      105 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
--rw-r--r--   0        0        0      282 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1054 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3401 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       82 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1097 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2402 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1086 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2024-03-05 16:27:19.272418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3235 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1559 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2941 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3108 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3093 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1555 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2869 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1465 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1148 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3385 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2024-03-05 16:27:19.276418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1547 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2657 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6503 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1878 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1048 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      976 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1073 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3157 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      889 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1052 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     4178 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     6879 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/build-release.yml
--rw-r--r--   0        0        0     2044 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/release-please.yml
--rw-r--r--   0        0        0     1732 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0     1029 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/extensions.json
--rw-r--r--   0        0        0      665 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       12 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2451 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     8200 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2024-03-05 16:27:19.280418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0   299680 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
--rw-r--r--   0        0        0     3728 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      174 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/release-please-config.json
--rw-r--r--   0        0        0       40 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/release-please-manifest.json
--rw-r--r--   0        0        0    40681 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      662 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/sonar-project.properties
--rw-r--r--   0        0        0      105 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0       85 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/datamodel/README.md
--rw-r--r--   0        0        0       48 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/logic/README.md
--rw-r--r--   0        0        0       64 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/logic/assets/README.md
--rw-r--r--   0        0        0      582 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0      686 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      560 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0       66 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/method_assets/README.md
--rw-r--r--   0        0        0      263 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      945 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       18 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0   749872 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
--rw-r--r--   0        0        0     9913 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_black.png
--rw-r--r--   0        0        0    17758 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_white.png
--rw-r--r--   0        0        0       37 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0       18 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
--rw-r--r--   0        0        0     3960 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/about_page.py
--rw-r--r--   0        0        0     3811 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
--rw-r--r--   0        0        0     7674 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0      715 2024-03-05 16:27:19.284418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
--rw-r--r--   0        0        0     1351 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/collector/otel-collector-config.yaml
--rw-r--r--   0        0        0     4160 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboard.json
--rw-r--r--   0        0        0      265 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboards.yml
--rw-r--r--   0        0        0     1478 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-datasources.yml
--rw-r--r--   0        0        0      267 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana.ini
--rw-r--r--   0        0        0      482 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/loki/loki.yml
--rw-r--r--   0        0        0      412 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/prometheus/prometheus.yml
--rw-r--r--   0        0        0     2826 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/compose.yaml
--rw-r--r--   0        0        0     1567 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml
--rw-r--r--   0        0        0       20 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1554 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     7308 2024-03-05 16:27:19.288418 ansys_templates-2.0.0/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11102 1970-01-01 00:00:00.000000 ansys_templates-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9568 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/README.rst
+-rw-r--r--   0        0        0     3987 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2273 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     4557 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0     1353 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3565 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      420 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      545 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     8152 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     3301 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      866 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      379 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
+-rw-r--r--   0        0        0      184 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      105 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      282 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1054 2024-05-14 15:41:18.396408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      672 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1050 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      481 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/changelog.d/changelog_template.jinja
+-rw-r--r--   0        0        0      969 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      170 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/changelog.rst
+-rwxr-xr-x   0        0        0     4742 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      509 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/examples.rst
+-rw-r--r--   0        0        0     5082 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/getting_started/index.rst
+-rw-r--r--   0        0        0      310 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       99 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       39 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/config/vocabularies/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/config/vocabularies/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     4317 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       82 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1097 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1116 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2229 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3235 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1201 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1621 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     3124 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1619 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3291 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1618 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3276 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-14 15:41:18.400408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1617 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     3052 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1519 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1283 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3385 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1688 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2840 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     4264 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      200 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1908 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1048 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0     1038 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1208 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3157 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      889 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1150 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     4449 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0      545 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     7263 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/build-release.yml
+-rw-r--r--   0        0        0     3301 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2044 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0     1732 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0     1029 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/extensions.json
+-rw-r--r--   0        0        0      665 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       12 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2471 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      670 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      481 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/changelog.d/changelog_template.jinja
+-rw-r--r--   0        0        0      928 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2024-05-14 15:41:18.404408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0      170 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/changelog.rst
+-rw-r--r--   0        0        0     8834 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      509 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/examples.rst
+-rw-r--r--   0        0        0     5092 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/getting_started/index.rst
+-rw-r--r--   0        0        0      310 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       32 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/config/vocabularies/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/config/vocabularies/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   299680 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0     4632 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/release-please-config.json
+-rw-r--r--   0        0        0       40 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/release-please-manifest.json
+-rw-r--r--   0        0        0    42151 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      662 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/sonar-project.properties
+-rw-r--r--   0        0        0      105 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/datamodel/README.md
+-rw-r--r--   0        0        0       48 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/logic/README.md
+-rw-r--r--   0        0        0       64 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/logic/assets/README.md
+-rw-r--r--   0        0        0      582 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0      686 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      560 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0       66 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/method_assets/README.md
+-rw-r--r--   0        0        0      263 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      945 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2024-05-14 15:41:18.408408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_black.png
+-rw-r--r--   0        0        0    17758 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_white.png
+-rw-r--r--   0        0        0       37 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     3960 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/about_page.py
+-rw-r--r--   0        0        0     3811 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     7674 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      715 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0     1351 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/collector/otel-collector-config.yaml
+-rw-r--r--   0        0        0     4160 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboard.json
+-rw-r--r--   0        0        0      265 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboards.yml
+-rw-r--r--   0        0        0     1478 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-datasources.yml
+-rw-r--r--   0        0        0      267 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana.ini
+-rw-r--r--   0        0        0      482 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/loki/loki.yml
+-rw-r--r--   0        0        0      412 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/prometheus/prometheus.yml
+-rw-r--r--   0        0        0     2826 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/compose.yaml
+-rw-r--r--   0        0        0     1567 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml
+-rw-r--r--   0        0        0       20 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1554 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4042 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     7315 2024-05-14 15:41:18.412408 ansys_templates-2.1.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11097 1970-01-01 00:00:00.000000 ansys_templates-2.1.0/PKG-INFO
```

### Comparing `ansys_templates-2.0.0/LICENSES/MIT.txt` & `ansys_templates-2.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 ANSYS, Inc. and/or its affiliates.
+Copyright (c) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `ansys_templates-2.0.0/README.rst` & `ansys_templates-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/__init__.py` & `ansys_templates-2.1.0/src/ansys/templates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/__main__.py` & `ansys_templates-2.1.0/src/ansys/templates/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/cli.py` & `ansys_templates-2.1.0/src/ansys/templates/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-2.1.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/paths.py` & `ansys_templates-2.1.0/src/ansys/templates/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 name: Labeler
 on:
   pull_request:
+    # opened, reopened, and synchronize are default for pull_request
+    # edited - when PR title or body is changed
+    # labeled - when labels are added to PR
+    types: [opened, reopened, synchronize, edited, labeled]
   push:
     branches: [ main ]
     paths:
       - '../labels.yml'
 
 concurrency:
   group: {{ '${{ github.workflow }}-${{ github.ref }}' }}
@@ -79,7 +83,19 @@
           Please add one of the following labels to add this contribution to the Release Notes :point_down:
           - [bug]({{ cookiecutter.__repository_url }}/pulls?q=label%3Abug+)
           - [documentation]({{ cookiecutter.__repository_url }}/pulls?q=label%3Adocumentation+)
           - [enhancement]({{ cookiecutter.__repository_url }}/pulls?q=label%3Aenhancement+)
           - [good first issue]({{ cookiecutter.__repository_url }}/pulls?q=label%3Agood+first+issue)
           - [maintenance]({{ cookiecutter.__repository_url }}/pulls?q=label%3Amaintenance+)
           - [release]({{ cookiecutter.__repository_url }}/pulls?q=label%3Arelease+)
+
+  changelog-fragment:
+    name: "Create changelog fragment"
+    needs: [labeler]
+    permissions:
+      contents: write
+      pull-requests: write
+    runs-on: ubuntu-latest
+    steps:
+    - uses: ansys/actions/doc-changelog@v6
+      with:
+        token: {{ '${{ secrets.PYANSYS_CI_BOT_TOKEN }}' }}
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 repos:
 
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 24.4.2
   hooks:
   - id: black
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.12.0
+  rev: 5.13.2
   hooks:
   - id: isort
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
+  rev: 7.0.0
   hooks:
   - id: flake8
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.6
   hooks:
   - id: codespell
 
 - repo: https://github.com/pycqa/pydocstyle
   rev: 6.3.0
   hooks:
   - id: pydocstyle
     additional_dependencies: [toml]
     exclude: "tests/"
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
   - id: check-merge-conflict
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.22.0
+  rev: 0.28.2
   hooks:
     - id: check-github-workflows
+
+- repo: https://github.com/ansys/pre-commit-hooks
+  rev: v0.3.1
+  hooks:
+  - id: add-license-headers
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files 14% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 # Define the Ansys vocabulary
 Vocab = ANSYS
 
 [*.{md,rst}]
 
 # Apply the following styles
 BasedOnStyles = Vale, Google
+Vale.Terms = NO
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
-SPHINXOPTS    = -j auto
+SPHINXOPTS    = -j auto -W --color --keep-going
 SPHINXBUILD   = sphinx-build
 SOURCEDIR     = source
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sphinx documentation configuration file."""
+
 from datetime import datetime
 import os
 
 from ansys_sphinx_theme import get_version_match
 {%- if cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "white" %}
 from ansys_sphinx_theme import ansys_logo_white as logo
 {%- elif cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "black" %}
@@ -27,15 +28,16 @@
 copyright = f"(c) {datetime.now().year} ANSYS, Inc. All rights reserved"
 author = "ANSYS, Inc."
 {%- if cookiecutter.__template_name != "doc-project" %}
 release = version = __version__
 {%- elif cookiecutter.__template_name == "doc-project" %}
 release = version = "{{ cookiecutter.__version }}"
 {%- endif %}
-cname = os.getenv("DOCUMENTATION_CNAME", "docs.pyansys.com")
+cname = os.getenv("DOCUMENTATION_CNAME", "{{ cookiecutter.__documentation_url }}")
+switcher_version = get_version_match(__version__)
 
 # Select desired logo, theme, and declare the html title
 html_logo = logo
 html_theme = "ansys_sphinx_theme"
 html_short_title = html_title = "{{ cookiecutter.__project_name_slug }}"
 
 # specify the location of your github repo
@@ -48,15 +50,15 @@
         ("Ansys", "https://dev.docs.ansys.com/"),
         {%- elif cookiecutter.__logo == "pyansys" %}
         ("PyAnsys", "https://docs.pyansys.com/"),
         {%- endif %}
     ],
     "switcher": {
         "json_url": f"https://{cname}/versions.json",
-        "version_match": get_version_match(__version__),
+        "version_match": switcher_version,
     },
     "check_switcher": False,
 }
 
 # Sphinx extensions
 extensions = [
     "sphinx.ext.autodoc",
@@ -108,7 +110,23 @@
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
+
+# Keep these while the repository is private
+linkcheck_ignore = [
+    "{{ cookiecutter.__repository_url }}/*",
+    {%- if cookiecutter.__template_name == "pyansys-advanced" %}
+    "{{ cookiecutter.__documentation_url }}/version/stable/*",
+    {%- endif %}
+    "https://pypi.org/project/{{cookiecutter.__pkg_name}}",
+]
+
+# If we are on a release, we have to ignore the "release" URLs, since it is not
+# available until the release is published.
+if switcher_version != "dev":
+    linkcheck_ignore.append(
+        f"https://github.com/ansys/{{ cookiecutter.__pkg_namespace }}/releases/tag/v{__version__}"
+    )
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-2.1.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tox]
 description = Default tox environments list
 envlist =
-    style,{py38,py39,py310,py311,py312}{,-coverage},doc
+    style,{py39,py310,py311,py312}{,-coverage},doc
 skip_missing_interpreters = true
 {%- if cookiecutter.__build_system != "setuptools" %}
 isolated_build = true
 {%- if cookiecutter.__build_system == "flit" %}
 isolated_build_env = build
 {%- endif %}
 {%- endif %}
 
 [testenv]
 description = Checks for project unit tests and coverage (if desired)
 basepython =
-    py38: python3.8
     py39: python3.9
     py310: python3.10
     py311: python3.11
     py312: python3.12
     py: python3
     {%- if cookiecutter.__build_system != "poetry" %}
     {style,reformat,doc,build}: python3
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9538461538461539%*

 * *Differences: {"'__documentation_url'": "''", "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "__build_system": "{{ cookiecutter.build_system }}",
     "__coverage_source": "",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "",
     "__logo": "{{ cookiecutter.logo | lower }}",
     "__logo_color": "black",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "",
     "__pkg_namespace": "",
@@ -25,15 +26,15 @@
         "Ansys",
         "PyAnsys"
     ],
     "max_linelength": "100",
     "project_name": "doc-project",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,93 @@
 """Post-processing script for cleaning the raw rendered project."""
 import os
 import shutil
 from pathlib import Path
 
 import isort
 
-from ansys.templates.utils import keep_files
-
+from ansys.templates.utils import keep_files, remove_file
 
 ALLOWED_BUILD_SYSTEMS = ["flit", "poetry", "setuptools"]
 """A list of all allowed build systems by the template."""
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
+    "doc/source/getting_started/index.rst",
+    "doc/source/changelog.rst",
+    "doc/source/examples.rst",
     "examples/README.md",
+    ".flake8",
     ".github/dependabot.yml",
     ".github/labeler.yml",
     ".github/labels.yml",
     ".github/workflows/ci_cd.yml",
     ".github/workflows/label.yml",
+    ".gitattributes",
     ".gitignore",
     "LICENSE",
-    "README.rst",
     ".pre-commit-config.yaml",
-    "requirements/requirements_build.txt",
-    "requirements/requirements_doc.txt",
+    "pyproject.toml",
+    "README.rst",
+    "src/ansys/{{ cookiecutter.__product_name_slug }}/{{ cookiecutter.__library_name_slug }}/__init__.py",
+    "tests/test_metadata.py",
     "tox.ini",
 ]
 """A list holding all desired files to be included in the project."""
 
-
 def main():
     """Entry point of the script."""
     # Get baked project location path
     project_path = Path(os.getcwd())
 
+    # Get the desired build system
+    build_system = "{{ cookiecutter.build_system }}"
+
     # Move all requirements files into a requirements/ directory
-    os.mkdir(project_path / "requirements")
     requirements_files = [
-            f"requirements_{name}.txt" for name in ["build", "doc"]
+        f"requirements_{name}.txt" for name in ["build", "doc", "tests"]
     ]
-    for file in requirements_files:
-        shutil.move(str(project_path / file), str(project_path / "requirements"))
+    if build_system == "poetry":
+        # Poetry required and extra dependencies are collected inside the
+        # 'pyproject.toml' file. Thus, there is no need to have requirements
+        # files
+        for file in requirements_files:
+            remove_file(file, project_path)
+    else:
+        os.mkdir(project_path / "requirements")
+        for file in requirements_files:
+            shutil.move(str(project_path / file), str(project_path / "requirements"))
 
     # Apply isort with desired config
     isort_config = isort.settings.Config(
         line_length="{{ cookiecutter.__max_linelength }}",
         profile="black",
     )
     filepaths_list = [
-        project_path / "doc" / "source" / "conf.py",
+        project_path / "doc/source/conf.py",
     ]
     for filepath in filepaths_list:
-        isort.api.sort_file(filepath, config=isort_config)
+        isort.api.sort_file(filepath, isort_config)
 
-    # Apply the desired structure to the project
+    # Remove non-desired files
+    if build_system == "setuptools":
+        DESIRED_STRUCTURE.append("setup.py")
     keep_files(DESIRED_STRUCTURE)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   hooks:
   - id: flake8
 
 - repo: https://github.com/codespell-project/codespell
   rev: v2.2.2
   hooks:
   - id: codespell
-    args: [--ignore-words=doc/styles/Vocab/ANSYS/accept.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
+    args: [--ignore-words=doc/styles/config/vocabularies/ANSYS/accept.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-merge-conflict
   - id: debug-statements
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-2.1.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.915625%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'__template_name'": "'pyace-pkg'",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,25 +1,27 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "",
     "__default_copyright": "{{ cookiecutter.copyright }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "{{ cookiecutter.logo | lower }}",
     "__logo_color": "{{ cookiecutter.logo_color }}",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "{{ cookiecutter.__project_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "src",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name | slugify(separator=('_')) }}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description }}",
-    "__template_name": "pyace-fastapi",
+    "__template_name": "pyace-pkg",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "ci_cd_platform": [
         "GitHub",
         "Azure DevOps"
     ],
     "copyright": "None",
     "enable_docker": [
         "No",
@@ -38,15 +40,15 @@
         "white",
         "black"
     ],
     "max_linelength": "100",
     "project_name": "project",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "A {{ cookiecutter.project_name }} Python project for {{ cookiecutter.project_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 DESIRED_STRUCTURE = [
     "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
@@ -34,16 +38,21 @@
     "requirements/requirements_build.txt",
     "requirements/requirements_doc.txt",
     "requirements/requirements_tests.txt",
     "setup.py",
     "src/__init__.py",
     "src/_version.py",
     "src/server.py",
+    "src/blueprints/__init__.py",
+    "src/blueprints/health.py",
+    "src/blueprints/version.py",
     "src/models/__init__.py",
+    "src/observability/__init__.py",
     "src/observability/logger.py",
+    "src/static/swagger.json",
     "tests/test_metadata.py",
     "tests/test_server.py",
     "tests/conftest.py",
     "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,25 +1,27 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "",
     "__default_copyright": "{{ cookiecutter.copyright }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "{{ cookiecutter.logo | lower }}",
     "__logo_color": "{{ cookiecutter.logo_color }}",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "{{ cookiecutter.__project_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "src",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name | slugify(separator=('_')) }}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description }}",
     "__template_name": "pyace-flask",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "ci_cd_platform": [
         "GitHub",
         "Azure DevOps"
     ],
     "copyright": "None",
     "enable_docker": [
         "No",
@@ -38,15 +40,15 @@
         "white",
         "black"
     ],
     "max_linelength": "100",
     "project_name": "project",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "A {{ cookiecutter.project_name }} Python project for {{ cookiecutter.project_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 DESIRED_STRUCTURE = [
     "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
@@ -34,21 +38,16 @@
     "requirements/requirements_build.txt",
     "requirements/requirements_doc.txt",
     "requirements/requirements_tests.txt",
     "setup.py",
     "src/__init__.py",
     "src/_version.py",
     "src/server.py",
-    "src/blueprints/__init__.py",
-    "src/blueprints/health.py",
-    "src/blueprints/version.py",
     "src/models/__init__.py",
-    "src/observability/__init__.py",
     "src/observability/logger.py",
-    "src/static/swagger.json",
     "tests/test_metadata.py",
     "tests/test_server.py",
     "tests/conftest.py",
     "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,25 +1,27 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "",
     "__default_copyright": "{{ cookiecutter.copyright }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "{{ cookiecutter.logo | lower }}",
     "__logo_color": "{{ cookiecutter.logo_color }}",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "{{ cookiecutter.__project_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "src",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name | slugify(separator=('_')) }}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description }}",
     "__template_name": "pyace-grpc",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "ci_cd_platform": [
         "GitHub",
         "Azure DevOps"
     ],
     "copyright": "None",
     "enable_docker": [
         "No",
@@ -38,15 +40,15 @@
         "white",
         "black"
     ],
     "max_linelength": "100",
     "project_name": "project",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "A {{ cookiecutter.project_name }} Python project for {{ cookiecutter.project_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 DESIRED_STRUCTURE = [
     "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.915625%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'__template_name'": "'pyace-fastapi'",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,25 +1,27 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "",
     "__default_copyright": "{{ cookiecutter.copyright }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "{{ cookiecutter.logo | lower }}",
     "__logo_color": "{{ cookiecutter.logo_color }}",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "{{ cookiecutter.__project_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "src",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name | slugify(separator=('_')) }}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description }}",
-    "__template_name": "pyace-pkg",
+    "__template_name": "pyace-fastapi",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "ci_cd_platform": [
         "GitHub",
         "Azure DevOps"
     ],
     "copyright": "None",
     "enable_docker": [
         "No",
@@ -38,15 +40,15 @@
         "white",
         "black"
     ],
     "max_linelength": "100",
     "project_name": "project",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "A {{ cookiecutter.project_name }} Python project for {{ cookiecutter.project_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 DESIRED_STRUCTURE = [
     "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9159999999999999%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": '{delete: [0]}'}*

```diff
@@ -1,30 +1,31 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "ansys.{{ cookiecutter.__product_name_slug }}",
+    "__documentation_url": "",
     "__is_pyansys": "True",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "pyansys",
     "__logo_color": "black",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "ansys-{{ cookiecutter.__product_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "ansys.{{ cookiecutter.__product_name_slug }}.{{ cookiecutter.__library_name_slug }}",
     "__product_name_slug": "{{ cookiecutter.product_name | slugify(separator=('_')) }}",
     "__project_name_slug": "py{{ cookiecutter.__product_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-')}}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description | capitalize }}",
     "__template_name": "pyansys",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "library_name": "Library",
     "max_linelength": "100",
     "product_name": "Product",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
         "3.11",
         "3.12"
     ],
     "short_description": "A Python wrapper for Ansys {{ cookiecutter.product_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     "LICENSE",
     "pyproject.toml",
     "README.rst",
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9192307692307692%*

 * *Differences: {"'__documentation_url'": "'{{ cookiecutter.documentation_url }}'",*

 * * "'documentation_url'": "'https://{{ cookiecutter.product_name }}.docs.pyansys.com'",*

 * * "'requires_python'": '{delete: [0]}'}*

```diff
@@ -1,10 +1,11 @@
 {
     "__build_system": "{{ cookiecutter.build_system }}",
     "__coverage_source": "ansys.{{ cookiecutter.__product_name_slug }}",
+    "__documentation_url": "{{ cookiecutter.documentation_url }}",
     "__is_pyansys": "True",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "pyansys",
     "__logo_color": "black",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "ansys-{{ cookiecutter.__product_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}",
     "__pkg_namespace": "ansys.{{ cookiecutter.__product_name_slug }}.{{ cookiecutter.__library_name_slug }}",
@@ -16,20 +17,20 @@
     "__template_name": "pyansys-advanced",
     "__version": "{{ cookiecutter.version }}",
     "build_system": [
         "flit",
         "poetry",
         "setuptools"
     ],
+    "documentation_url": "https://{{ cookiecutter.product_name }}.docs.pyansys.com",
     "library_name": "library",
     "max_linelength": "100",
     "product_name": "product",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
         "3.11",
         "3.12"
     ],
     "short_description": "A Python wrapper for Ansys {{ cookiecutter.product_name }} {{ cookiecutter.library_name }}",
     "version": "0.1.dev0"
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/getting_started/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,64 @@
-Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }}
-{{ '=' * (cookiecutter.__project_name_slug | length) }}
-|pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
-
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
-   :alt: PyAnsys
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/{{cookiecutter.__project_name_slug}}?logo=pypi
-   :target: https://pypi.org/project/{{cookiecutter.__project_name_slug}}/
-   :alt: Python
-
-.. |pypi| image:: https://img.shields.io/pypi/v/{{cookiecutter.__project_name_slug}}.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/{{cookiecutter.__project_name_slug}}
-   :alt: PyPI
-
-.. |codecov| image:: https://codecov.io/gh/ansys/{{cookiecutter.__project_name_slug}}/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/ansys/{{cookiecutter.__project_name_slug}}
-   :alt: Codecov
-
-.. |GH-CI| image:: https://github.com/ansys/{{cookiecutter.__project_name_slug}}/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/ansys/{{cookiecutter.__project_name_slug}}/actions/workflows/ci_cd.yml
-   :alt: GH-CI
-
-.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-   :alt: MIT
-
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
-   :target: https://github.com/psf/black
-   :alt: Black
-
-
-{{ cookiecutter.short_description }}
-
-
-How to install
---------------
+Getting started
+---------------
 
 At least two installation modes are provided: user and developer.
 
 For users
 ^^^^^^^^^
 
+{%- if cookiecutter.__product_name_slug != "" %}
 In order to install Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }}, make sure you
+{%- elif cookiecutter.__template_name != "solution" %}
+In order to install {{ cookiecutter.project_name }}, make sure you
+{%- else %}
+In order to install {{ cookiecutter.solution_name }}, make sure you
+{%- endif %}
 have the latest version of `pip`_. To do so, run:
 
 .. code:: bash
 
     python -m pip install -U pip
 
 Then, you can simply execute:
 
-{% if cookiecutter.build_system in ["flit", "setuptools"] -%}
+{% if cookiecutter.__build_system in ["flit", "setuptools"] -%}
 
 .. code:: bash
 
     python -m pip install {{ cookiecutter.__pkg_name }}
 
-{% elif cookiecutter.build_system == "poetry" -%}
+{% elif cookiecutter.__build_system == "poetry" -%}
 
 .. code:: bash
 
     poetry run python -m pip install {{ cookiecutter.__pkg_name }}
 
 {% endif -%}
 
 
 For developers
 ^^^^^^^^^^^^^^
 
+{%- if cookiecutter.__product_name_slug != "" %}
 Installing Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }} in developer mode allows
+{%- elif cookiecutter.__template_name != "solution" %}
+Installing Py{{ cookiecutter.project_name }} in developer mode allows
+{%- else %}
+Installing Py{{ cookiecutter.solution_name }} in developer mode allows
+{%- endif %}
 you to modify the source and enhance it.
 
-Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will
-need to follow these steps:
+Before contributing to the project, please refer to the `PyAnsys Developer's guide`_ and then follow these steps:
 
 #. Start by cloning this repository:
 
    .. code:: bash
 
-      git clone {{ cookiecutter.repository_url }}
+      git clone {{ cookiecutter.__repository_url }}
 
 #. Create a fresh-clean Python environment and activate it:
 
    .. code:: bash
 
       # Create a virtual environment
       python -m venv .venv
@@ -97,68 +72,68 @@
       # Activate it in Windows Powershell
       .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest required build system and doc, testing, and CI tools:
 
    .. code:: bash
 
-      python -m pip install -U pip {{ cookiecutter.build_system }} tox
+      python -m pip install -U pip {{ cookiecutter.__build_system }} tox
       python -m pip install -r requirements/requirements_build.txt
       python -m pip install -r requirements/requirements_doc.txt
       python -m pip install -r requirements/requirements_tests.txt
 
 
 #. Install the project in editable mode:
 
-    {% if cookiecutter.build_system in ["flit", "setuptools"] -%}
+    {% if cookiecutter.__build_system in ["flit", "setuptools"] -%}
 
    .. code:: bash
 
       python -m pip install --editable {{ cookiecutter.__pkg_name }}
 
-    {% elif cookiecutter.build_system == "poetry" -%}
+    {% elif cookiecutter.__build_system == "poetry" -%}
 
    .. code:: bash
 
       poetry run python -m pip install {{ cookiecutter.__pkg_name }}
 
     {% endif -%}
 
 #. Finally, verify your development installation by running:
 
    .. code:: bash
 
       tox
 
 
-How to testing
---------------
+How to test
+-----------
 
 This project takes advantage of `tox`_. This tool allows to automate common
 development tasks (similar to Makefile) but it is oriented towards Python
 development.
 
 Using tox
 ^^^^^^^^^
 
 As Makefile has rules, `tox`_ has environments. In fact, the tool creates its
 own virtual environment so anything being tested is isolated from the project in
 order to guarantee project's integrity. The following environments commands are provided:
 
-- **tox -e style**: will check for coding style quality.
+- **tox -e style**: checks for coding style quality.
 - **tox -e py**: checks for unit tests.
 - **tox -e py-coverage**: checks for unit testing and code coverage.
-- **tox -e doc**: checs for documentation building process.
+- **tox -e doc**: checks for documentation building process.
 
 
 Raw testing
 ^^^^^^^^^^^
 
 If required, you can always call the style commands (`black`_, `isort`_,
-`flake8`_...) or unit testing ones (`pytest`_) from the command line. However,
+`flake8`_) or unit testing ones (`pytest`_) from the command line. However,
 this does not guarantee that your project is being tested in an isolated
 environment, which is the reason why tools like `tox`_ exist.
 
 
 A note on pre-commit
 ^^^^^^^^^^^^^^^^^^^^
 
@@ -170,15 +145,15 @@
     python -m pip install pre-commit && pre-commit install
 
 
 Documentation
 -------------
 
 For building documentation, you can either run the usual rules provided in the
-`Sphinx`_ Makefile, such us:
+`Sphinx`_ Makefile, such as:
 
 .. code:: bash
 
     make -C doc/ html && open doc/html/index.html
 
 However, the recommended way of checking documentation integrity is using:
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9571428571428572%*

 * *Differences: {"'__documentation_url'": "''", "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "__build_system": "flit",
     "__coverage_source": "ansys.{{ cookiecutter.__product_name_slug }}",
+    "__documentation_url": "",
     "__is_pyansys": "True",
     "__library_name_slug": "{{ cookiecutter.library_name | slugify(separator=('_')) }}",
     "__logo": "",
     "__logo_color": "",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "ansys-{{ cookiecutter.__product_name_slug | replace('_', '-') }}-{{ cookiecutter.__library_name_slug | replace('_', '-') }}-openapi",
     "__pkg_namespace": "ansys.{{ cookiecutter.__product_name_slug }}.{{ cookiecutter.__library_name_slug }}_openapi",
@@ -19,16 +20,16 @@
     "__yaml_file_name": "{{ cookiecutter.yaml_file_name }}",
     "build_system": "flit",
     "library_name": "library",
     "max_linelength": "100",
     "product_name": "product",
     "repository_url": "https://github.com/ansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "Autogenerated client library for the {{ cookiecutter.product_name }} {{ cookiecutter.library_name }} library. Direct use of this package is unsupported, please use {{ cookiecutter.__wrapper_package_name }} instead.",
     "version": "0.1.dev0",
     "yaml_file_name": "library.yaml"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-2.1.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9083333333333333%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'build_system'": "'setuptools'",*

 * * "'requires_python'": "{insert: [(3, '3.12')], delete: [0]}"}*

```diff
@@ -1,29 +1,31 @@
 {
     "__build_system": "setuptools",
     "__coverage_source": "{{ cookiecutter.__project_name_slug }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "",
     "__logo": "pyansys",
     "__logo_color": "black",
     "__max_linelength": "{{ cookiecutter.max_linelength }}",
     "__pkg_name": "{{ cookiecutter.__project_name_slug | replace('_', '-')}}",
     "__pkg_namespace": "{{ cookiecutter.__project_name_slug }}",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.project_name | slugify(separator=('_')) }}",
     "__repository_url": "{{ cookiecutter.repository_url }}",
     "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "{{ cookiecutter.short_description | capitalize }}",
     "__template_name": "pybasic",
     "__version": "{{ cookiecutter.version }}",
+    "build_system": "setuptools",
     "max_linelength": "100",
     "project_name": "",
     "repository_url": "",
     "requires_python": [
-        "3.8",
         "3.9",
         "3.10",
-        "3.11"
+        "3.11",
+        "3.12"
     ],
     "short_description": "",
     "version": "0.1.dev0"
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,20 @@
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
+    "doc/source/getting_started/index.rst",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-2.1.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8958333333333334%*

 * *Differences: {"'__documentation_url'": "''",*

 * * "'__requires_python'": "'{{ cookiecutter.requires_python }}'",*

 * * "'requires_python'": "['3.9', '3.10']"}*

```diff
@@ -1,29 +1,34 @@
 {
     "__build_system": "poetry",
     "__coverage_source": "{{ cookiecutter.__solution_name_slug }}",
+    "__documentation_url": "",
     "__is_pyansys": "False",
     "__library_name_slug": "",
     "__logo": "solutions",
     "__logo_color": "black",
     "__max_linelength": "120",
     "__pkg_name": "ansys-solutions-{{ cookiecutter.solution_name.lower().replace('_', '-') }}",
     "__pkg_namespace": "ansys.solutions.{{ cookiecutter.solution_name.lower().replace('-', '_') }}",
     "__product_name_slug": "",
     "__project_name_slug": "{{ cookiecutter.solution_name.lower().replace('_', '-').replace(' ', '-') }}",
     "__repository_url": "",
-    "__requires_python": "3.8",
+    "__requires_python": "{{ cookiecutter.requires_python }}",
     "__short_description": "",
     "__solution_definition_name": "{{ cookiecutter.__solution_name_slug.title() }}Solution",
     "__solution_name_slug": "{{ cookiecutter.solution_name.lower().replace('-', '_').replace(' ', '_') }}",
     "__template_name": "solution",
     "__version": "0.1.dev0",
     "_copy_without_render": [
         "*.html"
     ],
+    "requires_python": [
+        "3.9",
+        "3.10"
+    ],
     "solution_display_name": "My Solution",
     "solution_name": "my_solution",
     "with_dash_ui": [
         "yes",
         "no"
     ]
 }
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from ansys.templates.utils import keep_files
 
 
 DESIRED_STRUCTURE = [
     ".github/workflows/build-release.yml",
     ".github/workflows/release-please.yml",
+    ".github/workflows/label.yml",
+    ".github/labeler.yml",
+    ".github/labels.yml",
     ".vscode/launch.json",
     ".vscode/extensions.json",
+    "doc/changelog.d/changelog_template.jinja",
     "doc/source/_static/ansys-solutions-logo-black-background.png",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
+    "doc/source/getting_started/index.rst",
+    "doc/source/changelog.rst",
     "doc/source/conf.py",
+    "doc/source/examples.rst",
     "doc/source/index.rst",
-    "doc/styles/Vocab/ANSYS/accept.txt",
-    "doc/styles/Vocab/ANSYS/reject.txt",
+    "doc/styles/config/vocabularies/ANSYS/accept.txt",
+    "doc/styles/config/vocabularies/ANSYS/reject.txt",
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
     "doc/Makefile",
     "examples/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/datamodel/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/logic/assets/README.md",
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/build-release.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/build-release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,26 @@
   HTML_DOCUMENTATION_ARTIFACT: "{{ cookiecutter.__project_name_slug }}-documentation"
 
 concurrency:
   group: {{ "${{ github.workflow }}-${{ github.ref }}" }}
   cancel-in-progress: true
 
 jobs:
+  update-changelog:
+    name: "Update CHANGELOG for new tag"
+    if: github.event_name == 'push' && contains(github.ref, 'refs/tags')
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+      pull-requests: write
+    steps:
+      - uses: ansys/actions/doc-deploy-changelog@v6
+        with:
+          token: {{ "${{ secrets.PYANSYS_CI_BOT_TOKEN }}" }}
+
   check-copyright:
     name: Check copyright
     runs-on: [ubuntu-latest]
     timeout-minutes: 10
     steps:
       - name: Check copyright
         uses: ansys-internal/solution-applications-actions/check-copyright@v11
@@ -136,15 +148,15 @@
           sbom-artifact: {{ "${{ env.SBOM_NAME }}" }}
           gh-token: {{ "${{ secrets.WORKFLOW_TOKEN }}" }}
 
   release:
     if: |
       github.event_name == 'release' && false
     name: Release
-    needs: [build-doc, check-copyright, check-code-style, build, run-tests, check-licenses, package-solution, generate-sbom, validate-sbom]
+    needs: [update-changelog, build-doc, check-copyright, check-code-style, build, run-tests, check-licenses, package-solution, generate-sbom, validate-sbom]
     runs-on: [ubuntu-latest]
     timeout-minutes: 10
     steps:
       - name: Release
         uses: ansys-internal/solution-applications-actions/release-to-private-pypi@v11
         with:
           python-version: {{ "${{ env.MAIN_PYTHON_VERSION }}" }}
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/release-please.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ##############################################
 {{cookiecutter.solution_name}}
 ##############################################
 |python|
 
+.. contribute_start
 
 Installation
 ============
 
 Prerequisites
 -------------
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files 2% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 # Define the Ansys vocabulary
 Vocab = ANSYS
 
 [*.{md,rst}]
 
 # Apply the following styles
 BasedOnStyles = Vale, Google
+Vale.Terms = NO
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 if documentation_url:
     repository_name = remove_scheme_from_url(repository_url)
 else:
     repository_name = None
 
 copyright = f"(c) {datetime.now().year} ANSYS, Inc. All rights reserved"
 author = "ANSYS Inc."
+switcher_version = get_version_match(package_version)
 
 
 # ---------- // General configuration // ------------------------------------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
@@ -174,15 +175,15 @@
 html_theme_options = {
     "show_prev_next": False,
     "show_breadcrumbs": True,
     "collapse_navigation": True,
     "use_edit_page_button": False,
     "switcher": {
         "json_url": f"https://{cname}/versions.json",
-        "version_match": get_version_match(package_version),
+        "version_match": switcher_version,
     },
 }
 
 if str(os.getenv("DISABLE_GITHUB_URL_LINK")).lower() != "true":
     html_theme_options["github_url"] = f"https://github.com/{ORGANIZATION_NAME}/{repository_name}"
 
 html_context = {
@@ -246,7 +247,21 @@
         "Ansys Solutions {{cookiecutter.solution_display_name}}",
         "Ansys Solutions {{cookiecutter.solution_display_name}} Documentation",
         author,
         "Ansys Solutions {{cookiecutter.solution_display_name}}",
         "Engineering Software",
     ),
 ]
+
+# Keep these while the repository is private
+linkcheck_ignore = [
+    "{{ cookiecutter.__repository_url }}/*",
+    {%- if cookiecutter.__template_name == "pyansys-advanced" %}
+    "{{ cookiecutter.__documentation_url }}/version/stable/*",
+    {%- endif %}
+    "https://pypi.org/project/{{cookiecutter.__pkg_name}}",
+]
+
+# If we are on a release, we have to ignore the "release" URLs, since it is not
+# available until the release is published.
+if switcher_version != "dev":
+    linkcheck_ignore.append(f"https://github.com/ansys/{{ cookiecutter.__pkg_namespace }}/releases/tag/v{package_version}")
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -126,7 +126,41 @@
 select = ['D107']
 
 [tool.coverage.run]
 source = ["ansys.solutions"]
 
 [tool.coverage.report]
 show_missing = true
+
+[tool.towncrier]
+package = "{{ cookiecutter.__pkg_namespace }}"
+directory = "doc/changelog.d"
+filename = "doc/source/changelog.rst"
+start_string = ".. towncrier release notes start\n"
+template = "doc/changelog.d/changelog_template.jinja"
+title_format = "`{version} <https://github.com/ansys/{{ cookiecutter.__pkg_namespace }}/releases/tag/v{version}>`_ - {project_date}"
+issue_format = "`#{issue} <https://github.com/ansys/{{ cookiecutter.__pkg_namespace }}/pull/{issue}>`_"
+
+[[tool.towncrier.type]]
+directory = "added"
+name = "Added"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "changed"
+name = "Changed"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "fixed"
+name = "Fixed"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "dependencies"
+name = "Dependencies"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "miscellaneous"
+name = "Miscellaneous"
+showcontent = true
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
-# solutions-common-files@v2.0.1
 
 """
 A Python script to automate the setup of the Python ecosystem of a project.
 
 Prerequisites
 -------------
 
@@ -113,14 +112,15 @@
 import platform
 import re
 import shutil
 import subprocess
 import sys
 import textwrap
 import time
+import winreg
 
 try:
     from packaging.markers import Marker
 except:
     sys.exit("Process stopped. The `packaging` library is missing. Install with: `pip install packaging`.")
 try:
     import toml
@@ -240,15 +240,15 @@
         print(
             f"Warning: poetry expects the name of the virtual environment name to be"
             f" {args.venv_name}. {old_name} is replaced by {args.venv_name}."
         )
 
 
 def check_python_version(args: object) -> None:
-    """Check if the version of the current Python interpreter is consistent with the python version specifications."""
+    """Check if current Python is consistent with the python specifications from the build system."""
     # Initialize lower/upper versions
     lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
     lower_specification, upper_specification, single_specification = None, None, None
     # Read TOML
     configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
     # Read Python version constraint
     python_compatibility = configuration["tool"]["poetry"]["dependencies"]["python"].replace(" ", "")
@@ -291,14 +291,41 @@
 
 
 def check_existing_install(args: object) -> str:
     """Check if an install exists already."""
     return os.path.isdir(args.venv_name)
 
 
+def is_long_paths_enabled():
+    """Check if long paths are enabled on Windows."""
+    try:
+        # Open the registry key
+        with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\CurrentControlSet\Control\FileSystem") as key:
+            # Read the value of LongPathsEnabled
+            value, _ = winreg.QueryValueEx(key, "LongPathsEnabled")
+            return value == 1
+    except FileNotFoundError:
+        # The key doesn't exist, which means long paths are not enabled
+        return False
+
+
+def is_path_too_long(path):
+    """Check if the path exceeds the maximum allowed length on Windows."""
+    # Maximum allowed path length for Windows
+    max_path_length_windows = 260
+
+    # Check if the path to each file is too long
+    for root, dirs, files in os.walk(path):
+        for file in files:
+            file_path = os.path.join(root, file)
+            if len(file_path) > max_path_length_windows:
+                return True
+    return False
+
+
 def check_inputs(args: object) -> None:
     """Check inputs consistency."""
     # Rework dependencies argument if all option is selected
     if "all" in args.dependencies:
         args.install_all = True
         args.dependencies = STANDARD_OPTIONAL_DEPENDENCY_GROUPS + ["run"]
     else:
@@ -307,16 +334,27 @@
     # Check virtual environment name
     check_virtual_environment_name(args)
     # Check python version
     check_python_version(args)
     # Check if an install already exists
     args.has_install = check_existing_install(args)
 
-    if args.local_wheels and not os.path.exists(args.local_wheels):
-        raise FileNotFoundError(f"The directory '{args.local_wheels}' does not exist.")
+    if args.local_wheels:
+        if not os.path.exists(args.local_wheels):
+            raise FileNotFoundError(f"The directory '{args.local_wheels}' does not exist.")
+
+        if sys.platform == "win32":
+            path_too_long = is_path_too_long(args.local_wheels)
+
+            if path_too_long and not is_long_paths_enabled():
+                raise Exception(
+                    f"Path length to file(s) in '{args.local_wheels}' exceeds the maximum limit in Windows."
+                    "Please enable Windows Long Path support or use a shorter path. You can find information on "
+                    "how to enable this at https://pip.pypa.io/warnings/enable-long-paths"
+                )
 
 
 def modify_toml_file_in_case_of_wheel_files(args: object) -> None:
     """Modify the toml file in case of wheel files."""
     if not args.local_wheels:
         return
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/sonar-project.properties` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_black.png` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_black.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_white.png` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys_solutions_logo_white.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/about_page.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/collector/otel-collector-config.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/collector/otel-collector-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboard.json` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-dashboard.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-datasources.yml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/_deploy/compose/grafana/grafana-datasources.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/grafana/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/telemetry/tracelens/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-2.1.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-2.0.0/src/ansys/templates/testing.py` & `ansys_templates-2.1.0/src/ansys/templates/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/src/ansys/templates/utils.py` & `ansys_templates-2.1.0/src/ansys/templates/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 # SPDX-License-Identifier: MIT
 #
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ansys_templates-2.0.0/PKG-INFO` & `ansys_templates-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 2.0.0
+Version: 2.1.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
-Maintainer-email: PyAnsys developers <pyansys.core@ansys.com>
+Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: click>=7.0,<9.0.0
 Requires-Dist: cookiecutter>=2.1.0,<2.3.0
 Requires-Dist: isort>=5.10.1
-Requires-Dist: ansys-sphinx-theme==0.13.1 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.14.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
 Requires-Dist: sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==7.4.4 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
 Project-URL: Source, https://github.com/ansys/ansys-templates
 Project-URL: Tracker, https://github.com/ansys/ansys-templates/issues
 Provides-Extra: doc
 Provides-Extra: tests
```


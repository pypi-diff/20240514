# Comparing `tmp/logfire-0.31.0.tar.gz` & `tmp/logfire-0.32.0.tar.gz`

## Comparing `logfire-0.31.0.tar` & `logfire-0.32.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.31.0/Makefile
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    55953 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    55300 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    18537 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_backfill.py
--rw-r--r--   0        0        0    45014 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    40637 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    43190 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.31.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.31.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.31.0/README.md
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.31.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.31.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.32.0/Makefile
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18465 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    55300 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/openai.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    43200 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.32.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.32.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.32.0/README.md
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.32.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.32.0/PKG-INFO
```

### Comparing `logfire-0.31.0/Makefile` & `logfire-0.32.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/__init__.py` & `logfire-0.32.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/propagate.py` & `logfire-0.32.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/testing.py` & `logfire-0.32.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/ast_utils.py` & `logfire-0.32.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/async_.py` & `logfire-0.32.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/auth.py` & `logfire-0.32.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/backfill.py` & `logfire-0.32.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/cli.py` & `logfire-0.32.0/logfire/_internal/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         for url, info in data['tokens'].items():
             f.write(f'[tokens."{url}"]\n')
             f.write(f'token = "{info["token"]}"\n')
             f.write(f'expiration = "{info["expiration"]}"\n')
 
     console.print()
     console.print(f'Your Logfire credentials are stored in [bold]{DEFAULT_FILE}[/]')
-    # TODO(Marcelo): Add a message to inform which commands can be used.
 
 
 def parse_list_projects(args: argparse.Namespace) -> None:
     """List user projects."""
     logfire_url = args.logfire_url
     console = Console(file=sys.stderr)
     projects = LogfireCredentials.get_user_projects(session=args._session, logfire_api_url=logfire_url)
@@ -322,14 +321,15 @@
 def parse_use_project(args: argparse.Namespace) -> None:
     """Use an existing project."""
     data_dir = Path(args.data_dir)
     logfire_url = args.logfire_url
     project_name = args.project_name
     organization = args.org
     console = Console(file=sys.stderr)
+
     projects = LogfireCredentials.get_user_projects(session=args._session, logfire_api_url=logfire_url)
     project_info = LogfireCredentials.use_existing_project(
         session=args._session,
         logfire_api_url=logfire_url,
         projects=projects,
         organization=organization,
         project_name=project_name,
@@ -434,15 +434,15 @@
     cmd_projects_new.add_argument('--org', help='project organization')
     cmd_projects_new.add_argument(
         '--default-org', action='store_true', help='whether to create project under user default organization'
     )
     cmd_projects_new.set_defaults(func=parse_create_new_project)
 
     cmd_projects_use = projects_subparsers.add_parser('use', help='use a project')
-    cmd_projects_use.add_argument('project_name', help='project name')
+    cmd_projects_use.add_argument('project_name', nargs='?', help='project name')
     cmd_projects_use.add_argument('--org', help='project organization')
     cmd_projects_use.add_argument('--data-dir', default='.logfire')
     cmd_projects_use.set_defaults(func=parse_use_project)
 
     cmd_info = subparsers.add_parser('info', help=parse_info.__doc__)
     cmd_info.set_defaults(func=parse_info)
```

### Comparing `logfire-0.31.0/logfire/_internal/config.py` & `logfire-0.32.0/logfire/_internal/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 from .exporters.otlp import OTLPExporterHttpSession, RetryFewerSpansSpanExporter
 from .exporters.processor_wrapper import SpanProcessorWrapper
 from .exporters.remove_pending import RemovePendingSpansExporter
 from .integrations.executors import instrument_executors
 from .metrics import ProxyMeterProvider, configure_metrics
 from .scrubbing import Scrubber, ScrubCallback
 from .tracer import PendingSpanProcessor, ProxyTracerProvider
-from .utils import UnexpectedResponse, ensure_data_dir_exists, read_toml_file
+from .utils import UnexpectedResponse, ensure_data_dir_exists, get_version, read_toml_file
 
 CREDENTIALS_FILENAME = 'logfire_credentials.json'
 """Default base URL for the Logfire API."""
 COMMON_REQUEST_HEADERS = {'User-Agent': f'logfire/{VERSION}'}
 """Common request headers for requests to the Logfire API."""
 PROJECT_NAME_PATTERN = r'^[a-z0-9]+(?:-[a-z0-9]+)*$'
 
@@ -390,14 +390,19 @@
                 min_log_level=param_manager.load_param('console_min_log_level'),
             )
 
         if isinstance(pydantic_plugin, dict):
             # This is particularly for deserializing from a dict as in executors.py
             pydantic_plugin = PydanticPlugin(**pydantic_plugin)  # type: ignore
         self.pydantic_plugin = pydantic_plugin or param_manager.pydantic_plugin
+        if self.pydantic_plugin.record != 'off':
+            import pydantic
+
+            if get_version(pydantic.__version__) < get_version('2.5.0'):  # pragma: no cover
+                raise RuntimeError('The Pydantic plugin requires Pydantic 2.5.0 or newer.')
         self.fast_shutdown = fast_shutdown
 
         self.id_generator = id_generator or RandomIdGenerator()
         self.ns_timestamp_generator = ns_timestamp_generator or time.time_ns
         self.processors = processors
         self.default_span_processor = default_span_processor or _get_default_span_processor
         self.metric_readers = metric_readers
@@ -904,15 +909,15 @@
             session: HTTP client session used to communicate with the Logfire API.
             logfire_api_url: The Logfire API base URL.
             projects: List of user projects.
             organization: Project organization.
             project_name: Name of project that has to be used.
 
         Returns:
-            The configured project informations.
+            The configured project information.
 
         Raises:
             LogfireConfigError: If there was an error configuring the project.
         """
         user_token = cls._get_user_token(logfire_api_url=logfire_api_url)
         headers = {**COMMON_REQUEST_HEADERS, 'Authorization': user_token}
 
@@ -1133,18 +1138,15 @@
         print(
             'No Logfire project credentials found.\n'  # TODO: Add a link to the docs about where we look
             'All data sent to Logfire must be associated with a project.\n'
         )
 
         projects = cls.get_user_projects(session=session, logfire_api_url=logfire_api_url)
         if projects:
-            use_existing_projects = Confirm.ask(
-                'Do you want to use one of your existing projects? ',
-                default=True,
-            )
+            use_existing_projects = Confirm.ask('Do you want to use one of your existing projects? ', default=True)
             if use_existing_projects:  # pragma: no branch
                 credentials = cls.use_existing_project(
                     session=session, logfire_api_url=logfire_api_url, projects=projects
                 )
 
         if not credentials:
             credentials = cls.create_new_project(
```

### Comparing `logfire-0.31.0/logfire/_internal/config_params.py` & `logfire-0.32.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/constants.py` & `logfire-0.32.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/formatter.py` & `logfire-0.32.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/instrument.py` & `logfire-0.32.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/json_encoder.py` & `logfire-0.32.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/json_formatter.py` & `logfire-0.32.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/json_schema.py` & `logfire-0.32.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/json_types.py` & `logfire-0.32.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/main.py` & `logfire-0.32.0/logfire/_internal/main.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/metrics.py` & `logfire-0.32.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/scrubbing.py` & `logfire-0.32.0/logfire/_internal/scrubbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     def __init__(self, patterns: Sequence[str] | None, callback: ScrubCallback | None = None):
         # See scrubbing_patterns and scrubbing_callback in logfire.configure for more info on these parameters.
         patterns = [*DEFAULT_PATTERNS, *(patterns or [])]
         self._pattern = re.compile('|'.join(patterns), re.IGNORECASE | re.DOTALL)
         self._callback = callback
 
     def scrub_span(self, span: ReadableSpanDict):
+        scope = span['instrumentation_scope']
+        if scope and scope.name == 'logfire.openai':
+            return
+
         # We need to use BoundedAttributes because:
         # 1. For events and links, we get an error otherwise:
         #      https://github.com/open-telemetry/opentelemetry-python/issues/3761
         # 2. The callback might return a value that isn't of the type required by OTEL,
         #      in which case BoundAttributes will discard it to prevent an error.
         # TODO silently throwing away the result is bad, and BoundedAttributes might be bad for performance.
         span['attributes'] = BoundedAttributes(attributes=self.scrub(('attributes',), span['attributes']))
```

### Comparing `logfire-0.31.0/logfire/_internal/stack_info.py` & `logfire-0.32.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/tracer.py` & `logfire-0.32.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/utils.py` & `logfire-0.32.0/logfire/_internal/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import json
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Mapping, Sequence, Tuple, TypedDict, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Sequence, Tuple, TypedDict, TypeVar, Union
 
 from opentelemetry import trace as trace_api
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import Event, ReadableSpan
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.trace.status import Status
 from opentelemetry.util import types as otel_types
 from requests import RequestException, Response
 
+if TYPE_CHECKING:
+    from packaging.version import Version
+
 T = TypeVar('T')
 
 JsonValue = Union[int, float, str, bool, None, List['JsonValue'], Tuple['JsonValue', ...], 'JsonDict']
 JsonDict = Dict[str, JsonValue]
 
 try:
     import pydantic_core
@@ -164,7 +167,20 @@
     if data_dir.exists():
         if not data_dir.is_dir():  # pragma: no cover
             raise ValueError(f'Data directory {data_dir} exists but is not a directory')
         return
     data_dir.mkdir(parents=True, exist_ok=True)
     gitignore = data_dir / '.gitignore'
     gitignore.write_text('*')
+
+
+def get_version(version: str) -> Version:
+    """Return a packaging.version.Version object from a version string.
+
+    We check if `packaging` is available, falling back to `setuptools._vendor.packaging` if it's not.
+    """
+    try:
+        from packaging.version import Version
+
+    except ImportError:  # pragma: no cover
+        from setuptools._vendor.packaging.version import Version
+    return Version(version)  # type: ignore
```

### Comparing `logfire-0.31.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.32.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.32.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.32.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/auto_trace/types.py` & `logfire-0.32.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/console.py` & `logfire-0.32.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/fallback.py` & `logfire-0.32.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/file.py` & `logfire-0.32.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/otlp.py` & `logfire-0.32.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.32.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.32.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.32.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/integrations/executors.py` & `logfire-0.32.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.32.0/logfire/_internal/integrations/fastapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import inspect
 from contextlib import contextmanager
 from functools import lru_cache
-from typing import Any, Callable, ContextManager, Iterable, Literal, cast
+from typing import Any, Awaitable, Callable, ContextManager, Iterable, cast
 from weakref import WeakKeyDictionary
 
 import fastapi.routing
 from fastapi import BackgroundTasks, FastAPI
 from fastapi.routing import APIRoute, APIWebSocketRoute
 from fastapi.security import SecurityScopes
 from starlette.requests import Request
@@ -84,19 +84,19 @@
 
 @lru_cache  # only patch once
 def patch_fastapi():
     """Globally monkeypatch fastapi functions and return a dictionary for recording instrumentation config per app."""
     registry: WeakKeyDictionary[FastAPI, FastAPIInstrumentation] = WeakKeyDictionary()
 
     async def patched_solve_dependencies(*, request: Request | WebSocket, **kwargs: Any):
-        result = await original_solve_dependencies(request=request, **kwargs)
+        original = original_solve_dependencies(request=request, **kwargs)
         if instrumentation := registry.get(request.app):
-            return await instrumentation.solve_dependencies(request, result)
+            return await instrumentation.solve_dependencies(request, original)
         else:
-            return result  # pragma: no cover
+            return await original  # pragma: no cover
 
     # `solve_dependencies` is actually defined in `fastapi.dependencies.utils`,
     # but it's imported into `fastapi.routing`, which is where we need to patch it.
     # It also calls itself recursively, but for now we don't want to intercept those calls,
     # so we don't patch it back into the original module.
     original_solve_dependencies = fastapi.routing.solve_dependencies  # type: ignore
     fastapi.routing.solve_dependencies = patched_solve_dependencies  # type: ignore
@@ -135,68 +135,81 @@
         # These lines, as well as the `excluded_urls_list.url_disabled` call below, are copied from OTEL.
         if excluded_urls is None:
             self.excluded_urls_list = get_excluded_urls('FASTAPI')
         else:
             self.excluded_urls_list = parse_excluded_urls(excluded_urls)  # pragma: no cover
 
     async def solve_dependencies(
-        self, request: Request | WebSocket, result: tuple[dict[str, Any], list[Any], Any, Any, Any]
+        self, request: Request | WebSocket, original: Awaitable[tuple[dict[str, Any], list[Any], Any, Any, Any]]
     ):
         try:
             url = cast(str, get_host_port_url_tuple(request.scope)[2])
-            if self.excluded_urls_list.url_disabled(url):
-                return result  # pragma: no cover
+            excluded = self.excluded_urls_list.url_disabled(url)
+        except Exception:  # pragma: no cover
+            excluded = False
+            self.logfire_instance.exception('Error checking if URL is excluded from instrumentation')
 
-            attributes: dict[str, Any] | None = {
-                # Shallow copy these so that the user can safely modify them, but we don't tell them that.
-                # We do explicitly tell them that the contents should not be modified.
-                # Making a deep copy could be very expensive and maybe even impossible.
-                'values': {
-                    k: v
-                    for k, v in result[0].items()
-                    if not isinstance(v, (Request, WebSocket, BackgroundTasks, SecurityScopes, Response))
-                },
-                'errors': result[1].copy(),
-            }
-
-            # Set the current app on `values` so that `patched_run_endpoint_function` can check it.
-            if isinstance(request, Request):  # pragma: no branch
-                instrumented_values = _InstrumentedValues(result[0])
-                instrumented_values.request = request
-                result = (instrumented_values, *result[1:])
-
-            attributes = self.request_attributes_mapper(request, attributes)
-            if not attributes:
-                # The user can return None to indicate that they don't want to log anything.
-                # We don't document it, but returning `False`, `{}` etc. seems like it should also work.
-                return result
-
-            # request_attributes_mapper may have removed the errors, so we need .get() here.
-            level: Literal['error', 'debug'] = 'error' if attributes.get('errors') else 'debug'
-
-            # Add a few basic attributes about the request, particularly so that the user can group logs by endpoint.
-            # Usually this will all be inside a span added by FastAPIInstrumentor with more detailed attributes.
-            # We only add these attributes after the request_attributes_mapper so that the user
-            # doesn't rely on what we add here - they can use `request` instead.
-            if isinstance(request, Request):  # pragma: no branch
-                attributes[SpanAttributes.HTTP_METHOD] = request.method
-            route: APIRoute | APIWebSocketRoute | None = request.scope.get('route')
-            if route:  # pragma: no branch
-                attributes.update(
-                    {
-                        SpanAttributes.HTTP_ROUTE: route.path,
-                        'fastapi.route.name': route.name,
-                    }
-                )
-                if isinstance(route, APIRoute):  # pragma: no branch
-                    attributes['fastapi.route.operation_id'] = route.operation_id
+        if excluded:
+            return await original  # pragma: no cover
 
-            self.logfire_instance.log(level, 'FastAPI arguments', attributes=attributes)
-        except Exception:  # pragma: no cover
-            self.logfire_instance.exception('Error logging FastAPI arguments')
+        with self.logfire_instance.span('FastAPI arguments') as span:
+            result = await original
+
+            try:
+                attributes: dict[str, Any] | None = {
+                    # Shallow copy these so that the user can safely modify them, but we don't tell them that.
+                    # We do explicitly tell them that the contents should not be modified.
+                    # Making a deep copy could be very expensive and maybe even impossible.
+                    'values': {
+                        k: v
+                        for k, v in result[0].items()
+                        if not isinstance(v, (Request, WebSocket, BackgroundTasks, SecurityScopes, Response))
+                    },
+                    'errors': result[1].copy(),
+                }
+
+                # Set the current app on `values` so that `patched_run_endpoint_function` can check it.
+                if isinstance(request, Request):  # pragma: no branch
+                    instrumented_values = _InstrumentedValues(result[0])
+                    instrumented_values.request = request
+                    result = (instrumented_values, *result[1:])
+
+                attributes = self.request_attributes_mapper(request, attributes)
+                if not attributes:
+                    # The user can return None to indicate that they don't want to log anything.
+                    # We don't document it, but returning `False`, `{}` etc. seems like it should also work.
+                    # We can't drop the span since it's already been created,
+                    # but we can set the level to debug so that it's hidden by default.
+                    span.set_level('debug')
+                    return result
+
+                # request_attributes_mapper may have removed the errors, so we need .get() here.
+                if attributes.get('errors'):
+                    span.set_level('error')
+
+                # Add a few basic attributes about the request, particularly so that the user can group logs by endpoint.
+                # Usually this will all be inside a span added by FastAPIInstrumentor with more detailed attributes.
+                # We only add these attributes after the request_attributes_mapper so that the user
+                # doesn't rely on what we add here - they can use `request` instead.
+                if isinstance(request, Request):  # pragma: no branch
+                    attributes[SpanAttributes.HTTP_METHOD] = request.method
+                route: APIRoute | APIWebSocketRoute | None = request.scope.get('route')
+                if route:  # pragma: no branch
+                    attributes.update(
+                        {
+                            SpanAttributes.HTTP_ROUTE: route.path,
+                            'fastapi.route.name': route.name,
+                        }
+                    )
+                    if isinstance(route, APIRoute):  # pragma: no branch
+                        attributes['fastapi.route.operation_id'] = route.operation_id
+
+                span.set_attributes(attributes)
+            except Exception as e:  # pragma: no cover
+                span.record_exception(e)
 
         return result
 
     async def run_endpoint_function(
         self,
         original_run_endpoint_function: Any,
         request: Request,
```

### Comparing `logfire-0.31.0/logfire/_internal/integrations/openai.py` & `logfire-0.32.0/logfire/_internal/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.32.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/integrations/logging.py` & `logfire-0.32.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/integrations/loguru.py` & `logfire-0.32.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/logfire/integrations/pydantic.py` & `logfire-0.32.0/logfire/integrations/pydantic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Integration for instrumenting Pydantic models."""
 
 from __future__ import annotations
 
 import functools
 import inspect
+import os
 import re
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Literal, TypedDict, TypeVar
 
+import pydantic
 from typing_extensions import ParamSpec
 
 import logfire
 from logfire import LogfireSpan
 
 from .._internal.config import GLOBAL_CONFIG, PydanticPlugin
 from .._internal.config_params import default_param_manager
+from .._internal.utils import get_version
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic import ValidationError
-    from pydantic.plugin import (
-        SchemaKind,
-        SchemaTypePath,
-    )
+    from pydantic.plugin import SchemaKind, SchemaTypePath
     from pydantic_core import CoreConfig, CoreSchema
 
 
 METER = GLOBAL_CONFIG._meter_provider.get_meter('pydantic-plugin-meter')  # type: ignore
 validation_counter = METER.create_counter('pydantic.validations')
 
 
@@ -288,69 +288,79 @@
         return schema['type']
 
 
 @dataclass
 class LogfirePydanticPlugin:
     """Implements a new API for pydantic plugins.
 
-    Patches pydantic to accept this new API shape.
-
-    Set the `LOGFIRE_DISABLE_PYDANTIC_PLUGIN` environment variable to `true` to disable the plugin.
-
-    Note:
-        In the future, you'll be able to use the `PYDANTIC_DISABLE_PLUGINS` instead.
+    Patches Pydantic to accept this new API shape.
 
-        See [pydantic/pydantic#7709](https://github.com/pydantic/pydantic/issues/7709) for more information.
+    Set the `LOGFIRE_PYDANTIC_RECORD` environment variable to `"off"` to disable the plugin, or
+    `PYDANTIC_DISABLE_PLUGINS` to `true` to disable all Pydantic plugins.
     """
 
-    def new_schema_validator(
-        self,
-        schema: CoreSchema,
-        schema_type: Any,
-        schema_type_path: SchemaTypePath,
-        schema_kind: SchemaKind,
-        config: CoreConfig | None,
-        plugin_settings: dict[str, Any],
-    ) -> tuple[_ValidateWrapper, ...] | tuple[None, ...]:
-        """This method is called every time a new `SchemaValidator` is created.
-
-        Args:
-            schema: The schema to validate against.
-            schema_type: The original type which the schema was created from, e.g. the model class.
-            schema_type_path: Path defining where `schema_type` was defined, or where `TypeAdapter` was called.
-            schema_kind: The kind of schema to validate against.
-            config: The config to use for validation.
-            plugin_settings: The plugin settings.
-
-        Returns:
-            A tuple of decorator factories for each of the three validation methods -
-                `validate_python`, `validate_json`, `validate_strings` or a tuple of
-                three `None` if recording is `off`.
-        """
-        # Patch a bug that occurs even if the plugin is disabled.
-        _patch_PluggableSchemaValidator()
-
-        logfire_settings = plugin_settings.get('logfire')
-        if logfire_settings and 'record' in logfire_settings:
-            record = logfire_settings['record']
-        else:
-            record = _pydantic_plugin_config().record
+    if (
+        get_version(pydantic.__version__) < get_version('2.5.0') or os.environ.get('LOGFIRE_PYDANTIC_RECORD') == 'off'
+    ):  # pragma: no cover
+
+        def new_schema_validator(  # type: ignore[reportRedeclaration]
+            self, *_: Any, **__: Any
+        ) -> tuple[_ValidateWrapper, ...] | tuple[None, ...]:
+            """Backwards compatibility for Pydantic < 2.5.0.
 
-        if record == 'off':
+            This method is called every time a new `SchemaValidator` is created, and is a NO-OP for Pydantic < 2.5.0.
+            """
             return None, None, None
+    else:
 
-        if _include_model(schema_type_path):
-            _patch_build_wrapper()
-            return (
-                _ValidateWrapper('validate_python', schema, config, plugin_settings, schema_type_path, record),
-                _ValidateWrapper('validate_json', schema, config, plugin_settings, schema_type_path, record),
-                _ValidateWrapper('validate_strings', schema, config, plugin_settings, schema_type_path, record),
-            )
+        def new_schema_validator(
+            self,
+            schema: CoreSchema,
+            schema_type: Any,
+            schema_type_path: SchemaTypePath,
+            schema_kind: SchemaKind,
+            config: CoreConfig | None,
+            plugin_settings: dict[str, Any],
+        ) -> tuple[_ValidateWrapper, ...] | tuple[None, ...]:
+            """This method is called every time a new `SchemaValidator` is created.
+
+            Args:
+                schema: The schema to validate against.
+                schema_type: The original type which the schema was created from, e.g. the model class.
+                schema_type_path: Path defining where `schema_type` was defined, or where `TypeAdapter` was called.
+                schema_kind: The kind of schema to validate against.
+                config: The config to use for validation.
+                plugin_settings: The plugin settings.
+
+            Returns:
+                A tuple of decorator factories for each of the three validation methods -
+                    `validate_python`, `validate_json`, `validate_strings` or a tuple of
+                    three `None` if recording is `off`.
+            """
+            # Patch a bug that occurs even if the plugin is disabled.
+            _patch_PluggableSchemaValidator()
+
+            logfire_settings = plugin_settings.get('logfire')
+            if logfire_settings and 'record' in logfire_settings:
+                record = logfire_settings['record']
+            else:
+                record = _pydantic_plugin_config().record
+
+            if record == 'off':
+                return None, None, None
+
+            if _include_model(schema_type_path):
+                _patch_build_wrapper()
+                return (
+                    _ValidateWrapper('validate_python', schema, config, plugin_settings, schema_type_path, record),
+                    _ValidateWrapper('validate_json', schema, config, plugin_settings, schema_type_path, record),
+                    _ValidateWrapper('validate_strings', schema, config, plugin_settings, schema_type_path, record),
+                )
 
-        return None, None, None
+            return None, None, None
 
 
 plugin = LogfirePydanticPlugin()
 
 # set of modules to ignore completely
 IGNORED_MODULES: tuple[str, ...] = 'fastapi', 'logfire_backend', 'fastui'
 IGNORED_MODULE_PREFIXES: tuple[str, ...] = tuple(f'{module}.' for module in IGNORED_MODULES)
```

### Comparing `logfire-0.31.0/logfire/integrations/structlog.py` & `logfire-0.32.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/conftest.py` & `logfire-0.32.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_auto_trace.py` & `logfire-0.32.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_backfill.py` & `logfire-0.32.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_cli.py` & `logfire-0.32.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -819,14 +819,67 @@
 
         assert json.loads((tmp_dir_cwd / '.logfire/logfire_credentials.json').read_text()) == {
             **create_project_response['json'],
             'logfire_api_url': 'https://logfire-api.pydantic.dev',
         }
 
 
+def test_projects_use_without_project_name(tmp_dir_cwd: Path, default_credentials: Path) -> None:
+    with ExitStack() as stack:
+        stack.enter_context(patch('logfire._internal.config.LogfireCredentials._get_user_token', return_value=''))
+        console = stack.enter_context(patch('logfire._internal.cli.Console'))
+        prompt_mock = stack.enter_context(patch('rich.prompt.Prompt.ask', side_effect=['1']))
+
+        m = requests_mock.Mocker()
+        stack.enter_context(m)
+        m.get(
+            'https://logfire-api.pydantic.dev/v1/projects/',
+            json=[
+                {'organization_name': 'fake_org', 'project_name': 'myproject'},
+                {'organization_name': 'fake_org', 'project_name': 'otherproject'},
+            ],
+        )
+        create_project_response = {
+            'json': {
+                'project_name': 'myproject',
+                'token': 'fake_token',
+                'project_url': 'fake_project_url',
+            }
+        }
+        m.post(
+            'https://logfire-api.pydantic.dev/v1/organizations/fake_org/projects/myproject/write-tokens/',
+            [create_project_response],
+        )
+
+        main(['projects', 'use'])
+
+        assert prompt_mock.mock_calls == [
+            call(
+                (
+                    'Please select one of the following projects by number:\n'
+                    '1. fake_org/myproject\n'
+                    '2. fake_org/otherproject\n'
+                ),
+                choices=['1', '2'],
+                default='1',
+            )
+        ]
+
+        console_calls = [re.sub(r'^call(\(\).)?', '', str(call)) for call in console.mock_calls]
+        assert console_calls == [
+            IsStr(regex=r'^\(file=.*'),
+            "print('Project configured successfully. You will be able to view it at: fake_project_url')",
+        ]
+
+        assert json.loads((tmp_dir_cwd / '.logfire/logfire_credentials.json').read_text()) == {
+            **create_project_response['json'],
+            'logfire_api_url': 'https://logfire-api.pydantic.dev',
+        }
+
+
 def test_projects_use_multiple(tmp_dir_cwd: Path, default_credentials: Path) -> None:
     with ExitStack() as stack:
         stack.enter_context(patch('logfire._internal.config.LogfireCredentials._get_user_token', return_value=''))
         console = stack.enter_context(patch('logfire._internal.cli.Console'))
         config_console = stack.enter_context(patch('logfire._internal.config.Console'))
         prompt_mock = stack.enter_context(patch('rich.prompt.Prompt.ask', side_effect=['1']))
```

### Comparing `logfire-0.31.0/tests/test_collect_package_resources.py` & `logfire-0.32.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_configure.py` & `logfire-0.32.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_console_exporter.py` & `logfire-0.32.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_formatter.py` & `logfire-0.32.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_json_args.py` & `logfire-0.32.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_json_args_formatting.py` & `logfire-0.32.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_logfire.py` & `logfire-0.32.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_loguru.py` & `logfire-0.32.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_metrics.py` & `logfire-0.32.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_no_production.py` & `logfire-0.32.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_pydantic_plugin.py` & `logfire-0.32.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_sampling.py` & `logfire-0.32.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_secret_scrubbing.py` & `logfire-0.32.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_slow_async_callbacks.py` & `logfire-0.32.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_source_code_extraction.py` & `logfire-0.32.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_stdlib_logging.py` & `logfire-0.32.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_structlog.py` & `logfire-0.32.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_testing.py` & `logfire-0.32.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/test_utils.py` & `logfire-0.32.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/utils.py` & `logfire-0.32.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.32.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/exporters/test_file_exporter.py` & `logfire-0.32.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/exporters/test_otlp_session.py` & `logfire-0.32.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/exporters/test_remove_pending.py` & `logfire-0.32.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.32.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.32.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_asgi.py` & `logfire-0.32.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.32.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_django.py` & `logfire-0.32.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.32.0/tests/otel_integrations/test_fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,78 +197,79 @@
                     'http.route': '/with_path_param/{param}',
                     'logfire.span_type': 'pending_span',
                     'logfire.msg': 'GET /with_path_param/param_val',
                     'logfire.pending_parent_id': '0000000000000000',
                 },
             },
             {
-                'name': '{method} {http.route} ({code.function}) (pending)',
+                'name': 'FastAPI arguments (pending)',
                 'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'start_time': 2000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'test_fastapi.py',
-                    'code.function': 'with_path_param',
-                    'code.lineno': 123,
-                    'method': 'GET',
-                    'http.route': '/with_path_param/{param}',
-                    'logfire.msg_template': '{method} {http.route} ({code.function})',
-                    'logfire.msg': 'GET /with_path_param/{param} (with_path_param)',
-                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000001',
                     'logfire.tags': ('fastapi',),
-                    'logfire.level_num': 5,
                 },
             },
             {
-                'name': '{method} {http.route} ({code.function})',
+                'name': 'FastAPI arguments',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
                 'end_time': 3000000000,
                 'attributes': {
-                    'code.filepath': 'test_fastapi.py',
-                    'code.function': 'with_path_param',
-                    'code.lineno': 123,
-                    'method': 'GET',
-                    'http.route': '/with_path_param/{param}',
-                    'logfire.msg_template': '{method} {http.route} ({code.function})',
-                    'logfire.msg': 'GET /with_path_param/{param} (with_path_param)',
-                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
                     'logfire.span_type': 'span',
                     'logfire.tags': ('fastapi',),
                     'logfire.level_num': 5,
                 },
             },
             {
-                'name': 'GET /with_path_param/{param} http send (pending)',
+                'name': '{method} {http.route} ({code.function}) (pending)',
                 'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'start_time': 4000000000,
                 'end_time': 4000000000,
                 'attributes': {
+                    'method': 'GET',
+                    'http.route': '/with_path_param/{param}',
+                    'code.filepath': 'test_fastapi.py',
+                    'code.function': 'with_path_param',
+                    'code.lineno': 123,
+                    'logfire.msg_template': '{method} {http.route} ({code.function})',
                     'logfire.span_type': 'pending_span',
-                    'logfire.msg': 'GET /with_path_param/{param} http send',
+                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
+                    'logfire.tags': ('fastapi',),
+                    'logfire.msg': 'GET /with_path_param/{param} (with_path_param)',
                     'logfire.level_num': 5,
                     'logfire.pending_parent_id': '0000000000000001',
                 },
             },
             {
-                'name': 'GET /with_path_param/{param} http send response.start',
+                'name': '{method} {http.route} ({code.function})',
                 'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 4000000000,
                 'end_time': 5000000000,
                 'attributes': {
+                    'method': 'GET',
+                    'http.route': '/with_path_param/{param}',
+                    'code.filepath': 'test_fastapi.py',
+                    'code.function': 'with_path_param',
+                    'code.lineno': 123,
+                    'logfire.msg_template': '{method} {http.route} ({code.function})',
                     'logfire.span_type': 'span',
-                    'logfire.msg': 'GET /with_path_param/{param} http send response.start',
-                    'http.status_code': 200,
-                    'type': 'http.response.start',
+                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
+                    'logfire.tags': ('fastapi',),
+                    'logfire.msg': 'GET /with_path_param/{param} (with_path_param)',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /with_path_param/{param} http send (pending)',
                 'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
@@ -278,32 +279,59 @@
                     'logfire.span_type': 'pending_span',
                     'logfire.msg': 'GET /with_path_param/{param} http send',
                     'logfire.level_num': 5,
                     'logfire.pending_parent_id': '0000000000000001',
                 },
             },
             {
-                'name': 'GET /with_path_param/{param} http send response.body',
+                'name': 'GET /with_path_param/{param} http send response.start',
                 'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 6000000000,
                 'end_time': 7000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
+                    'logfire.msg': 'GET /with_path_param/{param} http send response.start',
+                    'logfire.level_num': 5,
+                    'http.status_code': 200,
+                    'type': 'http.response.start',
+                },
+            },
+            {
+                'name': 'GET /with_path_param/{param} http send (pending)',
+                'context': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 8000000000,
+                'attributes': {
+                    'logfire.span_type': 'pending_span',
+                    'logfire.msg': 'GET /with_path_param/{param} http send',
+                    'logfire.level_num': 5,
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
+            },
+            {
+                'name': 'GET /with_path_param/{param} http send response.body',
+                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 9000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
                     'logfire.msg': 'GET /with_path_param/{param} http send response.body',
-                    'type': 'http.response.body',
                     'logfire.level_num': 5,
+                    'type': 'http.response.body',
                 },
             },
             {
                 'name': 'GET /with_path_param/{param}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 8000000000,
+                'end_time': 10000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /with_path_param/param_val',
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
@@ -370,129 +398,157 @@
                     'http.route': '/',
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000001',
                     'logfire.msg': 'GET /',
                 },
             },
             {
-                'name': '{method} {http.route} ({code.function}) (pending)',
+                'name': 'FastAPI arguments (pending)',
                 'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'start_time': 3000000000,
                 'end_time': 3000000000,
                 'attributes': {
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000003',
+                    'logfire.tags': ('fastapi',),
+                },
+            },
+            {
+                'name': 'FastAPI arguments',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.tags': ('fastapi',),
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
+                    'logfire.level_num': 5,
+                },
+            },
+            {
+                'name': '{method} {http.route} ({code.function}) (pending)',
+                'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'homepage',
                     'code.lineno': 123,
                     'method': 'GET',
                     'http.route': '/',
                     'logfire.msg_template': '{method} {http.route} ({code.function})',
-                    'logfire.msg': 'GET / (homepage)',
                     'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
                     'logfire.span_type': 'pending_span',
-                    'logfire.pending_parent_id': '0000000000000003',
+                    'logfire.msg': 'GET / (homepage)',
                     'logfire.tags': ('fastapi',),
                     'logfire.level_num': 5,
+                    'logfire.pending_parent_id': '0000000000000003',
                 },
             },
             {
                 'name': 'inside request handler',
-                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
-                'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
-                'start_time': 4000000000,
-                'end_time': 4000000000,
+                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'start_time': 6000000000,
+                'end_time': 6000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
-                    'logfire.level_num': 9,
                     'logfire.msg_template': 'inside request handler',
+                    'logfire.level_num': 9,
                     'logfire.msg': 'inside request handler',
-                    'code.lineno': 123,
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'homepage',
+                    'code.lineno': 123,
                 },
             },
             {
                 'name': '{method} {http.route} ({code.function})',
-                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 3000000000,
-                'end_time': 5000000000,
+                'start_time': 5000000000,
+                'end_time': 7000000000,
                 'attributes': {
+                    'method': 'GET',
+                    'http.route': '/',
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'homepage',
                     'code.lineno': 123,
-                    'method': 'GET',
-                    'http.route': '/',
                     'logfire.msg_template': '{method} {http.route} ({code.function})',
-                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
                     'logfire.span_type': 'span',
-                    'logfire.msg': 'GET / (homepage)',
+                    'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
                     'logfire.tags': ('fastapi',),
+                    'logfire.msg': 'GET / (homepage)',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET / http send (pending)',
-                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
-                'parent': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
-                'start_time': 6000000000,
-                'end_time': 6000000000,
+                'context': {'trace_id': 1, 'span_id': 11, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000003',
                     'logfire.level_num': 5,
                     'logfire.msg': 'GET / http send',
                 },
             },
             {
                 'name': 'GET / http send response.start',
-                'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 6000000000,
-                'end_time': 7000000000,
+                'start_time': 8000000000,
+                'end_time': 9000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET / http send response.start',
+                    'logfire.level_num': 5,
                     'http.status_code': 200,
                     'type': 'http.response.start',
-                    'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET / http send (pending)',
-                'context': {'trace_id': 1, 'span_id': 11, 'is_remote': False},
-                'parent': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
-                'start_time': 8000000000,
-                'end_time': 8000000000,
+                'context': {'trace_id': 1, 'span_id': 13, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 12, 'is_remote': False},
+                'start_time': 10000000000,
+                'end_time': 10000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
-                    'logfire.pending_parent_id': '0000000000000003',
-                    'logfire.level_num': 5,
                     'logfire.msg': 'GET / http send',
+                    'logfire.level_num': 5,
+                    'logfire.pending_parent_id': '0000000000000003',
                 },
             },
             {
                 'name': 'GET / http send response.body',
-                'context': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 12, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 8000000000,
-                'end_time': 9000000000,
+                'start_time': 10000000000,
+                'end_time': 11000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET / http send response.body',
-                    'type': 'http.response.body',
                     'logfire.level_num': 5,
+                    'type': 'http.response.body',
                 },
             },
             {
                 'name': 'GET /',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
-                'end_time': 10000000000,
+                'end_time': 12000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /',
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
@@ -508,22 +564,22 @@
                 },
             },
             {
                 'name': 'outside request handler',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 11000000000,
+                'end_time': 13000000000,
                 'attributes': {
-                    'code.lineno': 123,
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'test_fastapi_instrumentation',
+                    'code.lineno': 123,
                     'logfire.msg_template': 'outside request handler',
-                    'logfire.span_type': 'span',
                     'logfire.msg': 'outside request handler',
+                    'logfire.span_type': 'span',
                 },
             },
         ]
     )
 
 
 def test_fastapi_arguments(client: TestClient, exporter: TestExporter) -> None:
@@ -532,18 +588,18 @@
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'FastAPI arguments',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
-                'end_time': 2000000000,
+                'end_time': 3000000000,
                 'attributes': {
                     'custom_attr': 'custom_value',
-                    'logfire.span_type': 'log',
+                    'logfire.span_type': 'span',
                     'logfire.level_num': 17,
                     'logfire.msg_template': 'FastAPI arguments',
                     'logfire.msg': 'FastAPI arguments',
                     'values': '{"foo":"foo_val"}',
                     'errors': '[{"type":"int_parsing","loc":["query","bar"],"msg":"Input should be a valid integer, unable to parse string as an integer","input":"bar_val"}]',
                     'http.method': 'GET',
                     'http.route': '/other',
@@ -570,45 +626,45 @@
                         }
                     ),
                     'logfire.tags': ('fastapi',),
                 },
             },
             {
                 'name': 'GET /other http send response.start',
-                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 4000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /other http send response.start',
                     'http.status_code': 422,
                     'type': 'http.response.start',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /other http send response.body',
-                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 5000000000,
-                'end_time': 6000000000,
+                'start_time': 6000000000,
+                'end_time': 7000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /other http send response.body',
                     'type': 'http.response.body',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /other',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 7000000000,
+                'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /other',
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
@@ -630,51 +686,65 @@
 def test_fastapi_unhandled_exception(client: TestClient, exporter: TestExporter) -> None:
     with pytest.raises(ValueError):
         client.get('/exception')
 
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
-                'name': '{method} {http.route} ({code.function})',
+                'name': 'FastAPI arguments',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
-                'end_time': 4000000000,
+                'end_time': 3000000000,
                 'attributes': {
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
+                    'logfire.tags': ('fastapi',),
+                    'logfire.span_type': 'span',
+                    'logfire.level_num': 5,
+                },
+            },
+            {
+                'name': '{method} {http.route} ({code.function})',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 4000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'method': 'GET',
+                    'http.route': '/exception',
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'exception',
                     'code.lineno': 123,
-                    'method': 'GET',
-                    'http.route': '/exception',
                     'logfire.msg_template': '{method} {http.route} ({code.function})',
+                    'logfire.msg': 'GET /exception (exception)',
                     'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
-                    'logfire.span_type': 'span',
                     'logfire.tags': ('fastapi',),
-                    'logfire.msg': 'GET /exception (exception)',
+                    'logfire.span_type': 'span',
                     'logfire.level_num': 17,
                 },
                 'events': [
                     {
                         'name': 'exception',
-                        'timestamp': 3000000000,
+                        'timestamp': 5000000000,
                         'attributes': {
                             'exception.type': 'ValueError',
                             'exception.message': 'test exception',
                             'exception.stacktrace': 'ValueError: test exception',
                             'exception.escaped': 'True',
                         },
                     }
                 ],
             },
             {
                 'name': 'GET /exception',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 6000000000,
+                'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /exception',
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
@@ -686,15 +756,15 @@
                     'net.peer.ip': 'testclient',
                     'net.peer.port': 50000,
                     'http.route': '/exception',
                 },
                 'events': [
                     {
                         'name': 'exception',
-                        'timestamp': 5000000000,
+                        'timestamp': 7000000000,
                         'attributes': {
                             'exception.type': 'ValueError',
                             'exception.message': 'test exception',
                             'exception.stacktrace': 'ValueError: test exception',
                             'exception.escaped': 'False',
                         },
                     }
@@ -709,78 +779,92 @@
     # Our instrumentation still captures the exception as it happens in the endpoint.
     response = client.get('/validation_error')
     assert response.status_code == 422
 
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
-                'name': '{method} {http.route} ({code.function})',
+                'name': 'FastAPI arguments',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
-                'end_time': 4000000000,
+                'end_time': 3000000000,
                 'attributes': {
+                    'logfire.msg_template': 'FastAPI arguments',
+                    'logfire.msg': 'FastAPI arguments',
+                    'logfire.tags': ('fastapi',),
+                    'logfire.span_type': 'span',
+                    'logfire.level_num': 5,
+                },
+            },
+            {
+                'name': '{method} {http.route} ({code.function})',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 4000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'method': 'GET',
+                    'http.route': '/validation_error',
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'validation_error',
                     'code.lineno': 123,
-                    'method': 'GET',
-                    'http.route': '/validation_error',
                     'logfire.msg_template': '{method} {http.route} ({code.function})',
+                    'logfire.msg': 'GET /validation_error (validation_error)',
                     'logfire.json_schema': '{"type":"object","properties":{"method":{},"http.route":{}}}',
+                    'logfire.tags': ('fastapi',),
                     'logfire.span_type': 'span',
-                    'logfire.msg': 'GET /validation_error (validation_error)',
                     'logfire.level_num': 17,
-                    'logfire.tags': ('fastapi',),
                 },
                 'events': [
                     {
                         'name': 'exception',
-                        'timestamp': 3000000000,
+                        'timestamp': 5000000000,
                         'attributes': {
                             'exception.type': 'RequestValidationError',
                             'exception.message': '[]',
                             'exception.stacktrace': 'fastapi.exceptions.RequestValidationError: []',
                             'exception.escaped': 'True',
                         },
                     }
                 ],
             },
             {
                 'name': 'GET /validation_error http send response.start',
-                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 5000000000,
-                'end_time': 6000000000,
+                'start_time': 7000000000,
+                'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /validation_error http send response.start',
+                    'logfire.level_num': 5,
                     'http.status_code': 422,
                     'type': 'http.response.start',
-                    'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /validation_error http send response.body',
-                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 7000000000,
-                'end_time': 8000000000,
+                'start_time': 9000000000,
+                'end_time': 10000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /validation_error http send response.body',
-                    'type': 'http.response.body',
                     'logfire.level_num': 5,
+                    'type': 'http.response.body',
                 },
             },
             {
                 'name': 'GET /validation_error',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 9000000000,
+                'end_time': 11000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /validation_error',
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
@@ -812,18 +896,17 @@
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'FastAPI arguments',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
-                'end_time': 2000000000,
+                'end_time': 3000000000,
                 'attributes': {
-                    'logfire.span_type': 'log',
-                    'logfire.level_num': 5,
+                    'logfire.span_type': 'span',
                     'logfire.msg_template': 'FastAPI arguments',
                     'logfire.msg': 'FastAPI arguments',
                     'values': '{"path_param": "[Redacted due to \'auth\']", "foo": "foo_val", "password": "[Redacted due to \'password\']", "testauthorization": "[Redacted due to \'auth\']"}',
                     'errors': '[]',
                     'custom_attr': 'custom_value',
                     'http.method': 'GET',
                     'http.route': '/secret/{path_param}',
@@ -831,18 +914,18 @@
                     'logfire.null_args': ('fastapi.route.operation_id',),
                     'logfire.json_schema': '{"type":"object","properties":{"values":{"type":"object"},"errors":{"type":"array"},"custom_attr":{},"http.method":{},"http.route":{},"fastapi.route.name":{},"fastapi.route.operation_id":{}}}',
                     'logfire.tags': ('fastapi',),
                 },
             },
             {
                 'name': '{method} {http.route} ({code.function})',
-                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 4000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'test_fastapi.py',
                     'code.function': 'get_secret',
                     'code.lineno': 123,
                     'method': 'GET',
                     'http.route': '/secret/{path_param}',
                     'logfire.msg_template': '{method} {http.route} ({code.function})',
@@ -851,45 +934,45 @@
                     'logfire.tags': ('fastapi',),
                     'logfire.level_num': 5,
                     'logfire.span_type': 'span',
                 },
             },
             {
                 'name': 'GET /secret/{path_param} http send response.start',
-                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 5000000000,
-                'end_time': 6000000000,
+                'start_time': 6000000000,
+                'end_time': 7000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /secret/{path_param} http send response.start',
                     'http.status_code': 200,
                     'type': 'http.response.start',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /secret/{path_param} http send response.body',
-                'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
+                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 7000000000,
-                'end_time': 8000000000,
+                'start_time': 8000000000,
+                'end_time': 9000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': 'GET /secret/{path_param} http send response.body',
                     'type': 'http.response.body',
                     'logfire.level_num': 5,
                 },
             },
             {
                 'name': 'GET /secret/{path_param}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
-                'end_time': 9000000000,
+                'end_time': 10000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg': "GET /secret/test_auth ? foo='foo_val' & password='hunter2'",
                     'http.scheme': 'http',
                     'http.host': 'testserver',
                     'net.host.port': 80,
                     'http.flavor': '1.1',
```

### Comparing `logfire-0.31.0/tests/otel_integrations/test_flask.py` & `logfire-0.32.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_httpx.py` & `logfire-0.32.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_openai.py` & `logfire-0.32.0/tests/otel_integrations/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                         created=1,
                         model='gpt-4',
                         object='chat.completion.chunk',
                     ),
                     cc_chunk.ChatCompletionChunk(
                         id='2',
                         choices=[
-                            cc_chunk.Choice(index=1, delta=cc_chunk.ChoiceDelta(content=' is Nine', role='assistant'))
+                            cc_chunk.Choice(index=1, delta=cc_chunk.ChoiceDelta(content=' is secret', role='assistant'))
                         ],
                         created=1,
                         model='gpt-4',
                         object='chat.completion.chunk',
                     ),
                     cc_chunk.ChatCompletionChunk(
                         id='3',
@@ -476,15 +476,15 @@
         messages=[
             {'role': 'system', 'content': 'You are a helpful assistant.'},
             {'role': 'user', 'content': 'What is four plus five?'},
         ],
         stream=True,
     )
     combined = ''.join(chunk.choices[0].delta.content for chunk in response if chunk.choices[0].delta.content)
-    assert combined == 'The answer is Nine'
+    assert combined == 'The answer is secret'
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
@@ -514,15 +514,15 @@
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': '<genexpr>',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
-                    'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
+                    'response_data': '{"combined_chunk_content":"The answer is secret","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
@@ -535,15 +535,15 @@
             {'role': 'system', 'content': 'You are a helpful assistant.'},
             {'role': 'user', 'content': 'What is four plus five?'},
         ],
         stream=True,
     )
     chunk_content = [chunk.choices[0].delta.content async for chunk in response if chunk.choices[0].delta.content]
     combined = ''.join(chunk_content)
-    assert combined == 'The answer is Nine'
+    assert combined == 'The answer is secret'
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
@@ -573,15 +573,15 @@
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_async_chat_completions_stream',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
-                    'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
+                    'response_data': '{"combined_chunk_content":"The answer is secret","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
```

### Comparing `logfire-0.31.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.32.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_requests.py` & `logfire-0.32.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.32.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_starlette.py` & `logfire-0.32.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.32.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.32.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/LICENSE` & `logfire-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/README.md` & `logfire-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.31.0/pyproject.toml` & `logfire-0.32.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.31.0"
+version = "0.32.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.31.0/PKG-INFO` & `logfire-0.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.31.0
+Version: 0.32.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```


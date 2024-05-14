# Comparing `tmp/openbb_nightly-4.1.7.dev202405120010.tar.gz` & `tmp/openbb_nightly-4.1.7.dev202405130009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.7.dev202405120010.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.7.dev202405130009.tar", max compression
```

## Comparing `openbb_nightly-4.1.7.dev202405120010.tar` & `openbb_nightly-4.1.7.dev202405130009.tar`

### file list

```diff
@@ -1,791 +1,791 @@
--rw-r--r--   0        0        0     6818 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/README.md
--rw-r--r--   0        0        0       19 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    19033 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1908 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/api_settings.py
--rw-r--r--   0        0        0     1035 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      502 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2385 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1054 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/field.py
--rw-r--r--   0        0        0      694 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9240 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1477 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0      801 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/python_settings.py
--rw-r--r--   0        0        0       37 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     4044 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21634 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10402 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3511 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-05-12 00:10:37.182642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    66683 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2699 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     2121 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2702 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8297 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0     1377 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/available_indicators.py
--rw-r--r--   0        0        0      630 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1246 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     3722 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/country_profile.py
--rw-r--r--   0        0        0     1591 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      732 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1680 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/economic_indicators.py
--rw-r--r--   0        0        0     1750 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      912 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-05-12 00:10:37.186642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3073 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3526 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9699 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.190642 openbb_nightly-4.1.7.dev202405120010/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3605 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-05-12 00:10:37.198642 openbb_nightly-4.1.7.dev202405120010/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0    12007 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.202642 openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-05-12 00:10:37.206642 openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    63911 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0    21664 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    40926 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.210642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-05-12 00:10:37.214642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-05-12 00:10:37.230642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-05-12 00:10:37.250642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.250642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-05-12 00:10:37.254642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    26843 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3491 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0    16657 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
--rw-r--r--   0        0        0     1440 2024-05-12 00:10:37.258642 openbb_nightly-4.1.7.dev202405120010/openbb/__init__.py
--rw-r--r--   0        0        0  1244874 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/assets/reference.json
--rw-r--r--   0        0        0     2813 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/__extensions__.py
--rw-r--r--   0        0        0     3299 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/crypto.py
--rw-r--r--   0        0        0     6510 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    12915 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/currency.py
--rw-r--r--   0        0        0     6402 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12047 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    65943 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/economy.py
--rw-r--r--   0        0        0    12355 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27681 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity.py
--rw-r--r--   0        0        0    18353 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2807 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    25823 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    41180 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   164149 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30437 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26777 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3710 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75739 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/etf.py
--rw-r--r--   0        0        0     4538 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19482 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7001 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26229 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    10857 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11786 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/index.py
--rw-r--r--   0        0        0    20690 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/package/regulators.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/openbb/py.typed
--rw-r--r--   0        0        0     1452 2024-05-12 00:10:37.262642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5294 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      990 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    18109 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6206 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9807 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0     1609 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-05-12 00:10:37.266642 openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     2013 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8396 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9663 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8420 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4831 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     7796 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-05-12 00:10:37.270642 openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0     1122 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-05-12 00:10:37.274642 openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0     1199 2024-05-12 00:10:37.322642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/__init__.py
--rw-r--r--   0        0        0       21 2024-05-12 00:10:37.322642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/available_indicators.py
--rw-r--r--   0        0        0    12510 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/country_profile.py
--rw-r--r--   0        0        0    20336 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/economic_indicators.py
--rw-r--r--   0        0        0       24 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/__init__.py
--rw-r--r--   0        0        0    22209 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/helpers.py
--rw-r--r--   0        0        0    24368 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/indicator_countries.json
--rw-r--r--   0        0        0     5244 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
--rw-r--r--   0        0        0     8156 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/main_indicators.py
--rw-r--r--   0        0        0    66758 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/multipliers.json
--rw-r--r--   0        0        0    87109 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/scales.json
--rw-r--r--   0        0        0    73815 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
--rw-r--r--   0        0        0    90624 2024-05-12 00:10:37.326642 openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/units.json
--rw-r--r--   0        0        0     1117 2024-05-12 00:10:37.330642 openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-05-12 00:10:37.330642 openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-05-12 00:10:37.330642 openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3517 2024-05-12 00:10:37.330642 openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      834 2024-05-12 00:10:37.338642 openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-05-12 00:10:37.338642 openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-05-12 00:10:37.338642 openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-05-12 00:10:37.338642 openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-05-12 00:10:37.338642 openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1082 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9621 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8254 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    11039 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4385 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3932 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.394642 openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     9195 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2961 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5908 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5901 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     3208 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6082 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5924 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6114 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5314 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6499 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3452 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3162 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6772 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3623 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4304 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5056 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5832 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10619 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3527 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4238 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3276 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.398642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.402642 openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     4184 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2953 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6344 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6726 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2732 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-05-12 00:10:37.422643 openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0     1065 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5138 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-05-12 00:10:37.426643 openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5917 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22763 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     9166 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2939 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     9171 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2382 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4980 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7327 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29033 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8343 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8423 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9700 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5102 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3682 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12545 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3369 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6519 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     8655 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-05-12 00:10:37.430642 openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     2601 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5111 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5163 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-05-12 00:10:37.438643 openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0     1257 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2942 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     7039 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4606 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6289 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6261 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     5135 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     9871 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_snapshots.py
--rw-r--r--   0        0        0     7156 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6148 2024-05-12 00:10:37.446642 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-05-12 00:10:37.450643 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-05-12 00:10:37.450643 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.450643 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.450643 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-05-12 00:10:37.450643 openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1889 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1658 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0    10150 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     3154 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2681 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    39078 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2820 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2051 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2916 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3498 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1796 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    12574 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7587 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.466643 openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      669 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      737 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-05-12 00:10:37.554643 openbb_nightly-4.1.7.dev202405120010/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1352 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3657 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5313 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4680 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5341 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-12 00:10:37.558643 openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3411 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6306 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5166 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4653 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8853 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5461 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12481 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3644 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5093 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8463 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9711 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10349 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5996 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5132 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-05-12 00:10:37.570643 openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1807 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6588 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9228 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-05-12 00:10:37.670643 openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0     1023 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     5128 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1182 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4265 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2869 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3456 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3367 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6677 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5868 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3896 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10128 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4717 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4069 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-05-12 00:10:37.674643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10194 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4682 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4236 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6039 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-05-12 00:10:37.678643 openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     7021 2024-05-12 00:10:50.446695 openbb_nightly-4.1.7.dev202405120010/pyproject.toml
--rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405120010/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/README.md
+-rw-r--r--   0        0        0       19 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    19033 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:53.988248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2385 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9240 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21634 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10402 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    66683 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2699 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     2121 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2702 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8297 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-05-13 00:09:53.992248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      732 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1680 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-05-13 00:09:53.996248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3073 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3526 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.000248 openbb_nightly-4.1.7.dev202405130009/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3605 2024-05-13 00:09:54.004248 openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    12007 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.008248 openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.012248 openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    63911 2024-05-13 00:09:54.016248 openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    21664 2024-05-13 00:09:54.020248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-13 00:09:54.020248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-05-13 00:09:54.020248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.020248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-05-13 00:09:54.020248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-05-13 00:09:54.036248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-05-13 00:09:54.060248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0     1440 2024-05-13 00:09:54.064248 openbb_nightly-4.1.7.dev202405130009/openbb/__init__.py
+-rw-r--r--   0        0        0  1244874 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2813 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0     3299 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6510 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    12915 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/currency.py
+-rw-r--r--   0        0        0     6402 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12047 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    65943 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27681 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2807 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    41180 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   164149 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30437 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26777 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3710 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75739 2024-05-13 00:09:54.068248 openbb_nightly-4.1.7.dev202405130009/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19482 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7001 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11786 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/index.py
+-rw-r--r--   0        0        0    20690 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/package/regulators.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/openbb/py.typed
+-rw-r--r--   0        0        0     1452 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5294 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      990 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    18109 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6206 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9807 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-05-13 00:09:54.072248 openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0     1609 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     2013 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8396 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9663 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8420 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4831 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     7796 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-05-13 00:09:54.076248 openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0     1122 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-05-13 00:09:54.084248 openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0     1199 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/available_indicators.py
+-rw-r--r--   0        0        0    12510 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/country_profile.py
+-rw-r--r--   0        0        0    20336 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/economic_indicators.py
+-rw-r--r--   0        0        0       24 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/__init__.py
+-rw-r--r--   0        0        0    22209 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/helpers.py
+-rw-r--r--   0        0        0    24368 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/indicator_countries.json
+-rw-r--r--   0        0        0     5244 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
+-rw-r--r--   0        0        0     8156 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/main_indicators.py
+-rw-r--r--   0        0        0    66758 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/multipliers.json
+-rw-r--r--   0        0        0    87109 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/scales.json
+-rw-r--r--   0        0        0    73815 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
+-rw-r--r--   0        0        0    90624 2024-05-13 00:09:54.132248 openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/units.json
+-rw-r--r--   0        0        0     1117 2024-05-13 00:09:54.136248 openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-05-13 00:09:54.136248 openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-05-13 00:09:54.136248 openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3517 2024-05-13 00:09:54.136248 openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      834 2024-05-13 00:09:54.144248 openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-05-13 00:09:54.144248 openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-05-13 00:09:54.144248 openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-05-13 00:09:54.144248 openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-05-13 00:09:54.144248 openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1082 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9621 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8254 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    11039 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4385 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3932 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.200248 openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     9195 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2961 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5908 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5901 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     3208 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6082 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5924 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6114 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5314 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6499 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3452 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3162 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6772 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3623 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4304 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5056 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5832 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-05-13 00:09:54.204248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10619 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3527 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4238 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3276 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.208248 openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     4184 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2953 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6344 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6726 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2732 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-05-13 00:09:54.228248 openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0     1065 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5138 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-13 00:09:54.232248 openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5917 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22763 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     9166 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2939 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     9171 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2382 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4980 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29033 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8343 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8423 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9700 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5102 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3682 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12545 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3369 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6519 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     8655 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-05-13 00:09:54.236248 openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     2601 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5111 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5163 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-05-13 00:09:54.244248 openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0     1257 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2942 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     7039 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4606 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6289 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6261 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     5135 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9871 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7156 2024-05-13 00:09:54.252248 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6148 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-05-13 00:09:54.256249 openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1889 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10150 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     3154 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    39078 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2820 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2916 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3498 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    12574 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.272249 openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      669 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1352 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3657 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5313 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4680 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5341 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-13 00:09:54.360249 openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3411 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6306 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5166 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4653 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8853 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5461 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12481 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3644 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5093 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8463 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9711 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10349 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5996 2024-05-13 00:09:54.372249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5132 2024-05-13 00:09:54.376249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.376249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-05-13 00:09:54.376249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-05-13 00:09:54.376249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-05-13 00:09:54.376249 openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1807 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6588 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9228 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-13 00:09:54.472249 openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0     1023 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     5128 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1182 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4265 2024-05-13 00:09:54.476249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2869 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3456 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3367 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6677 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5868 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3896 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10128 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4717 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4069 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10194 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4682 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4236 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6039 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-05-13 00:09:54.480249 openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     7021 2024-05-13 00:10:02.852276 openbb_nightly-4.1.7.dev202405130009/pyproject.toml
+-rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405130009/PKG-INFO
```

### Comparing `openbb_nightly-4.1.7.dev202405120010/README.md` & `openbb_nightly-4.1.7.dev202405130009/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/command_runner.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/api_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/field.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/field.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/python_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/python_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/query.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/router.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/package_builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/app/version.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/env.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/country_profile.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.7.dev202405130009/extensions/technical/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/colors.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405130009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/assets/reference.json` & `openbb_nightly-4.1.7.dev202405130009/openbb/assets/reference.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/__extensions__.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/crypto.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/crypto_price.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/currency.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/currency.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/currency_price.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/derivatives.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/economy.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/economy.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_compare.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_fundamental.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_price.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/etf.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/etf.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/index.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/openbb/package/news.py` & `openbb_nightly-4.1.7.dev202405130009/openbb/package/news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.7.dev202405130009/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/country_profile.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/indicator_countries.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/indicator_countries.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/main_indicators.py` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/main_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/multipliers.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/multipliers.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/scales.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/scales.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/econdb/openbb_econdb/utils/units.json` & `openbb_nightly-4.1.7.dev202405130009/providers/econdb/openbb_econdb/utils/units.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405130009/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.7.dev202405130009/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.7.dev202405130009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.7.dev202405130009/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405130009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.7.dev202405130009/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.7.dev202405130009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.7.dev202405130009/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405120010/pyproject.toml` & `openbb_nightly-4.1.7.dev202405130009/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.7.dev202405120010"
+version = "4.1.7.dev202405130009"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
```

### Comparing `openbb_nightly-4.1.7.dev202405120010/PKG-INFO` & `openbb_nightly-4.1.7.dev202405130009/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.7.dev202405120010
+Version: 4.1.7.dev202405130009
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


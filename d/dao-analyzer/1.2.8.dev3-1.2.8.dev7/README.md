# Comparing `tmp/dao_analyzer-1.2.8.dev3.tar.gz` & `tmp/dao-analyzer-1.2.8.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_analyzer-1.2.8.dev3.tar", last modified: Tue May 14 08:56:11 2024, max compression
+gzip compressed data, was "dao-analyzer-1.2.8.dev7.tar", last modified: Tue Sep  5 14:50:54 2023, max compression
```

## Comparing `dao_analyzer-1.2.8.dev3.tar` & `dao-analyzer-1.2.8.dev7.tar`

### file list

```diff
@@ -1,412 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.993669 dao_analyzer-1.2.8.dev3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.993669 dao_analyzer-1.2.8.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/.hintrc
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.981670 dao_analyzer-1.2.8.dev3/dao_analyzer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.993669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.993669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)   399465 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.997669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.001669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/i_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.005669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.009669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/about_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.009669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.009669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.009669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.009669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   418772 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.013669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.017669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.017669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.017669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.017669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.017669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.021669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   461806 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.021669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.021669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.021669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.025669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.025669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.025669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.029669 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)    65944 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/aragon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/callbacks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/cc-by.png
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/dao-analyzer_header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/dao-analyzer_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54135 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/daohaus.png
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/daostack.png
--rw-r--r--   0 runner    (1001) docker     (127)   101409 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/ico-github.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/img_header.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   129808 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/kaggle_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-GPL.png
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-erc.png
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-grasia.png
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-ministerio.png
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-ucm.png
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer.png
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer/web/matomo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 08:56:10.000000 dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.029669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/.eslintrc
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/_validate_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/DataPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-14 08:56:03.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (127)   369420 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/public/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:10.985669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/demo/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/DAOInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/DataPoint.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/dao_analyzer_components/webpack.demo.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/gunicorn_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/init.sh
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.033669 dao_analyzer-1.2.8.dev3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/scripts/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/archive/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   339476 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/archive/names.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/archive/uploadToKaggle.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/checkContinue.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/datawarehouseDiff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/printArrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/updateAragonNames.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/scripts/uploadDataWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/mocks/api_requester_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/mocks/unix_date_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/graphql/test_query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.037669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/transfers/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.041669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/requesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:11.045669 dao_analyzer-1.2.8.dev3/test/unit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 08:56:02.000000 dao_analyzer-1.2.8.dev3/test/unit/components/test_dao_info.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/
+-rw-r--r--   0 runner    (1001) docker     (999)      354 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (999)      103 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.479232 dao-analyzer-1.2.8.dev7/.github/
+-rw-r--r--   0 runner    (1001) docker     (999)      808 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.479232 dao-analyzer-1.2.8.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (999)     5759 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     2146 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (999)       40 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/.hintrc
+-rw-r--r--   0 runner    (1001) docker     (999)     5571 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (999)     7401 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (999)      871 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (999)     1100 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (999)    35149 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     9904 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     8673 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.471232 dao-analyzer-1.2.8.dev7/dao_analyzer/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.479232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/
+-rw-r--r--   0 runner    (1001) docker     (999)      197 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)       30 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      173 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2792 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/app.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.479232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16209 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      674 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1131 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1765 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2070 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1416 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2084 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)   399465 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.483232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6301 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      922 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3467 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3669 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2089 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1656 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)      138 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)      192 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2428 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1896 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1873 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2506 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2622 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3139 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3747 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4574 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5890 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/presentation/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/resources/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2486 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      669 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/query.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1167 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      864 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1839 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (999)      431 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1275 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2337 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/
+-rw-r--r--   0 runner    (1001) docker     (999)      270 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4510 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5023 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5678 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2090 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1889 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
+-rw-r--r--   0 runner    (1001) docker     (999)      778 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3731 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1647 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.487232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1150 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
+-rw-r--r--   0 runner    (1001) docker     (999)      265 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)      217 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1025 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1215 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4554 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1561 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4369 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (999)      159 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3432 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
+-rw-r--r--   0 runner    (1001) docker     (999)      748 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1290 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/about_view/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      675 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1645 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1817 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1361 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.491232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/
+-rw-r--r--   0 runner    (1001) docker     (999)      198 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1533 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3711 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
+-rw-r--r--   0 runner    (1001) docker     (999)      114 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
+-rw-r--r--   0 runner    (1001) docker     (999)      366 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2355 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1172 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4723 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1578 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4532 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3435 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1158 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
+-rw-r--r--   0 runner    (1001) docker     (999)      299 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
+-rw-r--r--   0 runner    (1001) docker     (999)      549 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2702 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9375 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3859 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6670 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      799 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/colors.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3467 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16026 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.495232 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      675 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1132 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1765 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2102 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2233 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2072 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)   418772 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6081 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      698 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3092 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2275 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2097 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1702 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)      138 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)      194 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2516 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2057 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2534 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3745 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3526 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3652 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1892 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2884 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1913 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5274 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/presentation/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/resources/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2577 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.499233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.503233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17742 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.503233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      678 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1134 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2974 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1912 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2276 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1914 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2569 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)   461806 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.503233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.503233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.503233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6965 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      858 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.507233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2258 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3340 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1910 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)      138 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (999)      185 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2588 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2066 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5229 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9374 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2021 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1588 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3001 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3706 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1950 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1954 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5611 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.507233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/presentation/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.507233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/resources/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3213 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.511233 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/
+-rw-r--r--   0 runner    (1001) docker     (999)     5571 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (999)    65944 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/aragon.png
+-rw-r--r--   0 runner    (1001) docker     (999)     1410 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/callbacks.js
+-rw-r--r--   0 runner    (1001) docker     (999)     1239 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/cc-by.png
+-rw-r--r--   0 runner    (1001) docker     (999)    18045 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg
+-rw-r--r--   0 runner    (1001) docker     (999)    36174 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (999)    54135 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/daohaus.png
+-rw-r--r--   0 runner    (1001) docker     (999)    16481 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/daostack.png
+-rw-r--r--   0 runner    (1001) docker     (999)   101409 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (999)    58578 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (999)     4434 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/ico-github.svg
+-rw-r--r--   0 runner    (1001) docker     (999)    17972 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/img_header.jpg
+-rw-r--r--   0 runner    (1001) docker     (999)   129808 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/kaggle_logo.png
+-rw-r--r--   0 runner    (1001) docker     (999)     3548 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-GPL.png
+-rw-r--r--   0 runner    (1001) docker     (999)    10979 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-erc.png
+-rw-r--r--   0 runner    (1001) docker     (999)     5475 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-grasia.png
+-rw-r--r--   0 runner    (1001) docker     (999)    12180 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-ministerio.png
+-rw-r--r--   0 runner    (1001) docker     (999)     7539 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-ucm.png
+-rw-r--r--   0 runner    (1001) docker     (999)     5910 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png
+-rw-r--r--   0 runner    (1001) docker     (999)     5333 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg
+-rw-r--r--   0 runner    (1001) docker     (999)     1393 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
+-rw-r--r--   0 runner    (1001) docker     (999)    10237 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (999)      722 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/logs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1222 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer/web/matomo.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.479232 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     9904 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    18845 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       58 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       13 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      450 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       37 2023-09-05 14:50:54.000000 dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.511233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (999)      431 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (999)     3666 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (999)      229 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (999)      523 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)      262 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)     1701 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/_validate_init.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.515233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (999)     1992 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1668 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1396 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1554 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3270 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      240 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (999)      562 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
+-rw-r--r--   0 runner    (1001) docker     (999)    14551 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (999)    19068 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (999)     5984 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (999)     2410 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (999)   369525 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (999)     2410 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/package.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.515233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/public/
+-rw-r--r--   0 runner    (1001) docker     (999)      303 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (999)       55 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      704 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.475232 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.515233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/demo/
+-rw-r--r--   0 runner    (1001) docker     (999)      345 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/demo/index.js
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.515233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.515233 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/
+-rw-r--r--   0 runner    (1001) docker     (999)     3002 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (999)     2810 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx
+-rw-r--r--   0 runner    (1001) docker     (999)      725 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
+-rw-r--r--   0 runner    (1001) docker     (999)     2099 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (999)      306 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (999)     3544 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (999)      319 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/dao_analyzer_components/webpack.demo.config.js
+-rw-r--r--   0 runner    (1001) docker     (999)      337 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      312 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/gunicorn_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)      197 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/init.sh
+-rw-r--r--   0 runner    (1001) docker     (999)      118 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/scripts/archive/
+-rw-r--r--   0 runner    (1001) docker     (999)      134 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/archive/README.txt
+-rw-r--r--   0 runner    (1001) docker     (999)   339476 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/archive/names.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (999)     1010 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/archive/uploadToKaggle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (999)     1790 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/checkContinue.sh
+-rwxr-xr-x   0 runner    (1001) docker     (999)     4349 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/datawarehouseDiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)      251 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (999)      111 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/printArrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)     1148 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/updateAragonNames.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)     2900 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/scripts/uploadDataWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2464 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1471 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/mocks/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      747 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/mocks/api_requester_mock.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2442 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/mocks/unix_date_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/apps/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.519233 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2834 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2086 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2076 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3456 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2734 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2602 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2593 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/graphql/test_query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2614 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/transfers/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.523233 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2077 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2123 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2856 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3788 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2981 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3818 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3690 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3407 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2199 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3935 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3105 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3112 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6252 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2107 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4086 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/requesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:50:54.527233 dao-analyzer-1.2.8.dev7/test/unit/components/
+-rw-r--r--   0 runner    (1001) docker     (999)      250 2023-09-05 14:50:41.000000 dao-analyzer-1.2.8.dev7/test/unit/components/test_dao_info.py
```

### Comparing `dao_analyzer-1.2.8.dev3/.github/dependabot.yml` & `dao-analyzer-1.2.8.dev7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/.github/workflows/ci.yml` & `dao-analyzer-1.2.8.dev7/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   dao_analyzer_components:
     runs-on: ubuntu-latest
     defaults:
       run:
         working-directory: dao_analyzer_components
     steps:
     - uses: actions/checkout@v4
-    - uses: actions/setup-node@v4
+    - uses: actions/setup-node@v3
     - uses: actions/setup-python@v4
       with:
         python-version: '3.10'
         cache: 'pip'
     - name: Install dash and other deps
       run: pip install -r requirements.txt
     - name: Runtime versions
@@ -40,15 +40,15 @@
     needs: [dao_analyzer_components]
     if: github.ref == 'refs/heads/develop' || github.ref == 'refs/heads/master'
     defaults:
       run:
         working-directory: dao_analyzer_components
     steps:
     - uses: actions/checkout@v4
-    - uses: actions/setup-node@v4
+    - uses: actions/setup-node@v3
       with:
         registry-url: 'https://registry.npmjs.org'
     - name: Download artifact
       uses: actions/download-artifact@v3
       with:
         name: dao_analyzer_components
         path: ./dao_analyzer_components/dao_analyzer_components/
```

### Comparing `dao_analyzer-1.2.8.dev3/.gitignore` & `dao-analyzer-1.2.8.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/ABOUT.md` & `dao-analyzer-1.2.8.dev7/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/CHANGELOG.md` & `dao-analyzer-1.2.8.dev7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/CITATION.cff` & `dao-analyzer-1.2.8.dev7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/Dockerfile` & `dao-analyzer-1.2.8.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/LICENSE` & `dao-analyzer-1.2.8.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/PKG-INFO` & `dao-analyzer-1.2.8.dev7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.2.8.dev3
+Version: 1.2.8.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -21,48 +21,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dao-scripts==1.1.9
-Requires-Dist: dash<2.6.0,>=2.5.0
-Requires-Dist: dash-bootstrap-components>=1.1.0
-Requires-Dist: Werkzeug<2.1.0
-Requires-Dist: flask>=2.0.2
-Requires-Dist: gql>=3.0.0a1
-Requires-Dist: millify>=0.1.1
-Requires-Dist: numpy>=1.17.3
-Requires-Dist: pandas>=1.3.4
-Requires-Dist: portalocker>=2.3.2
-Requires-Dist: pyarrow>=6.0.0
-Requires-Dist: requests>=2.26.0
-Requires-Dist: requests-cache>=0.8.1
-Requires-Dist: requests-toolbelt>=0.9.1
-Requires-Dist: tenacity>=8.0.0
-Requires-Dist: tqdm>=4.62.3
-Requires-Dist: plotly-calplot==0.1.13
 Provides-Extra: docker
-Requires-Dist: gunicorn>=20.1.0; extra == "docker"
-Requires-Dist: kaggle>=1.5.12; extra == "docker"
-Requires-Dist: zenodo-client>=0.3.0; extra == "docker"
 Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pandas-vet; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: dash[dev,testing]; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: pandas-vet; extra == "dev"
-Requires-Dist: selenium; extra == "dev"
+License-File: LICENSE
 
 <p align="center">
     <img src="./dao_analyzer/web/assets/github_logo.png"
         height="130">
 </p>
 <p align="center">
     <a href="https://pypi.org/project/dao-analyzer/">
@@ -246,34 +215,15 @@
     * [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/71296/0543.pdf).
 
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan. (2020). An overview of Decentralized Autonomous Organizations on the blockchain. Proceedings of the 16th International Symposium on Open Collaboration (Opensym 2020) 11:1-11:8. ACM. 
     * [Freely available here](https://opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf).
 
 ## Acknowledgements
 
-<div align="center">
-<img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ministerio.png?raw=true"
-     alt="Logo Ministerio de Ciencia e Innovación. Gobierno de España"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-erc.png?raw=true"
-     alt="Logotipo European Research Council"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-grasia.png?raw=true"
-     alt="Logo GRASIA UCM"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ucm.png?raw=true"
-     alt="Logo Universidad Complutense de Madrid"
-     style="max-height: 3em"
->
-</div>
-
-DAO-Analyzer is created under the umbrella of multiple research projects: 
-- Chain Community, funded by the Spanish Ministry of Science and Innovation ([RTI2018‐096820‐A‐I00](https://produccioncientifica.ucm.es/proyectos/48103/detalle)) and led by Javier Arroyo and Samer Hassan
-- P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
-- DAOapplications, funded by the Spanish Ministry of Science and Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria Cruz Valiente
+DAO-Analyzer is created under the umbrella of two research projects: Chain Community, funded by the Spanish Ministry of Science and Innovation (RTI2018‐096820‐A‐I00) and led by Javier Arroyo and Samer Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
 
 ## Cite as
 
 You can just cite one of our publications:
 
 > Javier Arroyo, David Davó, Elena Martínez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in Blockchain Organizations.". Companion Publication of the 2022 Conference on Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion). ACM, 193–196.
```

#### html2text {}

```diff
@@ -1,39 +1,24 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.8.dev3 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.8.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
 :: Typed Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: dao-
-scripts==1.1.9 Requires-Dist: dash<2.6.0,>=2.5.0 Requires-Dist: dash-bootstrap-
-components>=1.1.0 Requires-Dist: Werkzeug<2.1.0 Requires-Dist: flask>=2.0.2
-Requires-Dist: gql>=3.0.0a1 Requires-Dist: millify>=0.1.1 Requires-Dist:
-numpy>=1.17.3 Requires-Dist: pandas>=1.3.4 Requires-Dist: portalocker>=2.3.2
-Requires-Dist: pyarrow>=6.0.0 Requires-Dist: requests>=2.26.0 Requires-Dist:
-requests-cache>=0.8.1 Requires-Dist: requests-toolbelt>=0.9.1 Requires-Dist:
-tenacity>=8.0.0 Requires-Dist: tqdm>=4.62.3 Requires-Dist: plotly-
-calplot==0.1.13 Provides-Extra: docker Requires-Dist: gunicorn>=20.1.0; extra
-== "docker" Requires-Dist: kaggle>=1.5.12; extra == "docker" Requires-Dist:
-zenodo-client>=0.3.0; extra == "docker" Provides-Extra: dev Requires-Dist:
-build; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-hypothesis; extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist:
-pandas-vet; extra == "dev" Requires-Dist: twine; extra == "dev" Requires-Dist:
-dash[dev,testing]; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev" Requires-Dist: pandas-vet; extra ==
-"dev" Requires-Dist: selenium; extra == "dev"
+Content-Type: text/markdown Provides-Extra: docker Provides-Extra: dev License-
+File: LICENSE
                   [./dao_analyzer/web/assets/github_logo.png]
                 _[_P_y_P_I_]_[_D_O_I_ _1_0_._5_2_8_1_/_z_e_n_o_d_o_._7_6_6_9_6_8_9_._s_v_g_][License]
 # DAO-Analyzer It is a tool to visualize DAO metrics. Currently, it shows DAO
 from [DAOstack](https://daostack.io/), [DAOhaus](https://daohaus.club/), and
 [Aragon](https://aragon.org/). Web site: [http://dao-analyzer.science/](http://
 dao-analyzer.science/) ## Table of contents - [Set-up \& Running (Download
 app)](#set-up--running-download-app) - [How to run it?](#how-to-run-it) -
@@ -121,27 +106,20 @@
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
 blockchain. Proceedings of the 16th International Symposium on Open
 Collaboration (Opensym 2020) 11:1-11:8. ACM. * [Freely available here](https://
 opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf). ##
-Acknowledgements
-   [Logo Ministerio de Ciencia e InnovaciÃ³n. Gobierno de EspaÃ±a][Logotipo
-  European Research Council][Logo GRASIA UCM][Logo Universidad Complutense de
-                                    Madrid]
-DAO-Analyzer is created under the umbrella of multiple research projects: -
-Chain Community, funded by the Spanish Ministry of Science and Innovation (
-[RTI2018â096820âAâI00](https://produccioncientifica.ucm.es/proyectos/
-48103/detalle)) and led by Javier Arroyo and Samer Hassan - P2P Models, funded
-by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by
-Samer Hassan. - DAOapplications, funded by the Spanish Ministry of Science and
-Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/
-proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria
-Cruz Valiente ## Cite as You can just cite one of our publications: > Javier
-Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer
-Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. Or, if you want to explicitly cite the application: > Arroyo,
-Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, & MartÃ­nez Vicente, Elena.
-(2023). DAO Analyzer. Zenodo. https://doi.org/10.5281/zenodo.7669689
+Acknowledgements DAO-Analyzer is created under the umbrella of two research
+projects: Chain Community, funded by the Spanish Ministry of Science and
+Innovation (RTI2018â096820âAâI00) and led by Javier Arroyo and Samer
+Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG
+625 grant no.: 75920), led by Samer Hassan. ## Cite as You can just cite one of
+our publications: > Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente,
+Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring
+Activity and Participation in Blockchain Organizations.". Companion Publication
+of the 2022 Conference on Computer Supported Cooperative Work and Social
+Computing (CSCW'22 Companion). ACM, 193â196. Or, if you want to explicitly
+cite the application: > Arroyo, Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, &
+MartÃ­nez Vicente, Elena. (2023). DAO Analyzer. Zenodo. https://doi.org/
+10.5281/zenodo.7669689
```

### Comparing `dao_analyzer-1.2.8.dev3/README.md` & `dao-analyzer-1.2.8.dev7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -184,34 +184,15 @@
     * [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/71296/0543.pdf).
 
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan. (2020). An overview of Decentralized Autonomous Organizations on the blockchain. Proceedings of the 16th International Symposium on Open Collaboration (Opensym 2020) 11:1-11:8. ACM. 
     * [Freely available here](https://opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf).
 
 ## Acknowledgements
 
-<div align="center">
-<img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ministerio.png?raw=true"
-     alt="Logo Ministerio de Ciencia e Innovación. Gobierno de España"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-erc.png?raw=true"
-     alt="Logotipo European Research Council"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-grasia.png?raw=true"
-     alt="Logo GRASIA UCM"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ucm.png?raw=true"
-     alt="Logo Universidad Complutense de Madrid"
-     style="max-height: 3em"
->
-</div>
-
-DAO-Analyzer is created under the umbrella of multiple research projects: 
-- Chain Community, funded by the Spanish Ministry of Science and Innovation ([RTI2018‐096820‐A‐I00](https://produccioncientifica.ucm.es/proyectos/48103/detalle)) and led by Javier Arroyo and Samer Hassan
-- P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
-- DAOapplications, funded by the Spanish Ministry of Science and Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria Cruz Valiente
+DAO-Analyzer is created under the umbrella of two research projects: Chain Community, funded by the Spanish Ministry of Science and Innovation (RTI2018‐096820‐A‐I00) and led by Javier Arroyo and Samer Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
 
 ## Cite as
 
 You can just cite one of our publications:
 
 > Javier Arroyo, David Davó, Elena Martínez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in Blockchain Organizations.". Companion Publication of the 2022 Conference on Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion). ACM, 193–196.
```

#### html2text {}

```diff
@@ -89,27 +89,20 @@
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
 blockchain. Proceedings of the 16th International Symposium on Open
 Collaboration (Opensym 2020) 11:1-11:8. ACM. * [Freely available here](https://
 opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf). ##
-Acknowledgements
-   [Logo Ministerio de Ciencia e InnovaciÃ³n. Gobierno de EspaÃ±a][Logotipo
-  European Research Council][Logo GRASIA UCM][Logo Universidad Complutense de
-                                    Madrid]
-DAO-Analyzer is created under the umbrella of multiple research projects: -
-Chain Community, funded by the Spanish Ministry of Science and Innovation (
-[RTI2018â096820âAâI00](https://produccioncientifica.ucm.es/proyectos/
-48103/detalle)) and led by Javier Arroyo and Samer Hassan - P2P Models, funded
-by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by
-Samer Hassan. - DAOapplications, funded by the Spanish Ministry of Science and
-Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/
-proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria
-Cruz Valiente ## Cite as You can just cite one of our publications: > Javier
-Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer
-Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. Or, if you want to explicitly cite the application: > Arroyo,
-Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, & MartÃ­nez Vicente, Elena.
-(2023). DAO Analyzer. Zenodo. https://doi.org/10.5281/zenodo.7669689
+Acknowledgements DAO-Analyzer is created under the umbrella of two research
+projects: Chain Community, funded by the Spanish Ministry of Science and
+Innovation (RTI2018â096820âAâI00) and led by Javier Arroyo and Samer
+Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG
+625 grant no.: 75920), led by Samer Hassan. ## Cite as You can just cite one of
+our publications: > Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente,
+Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring
+Activity and Participation in Blockchain Organizations.". Companion Publication
+of the 2022 Conference on Computer Supported Cooperative Work and Social
+Computing (CSCW'22 Companion). ACM, 193â196. Or, if you want to explicitly
+cite the application: > Arroyo, Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, &
+MartÃ­nez Vicente, Elena. (2023). DAO Analyzer. Zenodo. https://doi.org/
+10.5281/zenodo.7669689
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/app.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/app.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/app_service.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/class_diagram.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/aragon/resources/strings.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/aragon/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/query.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/query.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/api/graphql/query_builder.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/i_metric_adapter.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/singleton.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/singleton.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/organization/platform.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/serie.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/business/transfers/tabular_data.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/pandas_utils.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/irequester.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/about_view/about_view.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/main_view.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/colors.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/colors.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/common/resources/strings.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/common/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/app_service.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/class_diagram.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daohaus/resources/strings.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/app_service.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/class_diagram.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/apps/daostack/resources/strings.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/apps/daostack/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/ABOUT.md` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/aragon.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/aragon.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/callbacks.js` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/callbacks.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/cc-by.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/cc-by.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/dao-analyzer_header.svg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/dao-analyzer_logo.svg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/daohaus.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/daohaus.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/daostack.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/daostack.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/favicon.ico` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/github_logo.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/github_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/ico-github.svg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/ico-github.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/img_header.jpg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/img_header.jpg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/kaggle_logo.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/kaggle_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-GPL.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-GPL.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-erc.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-erc.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-grasia.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-grasia.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-ministerio.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-ministerio.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo-ucm.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo-ucm.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer.png` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer.svg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/assets/stylesheet.css` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/assets/stylesheet.css`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/logs.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/logs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer/web/matomo.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer/web/matomo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/PKG-INFO` & `dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.2.8.dev3
+Version: 1.2.8.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -21,48 +21,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dao-scripts==1.1.9
-Requires-Dist: dash<2.6.0,>=2.5.0
-Requires-Dist: dash-bootstrap-components>=1.1.0
-Requires-Dist: Werkzeug<2.1.0
-Requires-Dist: flask>=2.0.2
-Requires-Dist: gql>=3.0.0a1
-Requires-Dist: millify>=0.1.1
-Requires-Dist: numpy>=1.17.3
-Requires-Dist: pandas>=1.3.4
-Requires-Dist: portalocker>=2.3.2
-Requires-Dist: pyarrow>=6.0.0
-Requires-Dist: requests>=2.26.0
-Requires-Dist: requests-cache>=0.8.1
-Requires-Dist: requests-toolbelt>=0.9.1
-Requires-Dist: tenacity>=8.0.0
-Requires-Dist: tqdm>=4.62.3
-Requires-Dist: plotly-calplot==0.1.13
 Provides-Extra: docker
-Requires-Dist: gunicorn>=20.1.0; extra == "docker"
-Requires-Dist: kaggle>=1.5.12; extra == "docker"
-Requires-Dist: zenodo-client>=0.3.0; extra == "docker"
 Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pandas-vet; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: dash[dev,testing]; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: pandas-vet; extra == "dev"
-Requires-Dist: selenium; extra == "dev"
+License-File: LICENSE
 
 <p align="center">
     <img src="./dao_analyzer/web/assets/github_logo.png"
         height="130">
 </p>
 <p align="center">
     <a href="https://pypi.org/project/dao-analyzer/">
@@ -246,34 +215,15 @@
     * [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/71296/0543.pdf).
 
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan. (2020). An overview of Decentralized Autonomous Organizations on the blockchain. Proceedings of the 16th International Symposium on Open Collaboration (Opensym 2020) 11:1-11:8. ACM. 
     * [Freely available here](https://opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf).
 
 ## Acknowledgements
 
-<div align="center">
-<img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ministerio.png?raw=true"
-     alt="Logo Ministerio de Ciencia e Innovación. Gobierno de España"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-erc.png?raw=true"
-     alt="Logotipo European Research Council"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-grasia.png?raw=true"
-     alt="Logo GRASIA UCM"
-     style="max-height: 3em"
-><img src="https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/web/assets/logo-ucm.png?raw=true"
-     alt="Logo Universidad Complutense de Madrid"
-     style="max-height: 3em"
->
-</div>
-
-DAO-Analyzer is created under the umbrella of multiple research projects: 
-- Chain Community, funded by the Spanish Ministry of Science and Innovation ([RTI2018‐096820‐A‐I00](https://produccioncientifica.ucm.es/proyectos/48103/detalle)) and led by Javier Arroyo and Samer Hassan
-- P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
-- DAOapplications, funded by the Spanish Ministry of Science and Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria Cruz Valiente
+DAO-Analyzer is created under the umbrella of two research projects: Chain Community, funded by the Spanish Ministry of Science and Innovation (RTI2018‐096820‐A‐I00) and led by Javier Arroyo and Samer Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by Samer Hassan.
 
 ## Cite as
 
 You can just cite one of our publications:
 
 > Javier Arroyo, David Davó, Elena Martínez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in Blockchain Organizations.". Companion Publication of the 2022 Conference on Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion). ACM, 193–196.
```

#### html2text {}

```diff
@@ -1,39 +1,24 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.8.dev3 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.8.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
 :: Typed Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: dao-
-scripts==1.1.9 Requires-Dist: dash<2.6.0,>=2.5.0 Requires-Dist: dash-bootstrap-
-components>=1.1.0 Requires-Dist: Werkzeug<2.1.0 Requires-Dist: flask>=2.0.2
-Requires-Dist: gql>=3.0.0a1 Requires-Dist: millify>=0.1.1 Requires-Dist:
-numpy>=1.17.3 Requires-Dist: pandas>=1.3.4 Requires-Dist: portalocker>=2.3.2
-Requires-Dist: pyarrow>=6.0.0 Requires-Dist: requests>=2.26.0 Requires-Dist:
-requests-cache>=0.8.1 Requires-Dist: requests-toolbelt>=0.9.1 Requires-Dist:
-tenacity>=8.0.0 Requires-Dist: tqdm>=4.62.3 Requires-Dist: plotly-
-calplot==0.1.13 Provides-Extra: docker Requires-Dist: gunicorn>=20.1.0; extra
-== "docker" Requires-Dist: kaggle>=1.5.12; extra == "docker" Requires-Dist:
-zenodo-client>=0.3.0; extra == "docker" Provides-Extra: dev Requires-Dist:
-build; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-hypothesis; extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist:
-pandas-vet; extra == "dev" Requires-Dist: twine; extra == "dev" Requires-Dist:
-dash[dev,testing]; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: hypothesis; extra == "dev" Requires-Dist: pandas-vet; extra ==
-"dev" Requires-Dist: selenium; extra == "dev"
+Content-Type: text/markdown Provides-Extra: docker Provides-Extra: dev License-
+File: LICENSE
                   [./dao_analyzer/web/assets/github_logo.png]
                 _[_P_y_P_I_]_[_D_O_I_ _1_0_._5_2_8_1_/_z_e_n_o_d_o_._7_6_6_9_6_8_9_._s_v_g_][License]
 # DAO-Analyzer It is a tool to visualize DAO metrics. Currently, it shows DAO
 from [DAOstack](https://daostack.io/), [DAOhaus](https://daohaus.club/), and
 [Aragon](https://aragon.org/). Web site: [http://dao-analyzer.science/](http://
 dao-analyzer.science/) ## Table of contents - [Set-up \& Running (Download
 app)](#set-up--running-download-app) - [How to run it?](#how-to-run-it) -
@@ -121,27 +106,20 @@
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
 blockchain. Proceedings of the 16th International Symposium on Open
 Collaboration (Opensym 2020) 11:1-11:8. ACM. * [Freely available here](https://
 opensym.org/wp-content/uploads/2020/08/os20-paper-a11-el-faqir.pdf). ##
-Acknowledgements
-   [Logo Ministerio de Ciencia e InnovaciÃ³n. Gobierno de EspaÃ±a][Logotipo
-  European Research Council][Logo GRASIA UCM][Logo Universidad Complutense de
-                                    Madrid]
-DAO-Analyzer is created under the umbrella of multiple research projects: -
-Chain Community, funded by the Spanish Ministry of Science and Innovation (
-[RTI2018â096820âAâI00](https://produccioncientifica.ucm.es/proyectos/
-48103/detalle)) and led by Javier Arroyo and Samer Hassan - P2P Models, funded
-by the European Research Council (ERC-2017-STG 625 grant no.: 75920), led by
-Samer Hassan. - DAOapplications, funded by the Spanish Ministry of Science and
-Innovation ([PID2021-127956OB-I00](https://produccioncientifica.ucm.es/
-proyectos/551171/detalle)) and led by Javier Arroyo, Samer Hassan and maria
-Cruz Valiente ## Cite as You can just cite one of our publications: > Javier
-Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer
-Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. Or, if you want to explicitly cite the application: > Arroyo,
-Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, & MartÃ­nez Vicente, Elena.
-(2023). DAO Analyzer. Zenodo. https://doi.org/10.5281/zenodo.7669689
+Acknowledgements DAO-Analyzer is created under the umbrella of two research
+projects: Chain Community, funded by the Spanish Ministry of Science and
+Innovation (RTI2018â096820âAâI00) and led by Javier Arroyo and Samer
+Hassan; and P2P Models, funded by the European Research Council (ERC-2017-STG
+625 grant no.: 75920), led by Samer Hassan. ## Cite as You can just cite one of
+our publications: > Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente,
+Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-Analyzer: Exploring
+Activity and Participation in Blockchain Organizations.". Companion Publication
+of the 2022 Conference on Computer Supported Cooperative Work and Social
+Computing (CSCW'22 Companion). ACM, 193â196. Or, if you want to explicitly
+cite the application: > Arroyo, Javier, DavÃ³, David, Faqir-Rhazoui, Youssef, &
+MartÃ­nez Vicente, Elena. (2023). DAO Analyzer. Zenodo. https://doi.org/
+10.5281/zenodo.7669689
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer.egg-info/SOURCES.txt` & `dao-analyzer-1.2.8.dev7/dao_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/.eslintrc` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/.eslintrc`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/MANIFEST.in` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/_validate_init.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/_validate_init.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/DAOInfo.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/DataPoint.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/__init__.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
             var e = function(t) {
                     return /\/_dash-component-suites\//.test(t.src)
                 }(r()),
                 o = n(t);
             if (!e) return o;
             var i = o.split("/"),
                 a = i.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_23m1715676914"), i.splice(-1, 1, a.join(".")), i.join("/")
+            return a.splice(1, 0, "v0_0_23m1693925376"), i.splice(-1, 1, a.join(".")), i.join("/")
         }
     }
     var o = {};
     e.r(o), e.d(o, {
         DAOInfo: () => g,
         DataPoint: () => C,
         ParticipationStat: () => m,
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'sourcesContent'": "{insert: [(1, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc_ […]*

```diff
@@ -118,15 +118,15 @@
         "webpack:///./src/lib/components/ParticipationStat.jsx",
         "webpack:///./src/lib/components/DAOInfo.jsx",
         "webpack:///./src/lib/components/PlatformInfo.jsx",
         "webpack:///./src/lib/components/DataPoint.jsx"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1715676914\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1693925376\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
         "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n/** \n * This class will be used by DAOInfo and PlatformInfo\n */\nexport default class ParticipationStat extends Component {\n    render () {\n        const { text, value } = this.props;\n        if (value) {\n            return (<div><b>{value}</b> {text}</div>);\n        } else {\n            return (<div>{text}</div>);\n        }\n    }\n}\n\nParticipationStat.propTypes = {\n    /**\n     * The text to show\n     */\n    text: PropTypes.string.isRequired,\n\n    /**\n     * The value to highlight, which will be appended to text\n     */\n    value: PropTypes.string,\n\n    /**\n     * The key used by React for optimization\n     */\n    key: PropTypes.string,\n}\n",
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/metadata.json` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/dao_analyzer_components/package-info.json` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982051282051282%*

 * *Differences: {"'dependencies'": "{'ramda': '^0.29.0'}",*

 * * "'devDependencies'": "{'eslint-config-prettier': '^9.0.0', 'webpack-cli': '^5.1.4'}"}*

```diff
@@ -1,42 +1,42 @@
 {
     "author": "David Dav\u00f3 <ddavo@ucm.es>",
     "bugs": {
         "url": "https://github.com/Grasia/dao-analyzer/issues"
     },
     "dependencies": {
-        "ramda": "^0.28.0"
+        "ramda": "^0.29.0"
     },
     "description": "Components for dao-analyzer",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
         "@babel/preset-react": "^7.0.0",
         "@plotly/dash-component-plugins": "^1.2.0",
         "@plotly/webpack-dash-dynamic-import": "^1.2.0",
         "babel-eslint": "^10.0.2",
         "babel-loader": "^9.1.3",
         "copyfiles": "^2.1.1",
         "css-loader": "^6.7.1",
         "eslint": "^8.24.0",
-        "eslint-config-prettier": "^8.5.0",
+        "eslint-config-prettier": "^9.0.0",
         "eslint-plugin-import": "^2.18.0",
         "eslint-plugin-react": "^7.14.2",
         "is-published": "^0.2.0",
         "npm-watch": "^0.11.0",
         "prop-types": "^15.7.2",
         "react": "^18.2.0",
         "react-docgen": "^5.4.3",
         "react-dom": "^18.2.0",
         "style-loader": "^3.3.1",
         "styled-jsx": "^5.0.7",
         "terser-webpack-plugin": "^5.3.6",
         "webpack": "^5.74.0",
-        "webpack-cli": "^4.10.0",
+        "webpack-cli": "^5.1.4",
         "webpack-dev-server": "^4.11.1"
     },
     "engines": {
         "node": ">=8.11.0",
         "npm": ">=6.1.0"
     },
     "files": [
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/package-lock.json` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997903932005494%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'ramda': '^0.29.0'}, 'devDependencies': "*

 * *               "{'eslint-config-prettier': '^9.0.0', 'webpack-cli': '^5.1.4'}}, "*

 * *               "'node_modules/@webpack-cli/configtest': {'version': '2.1.1', 'resolved': "*

 * *               "'https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.1.1.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==', "*

 * *                […]*

```diff
@@ -1,41 +1,41 @@
 {
     "lockfileVersion": 3,
     "name": "dao-analyzer-components",
     "packages": {
         "": {
             "dependencies": {
-                "ramda": "^0.28.0"
+                "ramda": "^0.29.0"
             },
             "devDependencies": {
                 "@babel/core": "^7.5.4",
                 "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
                 "@babel/preset-env": "^7.5.4",
                 "@babel/preset-react": "^7.0.0",
                 "@plotly/dash-component-plugins": "^1.2.0",
                 "@plotly/webpack-dash-dynamic-import": "^1.2.0",
                 "babel-eslint": "^10.0.2",
                 "babel-loader": "^9.1.3",
                 "copyfiles": "^2.1.1",
                 "css-loader": "^6.7.1",
                 "eslint": "^8.24.0",
-                "eslint-config-prettier": "^8.5.0",
+                "eslint-config-prettier": "^9.0.0",
                 "eslint-plugin-import": "^2.18.0",
                 "eslint-plugin-react": "^7.14.2",
                 "is-published": "^0.2.0",
                 "npm-watch": "^0.11.0",
                 "prop-types": "^15.7.2",
                 "react": "^18.2.0",
                 "react-docgen": "^5.4.3",
                 "react-dom": "^18.2.0",
                 "style-loader": "^3.3.1",
                 "styled-jsx": "^5.0.7",
                 "terser-webpack-plugin": "^5.3.6",
                 "webpack": "^5.74.0",
-                "webpack-cli": "^4.10.0",
+                "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.11.1"
             },
             "engines": {
                 "node": ">=8.11.0",
                 "npm": ">=6.1.0"
             },
             "license": "GPL-3.0",
@@ -2488,47 +2488,55 @@
             "dev": true,
             "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
-            "integrity": "sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==",
+            "engines": {
+                "node": ">=14.15.0"
+            },
+            "integrity": "sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==",
             "peerDependencies": {
-                "webpack": "4.x.x || 5.x.x",
-                "webpack-cli": "4.x.x"
+                "webpack": "5.x.x",
+                "webpack-cli": "5.x.x"
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-1.2.0.tgz",
-            "version": "1.2.0"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.1.1.tgz",
+            "version": "2.1.1"
         },
         "node_modules/@webpack-cli/info": {
-            "dependencies": {
-                "envinfo": "^7.7.3"
-            },
             "dev": true,
-            "integrity": "sha512-e8tSXZpw2hPl2uMJY6fsMswaok5FdlGNRTktvFk2sD8RjH0hE2+XistawJx1vmKteh4NmGmNUrp+Tb2w+udPcQ==",
+            "engines": {
+                "node": ">=14.15.0"
+            },
+            "integrity": "sha512-zLHQdI/Qs1UyT5UBdWNqsARasIA+AaF8t+4u2aS2nEpBQh2mWIVb8qAklq0eUENnC5mOItrIB4LiS9xMtph18A==",
             "peerDependencies": {
-                "webpack-cli": "4.x.x"
+                "webpack": "5.x.x",
+                "webpack-cli": "5.x.x"
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/info/-/info-1.5.0.tgz",
-            "version": "1.5.0"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/info/-/info-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/@webpack-cli/serve": {
             "dev": true,
-            "integrity": "sha512-oxnCNGj88fL+xzV+dacXs44HcDwf1ovs3AuEzvP7mqXw7fQntqIhQ1BRmynh4qEKQSSSRSWVyXRjmTbZIX9V2Q==",
+            "engines": {
+                "node": ">=14.15.0"
+            },
+            "integrity": "sha512-lqaoKnRYBdo1UgDX8uF24AfGMifWK19TxPmM5FHc2vAGxrJ/qtyUyFBWoY1tISZdelsQ5fBcOusifo5o5wSJxQ==",
             "peerDependencies": {
-                "webpack-cli": "4.x.x"
+                "webpack": "5.x.x",
+                "webpack-cli": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-1.7.0.tgz",
-            "version": "1.7.0"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.5.tgz",
+            "version": "2.0.5"
         },
         "node_modules/@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -4017,20 +4025,20 @@
             "version": "8.48.0"
         },
         "node_modules/eslint-config-prettier": {
             "bin": {
                 "eslint-config-prettier": "bin/cli.js"
             },
             "dev": true,
-            "integrity": "sha512-SM8AMJdeQqRYT9O9zguiruQZaN7+z+E4eAP9oiLNGKMtomwaB1E9dcgUD6ZAn/eQAb52USbvezbiljfZUhbJcg==",
+            "integrity": "sha512-IcJsTkJae2S35pRsRAwoCE+925rJJStOdkKnLVgtE+tEpqU0EVVM7OqrwxqgptKdX29NUwC82I5pXsGFIgSevw==",
             "peerDependencies": {
                 "eslint": ">=7.0.0"
             },
-            "resolved": "https://registry.npmjs.org/eslint-config-prettier/-/eslint-config-prettier-8.10.0.tgz",
-            "version": "8.10.0"
+            "resolved": "https://registry.npmjs.org/eslint-config-prettier/-/eslint-config-prettier-9.0.0.tgz",
+            "version": "9.0.0"
         },
         "node_modules/eslint-import-resolver-node": {
             "dependencies": {
                 "debug": "^3.2.7",
                 "is-core-module": "^2.13.0",
                 "resolve": "^1.22.4"
             },
@@ -5457,19 +5465,19 @@
             "integrity": "sha512-Y+R5hJrzs52QCG2laLn4udYVnxsfny9CpOhNhUvk/SSSVyF6T27FzRbF0sroPidSu3X8oEAkOn2K804mjpt6UQ==",
             "resolved": "https://registry.npmjs.org/internal-slot/-/internal-slot-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/interpret": {
             "dev": true,
             "engines": {
-                "node": ">= 0.10"
+                "node": ">=10.13.0"
             },
-            "integrity": "sha512-Ju0Bz/cEia55xDwUWEa8+olFpCiQoypjnQySseKtmjNrnps3P+xfpUmGr90T7yjlVJmOtybRvPXhKMbHr+fWnw==",
-            "resolved": "https://registry.npmjs.org/interpret/-/interpret-2.2.0.tgz",
-            "version": "2.2.0"
+            "integrity": "sha512-6xwYfHbajpoF0xLW+iwLkhwgvLoZDfjYfoFNu8ftMoXINzwuymNLd9u/KmwtdT2GbR+/Cz66otEGEVVUHX9QLQ==",
+            "resolved": "https://registry.npmjs.org/interpret/-/interpret-3.1.1.tgz",
+            "version": "3.1.1"
         },
         "node_modules/ip": {
             "dev": true,
             "integrity": "sha512-WKa+XuLG1A1R0UWhl2+1XQSi+fZWMsYKffMZTTYsiZaUD8k2yDAj5atimTUD2TZkyCkNEeYE5NhFZmupOGtjYQ==",
             "resolved": "https://registry.npmjs.org/ip/-/ip-2.0.0.tgz",
             "version": "2.0.0"
         },
@@ -7602,17 +7610,17 @@
             "version": "1.2.3"
         },
         "node_modules/ramda": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/ramda"
             },
-            "integrity": "sha512-9QnLuG/kPVgWvMQ4aODhsBUFKOUmnbUnsSXACv+NCQZcHbeb+v8Lodp8OVxtRULN1/xOyYLLaL6npE6dMq5QTA==",
-            "resolved": "https://registry.npmjs.org/ramda/-/ramda-0.28.0.tgz",
-            "version": "0.28.0"
+            "integrity": "sha512-BBea6L67bYLtdbOqfp8f58fPMqEwx0doL+pAi8TZyp2YWz8R9G8z9x75CZI8W+ftqhFHCpEX2cRnUUXK130iKA==",
+            "resolved": "https://registry.npmjs.org/ramda/-/ramda-0.29.0.tgz",
+            "version": "0.29.0"
         },
         "node_modules/randombytes": {
             "dependencies": {
                 "safe-buffer": "^5.1.0"
             },
             "dev": true,
             "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
@@ -7741,23 +7749,23 @@
             },
             "integrity": "sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==",
             "resolved": "https://registry.npmjs.org/readdirp/-/readdirp-3.6.0.tgz",
             "version": "3.6.0"
         },
         "node_modules/rechoir": {
             "dependencies": {
-                "resolve": "^1.9.0"
+                "resolve": "^1.20.0"
             },
             "dev": true,
             "engines": {
-                "node": ">= 0.10"
+                "node": ">= 10.13.0"
             },
-            "integrity": "sha512-/njmZ8s1wVeR6pjTZ+0nCnv8SpZNRMT2D1RLOJQESlYFDBvwpTA4KWJpZ+sBJ4+vhjILRcK7JIFdGCdxEAAitg==",
-            "resolved": "https://registry.npmjs.org/rechoir/-/rechoir-0.7.1.tgz",
-            "version": "0.7.1"
+            "integrity": "sha512-/vxpCXddiX8NGfGO/mTafwjq4aFa/71pvamip0++IQk3zG8cbCj0fifNPrjjF1XMXUne91jL9OoxmdykoEtifQ==",
+            "resolved": "https://registry.npmjs.org/rechoir/-/rechoir-0.8.0.tgz",
+            "version": "0.8.0"
         },
         "node_modules/reflect.getprototypeof": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.2.0",
                 "es-abstract": "^1.22.1",
                 "get-intrinsic": "^1.2.1",
@@ -9352,63 +9360,61 @@
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
-                "@webpack-cli/configtest": "^1.2.0",
-                "@webpack-cli/info": "^1.5.0",
-                "@webpack-cli/serve": "^1.7.0",
+                "@webpack-cli/configtest": "^2.1.1",
+                "@webpack-cli/info": "^2.0.2",
+                "@webpack-cli/serve": "^2.0.5",
                 "colorette": "^2.0.14",
-                "commander": "^7.0.0",
+                "commander": "^10.0.1",
                 "cross-spawn": "^7.0.3",
+                "envinfo": "^7.7.3",
                 "fastest-levenshtein": "^1.0.12",
                 "import-local": "^3.0.2",
-                "interpret": "^2.2.0",
-                "rechoir": "^0.7.0",
+                "interpret": "^3.1.1",
+                "rechoir": "^0.8.0",
                 "webpack-merge": "^5.7.3"
             },
             "dev": true,
             "engines": {
-                "node": ">=10.13.0"
+                "node": ">=14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-NLhDfH/h4O6UOy+0LSso42xvYypClINuMNBVVzX4vX98TmTaTUxwRbXdhucbFMd2qLaCTcLq/PdYrvi8onw90w==",
+            "integrity": "sha512-pIDJHIEI9LR0yxHXQ+Qh95k2EvXpWzZ5l+d+jIo+RdSm9MiHfzazIxwwni/p7+x4eJZuvG1AJwgC4TNQ7NRgsg==",
             "peerDependencies": {
-                "webpack": "4.x.x || 5.x.x"
+                "webpack": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "@webpack-cli/generators": {
                     "optional": true
                 },
-                "@webpack-cli/migrate": {
-                    "optional": true
-                },
                 "webpack-bundle-analyzer": {
                     "optional": true
                 },
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-4.10.0.tgz",
-            "version": "4.10.0"
+            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.1.4.tgz",
+            "version": "5.1.4"
         },
         "node_modules/webpack-cli/node_modules/commander": {
             "dev": true,
             "engines": {
-                "node": ">= 10"
+                "node": ">=14"
             },
-            "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
-            "version": "7.2.0"
+            "integrity": "sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==",
+            "resolved": "https://registry.npmjs.org/commander/-/commander-10.0.1.tgz",
+            "version": "10.0.1"
         },
         "node_modules/webpack-dev-middleware": {
             "dependencies": {
                 "colorette": "^2.0.10",
                 "memfs": "^3.4.3",
                 "mime-types": "^2.1.31",
                 "range-parser": "^1.2.1",
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/package.json` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982051282051282%*

 * *Differences: {"'dependencies'": "{'ramda': '^0.29.0'}",*

 * * "'devDependencies'": "{'eslint-config-prettier': '^9.0.0', 'webpack-cli': '^5.1.4'}"}*

```diff
@@ -1,42 +1,42 @@
 {
     "author": "David Dav\u00f3 <ddavo@ucm.es>",
     "bugs": {
         "url": "https://github.com/Grasia/dao-analyzer/issues"
     },
     "dependencies": {
-        "ramda": "^0.28.0"
+        "ramda": "^0.29.0"
     },
     "description": "Components for dao-analyzer",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
         "@babel/preset-react": "^7.0.0",
         "@plotly/dash-component-plugins": "^1.2.0",
         "@plotly/webpack-dash-dynamic-import": "^1.2.0",
         "babel-eslint": "^10.0.2",
         "babel-loader": "^9.1.3",
         "copyfiles": "^2.1.1",
         "css-loader": "^6.7.1",
         "eslint": "^8.24.0",
-        "eslint-config-prettier": "^8.5.0",
+        "eslint-config-prettier": "^9.0.0",
         "eslint-plugin-import": "^2.18.0",
         "eslint-plugin-react": "^7.14.2",
         "is-published": "^0.2.0",
         "npm-watch": "^0.11.0",
         "prop-types": "^15.7.2",
         "react": "^18.2.0",
         "react-docgen": "^5.4.3",
         "react-dom": "^18.2.0",
         "style-loader": "^3.3.1",
         "styled-jsx": "^5.0.7",
         "terser-webpack-plugin": "^5.3.6",
         "webpack": "^5.74.0",
-        "webpack-cli": "^4.10.0",
+        "webpack-cli": "^5.1.4",
         "webpack-dev-server": "^4.11.1"
     },
     "engines": {
         "node": ">=8.11.0",
         "npm": ">=6.1.0"
     },
     "files": [
```

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/setup.py` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/DAOInfo.jsx` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/DataPoint.jsx` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/ParticipationStat.jsx` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/src/lib/components/PlatformInfo.jsx` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/dao_analyzer_components/webpack.config.js` & `dao-analyzer-1.2.8.dev7/dao_analyzer_components/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/archive/names.ipynb` & `dao-analyzer-1.2.8.dev7/scripts/archive/names.ipynb`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/archive/uploadToKaggle.sh` & `dao-analyzer-1.2.8.dev7/scripts/archive/uploadToKaggle.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/checkContinue.sh` & `dao-analyzer-1.2.8.dev7/scripts/checkContinue.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/datawarehouseDiff.py` & `dao-analyzer-1.2.8.dev7/scripts/datawarehouseDiff.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/updateAragonNames.py` & `dao-analyzer-1.2.8.dev7/scripts/updateAragonNames.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/scripts/uploadDataWarehouse.py` & `dao-analyzer-1.2.8.dev7/scripts/uploadDataWarehouse.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/setup.cfg` & `dao-analyzer-1.2.8.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/setup.py` & `dao-analyzer-1.2.8.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/mocks/api_requester_mock.py` & `dao-analyzer-1.2.8.dev7/test/mocks/api_requester_mock.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/mocks/unix_date_builder.py` & `dao-analyzer-1.2.8.dev7/test/mocks/unix_date_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/common/api/graphql/test_query_builder.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/common/api/graphql/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/common/business/transfers/test_organization.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/common/business/transfers/test_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.2.8.dev3/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py` & `dao-analyzer-1.2.8.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py`

 * *Files identical despite different names*


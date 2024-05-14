# Comparing `tmp/ffun-1.4.0.tar.gz` & `tmp/ffun-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.4.0.tar", max compression
+gzip compressed data, was "ffun-1.5.0.tar", max compression
```

## Comparing `ffun-1.4.0.tar` & `ffun-1.5.0.tar`

### file list

```diff
@@ -1,210 +1,230 @@
--rw-r--r--   0        0        0      344 2024-03-24 14:40:49.457107 ffun-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/api/__init__.py
--rw-r--r--   0        0        0    10249 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/api/entities.py
--rw-r--r--   0        0        0    13578 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/api/http_handlers.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/application.py
--rw-r--r--   0        0        0      390 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0     1001 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1238 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-03-24 14:40:49.457107 ffun-1.4.0/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/migrations.py
--rw-r--r--   0        0        0     3993 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     4551 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     4012 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     1131 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      779 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1719 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0     3766 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0      905 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     6728 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      250 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     1664 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     4734 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3512 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     2995 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     2737 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/__init__.py
--rw-r--r--   0        0        0     1297 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/entities.py
--rw-r--r--   0        0        0     1498 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     4676 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/operations.py
--rw-r--r--   0        0        0      294 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1412 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    11174 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/__init__.py
--rw-r--r--   0        0        0      882 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/background_loader.py
--rw-r--r--   0        0        0     9845 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/errors.py
--rw-r--r--   0        0        0      477 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     7271 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/markers/__init__.py
--rw-r--r--   0        0        0      150 2024-03-24 14:40:49.461107 ffun-1.4.0/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     1530 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3375 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     4196 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      551 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2355 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6776 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-03-24 14:40:49.465107 ffun-1.4.0/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0     4178 2024-03-24 14:40:56.957103 ffun-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-05-14 08:20:40.141923 ffun-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/api/entities.py
+-rw-r--r--   0        0        0    13578 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1333 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/entities.py
+-rw-r--r--   0        0        0      552 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/register.py
+-rw-r--r--   0        0        0     1442 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     4551 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6590 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     3811 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1719 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      641 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0     1091 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.141923 ffun-1.5.0/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      810 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     4734 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3512 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3035 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     2737 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/errors.py
+-rw-r--r--   0        0        0     1498 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1288 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      710 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1194 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5590 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/operations.py
+-rw-r--r--   0        0        0      294 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15557 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0    10644 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/domain.py
+-rw-r--r--   0        0        0      181 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/errors.py
+-rw-r--r--   0        0        0      477 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     7271 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/entities.py
+-rw-r--r--   0        0        0      855 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     2582 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/meta/domain.py
+-rw-r--r--   0        0        0     1639 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    12775 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      520 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      799 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1008 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-14 08:20:40.145923 ffun-1.5.0/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1919 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2833 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      560 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2355 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      966 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/errors.py
+-rw-r--r--   0        0        0      865 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/errors.py
+-rw-r--r--   0        0        0      851 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      732 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      534 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/errors.py
+-rw-r--r--   0        0        0      718 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-05-14 08:20:40.149923 ffun-1.5.0/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4263 2024-05-14 08:20:49.941999 ffun-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.0/PKG-INFO
```

### Comparing `ffun-1.4.0/ffun/api/entities.py` & `ffun-1.5.0/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/api/http_handlers.py` & `ffun-1.5.0/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/application/application.py` & `ffun-1.5.0/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/application/settings.py` & `ffun-1.5.0/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/application/user_settings.py` & `ffun-1.5.0/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/application/workers.py` & `ffun-1.5.0/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/auth/dependencies.py` & `ffun-1.5.0/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/auth/settings.py` & `ffun-1.5.0/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/auth/supertokens.py` & `ffun-1.5.0/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/cli/commands/configs.py` & `ffun-1.5.0/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/cli/commands/entries.py` & `ffun-1.5.0/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/cli/commands/failed_entries.py` & `ffun-1.5.0/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/cli/commands/supertokens.py` & `ffun-1.5.0/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/cli/commands/workers.py` & `ffun-1.5.0/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/conftest.py` & `ffun-1.5.0/ffun/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,10 +30,13 @@
 
 
 @pytest_asyncio.fixture(scope="session", autouse=True)
 async def prepare_db(
     app: AsyncGenerator[fastapi.FastAPI, None],
     event_loop: asyncio.AbstractEventLoop,
 ) -> AsyncGenerator[None, None]:
+    # database migrations may be in an inconsistent state
+    await migrations.rollback_all()
+
     await migrations.apply_all()
     yield
     await migrations.rollback_all()
```

### Comparing `ffun-1.4.0/ffun/core/api.py` & `ffun-1.5.0/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/background_tasks.py` & `ffun-1.5.0/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/errors.py` & `ffun-1.5.0/ffun/core/errors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/json.py` & `ffun-1.5.0/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/logging.py` & `ffun-1.5.0/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/middlewares.py` & `ffun-1.5.0/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/migrations.py` & `ffun-1.5.0/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/postgresql.py` & `ffun-1.5.0/ffun/core/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from psycopg.pq import ExecStatus
 from psycopg.rows import dict_row
 
 from ffun.core import logging
 
 logger = logging.get_module_logger()
 
+MAX_INTEGER = 2147483647
+
 POOL: psycopg_pool.AsyncConnectionPool | None = None
 
 
 DB_RESULT = list[dict[str, Any]]
 SQL_ARGUMENTS = dict[str, Any] | tuple[list[Any]]
```

### Comparing `ffun-1.4.0/ffun/core/register.py` & `ffun-1.5.0/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/sentry.py` & `ffun-1.5.0/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/tests/helpers.py` & `ffun-1.5.0/ffun/core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/core/utils.py` & `ffun-1.5.0/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds/domain.py` & `ffun-1.5.0/ffun/feeds/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 save_feed = operations.save_feed
 update_feed_info = operations.update_feed_info
 get_next_feeds_to_load = operations.get_next_feeds_to_load
 mark_feed_as_loaded = operations.mark_feed_as_loaded
 mark_feed_as_failed = operations.mark_feed_as_failed
 mark_feed_as_orphaned = operations.mark_feed_as_orphaned
 get_feeds = operations.get_feeds
+tech_remove_feed = operations.tech_remove_feed
 
 
 async def save_feeds(feeds: list[Feed]) -> list[uuid.UUID]:
     real_ids = []
 
     for feed in feeds:
         real_ids.append(await save_feed(feed))
```

### Comparing `ffun-1.4.0/ffun/feeds/entities.py` & `ffun-1.5.0/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.5.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.5.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds/operations.py` & `ffun-1.5.0/ffun/feeds/operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 from typing import Any, Iterable
 
 import psycopg
 
 from ffun.core import logging
 from ffun.core.postgresql import ExecuteType, execute, run_in_transaction
+from ffun.domain import urls as domain_urls
 from ffun.feeds.entities import Feed, FeedError, FeedState
 
 logger = logging.get_module_logger()
 
 
 def row_to_feed(row: dict[str, Any]) -> Feed:
     return Feed(
@@ -22,35 +23,38 @@
         title=row["title"],
         description=row["description"],
     )
 
 
 async def save_feed(feed: Feed) -> uuid.UUID:
     sql = """
-    INSERT INTO f_feeds (id, url, state, title, description)
-    VALUES (%(id)s, %(url)s, %(state)s, %(title)s, %(description)s)
+    INSERT INTO f_feeds (id, url, state, title, description, uid)
+    VALUES (%(id)s, %(url)s, %(state)s, %(title)s, %(description)s, %(uid)s)
     """
 
+    uid = domain_urls.url_to_uid(feed.url)
+
     try:
         await execute(
             sql,
             {
                 "id": feed.id,
                 "url": feed.url,
                 "state": feed.state,
                 "title": feed.title,
                 "description": feed.description,
+                "uid": uid,
             },
         )
 
         return feed.id
     except psycopg.errors.UniqueViolation as e:
-        logger.warning("unique_violation_while_saving_feed", feed_id=feed.id)
+        logger.warning("unique_violation_while_saving_feed", feed=feed)
 
-        result = await execute("SELECT id FROM f_feeds WHERE url = %(url)s", {"url": feed.url})
+        result = await execute("SELECT id FROM f_feeds WHERE uid = %(uid)s", {"uid": uid})
 
         if not result:
             raise NotImplementedError("something went wrong") from e
 
         assert isinstance(result[0]["id"], uuid.UUID)
 
         return result[0]["id"]
@@ -139,7 +143,16 @@
     FROM f_feeds
     WHERE id = ANY(%(ids)s)
     """
 
     rows = await execute(sql, {"ids": list(ids)})
 
     return [row_to_feed(row) for row in rows]
+
+
+async def tech_remove_feed(feed_id: uuid.UUID) -> None:
+    sql = """
+    DELETE FROM f_feeds
+    WHERE id = %(feed_id)s
+    """
+
+    await execute(sql, {"feed_id": feed_id})
```

### Comparing `ffun-1.4.0/ffun/feeds/tests/fixtures.py` & `ffun-1.5.0/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds/tests/test_operations.py` & `ffun-1.5.0/ffun/feeds/tests/test_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import random
 import uuid
 
 import pytest
 
 from ffun.core import utils
+from ffun.core.tests.helpers import TableSizeDelta
 from ffun.feeds import errors
 from ffun.feeds.domain import get_feed, save_feeds
 from ffun.feeds.entities import Feed, FeedError, FeedState
 from ffun.feeds.operations import (
     get_feeds,
     get_next_feeds_to_load,
     mark_feed_as_failed,
     mark_feed_as_loaded,
     mark_feed_as_orphaned,
     save_feed,
+    tech_remove_feed,
     update_feed_info,
 )
 from ffun.feeds.tests import make
 
 
 class TestSaveFeed:
     @pytest.mark.asyncio
@@ -38,14 +40,31 @@
         assert original_feed_id == saved_feed_id
 
         assert await get_feed(original_feed_id) == new_feed
 
         with pytest.raises(errors.NoFeedFound):
             await get_feed(cloned_feed.id)
 
+    @pytest.mark.asyncio
+    async def test_same_uid_different_urls(self, new_feed: Feed) -> None:
+        url_part = uuid.uuid4().hex
+
+        feed_1 = new_feed.replace(url=f"http://example.com/{url_part}")
+        feed_2 = new_feed.replace(id=uuid.uuid4(), url=f"https://example.com/{url_part}")
+
+        feed_1_id = await save_feed(feed_1)
+        feed_2_id = await save_feed(feed_2)
+
+        assert feed_1_id == feed_2_id
+
+        assert await get_feed(feed_1_id) == feed_1
+
+        with pytest.raises(errors.NoFeedFound):
+            await get_feed(feed_2.id)
+
 
 class TestGetNextFeedToLoad:
     @pytest.mark.asyncio
     async def test_find_new_feed(self, saved_feed_id: uuid.UUID) -> None:
         now = utils.now()
 
         found_feeds = await get_next_feeds_to_load(number=100500, loaded_before=now)
@@ -221,7 +240,21 @@
             feed_ids.append(feed_id)
 
         loaded_feeds = await get_feeds(feed_ids[1:-1])
 
         assert len(loaded_feeds) == n
 
         assert set(feed_ids[1:-1]) == {feed.id for feed in loaded_feeds}
+
+
+class TestTechRemoveFeed:
+    @pytest.mark.asyncio
+    async def test(self, saved_feed: Feed) -> None:
+        async with TableSizeDelta("f_feeds", delta=-1):
+            await tech_remove_feed(saved_feed.id)
+
+        with pytest.raises(errors.NoFeedFound):
+            await get_feed(saved_feed.id)
+
+    @pytest.mark.asyncio
+    async def test_no_feed(self) -> None:
+        await tech_remove_feed(uuid.uuid4())
```

### Comparing `ffun-1.4.0/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.5.0/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_collections/domain.py` & `ffun-1.5.0/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_collections/predefines.py` & `ffun-1.5.0/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.5.0/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_discoverer/domain.py` & `ffun-1.5.0/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.5.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/feeds_links/operations.py` & `ffun-1.5.0/ffun/feeds_links/operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,83 @@
 import uuid
 from typing import Any
 
 from ffun.core import logging
-from ffun.core.postgresql import execute
+from ffun.core.postgresql import ExecuteType, execute
 from ffun.feeds_links.entities import FeedLink
 
 logger = logging.get_module_logger()
 
 
 def row_to_feed_link(row: dict[str, Any]) -> FeedLink:
     return FeedLink(user_id=row["user_id"], feed_id=row["feed_id"], created_at=row["created_at"])
 
 
+# TODO: tests
 async def add_link(user_id: uuid.UUID, feed_id: uuid.UUID) -> None:
     sql = """
         INSERT INTO fl_links (id, user_id, feed_id)
         VALUES (%(id)s, %(user_id)s, %(feed_id)s)
         ON CONFLICT (user_id, feed_id) DO NOTHING
     """
 
     await execute(sql, {"id": uuid.uuid4(), "user_id": user_id, "feed_id": feed_id})
 
 
+# TODO: tests
 async def remove_link(user_id: uuid.UUID, feed_id: uuid.UUID) -> None:
     sql = """
         DELETE FROM fl_links WHERE user_id = %(user_id)s AND feed_id = %(feed_id)s
     """
 
     await execute(sql, {"user_id": user_id, "feed_id": feed_id})
 
 
+# TODO: tests
 async def get_linked_feeds(user_id: uuid.UUID) -> list[FeedLink]:
     sql = """
         SELECT * FROM fl_links WHERE user_id = %(user_id)s
     """
 
     result = await execute(sql, {"user_id": user_id})
 
     return [row_to_feed_link(row) for row in result]
 
 
+# TODO: tests
 async def get_linked_users(feed_id: uuid.UUID) -> list[uuid.UUID]:
     sql = """
         SELECT user_id FROM fl_links WHERE feed_id = %(feed_id)s
     """
 
     result = await execute(sql, {"feed_id": feed_id})
 
     return [row["user_id"] for row in result]
 
 
+# TODO: tests
 async def has_linked_users(feed_id: uuid.UUID) -> bool:
     sql = """
         SELECT 1 FROM fl_links WHERE feed_id = %(feed_id)s LIMIT 1
     """
 
     result = await execute(sql, {"feed_id": feed_id})
 
     return bool(result)
+
+
+async def tech_merge_feeds(execute: ExecuteType, from_feed_id: uuid.UUID, to_feed_id: uuid.UUID) -> None:
+    sql = """
+    DELETE FROM fl_links as fll
+    WHERE feed_id = %(from_feed_id)s
+          AND EXISTS (SELECT 1 FROM fl_links WHERE feed_id = %(to_feed_id)s AND user_id = fll.user_id)
+    """
+
+    await execute(sql, {"from_feed_id": from_feed_id, "to_feed_id": to_feed_id})
+
+    sql = """
+    UPDATE fl_links
+    SET feed_id = %(to_feed_id)s
+    WHERE feed_id = %(from_feed_id)s
+    """
+
+    await execute(sql, {"from_feed_id": from_feed_id, "to_feed_id": to_feed_id})
```

### Comparing `ffun-1.4.0/ffun/librarian/background_processors.py` & `ffun-1.5.0/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/domain.py` & `ffun-1.5.0/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.5.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.5.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any
 
 from psycopg import Connection
 from psycopg.rows import dict_row
 from pypika import PostgreSQLQuery
 from yoyo import step
 
-__depends__ = {"20240313_01_Yv74T-processors-pointers"}
+__depends__ = {"20240313_01_Yv74T-processors-pointers", "20240315_01_tWftt-optimize-l-entries"}
 
 
 def get_actual_entries(cursor: Any) -> set[uuid.UUID]:
     cursor.execute("SELECT id FROM l_entries")
 
     return {row["id"] for row in cursor.fetchall()}
```

### Comparing `ffun-1.4.0/ffun/librarian/operations.py` & `ffun-1.5.0/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/processors/base.py` & `ffun-1.5.0/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/processors/domain.py` & `ffun-1.5.0/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.5.0/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.5.0/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.5.0/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/settings.py` & `ffun-1.5.0/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/tests/fixtures.py` & `ffun-1.5.0/ffun/librarian/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/tests/make.py` & `ffun-1.5.0/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/tests/test_background_processors.py` & `ffun-1.5.0/ffun/librarian/tests/test_background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/tests/test_domain.py` & `ffun-1.5.0/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/librarian/tests/test_operations.py` & `ffun-1.5.0/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/domain.py` & `ffun-1.5.0/ffun/library/domain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import uuid
 
+from ffun.core.postgresql import ExecuteType, run_in_transaction
 from ffun.domain import urls as d_urls
 from ffun.feeds import domain as f_domain
 from ffun.library import operations
 from ffun.library.entities import Entry, EntryChange
 
 catalog_entries = operations.catalog_entries
 get_entries_by_ids = operations.get_entries_by_ids
 get_entries_by_filter = operations.get_entries_by_filter
 check_stored_entries_by_external_ids = operations.check_stored_entries_by_external_ids
 all_entries_iterator = operations.all_entries_iterator
 get_entries_after_pointer = operations.get_entries_after_pointer
+tech_move_entry = operations.tech_move_entry
 
 
 async def get_entry(entry_id: uuid.UUID) -> Entry:
     entries = await get_entries_by_ids([entry_id])
     found_entry = entries.get(entry_id)
     assert found_entry is not None
     return found_entry
@@ -31,7 +33,12 @@
         changes.append(
             EntryChange(id=entry.id, field="external_url", old_value=entry.external_url, new_value=new_external_url)
         )
         if apply:
             await operations.update_external_url(entry.id, new_external_url)
 
     return changes
+
+
+@run_in_transaction
+async def tech_remove_entries_by_feed_id(execute: ExecuteType, feed_id: uuid.UUID) -> None:
+    await operations.tech_remove_entries_by_feed_id(execute, feed_id)
```

### Comparing `ffun-1.4.0/ffun/library/entities.py` & `ffun-1.5.0/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.5.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.5.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.5.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.5.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/operations.py` & `ffun-1.5.0/ffun/library/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 import uuid
 from typing import Any, AsyncGenerator, Iterable
 
 import psycopg
 
 from ffun.core import logging
-from ffun.core.postgresql import execute
+from ffun.core.postgresql import ExecuteType, execute
+from ffun.library import errors
 from ffun.library.entities import Entry
 
 logger = logging.get_module_logger()
 
 
 sql_insert_entry = """
 INSERT INTO l_entries (id, feed_id, title, body,
@@ -139,7 +140,38 @@
     sql = """
     UPDATE l_entries
     SET external_url = %(url)s
     WHERE id = %(entity_id)s
     """
 
     await execute(sql, {"entity_id": entity_id, "url": url})
+
+
+async def tech_remove_entries_by_ids(execute: ExecuteType, entries_ids: Iterable[uuid.UUID]) -> None:
+    sql = """
+    DELETE FROM l_entries
+    WHERE id = ANY(%(entries_ids)s)
+    """
+
+    await execute(sql, {"entries_ids": list(entries_ids)})
+
+
+async def tech_remove_entries_by_feed_id(execute: ExecuteType, feed_id: uuid.UUID) -> None:
+    sql = """
+    DELETE FROM l_entries
+    WHERE feed_id = %(feed_id)s
+    """
+
+    await execute(sql, {"feed_id": feed_id})
+
+
+async def tech_move_entry(entry_id: uuid.UUID, feed_id: uuid.UUID) -> None:
+    sql = """
+    UPDATE l_entries
+    SET feed_id = %(feed_id)s
+    WHERE id = %(entry_id)s
+    """
+
+    try:
+        await execute(sql, {"entry_id": entry_id, "feed_id": feed_id})
+    except psycopg.errors.UniqueViolation as e:
+        raise errors.CanNotMoveEntryAlreadyInFeed(entry_id=entry_id, feed_id=feed_id) from e
```

### Comparing `ffun-1.4.0/ffun/library/tests/fixtures.py` & `ffun-1.5.0/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/tests/make.py` & `ffun-1.5.0/ffun/library/tests/make.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,7 +32,16 @@
     )
 
 
 async def n_entries(loaded_feed_id: uuid.UUID, n: int) -> dict[uuid.UUID, Entry]:
     new_entries = [fake_entry(loaded_feed_id) for _ in range(n)]
     await domain.catalog_entries(new_entries)
     return await domain.get_entries_by_ids([entry.id for entry in new_entries])  # type: ignore
+
+
+async def n_entries_list(loaded_feed_id: uuid.UUID, n: int) -> list[Entry]:
+    entries = await n_entries(loaded_feed_id, n)
+    result = list(entries.values())
+
+    result.sort(key=lambda entry: entry.cataloged_at, reverse=True)
+
+    return result
```

### Comparing `ffun-1.4.0/ffun/library/tests/test_domain.py` & `ffun-1.5.0/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/library/tests/test_operations.py` & `ffun-1.5.0/ffun/library/tests/test_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 import pytest_asyncio
 
 from ffun.core import utils
 from ffun.core.postgresql import execute
 from ffun.core.tests.helpers import TableSizeDelta, TableSizeNotChanged, assert_times_is_near
 from ffun.feeds import domain as f_domain
 from ffun.feeds.tests import make as f_make
+from ffun.library import errors
 from ffun.library.domain import get_entry
 from ffun.library.entities import Entry
 from ffun.library.operations import (
     all_entries_iterator,
     catalog_entries,
     check_stored_entries_by_external_ids,
     get_entries_after_pointer,
     get_entries_by_filter,
     get_entries_by_ids,
+    tech_move_entry,
+    tech_remove_entries_by_feed_id,
+    tech_remove_entries_by_ids,
     update_external_url,
 )
 from ffun.library.tests import make
 
 
 class TestCatalogEntries:
     @pytest.mark.asyncio
@@ -278,7 +282,111 @@
         await update_external_url(cataloged_entry.id, new_url)
 
         loaded_entry = await get_entry(cataloged_entry.id)
         assert loaded_entry.external_url == new_url
 
         loaded_another_entry = await get_entry(another_cataloged_entry.id)
         assert loaded_another_entry.external_url == another_cataloged_entry.external_url
+
+
+class TestTechMoveEntry:
+    @pytest.mark.asyncio
+    async def test_moved(
+        self, loaded_feed_id: uuid.UUID, another_loaded_feed_id: uuid.UUID, cataloged_entry: Entry
+    ) -> None:
+        async with TableSizeNotChanged("l_entries"):
+            await tech_move_entry(cataloged_entry.id, another_loaded_feed_id)
+
+        loaded_entry = await get_entry(cataloged_entry.id)
+
+        assert loaded_entry.feed_id == another_loaded_feed_id
+
+        assert cataloged_entry.replace(feed_id=another_loaded_feed_id) == loaded_entry
+
+    @pytest.mark.asyncio
+    async def test_feed_has_the_same_entry(
+        self, loaded_feed_id: uuid.UUID, another_loaded_feed_id: uuid.UUID, new_entry: Entry
+    ) -> None:
+        duplicated_entry = new_entry.replace(feed_id=another_loaded_feed_id, id=uuid.uuid4())
+
+        await catalog_entries([new_entry, duplicated_entry])
+
+        async with TableSizeNotChanged("l_entries"):
+            with pytest.raises(errors.CanNotMoveEntryAlreadyInFeed):
+                await tech_move_entry(duplicated_entry.id, loaded_feed_id)
+
+        loaded_entry = await get_entry(new_entry.id)
+
+        assert loaded_entry == new_entry.replace(cataloged_at=loaded_entry.cataloged_at)
+
+        loaded_duplicated_entries = await get_entry(duplicated_entry.id)
+
+        assert loaded_duplicated_entries == duplicated_entry.replace(
+            cataloged_at=loaded_duplicated_entries.cataloged_at
+        )
+
+
+class TestTechRemoveEntriesByIds:
+    @pytest.mark.asyncio
+    async def test_removed(self, loaded_feed_id: uuid.UUID, another_loaded_feed_id: uuid.UUID) -> None:
+        entries = await make.n_entries(loaded_feed_id, n=3)
+        another_entries = await make.n_entries(another_loaded_feed_id, n=3)
+
+        entries_list = list(entries.values())
+        another_entries_list = list(another_entries.values())
+
+        async with TableSizeDelta("l_entries", delta=-2):
+            await tech_remove_entries_by_ids(execute, [entries_list[0].id, another_entries_list[0].id])
+
+        loaded_entries = await get_entries_by_ids([entry.id for entry in entries_list + another_entries_list])
+
+        assert loaded_entries[entries_list[0].id] is None
+        assert loaded_entries[another_entries_list[0].id] is None
+
+    @pytest.mark.asyncio
+    async def test_no_entries(self) -> None:
+        async with TableSizeNotChanged("l_entries"):
+            await tech_remove_entries_by_ids(execute, [])
+            await tech_remove_entries_by_ids(execute, [uuid.uuid4()])
+
+    @pytest.mark.asyncio
+    async def test_already_removed(self, loaded_feed_id: uuid.UUID) -> None:
+        entries = await make.n_entries(loaded_feed_id, n=3)
+
+        entries_list = list(entries.values())
+
+        await tech_remove_entries_by_ids(execute, [entry.id for entry in entries_list])
+
+        async with TableSizeNotChanged("l_entries"):
+            await tech_remove_entries_by_ids(execute, [entry.id for entry in entries_list])
+
+
+class TestTechRemoveEntriesByFeedId:
+    @pytest.mark.asyncio
+    async def test_removed(self, loaded_feed_id: uuid.UUID, another_loaded_feed_id: uuid.UUID) -> None:
+        entries = await make.n_entries(loaded_feed_id, n=3)
+        another_entries = await make.n_entries(another_loaded_feed_id, n=3)
+
+        async with TableSizeDelta("l_entries", delta=-3):
+            await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
+
+        loaded_entries = await get_entries_by_ids([entry.id for entry in entries.values()])
+
+        assert loaded_entries == {entry.id: None for entry in entries.values()}
+
+        another_loaded_entries = await get_entries_by_ids([entry.id for entry in another_entries.values()])
+
+        assert another_loaded_entries == another_entries
+
+    @pytest.mark.asyncio
+    async def test_no_entries(self) -> None:
+        async with TableSizeNotChanged("l_entries"):
+            await tech_remove_entries_by_feed_id(execute, uuid.uuid4())
+
+    @pytest.mark.asyncio
+    async def test_already_removed(self, loaded_feed_id: uuid.UUID) -> None:
+        await make.n_entries(loaded_feed_id, n=3)
+
+        await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
+
+        async with TableSizeNotChanged("l_entries"):
+            await tech_remove_entries_by_feed_id(execute, loaded_feed_id)
```

### Comparing `ffun-1.4.0/ffun/loader/background_loader.py` & `ffun-1.5.0/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/loader/domain.py` & `ffun-1.5.0/ffun/loader/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ssl
 import uuid
 
 import anyio
 import httpx
+from furl import furl
 
 from ffun.core import logging, utils
 from ffun.feeds import domain as f_domain
 from ffun.feeds.entities import Feed, FeedError, FeedState
 from ffun.feeds_collections import domain as fc_domain
 from ffun.feeds_links import domain as fl_domain
 from ffun.library import domain as l_domain
@@ -182,23 +183,38 @@
     if not feed_info.entries:
         raise errors.LoadError(feed_error_code=FeedError.protocol_no_entries_in_feed)
 
     return feed_info
 
 
 # TODO: tests
-async def load_content_with_proxies(url: str) -> httpx.Response:
+async def load_content_with_proxies(url: str) -> httpx.Response:  # noqa: CCR001
+    url_object = furl(url)
+
     first_exception = None
 
-    for proxy in settings.proxies:
-        try:
-            return await load_content(url, proxy)
-        except Exception as e:
-            if first_exception is None:
-                first_exception = e
+    # We try different protocols because users often make mistakes in the urls
+    # to fix them we unity similar urls like http://example.com and https://example.com
+    # => we need to check both protocols
+    #
+    # For now it is straightforward solution, but it should work
+    # Most of the domains should support HTTPS => HTTP urls will not be used
+    # but in case of full problem with url, we'll be doing unnecessary requests
+    # and in case of HTTP-only urls we'll be doing unnecessary requests too
+    #
+    # TODO: build a separate system of choosing protocol for the url with caching and periodic checks
+    for protocol in ("https", "http"):
+        url_object.scheme = protocol
+
+        for proxy in settings.proxies:
+            try:
+                return await load_content(str(url_object), proxy)
+            except Exception as e:
+                if first_exception is None:
+                    first_exception = e
 
     # in case of error raise the first exception occurred
     # because we should use the most common proxy first
     raise first_exception  # type: ignore
 
 
 async def detect_orphaned(feed_id: uuid.UUID) -> bool:
```

### Comparing `ffun-1.4.0/ffun/loader/tests/test_domain.py` & `ffun-1.5.0/ffun/loader/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.5.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/markers/operations.py` & `ffun-1.5.0/ffun/markers/operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import uuid
 from typing import Iterable
 
 from ffun.core import logging
-from ffun.core.postgresql import execute
+from ffun.core.postgresql import ExecuteType, execute
 from ffun.markers.entities import Marker
 
 logger = logging.get_module_logger()
 
 
+# TODO: tests
 async def set_marker(user_id: uuid.UUID, marker: Marker, entry_id: uuid.UUID) -> None:
     sql = """
         INSERT INTO m_markers (id, user_id, marker, entry_id)
         VALUES (%(id)s, %(user_id)s, %(marker)s, %(entry_id)s)
         ON CONFLICT (user_id, marker, entry_id) DO NOTHING
     """
 
     await execute(sql, {"id": uuid.uuid4(), "user_id": user_id, "marker": marker, "entry_id": entry_id})
 
 
+# TODO: tests
 async def remove_marker(user_id: uuid.UUID, marker: Marker, entry_id: uuid.UUID) -> None:
     sql = """
         DELETE FROM m_markers
         WHERE user_id = %(user_id)s AND marker = %(marker)s AND entry_id = %(entry_id)s
     """
 
     await execute(sql, {"user_id": user_id, "marker": marker, "entry_id": entry_id})
 
 
+# TODO: tests
 async def get_markers(user_id: uuid.UUID, entries_ids: Iterable[uuid.UUID]) -> dict[uuid.UUID, set[Marker]]:
     sql = """
         SELECT entry_id, marker
         FROM m_markers
         WHERE user_id = %(user_id)s AND entry_id = ANY(%(entries_ids)s)
     """
 
@@ -44,7 +47,34 @@
 
         if entry_id not in result:
             result[entry_id] = set()
 
         result[entry_id].add(marker)
 
     return result
+
+
+async def tech_merge_markers(execute: ExecuteType, from_entry_id: uuid.UUID, to_entry_id: uuid.UUID) -> None:
+    sql = """
+        DELETE FROM m_markers AS m
+        WHERE entry_id = %(from_entry_id)s
+              AND EXISTS (SELECT 1 FROM m_markers WHERE entry_id = %(to_entry_id)s AND user_id = m.user_id)
+    """
+
+    await execute(sql, {"from_entry_id": from_entry_id, "to_entry_id": to_entry_id})
+
+    sql = """
+        UPDATE m_markers
+        SET entry_id = %(to_entry_id)s
+        WHERE entry_id = %(from_entry_id)s
+    """
+
+    await execute(sql, {"from_entry_id": from_entry_id, "to_entry_id": to_entry_id})
+
+
+async def remove_markers_for_entries(entries_ids: Iterable[uuid.UUID]) -> None:
+    sql = """
+        DELETE FROM m_markers
+        WHERE entry_id = ANY(%(entries_ids)s)
+    """
+
+    await execute(sql, {"entries_ids": list(entries_ids)})
```

### Comparing `ffun-1.4.0/ffun/ontology/domain.py` & `ffun-1.5.0/ffun/ontology/domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 from typing import Iterable
 
 from bidict import bidict
 
-from ffun.core.postgresql import transaction
+from ffun.core.postgresql import ExecuteType, execute, run_in_transaction, transaction
 from ffun.ontology import operations
 from ffun.ontology.entities import ProcessorTag, Tag, TagCategory, TagPropertyType
 from ffun.tags import converters
 
 _tags_cache: bidict[str, int] = bidict()
 
 
@@ -61,19 +61,19 @@
 
     async with transaction() as execute:
         await operations.apply_tags(execute, entry_id, processor_id, uids_to_ids.values())
         await operations.apply_tags_properties(execute, properties)
 
 
 async def get_tags_ids_for_entries(entries_ids: list[uuid.UUID]) -> dict[uuid.UUID, set[int]]:
-    return await operations.get_tags_for_entries(entries_ids)
+    return await operations.get_tags_for_entries(execute, entries_ids)
 
 
 async def get_tags_for_entries(entries_ids: list[uuid.UUID]) -> dict[uuid.UUID, set[str]]:
-    tags_ids = await operations.get_tags_for_entries(entries_ids)
+    tags_ids = await operations.get_tags_for_entries(execute, entries_ids)
 
     all_tags = set()
 
     for tags in tags_ids.values():
         all_tags.update(tags)
 
     tags_mapping = await get_tags_by_ids(all_tags)
@@ -107,7 +107,17 @@
         if property.type == TagPropertyType.categories:
             tag.categories.update(TagCategory(cat) for cat in property.value.split(","))
             continue
 
         raise NotImplementedError(f"Unknown property type: {property.type}")
 
     return info
+
+
+@run_in_transaction
+async def remove_relations_for_entries(execute: ExecuteType, entries_ids: list[uuid.UUID]) -> None:
+    await operations.remove_relations_for_entries(execute, entries_ids)
+
+
+@run_in_transaction
+async def tech_copy_relations(execute: ExecuteType, entry_from_id: uuid.UUID, entry_to_id: uuid.UUID) -> None:
+    await operations.tech_copy_relations(execute, entry_from_id, entry_to_id)
```

### Comparing `ffun-1.4.0/ffun/ontology/entities.py` & `ffun-1.5.0/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.5.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.5.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.5.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.5.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/ontology/tests/fixtures.py` & `ffun-1.5.0/ffun/ontology/tests/fixtures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import uuid
 
 import pytest
 import pytest_asyncio
 
 from ffun.ontology.domain import get_ids_by_uids
+from ffun.ontology.entities import ProcessorTag
 
 
 @pytest_asyncio.fixture
-async def tree_tags_by_uids() -> dict[str, int]:
+async def three_tags_by_uids() -> dict[str, int]:
     return await get_ids_by_uids([uuid.uuid4().hex for _ in range(3)])
 
 
 @pytest.fixture
-def tree_tags_by_ids(tree_tags_by_uids: dict[str, int]) -> dict[int, str]:
-    return {v: k for k, v in tree_tags_by_uids.items()}
+def three_tags_by_ids(three_tags_by_uids: dict[str, int]) -> dict[int, str]:
+    return {v: k for k, v in three_tags_by_uids.items()}
 
 
 @pytest.fixture
-def tree_tags_ids(tree_tags_by_uids: dict[str, int]) -> tuple[int, int, int]:
-    return tuple(tree_tags_by_uids.values())  # type: ignore
+def three_tags_ids(three_tags_by_uids: dict[str, int]) -> tuple[int, int, int]:
+    return tuple(three_tags_by_uids.values())  # type: ignore
+
+
+@pytest.fixture
+def three_processor_tags(three_tags_by_ids: dict[int, str]) -> tuple[ProcessorTag, ProcessorTag, ProcessorTag]:
+    return tuple(ProcessorTag(raw_uid=tag) for tag in three_tags_by_ids.values())  # type: ignore
```

### Comparing `ffun-1.4.0/ffun/openai/client.py` & `ffun-1.5.0/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/entities.py` & `ffun-1.5.0/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/keys_rotator.py` & `ffun-1.5.0/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/keys_statuses.py` & `ffun-1.5.0/ffun/openai/keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/tests/fixtures.py` & `ffun-1.5.0/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.5.0/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.5.0/ffun/openai/tests/test_keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/entities.py` & `ffun-1.5.0/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/feed.py` & `ffun-1.5.0/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/feedly.py` & `ffun-1.5.0/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.5.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/make.py` & `ffun-1.5.0/ffun/parsers/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/parsers/tests/test_feed.py` & `ffun-1.5.0/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/resources/domain.py` & `ffun-1.5.0/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.5.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/resources/operations.py` & `ffun-1.5.0/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/resources/tests/test_domain.py` & `ffun-1.5.0/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/resources/tests/test_operations.py` & `ffun-1.5.0/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/domain.py` & `ffun-1.5.0/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.5.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.5.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/operations.py` & `ffun-1.5.0/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/tests/test_domain.py` & `ffun-1.5.0/ffun/scores/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/scores/tests/test_operations.py` & `ffun-1.5.0/ffun/scores/tests/test_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,160 +4,160 @@
 
 from ffun.core.tests.helpers import TableSizeDelta, TableSizeNotChanged
 from ffun.scores import domain, errors, operations
 
 
 class TestCreateOrUpdateRule:
     @pytest.mark.asyncio
-    async def test_create_new_rule(self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]) -> None:
+    async def test_create_new_rule(self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]) -> None:
         async with TableSizeDelta("s_rules", delta=1):
-            created_rule = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
+            created_rule = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [created_rule]
 
         assert created_rule.user_id == internal_user_id
-        assert created_rule.tags == set(tree_tags_ids)
+        assert created_rule.tags == set(three_tags_ids)
         assert created_rule.score == 13
 
     @pytest.mark.asyncio
     async def test_tags_order_does_not_affect_creation(
-        self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
         async with TableSizeDelta("s_rules", delta=1):
-            created_rule_1 = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
-            created_rule_2 = await operations.create_or_update_rule(internal_user_id, reversed(tree_tags_ids), 17)
+            created_rule_1 = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
+            created_rule_2 = await operations.create_or_update_rule(internal_user_id, reversed(three_tags_ids), 17)
 
         assert created_rule_1.tags == created_rule_2.tags
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [created_rule_2]
 
     @pytest.mark.asyncio
     async def test_update_scores_of_existed_rule(
-        self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
-        await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
+        await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
 
         async with TableSizeNotChanged("s_rules"):
-            updated_rule = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 17)
+            updated_rule = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 17)
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [updated_rule]
 
         assert updated_rule.user_id == internal_user_id
-        assert updated_rule.tags == set(tree_tags_ids)
+        assert updated_rule.tags == set(three_tags_ids)
         assert updated_rule.score == 17
 
     @pytest.mark.asyncio
     async def test_multiple_entities(
-        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
-        await operations.create_or_update_rule(internal_user_id, tree_tags_ids[:2], 3)
-        await operations.create_or_update_rule(another_internal_user_id, tree_tags_ids[:2], 5)
-        await operations.create_or_update_rule(another_internal_user_id, tree_tags_ids[1:], 7)
-        await operations.create_or_update_rule(internal_user_id, tree_tags_ids[:2], 11)
+        await operations.create_or_update_rule(internal_user_id, three_tags_ids[:2], 3)
+        await operations.create_or_update_rule(another_internal_user_id, three_tags_ids[:2], 5)
+        await operations.create_or_update_rule(another_internal_user_id, three_tags_ids[1:], 7)
+        await operations.create_or_update_rule(internal_user_id, three_tags_ids[:2], 11)
 
         rules = await domain.get_rules(internal_user_id)
 
         assert len(rules) == 1
 
         assert rules[0].user_id == internal_user_id
-        assert rules[0].tags == set(tree_tags_ids[:2])
+        assert rules[0].tags == set(three_tags_ids[:2])
         assert rules[0].score == 11
 
         rules = await domain.get_rules(another_internal_user_id)
 
         rules.sort(key=lambda r: r.score)
 
         assert len(rules) == 2
 
         assert rules[0].user_id == another_internal_user_id
-        assert rules[0].tags == set(tree_tags_ids[:2])
+        assert rules[0].tags == set(three_tags_ids[:2])
         assert rules[0].score == 5
 
         assert rules[1].user_id == another_internal_user_id
-        assert rules[1].tags == set(tree_tags_ids[1:])
+        assert rules[1].tags == set(three_tags_ids[1:])
         assert rules[1].score == 7
 
 
 class TestDeleteRule:
     @pytest.mark.asyncio
     async def test_delete_rule(
-        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
-        rule_to_delete = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
-        rule_2 = await operations.create_or_update_rule(internal_user_id, tree_tags_ids[:2], 17)
-        rule_3 = await operations.create_or_update_rule(another_internal_user_id, tree_tags_ids, 19)
+        rule_to_delete = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
+        rule_2 = await operations.create_or_update_rule(internal_user_id, three_tags_ids[:2], 17)
+        rule_3 = await operations.create_or_update_rule(another_internal_user_id, three_tags_ids, 19)
 
         async with TableSizeDelta("s_rules", delta=-1):
             await operations.delete_rule(internal_user_id, rule_to_delete.id)
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [rule_2]
 
         rules = await domain.get_rules(another_internal_user_id)
 
         assert rules == [rule_3]
 
     @pytest.mark.asyncio
     async def test_delete_not_existed_rule(
-        self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
         async with TableSizeNotChanged("s_rules"):
             await operations.delete_rule(internal_user_id, uuid.uuid4())
 
     @pytest.mark.asyncio
     async def test_delete_for_wrong_user(
-        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
-        rule_to_delete = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
+        rule_to_delete = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
 
         async with TableSizeNotChanged("s_rules"):
             await operations.delete_rule(another_internal_user_id, rule_to_delete.id)
 
 
 class TestUpdateRule:
     @pytest.mark.asyncio
-    async def test_update_rule(self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]) -> None:
-        rule_to_update = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
+    async def test_update_rule(self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]) -> None:
+        rule_to_update = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
 
         async with TableSizeNotChanged("s_rules"):
-            updated_rule = await operations.update_rule(internal_user_id, rule_to_update.id, tree_tags_ids[:2], 17)
+            updated_rule = await operations.update_rule(internal_user_id, rule_to_update.id, three_tags_ids[:2], 17)
 
         assert updated_rule.id == rule_to_update.id
         assert updated_rule.user_id == internal_user_id
-        assert updated_rule.tags == set(tree_tags_ids[:2])
+        assert updated_rule.tags == set(three_tags_ids[:2])
         assert updated_rule.score == 17
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [updated_rule]
 
     @pytest.mark.asyncio
     async def test_update_not_existed_rule(
-        self, internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
         async with TableSizeNotChanged("s_rules"):
             with pytest.raises(errors.NoRuleFound):
-                await operations.update_rule(internal_user_id, uuid.uuid4(), tree_tags_ids[:2], 17)
+                await operations.update_rule(internal_user_id, uuid.uuid4(), three_tags_ids[:2], 17)
 
     @pytest.mark.asyncio
     async def test_wrong_user(
-        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, tree_tags_ids: tuple[int, int, int]
+        self, internal_user_id: uuid.UUID, another_internal_user_id: uuid.UUID, three_tags_ids: tuple[int, int, int]
     ) -> None:
-        rule_to_update = await operations.create_or_update_rule(internal_user_id, tree_tags_ids, 13)
+        rule_to_update = await operations.create_or_update_rule(internal_user_id, three_tags_ids, 13)
 
         async with TableSizeNotChanged("s_rules"):
             with pytest.raises(errors.NoRuleFound):
-                await operations.update_rule(another_internal_user_id, rule_to_update.id, tree_tags_ids, 17)
+                await operations.update_rule(another_internal_user_id, rule_to_update.id, three_tags_ids, 17)
 
         rules = await domain.get_rules(internal_user_id)
 
         assert rules == [rule_to_update]
 
 
 # most of the logic of this function is validated in other tests
```

### Comparing `ffun-1.4.0/ffun/tags/converters.py` & `ffun-1.5.0/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/tags/tests/test_converters.py` & `ffun-1.5.0/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/domain.py` & `ffun-1.5.0/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.5.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.5.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/operations.py` & `ffun-1.5.0/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/settings.py` & `ffun-1.5.0/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/tests/test_domain.py` & `ffun-1.5.0/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/tests/test_operations.py` & `ffun-1.5.0/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/user_settings/types.py` & `ffun-1.5.0/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/users/domain.py` & `ffun-1.5.0/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.5.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/users/operations.py` & `ffun-1.5.0/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/ffun/users/tests/fixtures.py` & `ffun-1.5.0/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.4.0/pyproject.toml` & `ffun-1.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.4.0"
+version = "1.5.0"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
@@ -148,14 +148,18 @@
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = "furl.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "orderedmultidict.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "pypika.*"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = """-x -vv --strict-markers -p no:cacheprovider"""
 filterwarnings = [
    "error",
```

### Comparing `ffun-1.4.0/PKG-INFO` & `ffun-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.4.0
+Version: 1.5.0
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```


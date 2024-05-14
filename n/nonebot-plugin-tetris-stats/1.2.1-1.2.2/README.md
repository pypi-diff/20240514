# Comparing `tmp/nonebot_plugin_tetris_stats-1.2.1.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.2.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.2.1.tar` & `nonebot_plugin_tetris_stats-1.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    34523 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/README.md
--rw-r--r--   0        0        0      791 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     1730 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
--rw-r--r--   0        0        0     1367 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
--rw-r--r--   0        0        0    14144 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
--rw-r--r--   0        0        0     2052 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
--rw-r--r--   0        0        0     3026 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
--rw-r--r--   0        0        0     6279 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3256 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5458 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     3908 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
--rw-r--r--   0        0        0     1005 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
--rw-r--r--   0        0        0     3972 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     1435 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      208 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     2641 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0      323 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
--rw-r--r--   0        0        0     1294 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
--rw-r--r--   0        0        0      771 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
--rw-r--r--   0        0        0     4114 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
--rw-r--r--   0        0        0      334 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
--rw-r--r--   0        0        0     1028 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
--rw-r--r--   0        0        0      318 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3062 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0     2219 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
--rw-r--r--   0        0        0     1079 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
--rw-r--r--   0        0        0      231 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
--rw-r--r--   0        0        0     2917 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
--rw-r--r--   0        0        0      536 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1122 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0    12623 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
--rw-r--r--   0        0        0     7818 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
--rw-r--r--   0        0        0      496 2024-05-14 09:01:12.389547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     2111 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
--rw-r--r--   0        0        0      742 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
--rw-r--r--   0        0        0     2824 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
--rw-r--r--   0        0        0      319 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0      189 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2635 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
--rw-r--r--   0        0        0      173 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     2939 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
--rw-r--r--   0        0        0     2548 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
--rw-r--r--   0        0        0      851 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
--rw-r--r--   0        0        0     5090 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
--rw-r--r--   0        0        0      325 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3436 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0      603 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2712 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
--rw-r--r--   0        0        0      463 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0     6463 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
--rw-r--r--   0        0        0     1769 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/avatar.py
--rw-r--r--   0        0        0     3006 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      945 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     2097 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/host.py
--rw-r--r--   0        0        0     7337 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0      935 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/__init__.py
--rw-r--r--   0        0        0      197 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
--rw-r--r--   0        0        0      282 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
--rw-r--r--   0        0        0     1521 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
--rw-r--r--   0        0        0     6263 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1412 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      394 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/screenshot.py
--rw-r--r--   0        0        0     2594 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/templates.py
--rw-r--r--   0        0        0      922 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     3615 2024-05-14 09:01:12.393547 nonebot_plugin_tetris_stats-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/README.md
+-rw-r--r--   0        0        0      791 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     1730 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
+-rw-r--r--   0        0        0     1367 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
+-rw-r--r--   0        0        0    14144 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
+-rw-r--r--   0        0        0     2052 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
+-rw-r--r--   0        0        0     3026 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
+-rw-r--r--   0        0        0     6279 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3256 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5458 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     3908 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
+-rw-r--r--   0        0        0     1005 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
+-rw-r--r--   0        0        0     3972 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     2790 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     1435 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-14 09:10:37.643365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/constant.py
+-rw-r--r--   0        0        0     2641 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
+-rw-r--r--   0        0        0      771 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
+-rw-r--r--   0        0        0     4114 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
+-rw-r--r--   0        0        0      334 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
+-rw-r--r--   0        0        0     1028 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
+-rw-r--r--   0        0        0      318 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3062 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0     2219 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
+-rw-r--r--   0        0        0     1079 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
+-rw-r--r--   0        0        0      231 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
+-rw-r--r--   0        0        0     2917 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
+-rw-r--r--   0        0        0      536 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
+-rw-r--r--   0        0        0     1122 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
+-rw-r--r--   0        0        0    12623 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
+-rw-r--r--   0        0        0     7818 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
+-rw-r--r--   0        0        0      496 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
+-rw-r--r--   0        0        0     2111 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
+-rw-r--r--   0        0        0     2824 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
+-rw-r--r--   0        0        0      319 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0      189 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2635 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
+-rw-r--r--   0        0        0      173 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
+-rw-r--r--   0        0        0     2939 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
+-rw-r--r--   0        0        0     2548 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
+-rw-r--r--   0        0        0     5090 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
+-rw-r--r--   0        0        0      325 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3436 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0      603 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2712 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
+-rw-r--r--   0        0        0      463 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
+-rw-r--r--   0        0        0     6463 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
+-rw-r--r--   0        0        0     1769 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/avatar.py
+-rw-r--r--   0        0        0     3006 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      945 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     2097 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/host.py
+-rw-r--r--   0        0        0     7337 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0      935 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
+-rw-r--r--   0        0        0      282 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
+-rw-r--r--   0        0        0     1521 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
+-rw-r--r--   0        0        0     6263 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1412 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      394 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/screenshot.py
+-rw-r--r--   0        0        0     2594 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/templates.py
+-rw-r--r--   0        0        0      922 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     3615 2024-05-14 09:10:37.647365 nonebot_plugin_tetris_stats-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.2.1/LICENSE` & `nonebot_plugin_tetris_stats-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/README.md` & `nonebot_plugin_tetris_stats-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/db/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/db/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,31 +29,31 @@
         super().__init__(*args, **kwargs)
 
     if PYDANTIC_V2:
 
         @override
         def process_bind_param(self, value: Any | None, dialect: Dialect) -> str:
             # 将 Pydantic 模型实例转换为 JSON
-            if isinstance(value, tuple(self.pydantic_models)):
+            if isinstance(value, tuple(self.models)):
                 return value.model_dump_json(by_alias=True)  # type: ignore[union-attr]
             raise TypeError
     else:
 
         @override
         def process_bind_param(self, value: Any | None, dialect: Dialect) -> str:
             # 将 Pydantic 模型实例转换为 JSON
-            if isinstance(value, tuple(self.pydantic_models)):
+            if isinstance(value, tuple(self.models)):
                 return value.json(by_alias=True)  # type: ignore[union-attr]
             raise TypeError
 
     @override
     def process_result_value(self, value: Any | None, dialect: Dialect) -> BaseModel:
         # 将 JSON 转换回 Pydantic 模型实例
         if isinstance(value, str | bytes):
-            for i in self.pydantic_models:
+            for i in self.models:
                 try:
                     return type_validate_json(i, value)
                 except ValidationError:  # noqa: PERF203
                     ...
         raise ValueError
```

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/avatar.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/host.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/host.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/__init__.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/templates.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/templates.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.2.2/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.1/pyproject.toml` & `nonebot_plugin_tetris_stats-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.2.1'
+version = '1.2.2'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
```

### Comparing `nonebot_plugin_tetris_stats-1.2.1/PKG-INFO` & `nonebot_plugin_tetris_stats-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.2.1
+Version: 1.2.2
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.2 Summary:
 ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸ææ°æ®çæä»¶ Home-
 page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats License:
 AGPL-3.0 Author: scdhh Author-email: wallfjjd@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
```


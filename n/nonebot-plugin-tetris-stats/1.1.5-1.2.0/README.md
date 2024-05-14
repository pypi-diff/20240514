# Comparing `tmp/nonebot_plugin_tetris_stats-1.1.5.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.0.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.1.5.tar` & `nonebot_plugin_tetris_stats-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,74 @@
--rw-r--r--   0        0        0    34523 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/README.md
--rw-r--r--   0        0        0      719 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     1674 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
--rw-r--r--   0        0        0     1311 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
--rw-r--r--   0        0        0     1995 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
--rw-r--r--   0        0        0     2985 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
--rw-r--r--   0        0        0     6222 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3262 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5483 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     3911 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
--rw-r--r--   0        0        0      948 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
--rw-r--r--   0        0        0     1407 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     3417 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     3167 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      108 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     7346 2024-05-12 20:20:49.654292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py
--rw-r--r--   0        0        0      422 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1148 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0    21094 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
--rw-r--r--   0        0        0      334 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/base.py
--rw-r--r--   0        0        0     1483 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py
--rw-r--r--   0        0        0      590 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py
--rw-r--r--   0        0        0      368 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user.py
--rw-r--r--   0        0        0     4264 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0     2538 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py
--rw-r--r--   0        0        0      231 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/typing.py
--rw-r--r--   0        0        0      625 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     4195 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0      103 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     6313 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py
--rw-r--r--   0        0        0      357 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/schemas/response.py
--rw-r--r--   0        0        0     6412 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0      293 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0    10066 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py
--rw-r--r--   0        0        0      524 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py
--rw-r--r--   0        0        0     3847 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0      690 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py
--rw-r--r--   0        0        0     1725 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/avatar.py
--rw-r--r--   0        0        0     2996 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      945 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     2045 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/host.py
--rw-r--r--   0        0        0     8031 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0     3064 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/recorder.py
--rw-r--r--   0        0        0     2804 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/render.py
--rw-r--r--   0        0        0     6222 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1390 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      394 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/screenshot.py
--rw-r--r--   0        0        0     2558 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/templates.py
--rw-r--r--   0        0        0      922 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2024-05-12 20:20:49.658292 nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     3054 2024-05-12 20:20:49.662292 nonebot_plugin_tetris_stats-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/README.md
+-rw-r--r--   0        0        0      791 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     1730 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
+-rw-r--r--   0        0        0     1367 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
+-rw-r--r--   0        0        0    14144 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
+-rw-r--r--   0        0        0     2052 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
+-rw-r--r--   0        0        0     3026 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
+-rw-r--r--   0        0        0     6279 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3256 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5458 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     3908 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
+-rw-r--r--   0        0        0     1005 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
+-rw-r--r--   0        0        0     4030 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     1435 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/constant.py
+-rw-r--r--   0        0        0     2641 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
+-rw-r--r--   0        0        0      771 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
+-rw-r--r--   0        0        0     4114 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
+-rw-r--r--   0        0        0      334 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
+-rw-r--r--   0        0        0     1028 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
+-rw-r--r--   0        0        0      318 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3062 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0     2179 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
+-rw-r--r--   0        0        0     1079 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
+-rw-r--r--   0        0        0      231 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
+-rw-r--r--   0        0        0     2917 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
+-rw-r--r--   0        0        0      536 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
+-rw-r--r--   0        0        0     1122 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
+-rw-r--r--   0        0        0    12623 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
+-rw-r--r--   0        0        0     7818 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
+-rw-r--r--   0        0        0      496 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
+-rw-r--r--   0        0        0     2111 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
+-rw-r--r--   0        0        0     2824 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
+-rw-r--r--   0        0        0      319 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0      189 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2635 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
+-rw-r--r--   0        0        0      173 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
+-rw-r--r--   0        0        0     2939 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
+-rw-r--r--   0        0        0     2548 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
+-rw-r--r--   0        0        0     5090 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
+-rw-r--r--   0        0        0      325 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3436 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0      603 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2712 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
+-rw-r--r--   0        0        0      463 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
+-rw-r--r--   0        0        0     6463 2024-05-14 07:41:07.367675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
+-rw-r--r--   0        0        0     1769 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/avatar.py
+-rw-r--r--   0        0        0     3006 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      945 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     2097 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/host.py
+-rw-r--r--   0        0        0     7337 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0      935 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/render/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
+-rw-r--r--   0        0        0      282 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
+-rw-r--r--   0        0        0     1521 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
+-rw-r--r--   0        0        0     6263 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1412 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      394 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/screenshot.py
+-rw-r--r--   0        0        0     2594 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/templates.py
+-rw-r--r--   0        0        0      922 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     3615 2024-05-14 07:41:07.371675 nonebot_plugin_tetris_stats-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/LICENSE` & `nonebot_plugin_tetris_stats-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.5/README.md` & `nonebot_plugin_tetris_stats-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
-require('nonebot_plugin_localstore')
-require('nonebot_plugin_orm')
 require('nonebot_plugin_alconna')
 require('nonebot_plugin_apscheduler')
+require('nonebot_plugin_localstore')
+require('nonebot_plugin_orm')
+require('nonebot_plugin_session')
+require('nonebot_plugin_session_orm')
 
 from .config.config import migrations  # noqa: E402
 
 __plugin_meta__ = PluginMetadata(
     name='Tetris Stats',
     description='一个用于查询 Tetris 相关游戏玩家数据的插件',
     usage='发送 {游戏名} --help 查询使用方法',
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 父迁移: b9d65badc713
 创建时间: 2024-04-23 23:42:04.541672
 
 """
 
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import op
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '09d4bb60160d'
 down_revision: str | Sequence[str] | None = 'b9d65badc713'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 父迁移: 09d4bb60160d
 创建时间: 2024-04-24 14:55:08.064098
 
 """
 
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import op
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '0d50142b780f'
 down_revision: str | Sequence[str] | None = '09d4bb60160d'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Add redundant platform field
 
 迁移 ID: 6c3206f90cc3
 父迁移: 9f6582279ce2
 创建时间: 2023-11-26 20:15:56.033892
 
 """
+
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 from alembic import op
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import Session
 from ujson import dumps, loads
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '6c3206f90cc3'
 down_revision: str | Sequence[str] | None = '9f6582279ce2'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,49 +4,53 @@
 父迁移: 0d50142b780f
 创建时间: 2024-05-06 08:16:38.487214
 
 """
 
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 from alembic import op
 from nonebot.log import logger
 from sqlalchemy import select
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import Session
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '8a91210ce14d'
 down_revision: str | Sequence[str] | None = '0d50142b780f'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
-def upgrade(name: str = '') -> None:
+def upgrade(name: str = '') -> None:  # noqa: C901
     if name:
         return
     from nonebot_plugin_tetris_stats.version import __version__
 
     if __version__ != '1.0.3':
-        logger.critical('本迁移需要1.0.3版本, 请先锁定版本至1.0.3版本再执行本迁移')
-        raise RuntimeError('本迁移需要1.0.3版本, 请先锁定版本至1.0.3版本再执行本迁移')
+        msg = '本迁移需要1.0.3版本, 请先锁定版本至1.0.3版本再执行本迁移'
+        logger.critical(msg)
+        raise RuntimeError(msg)
 
     from nonebot.compat import PYDANTIC_V2, type_validate_json
     from pydantic import BaseModel, ValidationError
     from rich.progress import (
         BarColumn,
         MofNCompleteColumn,
         Progress,
         TaskProgressColumn,
         TextColumn,
         TimeRemainingColumn,
     )
 
-    from nonebot_plugin_tetris_stats.game_data_processor.schemas import BaseProcessedData
+    from nonebot_plugin_tetris_stats.game_data_processor.schemas import BaseProcessedData  # type: ignore[attr-defined]
 
     Base = automap_base()  # noqa: N806
     Base.prepare(autoload_with=op.get_bind())
     HistoricalData = Base.classes.nonebot_plugin_tetris_stats_historicaldata  # noqa: N806
     if PYDANTIC_V2:
 
         def model_to_json(value: BaseModel) -> str:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """init db
 
 迁移 ID: 9866f53ce44f
 父迁移:
 创建时间: 2023-11-11 16:24:11.826667
 
 """
+
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import op
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '9866f53ce44f'
 down_revision: str | Sequence[str] | None = None
 branch_labels: str | Sequence[str] | None = ('nonebot_plugin_tetris_stats',)
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Merge old db
 
 迁移 ID: 9cd1647db502
 父迁移: 9866f53ce44f
 创建时间: 2023-11-11 16:51:30.718277
 
 """
+
 from __future__ import annotations
 
-from collections.abc import Sequence
 from pathlib import Path
 from shutil import copyfile
+from typing import TYPE_CHECKING
 
 from alembic import op
 from nonebot import get_driver
 from nonebot.log import logger
 from sqlalchemy import Connection, create_engine, inspect, text
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import Session
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = '9cd1647db502'
 down_revision: str | Sequence[str] | None = '9866f53ce44f'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 driver = get_driver()
 config = driver.config
@@ -76,16 +80,17 @@
     with engine.connect() as connection:
         tables = inspect(connection).get_table_names()
         if 'IOBIND' not in tables or 'TOPBIND' not in tables:
             logger.warning('nonebot_plugin_tetris_stats: 未发现老版本的数据')
             logger.success('nonebot_plugin_tetris_stats: 跳过迁移')
             return
         if 'IORANK' not in tables:
-            logger.warning('nonebot_plugin_tetris_stats: 发现过早版本的数据, 请先更新到 0.4.4 版本')
-            raise RuntimeError('nonebot_plugin_tetris_stats: 请先安装 0.4.4 版本完成迁移之后再升级')
+            msg = 'nonebot_plugin_tetris_stats: 请先安装 0.4.4 版本完成迁移之后再升级'
+            logger.warning(msg)
+            raise RuntimeError(msg)
         logger.info('nonebot_plugin_tetris_stats: 发现来自老版本的数据, 正在迁移...')
         migrate_old_data(connection)
     db_path.unlink()
 
 
 def downgrade(name: str = '') -> None:
     if name:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Recreate HistoricalData
 
 迁移 ID: 9f6582279ce2
 父迁移: 9cd1647db502
 创建时间: 2023-11-21 08:35:50.393246
 
 """
+
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import sqlite
 
-from nonebot_plugin_tetris_stats.db.models import PydanticType
+if TYPE_CHECKING:
+    from collections.abc import Sequence
 
 revision: str = '9f6582279ce2'
 down_revision: str | Sequence[str] | None = '9cd1647db502'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
@@ -41,16 +43,16 @@
         sa.Column('bot_account', sa.String(), nullable=True),
         sa.Column('source_type', sa.String(length=32), nullable=True),
         sa.Column('source_account', sa.String(), nullable=True),
         sa.Column('message', sa.PickleType(), nullable=True),
         sa.Column('game_platform', sa.String(length=32), nullable=False),
         sa.Column('command_type', sa.String(length=16), nullable=False),
         sa.Column('command_args', sa.JSON(), nullable=False),
-        sa.Column('game_user', PydanticType(list), nullable=False),
-        sa.Column('processed_data', PydanticType(list), nullable=False),
+        sa.Column('game_user', sa.JSON(), nullable=False),
+        sa.Column('processed_data', sa.JSON(), nullable=False),
         sa.Column('finish_time', sa.DateTime(), nullable=False),
         sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_tetris_stats_historicaldata')),
     )
     with op.batch_alter_table('nonebot_plugin_tetris_stats_historicaldata', schema=None) as batch_op:
         batch_op.create_index(
             batch_op.f('ix_nonebot_plugin_tetris_stats_historicaldata_command_type'), ['command_type'], unique=False
         )
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 父迁移: 8a91210ce14d
 创建时间: 2024-05-07 16:55:29.527215
 
 """
 
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import op
 from nonebot.log import logger
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = 'b7fbdafc339a'
 down_revision: str | Sequence[str] | None = '8a91210ce14d'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
     if name:
         return
     from nonebot_plugin_tetris_stats.version import __version__
 
     if __version__ != '1.0.4':
-        logger.critical('本迁移需要1.0.4版本, 请先锁定版本至1.0.4版本再执行本迁移')
-        raise RuntimeError('本迁移需要1.0.4版本, 请先锁定版本至1.0.4版本再执行本迁移')
+        msg = '本迁移需要1.0.4版本, 请先锁定版本至1.0.4版本再执行本迁移'
+        logger.critical(msg)
+        raise RuntimeError(msg)
     from nonebot.compat import type_validate_json
     from pydantic import ValidationError
     from rich.progress import (
         BarColumn,
         MofNCompleteColumn,
         Progress,
         TaskProgressColumn,
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Del old TOS bind data
 
 迁移 ID: b9d65badc713
 父迁移: 6c3206f90cc3
 创建时间: 2023-12-30 00:27:40.991704
 
 """
+
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 from alembic import op
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import Session
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 revision: str = 'b9d65badc713'
 down_revision: str | Sequence[str] | None = '6c3206f90cc3'
 branch_labels: str | Sequence[str] | None = None
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = '') -> None:
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/db/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from collections.abc import Callable, Sequence
 from datetime import datetime
-from typing import Any
+from typing import Any, Literal
 
-from nonebot.adapters import Message
 from nonebot.compat import PYDANTIC_V2, type_validate_json
 from nonebot_plugin_orm import Model
 from pydantic import BaseModel, ValidationError
-from sqlalchemy import JSON, DateTime, Dialect, PickleType, String, TypeDecorator
+from sqlalchemy import JSON, DateTime, Dialect, String, TypeDecorator
 from sqlalchemy.orm import Mapped, MappedAsDataclass, mapped_column
 from typing_extensions import override
 
-from ..game_data_processor.schemas import BaseProcessedData, BaseUser
 from ..utils.typing import CommandType, GameType
 
 
 class PydanticType(TypeDecorator):
     impl = JSON
 
     @override
-    def __init__(self, get_model: Callable[[], Sequence[type[BaseModel]]], *args: Any, **kwargs: Any):
-        self.get_model = get_model
+    def __init__(
+        self,
+        get_model: Sequence[Callable[[], Sequence[type[BaseModel]]]],
+        models: set[type[BaseModel]],
+        *args: Any,
+        **kwargs: Any,
+    ):
+        for i in get_model:
+            models.update(i())
+        self.models = models
         super().__init__(*args, **kwargs)
 
     if PYDANTIC_V2:
 
         @override
         def process_bind_param(self, value: Any | None, dialect: Dialect) -> str:
             # 将 Pydantic 模型实例转换为 JSON
-            if isinstance(value, tuple(self.get_model())):
+            if isinstance(value, tuple(self.pydantic_models)):
                 return value.model_dump_json(by_alias=True)  # type: ignore[union-attr]
             raise TypeError
     else:
 
         @override
         def process_bind_param(self, value: Any | None, dialect: Dialect) -> str:
             # 将 Pydantic 模型实例转换为 JSON
-            if isinstance(value, tuple(self.get_model())):
+            if isinstance(value, tuple(self.pydantic_models)):
                 return value.json(by_alias=True)  # type: ignore[union-attr]
             raise TypeError
 
     @override
     def process_result_value(self, value: Any | None, dialect: Dialect) -> BaseModel:
         # 将 JSON 转换回 Pydantic 模型实例
         if isinstance(value, str | bytes):
-            for i in self.get_model():
+            for i in self.pydantic_models:
                 try:
                     return type_validate_json(i, value)
                 except ValidationError:  # noqa: PERF203
                     ...
         raise ValueError
 
 
@@ -55,24 +61,15 @@
     id: Mapped[int] = mapped_column(init=False, primary_key=True)
     chat_platform: Mapped[str] = mapped_column(String(32), index=True)
     chat_account: Mapped[str] = mapped_column(index=True)
     game_platform: Mapped[GameType] = mapped_column(String(32))
     game_account: Mapped[str]
 
 
-class HistoricalData(MappedAsDataclass, Model):
+class TriggerHistoricalData(MappedAsDataclass, Model):
     id: Mapped[int] = mapped_column(init=False, primary_key=True)
     trigger_time: Mapped[datetime] = mapped_column(DateTime)
-    bot_platform: Mapped[str | None] = mapped_column(String(32))
-    bot_account: Mapped[str | None]
-    source_type: Mapped[str | None] = mapped_column(String(32), index=True)
-    source_account: Mapped[str | None] = mapped_column(index=True)
-    message: Mapped[Message | None] = mapped_column(PickleType)
-    game_platform: Mapped[GameType] = mapped_column(String(32), index=True, init=False)
-    command_type: Mapped[CommandType] = mapped_column(String(16), index=True, init=False)
-    command_args: Mapped[list[str]] = mapped_column(JSON, init=False)
-    user_unique_identifier: Mapped[str] = mapped_column(String(32), index=True, init=False)
-    game_user: Mapped[BaseUser] = mapped_column(PydanticType(get_model=BaseUser.__subclasses__), init=False)
-    processed_data: Mapped[BaseProcessedData] = mapped_column(
-        PydanticType(get_model=BaseProcessedData.__subclasses__), init=False
-    )
-    finish_time: Mapped[datetime] = mapped_column(DateTime, init=False)
+    session_persist_id: Mapped[int]
+    game_platform: Mapped[GameType] = mapped_column(String(32), index=True)
+    command_type: Mapped[CommandType | Literal['rank']] = mapped_column(String(16), index=True)
+    command_args: Mapped[list[str]] = mapped_column(JSON)
+    finish_time: Mapped[datetime] = mapped_column(DateTime)
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,196 +1,174 @@
+from collections import defaultdict
+from collections.abc import Callable
 from datetime import datetime, timedelta, timezone
+from hashlib import sha512
+from math import floor
+from statistics import mean
 from zoneinfo import ZoneInfo
 
-from arclet.alconna import Alconna, AllParam, Arg, ArgFlag, Args, CommandMeta, Option
-from nonebot.adapters import Bot, Event
+from aiofiles import open
+from nonebot import get_driver
+from nonebot.compat import model_dump
 from nonebot.matcher import Matcher
-from nonebot_plugin_alconna import At, on_alconna
-from nonebot_plugin_alconna.uniseg import UniMessage
+from nonebot.utils import run_sync
+from nonebot_plugin_apscheduler import scheduler  # type: ignore[import-untyped]
+from nonebot_plugin_localstore import get_data_file  # type: ignore[import-untyped]
 from nonebot_plugin_orm import get_session
-from nonebot_plugin_userinfo import BotUserInfo, UserInfo  # type: ignore[import-untyped]
+from nonebot_plugin_session import EventSession  # type: ignore[import-untyped]
+from nonebot_plugin_session_orm import get_session_persist_id  # type: ignore[import-untyped]
 from sqlalchemy import func, select
+from zstandard import ZstdCompressor
 
-from ...db import query_bind_info
-from ...utils.exception import HandleNotFinishedError, NeedCatchError
+from ...db import trigger
+from ...utils.exception import RequestError
 from ...utils.metrics import get_metrics
-from ...utils.platform import get_platform
-from ...utils.typing import Me
-from .. import add_default_handlers
-from ..constant import BIND_COMMAND, QUERY_COMMAND
-from .constant import GAME_TYPE
+from ...utils.retry import retry
+from . import alc
+from .api.schemas.base import FailedModel
+from .api.schemas.tetra_league import ValidUser
+from .api.schemas.user import User
+from .api.tetra_league import full_export
+from .api.typing import Rank
+from .constant import GAME_TYPE, RANK_PERCENTILE
 from .model import IORank
-from .processor import Processor, User, identify_user_info
-from .typing import Rank
 
 UTC = timezone.utc
 
-alc = on_alconna(
-    Alconna(
-        'io',
-        Option(
-            BIND_COMMAND[0],
-            Args(
-                Arg(
-                    'account',
-                    identify_user_info,
-                    notice='IO 用户名 / ID',
-                    flags=[ArgFlag.HIDDEN],
-                )
-            ),
-            alias=BIND_COMMAND[1:],
-            compact=True,
-            dest='bind',
-            help_text='绑定 IO 账号',
-        ),
-        Option(
-            QUERY_COMMAND[0],
-            Args(
-                Arg(
-                    'target',
-                    At | Me,
-                    notice='@想要查询的人 | 自己',
-                    flags=[ArgFlag.HIDDEN, ArgFlag.OPTIONAL],
-                ),
-                Arg(
-                    'account',
-                    identify_user_info,
-                    notice='IO 用户名 / ID',
-                    flags=[ArgFlag.HIDDEN, ArgFlag.OPTIONAL],
-                ),
-            ),
-            alias=QUERY_COMMAND[1:],
-            compact=True,
-            dest='query',
-            help_text='查询 IO 游戏信息',
-        ),
-        Option(
-            'rank',
-            Args(Arg('rank', Rank, notice='IO 段位')),
-            alias={'Rank', 'RANK', '段位'},
-            compact=True,
-            dest='rank',
-            help_text='查询 IO 段位信息',
-        ),
-        Arg('other', AllParam, flags=[ArgFlag.HIDDEN, ArgFlag.OPTIONAL]),
-        meta=CommandMeta(
-            description='查询 TETR.IO 的信息',
-            example='io绑定scdhh\nio查我\niorankx',
-            compact=True,
-            fuzzy_match=True,
-        ),
-    ),
-    skip_for_unmatch=False,
-    auto_send_output=True,
-    aliases={'IO'},
-)
-
-alc.shortcut('fkosk', {'command': 'io查', 'args': ['我']})
-
-
-@alc.assign('bind')
-async def _(bot: Bot, event: Event, matcher: Matcher, account: User, bot_info: UserInfo = BotUserInfo()):  # noqa: B008
-    proc = Processor(event_id=id(event), user=account, command_args=[])
-    try:
-        await (
-            await proc.handle_bind(platform=get_platform(bot), account=event.get_user_id(), bot_info=bot_info)
-        ).finish()
-    except NeedCatchError as e:
-        await matcher.send(str(e))
-        raise HandleNotFinishedError from e
-
-
-@alc.assign('query')
-async def _(bot: Bot, event: Event, matcher: Matcher, target: At | Me):
-    async with get_session() as session:
-        bind = await query_bind_info(
-            session=session,
-            chat_platform=get_platform(bot),
-            chat_account=(target.target if isinstance(target, At) else event.get_user_id()),
-            game_platform=GAME_TYPE,
-        )
-    if bind is None:
-        await matcher.finish('未查询到绑定信息')
-    message = '* 由于无法验证绑定信息, 不能保证查询到的用户为本人\n'
-    proc = Processor(
-        event_id=id(event),
-        user=User(ID=bind.game_account),
-        command_args=[],
-    )
-    try:
-        await (UniMessage(message) + await proc.handle_query()).finish()
-    except NeedCatchError as e:
-        await matcher.send(str(e))
-        raise HandleNotFinishedError from e
-
-
-@alc.assign('query')
-async def _(event: Event, matcher: Matcher, account: User):
-    proc = Processor(
-        event_id=id(event),
-        user=account,
-        command_args=[],
-    )
-    try:
-        await (await proc.handle_query()).finish()
-    except NeedCatchError as e:
-        await matcher.send(str(e))
-        raise HandleNotFinishedError from e
+driver = get_driver()
 
 
 @alc.assign('rank')
-async def _(matcher: Matcher, rank: Rank):
-    if rank == 'z':
-        await matcher.finish('暂不支持查询未知段位')
-    async with get_session() as session:
-        latest_data = (
-            await session.scalars(select(IORank).where(IORank.rank == rank).order_by(IORank.id.desc()).limit(1))
-        ).one()
-        compare_data = (
-            await session.scalars(
-                select(IORank)
-                .where(IORank.rank == rank)
-                .order_by(
-                    func.abs(
-                        func.julianday(IORank.update_time)
-                        - func.julianday(latest_data.update_time - timedelta(hours=24))
+async def _(matcher: Matcher, rank: Rank, event_session: EventSession):
+    async with trigger(
+        session_persist_id=await get_session_persist_id(event_session),
+        game_platform=GAME_TYPE,
+        command_type='rank',
+        command_args=[],
+    ):
+        if rank == 'z':
+            await matcher.finish('暂不支持查询未知段位')
+        async with get_session() as session:
+            latest_data = (
+                await session.scalars(select(IORank).where(IORank.rank == rank).order_by(IORank.id.desc()).limit(1))
+            ).one()
+            compare_data = (
+                await session.scalars(
+                    select(IORank)
+                    .where(IORank.rank == rank)
+                    .order_by(
+                        func.abs(
+                            func.julianday(IORank.update_time)
+                            - func.julianday(latest_data.update_time - timedelta(hours=24))
+                        )
                     )
+                    .limit(1)
                 )
-                .limit(1)
+            ).one()
+        message = ''
+        if (datetime.now(UTC) - latest_data.update_time.replace(tzinfo=UTC)) > timedelta(hours=7):
+            message += 'Warning: 数据超过7小时未更新, 请联系Bot主人查看后台\n'
+        message += f'{rank.upper()} 段 分数线 {latest_data.tr_line:.2f} TR, {latest_data.player_count} 名玩家\n'
+        if compare_data.id != latest_data.id:
+            message += f'对比 {(latest_data.update_time-compare_data.update_time).total_seconds()/3600:.2f} 小时前趋势: {f"↑{difference:.2f}" if (difference:=latest_data.tr_line-compare_data.tr_line) > 0 else f"↓{-difference:.2f}" if difference < 0 else "→"}'
+        else:
+            message += '暂无对比数据'
+        avg = get_metrics(pps=latest_data.avg_pps, apm=latest_data.avg_apm, vs=latest_data.avg_vs)
+        low_pps = get_metrics(pps=latest_data.low_pps[1])
+        low_vs = get_metrics(vs=latest_data.low_vs[1])
+        max_pps = get_metrics(pps=latest_data.high_pps[1])
+        max_vs = get_metrics(vs=latest_data.high_vs[1])
+        message += (
+            '\n'
+            '平均数据:\n'
+            f"L'PM: {avg.lpm} ( {avg.pps} pps )\n"
+            f'APM: {avg.apm} ( x{avg.apl} )\n'
+            f'ADPM: {avg.adpm} ( x{avg.adpl} ) ( {avg.vs}vs )\n'
+            '\n'
+            '最低数据:\n'
+            f"L'PM: {low_pps.lpm} ( {low_pps.pps} pps ) By: {latest_data.low_pps[0]['name'].upper()}\n"
+            f'APM: {latest_data.low_apm[1]} By: {latest_data.low_apm[0]["name"].upper()}\n'
+            f'ADPM: {low_vs.adpm} ( {low_vs.vs}vs ) By: {latest_data.low_vs[0]["name"].upper()}\n'
+            '\n'
+            '最高数据:\n'
+            f"L'PM: {max_pps.lpm} ( {max_pps.pps} pps ) By: {latest_data.high_pps[0]['name'].upper()}\n"
+            f'APM: {latest_data.high_apm[1]} By: {latest_data.high_apm[0]["name"].upper()}\n'
+            f'ADPM: {max_vs.adpm} ( {max_vs.vs}vs ) By: {latest_data.high_vs[0]["name"].upper()}\n'
+            '\n'
+            f'数据更新时间: {latest_data.update_time.replace(tzinfo=UTC).astimezone(ZoneInfo("Asia/Shanghai")).strftime("%Y-%m-%d %H:%M:%S")}'
+        )
+        await matcher.finish(message)
+
+
+@scheduler.scheduled_job('cron', hour='0,6,12,18', minute=0)
+@retry(exception_type=RequestError, delay=timedelta(minutes=15))
+async def get_tetra_league_data() -> None:
+    league, original = await full_export(with_original=True)
+    if isinstance(league, FailedModel):
+        msg = f'排行榜数据请求错误:\n{league.error}'
+        raise RequestError(msg)
+
+    def pps(user: ValidUser) -> float:
+        return user.league.pps
+
+    def apm(user: ValidUser) -> float:
+        return user.league.apm
+
+    def vs(user: ValidUser) -> float:
+        return user.league.vs
+
+    def _min(users: list[ValidUser], field: Callable[[ValidUser], float]) -> ValidUser:
+        return min(users, key=field)
+
+    def _max(users: list[ValidUser], field: Callable[[ValidUser], float]) -> ValidUser:
+        return max(users, key=field)
+
+    def build_extremes_data(
+        users: list[ValidUser],
+        field: Callable[[ValidUser], float],
+        sort: Callable[[list[ValidUser], Callable[[ValidUser], float]], ValidUser],
+    ) -> tuple[dict[str, str], float]:
+        user = sort(users, field)
+        return model_dump(User(ID=user.id, name=user.username)), field(user)
+
+    data_hash: str | None = await run_sync((await run_sync(sha512)(original)).hexdigest)()
+    async with open(get_data_file('nonebot_plugin_tetris_stats', f'{data_hash}.json.zst'), mode='wb') as file:
+        await file.write(await run_sync(ZstdCompressor(level=12, threads=-1).compress)(original))
+
+    users = [i for i in league.data.users if isinstance(i, ValidUser)]
+    rank_to_users: defaultdict[Rank, list[ValidUser]] = defaultdict(list)
+    for i in users:
+        rank_to_users[i.league.rank].append(i)
+    rank_info: list[IORank] = []
+    for rank, percentile in RANK_PERCENTILE.items():
+        offset = floor((percentile / 100) * len(users)) - 1
+        tr_line = users[offset].league.rating
+        rank_users = rank_to_users[rank]
+        rank_info.append(
+            IORank(
+                rank=rank,
+                tr_line=tr_line,
+                player_count=len(rank_users),
+                low_pps=(build_extremes_data(rank_users, pps, _min)),
+                low_apm=(build_extremes_data(rank_users, apm, _min)),
+                low_vs=(build_extremes_data(rank_users, vs, _min)),
+                avg_pps=mean({i.league.pps for i in rank_users}),
+                avg_apm=mean({i.league.apm for i in rank_users}),
+                avg_vs=mean({i.league.vs for i in rank_users}),
+                high_pps=(build_extremes_data(rank_users, pps, _max)),
+                high_apm=(build_extremes_data(rank_users, apm, _max)),
+                high_vs=(build_extremes_data(rank_users, vs, _max)),
+                update_time=league.cache.cached_at,
+                file_hash=data_hash,
             )
-        ).one()
-    message = ''
-    if (datetime.now(UTC) - latest_data.update_time.replace(tzinfo=UTC)) > timedelta(hours=7):
-        message += 'Warning: 数据超过7小时未更新, 请联系Bot主人查看后台\n'
-    message += f'{rank.upper()} 段 分数线 {latest_data.tr_line:.2f} TR, {latest_data.player_count} 名玩家\n'
-    if compare_data.id != latest_data.id:
-        message += f'对比 {(latest_data.update_time-compare_data.update_time).total_seconds()/3600:.2f} 小时前趋势: {f"↑{difference:.2f}" if (difference:=latest_data.tr_line-compare_data.tr_line) > 0 else f"↓{-difference:.2f}" if difference < 0 else "→"}'
-    else:
-        message += '暂无对比数据'
-    avg = get_metrics(pps=latest_data.avg_pps, apm=latest_data.avg_apm, vs=latest_data.avg_vs)
-    low_pps = get_metrics(pps=latest_data.low_pps[1])
-    low_vs = get_metrics(vs=latest_data.low_vs[1])
-    max_pps = get_metrics(pps=latest_data.high_pps[1])
-    max_vs = get_metrics(vs=latest_data.high_vs[1])
-    message += (
-        '\n'
-        '平均数据:\n'
-        f"L'PM: {avg.lpm} ( {avg.pps} pps )\n"
-        f'APM: {avg.apm} ( x{avg.apl} )\n'
-        f'ADPM: {avg.adpm} ( x{avg.adpl} ) ( {avg.vs}vs )\n'
-        '\n'
-        '最低数据:\n'
-        f"L'PM: {low_pps.lpm} ( {low_pps.pps} pps ) By: {latest_data.low_pps[0]['name'].upper()}\n"
-        f'APM: {latest_data.low_apm[1]} By: {latest_data.low_apm[0]["name"].upper()}\n'
-        f'ADPM: {low_vs.adpm} ( {low_vs.vs}vs ) By: {latest_data.low_vs[0]["name"].upper()}\n'
-        '\n'
-        '最高数据:\n'
-        f"L'PM: {max_pps.lpm} ( {max_pps.pps} pps ) By: {latest_data.high_pps[0]['name'].upper()}\n"
-        f'APM: {latest_data.high_apm[1]} By: {latest_data.high_apm[0]["name"].upper()}\n'
-        f'ADPM: {max_vs.adpm} ( {max_vs.vs}vs ) By: {latest_data.high_vs[0]["name"].upper()}\n'
-        '\n'
-        f'数据更新时间: {latest_data.update_time.replace(tzinfo=UTC).astimezone(ZoneInfo("Asia/Shanghai")).strftime("%Y-%m-%d %H:%M:%S")}'
-    )
-    await matcher.finish(message)
+        )
+    async with get_session() as session:
+        session.add_all(rank_info)
+        await session.commit()
 
 
-add_default_handlers(alc)
+@driver.on_startup
+async def _() -> None:
+    async with get_session() as session:
+        latest_time = await session.scalar(select(IORank.update_time).order_by(IORank.id.desc()).limit(1))
+    if latest_time is None or datetime.now(tz=UTC) - latest_time.replace(tzinfo=UTC) > timedelta(hours=6):
+        await get_tetra_league_data()
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from datetime import datetime, timezone
+from datetime import datetime
 
 from nonebot_plugin_orm import Model
 from sqlalchemy import JSON, DateTime, String
 from sqlalchemy.orm import Mapped, MappedAsDataclass, mapped_column
 
-from .typing import Rank
-
-UTC = timezone.utc
+from .api.typing import Rank
 
 
 class IORank(MappedAsDataclass, Model):
     id: Mapped[int] = mapped_column(init=False, primary_key=True)
     rank: Mapped[Rank] = mapped_column(String(2), index=True)
     tr_line: Mapped[float]
     player_count: Mapped[int]
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,49 +2,53 @@
 
 from pydantic import BaseModel, Field
 
 from .base import FailedModel
 from .base import SuccessModel as BaseSuccessModel
 
 
-class EndContext(BaseModel):
-    class Time(BaseModel):
-        start: int
-        zero: bool
-        locked: bool
-        prev: int
-        frameoffset: int | None = None
-
-    class Clears(BaseModel):
-        singles: int
-        doubles: int
-        triples: int
-        quads: int
-        pentas: int | None = None
-        realtspins: int
-        minitspins: int
-        minitspinsingles: int
-        tspinsingles: int
-        minitspindoubles: int
-        tspindoubles: int
-        tspintriples: int
-        tspinquads: int
-        allclear: int
-
-    class Garbage(BaseModel):
-        sent: int
-        received: int
-        attack: int | None = None
-        cleared: int
-
-    class Finesse(BaseModel):
-        combo: int
-        faults: int
-        perfectpieces: int
+class Time(BaseModel):
+    start: int
+    zero: bool
+    locked: bool
+    prev: int
+    frameoffset: int | None = None
+
+
+class Clears(BaseModel):
+    singles: int
+    doubles: int
+    triples: int
+    quads: int
+    pentas: int | None = None
+    realtspins: int
+    minitspins: int
+    minitspinsingles: int
+    tspinsingles: int
+    minitspindoubles: int
+    tspindoubles: int
+    tspintriples: int
+    tspinquads: int
+    allclear: int
+
+
+class Garbage(BaseModel):
+    sent: int
+    received: int
+    attack: int | None = None
+    cleared: int
+
+
+class Finesse(BaseModel):
+    combo: int
+    faults: int
+    perfectpieces: int
 
+
+class EndContext(BaseModel):
     seed: int
     lines: int
     level_lines: int
     level_lines_needed: int
     inputs: int
     holds: int | None = None
     time: Time
@@ -78,41 +82,40 @@
     stream: str
     replayid: str
     user: _User
     ts: datetime
     ismulti: bool | None = None
 
 
-class BaseModeRecord(BaseModel):
-    class SoloRecord(_Record):
-        endcontext: EndContext
+class SoloRecord(_Record):
+    endcontext: EndContext
+
 
-    class MultiRecord(_Record):
-        endcontext: list[EndContext]
+class MultiRecord(_Record):
+    endcontext: list[EndContext]
 
-    record: SoloRecord | MultiRecord | None = None
+
+class SoloModeRecord(BaseModel):
+    record: SoloRecord
     rank: int | None = None
 
 
-class SuccessModel(BaseSuccessModel):
-    class Data(BaseModel):
-        class Records(BaseModel):
-            class Sprint(BaseModeRecord): ...
-
-            class Blitz(BaseModeRecord): ...
-
-            sprint: Sprint = Field(..., alias='40l')
-            blitz: Blitz
-
-        class Zen(BaseModel):
-            level: int
-            score: int
+class Records(BaseModel):
+    sprint: SoloModeRecord = Field(..., alias='40l')
+    blitz: SoloModeRecord
+
+
+class Zen(BaseModel):
+    level: int
+    score: int
+
+
+class Data(BaseModel):
+    records: Records
+    zen: Zen
 
-        records: Records
-        zen: Zen
 
+class UserRecordsSuccess(BaseSuccessModel):
     data: Data
 
 
-SoloRecord = BaseModeRecord.SoloRecord
-MultiRecord = BaseModeRecord.MultiRecord
-UserRecords = SuccessModel | FailedModel
+UserRecords = UserRecordsSuccess | FailedModel
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,170 @@
-from contextlib import suppress
+from asyncio import gather
 from dataclasses import dataclass
-from io import StringIO
-from re import match
 from typing import Literal
-from urllib.parse import urlencode, urlunparse
 
-from lxml import etree
+from nonebot.adapters import Bot, Event
+from nonebot.matcher import Matcher
+from nonebot_plugin_alconna import At
 from nonebot_plugin_alconna.uniseg import UniMessage
 from nonebot_plugin_orm import get_session
-from nonebot_plugin_userinfo import UserInfo  # type: ignore[import-untyped]
-from pandas import read_html
-from typing_extensions import override
-
-from ...db import BindStatus, create_or_update_bind
-from ...utils.avatar import get_avatar
-from ...utils.exception import MessageFormatError, RequestError
-from ...utils.host import HostPage, get_self_netloc
-from ...utils.render import Bind, render
-from ...utils.request import Request, splice_url
-from ...utils.screenshot import screenshot
-from .. import Processor as ProcessorMeta
-from ..schemas import BaseUser
-from .constant import BASE_URL, GAME_TYPE
-from .schemas.response import ProcessedData, RawResponse
-
-
-class User(BaseUser):
-    platform: Literal['TOP'] = GAME_TYPE
-
-    name: str
-
-    @property
-    @override
-    def unique_identifier(self) -> str:
-        return self.name
+from nonebot_plugin_session import EventSession  # type: ignore[import-untyped]
+from nonebot_plugin_session_orm import get_session_persist_id  # type: ignore[import-untyped]
 
+from ...db import query_bind_info, trigger
+from ...utils.metrics import TetrisMetricsProWithLPMADPM, get_metrics
+from ...utils.platform import get_platform
+from ...utils.typing import Me
+from ..constant import CANT_VERIFY_MESSAGE
+from . import alc
+from .api import Player
+from .constant import GAME_TYPE
+
+
+def add_special_handlers(
+    teaid_prefix: Literal['onebot-', 'kook-', 'discord-', 'qqguild-'], match_event: type[Event]
+) -> None:
+    @alc.assign('query')
+    async def _(event: Event, target: At | Me, event_session: EventSession):
+        if isinstance(event, match_event):
+            async with trigger(
+                session_persist_id=await get_session_persist_id(event_session),
+                game_platform=GAME_TYPE,
+                command_type='query',
+                command_args=[],
+            ):
+                await (
+                    await make_query_text(
+                        Player(
+                            teaid=f'{teaid_prefix}{target.target}'
+                            if isinstance(target, At)
+                            else f'{teaid_prefix}{event.get_user_id()}',
+                            trust=True,
+                        )
+                    )
+                ).finish()
+
+
+try:
+    from nonebot.adapters.onebot.v11 import MessageEvent as OB11MessageEvent
+
+    add_special_handlers('onebot-', OB11MessageEvent)
+except ImportError:
+    pass
+
+try:
+    from nonebot.adapters.qq.event import GuildMessageEvent as QQGuildMessageEvent
+    from nonebot.adapters.qq.event import QQMessageEvent
+
+    add_special_handlers('qqguild-', QQGuildMessageEvent)
+    add_special_handlers('onebot-', QQMessageEvent)
+except ImportError:
+    pass
+
+try:
+    from nonebot.adapters.kaiheila.event import MessageEvent as KookMessageEvent
+
+    add_special_handlers('kook-', KookMessageEvent)
+except ImportError:
+    pass
+
+try:
+    from nonebot.adapters.discord import MessageEvent as DiscordMessageEvent
+
+    add_special_handlers('discord-', DiscordMessageEvent)
+except ImportError:
+    pass
+
+
+@alc.assign('query')
+async def _(bot: Bot, event: Event, matcher: Matcher, target: At | Me, event_session: EventSession):
+    async with trigger(
+        session_persist_id=await get_session_persist_id(event_session),
+        game_platform=GAME_TYPE,
+        command_type='query',
+        command_args=[],
+    ):
+        async with get_session() as session:
+            bind = await query_bind_info(
+                session=session,
+                chat_platform=get_platform(bot),
+                chat_account=(target.target if isinstance(target, At) else event.get_user_id()),
+                game_platform=GAME_TYPE,
+            )
+        if bind is None:
+            await matcher.finish('未查询到绑定信息')
+        message = CANT_VERIFY_MESSAGE
+        await (message + await make_query_text(Player(teaid=bind.game_account, trust=True))).finish()
 
-@dataclass
-class Data:
-    lpm: float
-    apm: float
+
+@alc.assign('query')
+async def _(account: Player, event_session: EventSession):
+    async with trigger(
+        session_persist_id=await get_session_persist_id(event_session),
+        game_platform=GAME_TYPE,
+        command_type='query',
+        command_args=[],
+    ):
+        await (await make_query_text(account)).finish()
 
 
 @dataclass
 class GameData:
-    day: Data | None
-    total: Data | None
+    game_num: int
+    metrics: TetrisMetricsProWithLPMADPM
 
 
-def identify_user_info(info: str) -> User | MessageFormatError:
-    if match(r'^[a-zA-Z0-9_]{1,16}$', info):
-        return User(name=info)
-    return MessageFormatError('用户名不合法')
-
-
-class Processor(ProcessorMeta):
-    user: User
-    raw_response: RawResponse
-    processed_data: ProcessedData
-
-    @override
-    def __init__(self, event_id: int, user: User, command_args: list[str]) -> None:
-        super().__init__(event_id, user, command_args)
-        self.raw_response = RawResponse()
-        self.processed_data = ProcessedData()
-
-    @property
-    @override
-    def game_platform(self) -> Literal['TOP']:
-        return GAME_TYPE
-
-    @override
-    async def handle_bind(self, platform: str, account: str, bot_info: UserInfo, user_info: UserInfo) -> UniMessage:
-        """处理绑定消息"""
-        self.command_type = 'bind'
-        await self.check_user()
-        async with get_session() as session:
-            bind_status = await create_or_update_bind(
-                session=session,
-                chat_platform=platform,
-                chat_account=account,
-                game_platform=GAME_TYPE,
-                game_account=self.user.name,
-            )
-        if bind_status in (BindStatus.SUCCESS, BindStatus.UPDATE):
-            async with HostPage(
-                await render(
-                    'binding',
-                    Bind(
-                        platform=self.game_platform,
-                        status='unknown',
-                        user=Bind.People(
-                            avatar=await get_avatar(user_info, 'Data URI', None),
-                            name=(await self.get_user_name()).upper(),
-                        ),
-                        bot=Bind.People(
-                            avatar=await get_avatar(bot_info, 'Data URI', '../../static/logo/logo.svg'),
-                            name=bot_info.user_name,
-                        ),
-                        command='top查我',
-                    ),
-                )
-            ) as page_hash:
-                message = UniMessage.image(
-                    raw=await screenshot(urlunparse(('http', get_self_netloc(), f'/host/{page_hash}.html', '', '', '')))
-                )
-        return message
-
-    @override
-    async def handle_query(self) -> UniMessage:
-        """处理查询消息"""
-        self.command_type = 'query'
-        await self.check_user()
-        game_data = await self.get_game_data()
-        message = ''
-        if game_data.day is not None:
-            message += f'用户 {self.user.name} 24小时内统计数据为: '
-            message += f"\nL'PM: {round(game_data.day.lpm,2)} ( {round(game_data.day.lpm/24,2)} pps )"
-            message += f'\nAPM: {round(game_data.day.apm,2)} ( x{round(game_data.day.apm/game_data.day.lpm,2)} )'
-        else:
-            message += f'用户 {self.user.name} 暂无24小时内统计数据'
-        if game_data.total is not None:
-            message += '\n历史统计数据为: '
-            message += f"\nL'PM: {round(game_data.total.lpm,2)} ( {round(game_data.total.lpm/24,2)} pps )"
-            message += f'\nAPM: {round(game_data.total.apm,2)} ( x{round(game_data.total.apm/game_data.total.lpm,2)} )'
-        else:
-            message += '\n暂无历史统计数据'
-        return UniMessage(message)
-
-    async def get_user_profile(self) -> str:
-        """获取用户信息"""
-        if self.processed_data.user_profile is None:
-            url = splice_url([BASE_URL, 'profile.php', f'?{urlencode({"user":self.user.name})}'])
-            self.raw_response.user_profile = await Request.request(url, is_json=False)
-            self.processed_data.user_profile = self.raw_response.user_profile.decode()
-        return self.processed_data.user_profile
-
-    async def check_user(self) -> None:
-        if 'user not found!' in await self.get_user_profile():
-            raise RequestError('用户不存在!')
-
-    async def get_user_name(self) -> str:
-        """获取用户名"""
-        data = etree.HTML(await self.get_user_profile()).xpath('//div[@class="mycontent"]/h1/text()')
-        return data[0].replace("'s profile", '')
-
-    async def get_game_data(self) -> GameData:
-        """获取游戏统计数据"""
-        html = etree.HTML(await self.get_user_profile())
-        day = None
-        with suppress(ValueError):
-            day = Data(
-                lpm=float(str(html.xpath('//div[@class="mycontent"]/text()[3]')[0]).replace('lpm:', '').strip()),
-                apm=float(str(html.xpath('//div[@class="mycontent"]/text()[4]')[0]).replace('apm:', '').strip()),
-            )
-        table = StringIO(
-            etree.tostring(
-                html.xpath('//div[@class="mycontent"]/table[@class="mytable"]')[0],
-                encoding='utf-8',
-            ).decode()
-        )
-        dataframe = read_html(table, encoding='utf-8', header=0)[0]
-        total = Data(lpm=dataframe['lpm'].mean(), apm=dataframe['apm'].mean()) if len(dataframe) != 0 else None
-        return GameData(day=day, total=total)
+async def get_game_data(player: Player, query_num: int = 50) -> GameData | None:
+    """获取游戏数据"""
+    user_profile = await player.get_profile()
+    if user_profile.data == []:
+        return None
+    weighted_total_lpm = weighted_total_apm = weighted_total_adpm = total_time = 0.0
+    num = 0
+    for i in user_profile.data:
+        # 排除单人局和时间为0的游戏
+        # 茶: 不计算没挖掘的局, 即使apm和lpm也如此
+        if i.num_players == 1 or i.time == 0 or i.dig is None:
+            continue
+        # 加权计算
+        time = i.time / 1000
+        lpm = 24 * (i.pieces / time)
+        apm = (i.attack / time) * 60
+        adpm = ((i.attack + i.dig) / time) * 60
+        weighted_total_lpm += lpm * time
+        weighted_total_apm += apm * time
+        weighted_total_adpm += adpm * time
+        total_time += time
+        num += 1
+        if num >= query_num:
+            break
+    if num == 0:
+        return None
+    # TODO: 如果有效局数小于 {查询数} , 并且没有无dig信息的局, 且 user_profile.data 内有{请求数}个局, 则继续往前获取信息
+    metrics = get_metrics(
+        lpm=weighted_total_lpm / total_time, apm=weighted_total_apm / total_time, adpm=weighted_total_adpm / total_time
+    )
+    lpm = weighted_total_lpm / total_time
+    apm = weighted_total_apm / total_time
+    adpm = weighted_total_adpm / total_time
+    return GameData(game_num=num, metrics=metrics)
+
+
+async def make_query_text(player: Player) -> UniMessage:
+    user_info, game_data = await gather(player.get_info(), get_game_data(player))
+    user_data = user_info.data
+    message = f'用户 {user_data.name} ({user_data.teaid}) '
+    if user_data.ranked_games == '0':
+        message += '暂无段位统计数据'
+    else:
+        message += f', 段位分 {round(float(user_data.rating_now),2)}±{round(float(user_data.rd_now),2)} ({round(float(user_data.vol_now),2)}) '
+    if game_data is None:
+        message += ', 暂无游戏数据'
+    else:
+        message += f', 最近 {game_data.game_num} 局数据'
+        message += f"\nL'PM: {game_data.metrics.lpm} ( {game_data.metrics.pps} pps )"
+        message += f'\nAPM: {game_data.metrics.apm} ( x{game_data.metrics.apl} )'
+        message += f'\nADPM: {game_data.metrics.adpm} ( x{game_data.metrics.adpl} ) ( {game_data.metrics.vs}vs )'
+    message += f'\n40L: {float(user_data.pb_sprint)/1000:.2f}s' if user_data.pb_sprint != '2147483647' else ''
+    message += f'\nMarathon: {user_data.pb_marathon}' if user_data.pb_marathon != '0' else ''
+    message += f'\nChallenge: {user_data.pb_challenge}' if user_data.pb_challenge != '0' else ''
+    return UniMessage(message)
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 from datetime import datetime
 from typing import Literal
 
 from pydantic import BaseModel, Field
 
 
-class SuccessModel(BaseModel):
-    class Data(BaseModel):
-        class PeriodMatch(BaseModel):
-            name: str
-            teaid: str = Field(..., alias='teaId')
-            rating: str
-            rd: str
-            start_time: datetime = Field(..., alias='startTime')
-            end_time: datetime = Field(..., alias='endTime')
-            win: str
-            lose: str
-            score: str
-
-        class UserDataTotalItem(BaseModel):
-            time_map: str = Field(..., alias='timeMap')
-            pieces_map: str = Field(..., alias='piecesMap')
-            clear_lines_map: str = Field(..., alias='clearLinesMap')
-            attacks_map: str = Field(..., alias='attacksMap')
-            dig_map: str = Field(..., alias='digMap')
-            send_map: str = Field(..., alias='sendMap')
-            rise_map: str = Field(..., alias='riseMap')
-            offset_map: str = Field(..., alias='offsetMap')
-            receive_map: str = Field(..., alias='receiveMap')
-            games_map: str = Field(..., alias='gamesMap')
-            tetris_map: str = Field(..., alias='tetrisMap')
-            combo_map: str = Field(..., alias='comboMap')
-            tspin_map: str = Field(..., alias='tspinMap')
-            b2b_map: str = Field(..., alias='b2bMap')
-            perfect_clear_map: str = Field(..., alias='perfectClearMap')
-            time_no_map: str = Field(..., alias='timeNoMap')
-            pieces_no_map: str = Field(..., alias='piecesNoMap')
-            clear_lines_no_map: str = Field(..., alias='clearLinesNoMap')
-            attacks_no_map: str = Field(..., alias='attacksNoMap')
-            dig_no_map: str = Field(..., alias='digNoMap')
-            send_no_map: str = Field(..., alias='sendNoMap')
-            rise_no_map: str = Field(..., alias='riseNoMap')
-            offset_no_map: str = Field(..., alias='offsetNoMap')
-            receive_no_map: str = Field(..., alias='receiveNoMap')
-            games_no_map: str = Field(..., alias='gamesNoMap')
-            tetris_no_map: str = Field(..., alias='tetrisNoMap')
-            combo_no_map: str = Field(..., alias='comboNoMap')
-            tspin_no_map: str = Field(..., alias='tspinNoMap')
-            b2b_no_map: str = Field(..., alias='b2bNoMap')
-            perfect_clear_no_map: str = Field(..., alias='perfectClearNoMap')
-
-        teaid: str = Field(..., alias='teaId')
-        name: str
-        total_exp: str = Field(..., alias='totalExp')
-        ranking: str
-        ranked_games: str = Field(..., alias='rankedGames')
-        rating_now: str = Field(..., alias='ratingNow')
-        rd_now: str = Field(..., alias='rdNow')
-        vol_now: str = Field(..., alias='volNow')
-        rating_last: str = Field(..., alias='ratingLast')
-        rd_last: str = Field(..., alias='rdLast')
-        vol_last: str = Field(..., alias='volLast')
-        period_matches: list[PeriodMatch] = Field(..., alias='periodMatches')
-        user_data_total: list[UserDataTotalItem] = Field(..., alias='userDataTotal')
-        ranking_items: str = Field(..., alias='rankingItems')
-        ranking_game_items: str = Field(..., alias='rankingGameItems')
-        training_level: str = Field(..., alias='trainingLevel')
-        training_wins: str = Field(..., alias='trainingWins')
-        pb_sprint: str = Field(..., alias='PBSprint')
-        pb_marathon: str = Field(..., alias='PBMarathon')
-        pb_challenge: str = Field(..., alias='PBChallenge')
-        register_date: datetime = Field(..., alias='registerDate')
-        last_login_date: datetime = Field(..., alias='lastLoginDate')
+class PeriodMatch(BaseModel):
+    name: str
+    teaid: str = Field(..., alias='teaId')
+    rating: str
+    rd: str
+    start_time: datetime = Field(..., alias='startTime')
+    end_time: datetime = Field(..., alias='endTime')
+    win: str
+    lose: str
+    score: str
+
+
+class UserDataTotalItem(BaseModel):
+    time_map: str = Field(..., alias='timeMap')
+    pieces_map: str = Field(..., alias='piecesMap')
+    clear_lines_map: str = Field(..., alias='clearLinesMap')
+    attacks_map: str = Field(..., alias='attacksMap')
+    dig_map: str = Field(..., alias='digMap')
+    send_map: str = Field(..., alias='sendMap')
+    rise_map: str = Field(..., alias='riseMap')
+    offset_map: str = Field(..., alias='offsetMap')
+    receive_map: str = Field(..., alias='receiveMap')
+    games_map: str = Field(..., alias='gamesMap')
+    tetris_map: str = Field(..., alias='tetrisMap')
+    combo_map: str = Field(..., alias='comboMap')
+    tspin_map: str = Field(..., alias='tspinMap')
+    b2b_map: str = Field(..., alias='b2bMap')
+    perfect_clear_map: str = Field(..., alias='perfectClearMap')
+    time_no_map: str = Field(..., alias='timeNoMap')
+    pieces_no_map: str = Field(..., alias='piecesNoMap')
+    clear_lines_no_map: str = Field(..., alias='clearLinesNoMap')
+    attacks_no_map: str = Field(..., alias='attacksNoMap')
+    dig_no_map: str = Field(..., alias='digNoMap')
+    send_no_map: str = Field(..., alias='sendNoMap')
+    rise_no_map: str = Field(..., alias='riseNoMap')
+    offset_no_map: str = Field(..., alias='offsetNoMap')
+    receive_no_map: str = Field(..., alias='receiveNoMap')
+    games_no_map: str = Field(..., alias='gamesNoMap')
+    tetris_no_map: str = Field(..., alias='tetrisNoMap')
+    combo_no_map: str = Field(..., alias='comboNoMap')
+    tspin_no_map: str = Field(..., alias='tspinNoMap')
+    b2b_no_map: str = Field(..., alias='b2bNoMap')
+    perfect_clear_no_map: str = Field(..., alias='perfectClearNoMap')
+
+
+class Data(BaseModel):
+    teaid: str = Field(..., alias='teaId')
+    name: str
+    total_exp: str = Field(..., alias='totalExp')
+    ranking: str
+    ranked_games: str = Field(..., alias='rankedGames')
+    rating_now: str = Field(..., alias='ratingNow')
+    rd_now: str = Field(..., alias='rdNow')
+    vol_now: str = Field(..., alias='volNow')
+    rating_last: str = Field(..., alias='ratingLast')
+    rd_last: str = Field(..., alias='rdLast')
+    vol_last: str = Field(..., alias='volLast')
+    period_matches: list[PeriodMatch] = Field(..., alias='periodMatches')
+    user_data_total: list[UserDataTotalItem] = Field(..., alias='userDataTotal')
+    ranking_items: str = Field(..., alias='rankingItems')
+    ranking_game_items: str = Field(..., alias='rankingGameItems')
+    training_level: str = Field(..., alias='trainingLevel')
+    training_wins: str = Field(..., alias='trainingWins')
+    pb_sprint: str = Field(..., alias='PBSprint')
+    pb_marathon: str = Field(..., alias='PBMarathon')
+    pb_challenge: str = Field(..., alias='PBChallenge')
+    register_date: datetime = Field(..., alias='registerDate')
+    last_login_date: datetime = Field(..., alias='lastLoginDate')
 
+
+class UserInfoSuccess(BaseModel):
     code: int
     success: Literal[True]
     data: Data
 
 
 class FailedModel(BaseModel):
     code: int
     success: Literal[False]
     error: str
 
 
-UserInfo = SuccessModel | FailedModel
+UserInfo = UserInfoSuccess | FailedModel
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from datetime import datetime
 from typing import Literal
 
 from pydantic import BaseModel
 
 
-class UserProfile(BaseModel):
-    class Data(BaseModel):
-        idmultiplayergameresult: int
-        iduser: str
-        teaid: str
-        time: int
-        clear_lines: int
-        attack: int
-        send: int
-        offset: int
-        receive: int
-        rise: int
-        dig: int
-        pieces: int
-        max_combo: int
-        pc_count: int
-        place: int
-        num_players: int
-        fumen_code: Literal['0', '1']  # wtf
-        rule_set: str
-        garbage: str
-        idmultiplayergame: int
-        datetime: datetime
+class Data(BaseModel):
+    idmultiplayergameresult: int
+    iduser: str
+    teaid: str
+    time: int
+    clear_lines: int
+    attack: int
+    send: int
+    offset: int
+    receive: int
+    rise: int
+    dig: int
+    pieces: int
+    max_combo: int
+    pc_count: int
+    place: int
+    num_players: int
+    fumen_code: Literal['0', '1']  # wtf
+    rule_set: str
+    garbage: str
+    idmultiplayergame: int
+    datetime: datetime
+
 
+class UserProfile(BaseModel):
     code: int
     success: bool
     data: list[Data]
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/avatar.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/avatar.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,18 @@
         bytes: bytes 格式的头像
     """
 
 
 async def get_avatar(user: UserInfo, scheme: Literal['Data URI', 'bytes'], default: str | None) -> str | bytes:
     if user.user_avatar is None:
         if default is None:
-            raise TypeError("Can't get avatar")
+            msg = "Can't get avatar"
+            raise TypeError(msg)
         return default
     bot_avatar = await user.user_avatar.get_image()
     if scheme == 'Data URI':
         avatar_format = Image.open(BytesIO(bot_avatar)).format
         if avatar_format is None:
-            raise TypeError("Can't get avatar format")
+            msg = "Can't get avatar format"
+            raise TypeError(msg)
         return f'data:{Image.MIME[avatar_format]};base64,{b64encode(bot_avatar).decode()}'
     return bot_avatar
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,48 +11,48 @@
 driver = get_driver()
 
 global_config = driver.config
 
 
 @driver.on_startup
 async def _():
-    await BrowserManager._init_playwright()
+    await BrowserManager.init_playwright()
 
 
 @driver.on_shutdown
 async def _():
-    await BrowserManager._close_browser()
+    await BrowserManager.close_browser()
 
 
 class BrowserManager:
     """浏览器管理类"""
 
     _browser: Browser | None = None
 
     @classmethod
-    async def _init_playwright(cls) -> None:
+    async def init_playwright(cls) -> None:
         if system() == 'Windows' and getattr(global_config, 'fastapi_reload', False):
-            raise ImportError('加载失败, Windows 必须设置 FASTAPI_RELOAD=false 才能正常运行 playwright')
+            msg = '加载失败, Windows 必须设置 FASTAPI_RELOAD=false 才能正常运行 playwright'
+            raise ImportError(msg)
         logger.info('开始 安装/更新 playwright 浏览器')
         environ['PLAYWRIGHT_DOWNLOAD_HOST'] = 'https://npmmirror.com/mirrors/playwright/'
         if cls._call_playwright(['', 'install', 'firefox']):
             logger.success('安装/更新 playwright 浏览器成功')
         else:
             logger.warning('playwright 浏览器 安装/更新 失败, 尝试使用原始仓库下载')
             del environ['PLAYWRIGHT_DOWNLOAD_HOST']
             if cls._call_playwright(['', 'install', 'firefox']):
                 logger.success('安装/更新 playwright 浏览器成功')
             else:
                 logger.error('安装/更新 playwright 浏览器失败')
         try:
             await cls._start_browser()
         except BaseException as e:  # 不知道会有什么异常, 交给用户解决
-            raise ImportError(
-                'playwright 启动失败, 请尝试在命令行运行 playwright install-deps firefox, 如果仍然启动失败, 请参考上面的报错👆'
-            ) from e
+            msg = 'playwright 启动失败, 请尝试在命令行运行 playwright install-deps firefox, 如果仍然启动失败, 请参考上面的报错👆'
+            raise ImportError(msg) from e
         else:
             logger.success('playwright 启动成功')
 
     @classmethod
     def _call_playwright(cls, argv: list[str]) -> bool:
         """等价于调用 playwright 的命令行程序"""
         argv_backup = sys.argv.copy()
@@ -77,11 +77,11 @@
 
     @classmethod
     async def get_browser(cls) -> Browser:
         """获取浏览器实例"""
         return cls._browser or await cls._start_browser()
 
     @classmethod
-    async def _close_browser(cls) -> None:
+    async def close_browser(cls) -> None:
         """关闭浏览器实例"""
         if isinstance(cls._browser, Browser):
             await cls._browser.close()
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/host.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/host.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from hashlib import sha256
 from ipaddress import IPv4Address, IPv6Address
-from typing import ClassVar
+from typing import TYPE_CHECKING, ClassVar
 
 from fastapi import FastAPI, status
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from nonebot import get_app, get_driver
 from nonebot.log import logger
 from nonebot_plugin_localstore import get_cache_dir  # type: ignore[import-untyped]
-from pydantic import IPvAnyAddress
 
 from .templates import templates_dir
 
+if TYPE_CHECKING:
+    from pydantic import IPvAnyAddress
+
 app = get_app()
 
 driver = get_driver()
 
 global_config = driver.config
 
 cache_dir = get_cache_dir('nonebot_plugin_tetris_stats')
 
 if not isinstance(app, FastAPI):
-    raise RuntimeError('本插件需要 FastAPI 驱动器才能运行')  # noqa: TRY004
+    msg = '本插件需要 FastAPI 驱动器才能运行'
+    raise RuntimeError(msg)  # noqa: TRY004
 
 NOT_FOUND = HTMLResponse('404 Not Found', status_code=status.HTTP_404_NOT_FOUND)
 
 
 class HostPage:
     pages: ClassVar[dict[str, str]] = {}
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -143,141 +143,101 @@
         return round(self._adpm / self._lpm, self.precision)
 
 
 @overload
 def get_metrics(
     *,
     pps: Number,
-    lpm: None = None,
-    apm: None = None,
-    vs: None = None,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsBaseWithPPS:
-    ...
+) -> TetrisMetricsBaseWithPPS: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
     lpm: Number,
-    apm: None = None,
-    vs: None = None,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsBaseWithLPM:
-    ...
+) -> TetrisMetricsBaseWithLPM: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
-    lpm: None = None,
-    apm: None = None,
     vs: Number,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsBaseWithVS:
-    ...
+) -> TetrisMetricsBaseWithVS: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
-    lpm: None = None,
-    apm: None = None,
-    vs: None = None,
     adpm: Number,
     precision: int = 2,
-) -> TetrisMetricsBaseWithADPM:
-    ...
+) -> TetrisMetricsBaseWithADPM: ...
 
 
 @overload
 def get_metrics(
     *,
     pps: Number,
-    lpm: None = None,
     apm: Number,
-    vs: None = None,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsBasicWithPPS:
-    ...
+) -> TetrisMetricsBasicWithPPS: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
     lpm: Number,
     apm: Number,
-    vs: None = None,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsBasicWithLPM:
-    ...
+) -> TetrisMetricsBasicWithLPM: ...
 
 
 @overload
 def get_metrics(
     *,
     pps: Number,
-    lpm: None = None,
     apm: Number,
     vs: Number,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsProWithPPSVS:
-    ...
+) -> TetrisMetricsProWithPPSVS: ...
 
 
 @overload
 def get_metrics(
     *,
     pps: Number,
-    lpm: None = None,
     apm: Number,
-    vs: None = None,
     adpm: Number,
     precision: int = 2,
-) -> TetrisMetricsProWithPPSADPM:
-    ...
+) -> TetrisMetricsProWithPPSADPM: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
     lpm: Number,
     apm: Number,
     vs: Number,
-    adpm: None = None,
     precision: int = 2,
-) -> TetrisMetricsProWithLPMVS:
-    ...
+) -> TetrisMetricsProWithLPMVS: ...
 
 
 @overload
 def get_metrics(
     *,
-    pps: None = None,
     lpm: Number,
     apm: Number,
-    vs: None = None,
     adpm: Number,
     precision: int = 2,
-) -> TetrisMetricsProWithLPMADPM:
-    ...
+) -> TetrisMetricsProWithLPMADPM: ...
 
 
-def get_metrics(  # noqa: PLR0911, PLR0912, PLR0913
+def get_metrics(  # noqa: PLR0911, PLR0912, PLR0913, C901
     *,
     pps: Number | None = None,
     lpm: Number | None = None,
     apm: Number | None = None,
     vs: Number | None = None,
     adpm: Number | None = None,
     precision: int = 2,
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 driver = get_driver()
 config = get_plugin_config(Config)
 
 
 @driver.on_startup
 async def _():
-    await Request._init_cache()
-    await Request._read_cache()
+    await Request.init_cache()
+    await Request.read_cache()
 
 
 @driver.on_shutdown
 async def _():
-    await Request._write_cache()
+    await Request.write_cache()
 
 
 def splice_url(url_list: list[str]) -> str:
     url = ''
     if len(url_list):
         url = url_list.pop(0)
         for i in url_list:
@@ -62,77 +62,78 @@
                     break
                 try:
                     loads(text)
                 except JSONDecodeError:
                     await page.wait_for_timeout(1000)
                 else:
                     if not isinstance(response, Response):
-                        raise RequestError('api请求失败')
+                        msg = 'api请求失败'
+                        raise RequestError(msg)
                     cls._headers = await response.request.all_headers()
                     try:
                         cls._cookies = {
                             name: value
                             for i in await context.cookies()
                             if (name := i.get('name')) is not None and (value := i.get('value')) is not None
                         }
                     except KeyError:
                         cls._cookies = None
                     return await response.body()
-        raise RequestError('绕过五秒盾失败')
+        msg = '绕过五秒盾失败'
+        raise RequestError(msg)
 
     @classmethod
-    async def _init_cache(cls) -> None:
+    async def init_cache(cls) -> None:
         """初始化缓存文件"""
         if not cls._CACHE_FILE.exists():
             async with open(file=cls._CACHE_FILE, mode='w', encoding='UTF-8') as file:
                 await file.write(dumps({'headers': cls._headers, 'cookies': cls._cookies}))
 
     @classmethod
-    async def _read_cache(cls) -> None:
+    async def read_cache(cls) -> None:
         """读取缓存文件"""
         try:
             async with open(file=cls._CACHE_FILE, mode='r', encoding='UTF-8') as file:
                 json = loads(await file.read())
         except FileNotFoundError:
-            await cls._init_cache()
+            await cls.init_cache()
         except (PermissionError, JSONDecodeError):
             cls._CACHE_FILE.unlink()
-            await cls._init_cache()
+            await cls.init_cache()
         else:
             cls._headers = json['headers']
             cls._cookies = json['cookies']
 
     @classmethod
-    async def _write_cache(cls) -> None:
+    async def write_cache(cls) -> None:
         """写入缓存文件"""
         try:
             async with open(file=cls._CACHE_FILE, mode='r+', encoding='UTF-8') as file:
                 await file.write(dumps({'headers': cls._headers, 'cookies': cls._cookies}))
         except FileNotFoundError:
-            await cls._init_cache()
+            await cls.init_cache()
         except (PermissionError, JSONDecodeError):
             cls._CACHE_FILE.unlink()
-            await cls._init_cache()
+            await cls.init_cache()
 
     @classmethod
     async def request(cls, url: str, *, is_json: bool = True) -> bytes:
         """请求api"""
         try:
             async with AsyncClient(cookies=cls._cookies, timeout=config.tetris_req_timeout) as session:
                 response = await session.get(url, headers=cls._headers)
                 if response.status_code != HTTPStatus.OK:
-                    raise RequestError(
-                        f'请求错误 code: {response.status_code} {HTTPStatus(response.status_code).phrase}\n{response.text}',
-                        status_code=response.status_code,
-                    )
+                    msg = f'请求错误 code: {response.status_code} {HTTPStatus(response.status_code).phrase}\n{response.text}'
+                    raise RequestError(msg, status_code=response.status_code)
                 if is_json:
                     loads(response.content)
                 return response.content
         except HTTPError as e:
-            raise RequestError(f'请求错误 \n{e!r}') from e
+            msg = f'请求错误 \n{e!r}'
+            raise RequestError(msg) from e
         except JSONDecodeError:
             if urlparse(url).netloc.lower().endswith('tetr.io'):
                 return await cls._anti_cloudflare(url)
             raise
 
     @classmethod
     async def failover_request(
@@ -158,8 +159,9 @@
                     if isinstance(tb.tb_frame.f_locals.get('exc_value'), failover_exc):
                         error_list.append(e)
                         break
                     tb = tb.tb_next
                 else:
                     raise
                 continue
-        raise RequestError(f'所有地址皆不可用\n{error_list!r}')
+        msg = f'所有地址皆不可用\n{error_list!r}'
+        raise RequestError(msg)
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,12 +26,13 @@
                     attempts += 1
                     if attempts <= max_attempts:
                         if delay is not None:
                             await sleep(delay.total_seconds())
                         logger.debug(f'Retrying: {func.__name__} ({attempts}/{max_attempts})')
                         continue
                     raise
-            raise RuntimeError('Unexpectedly reached the end of the retry loop')
+            msg = 'Unexpectedly reached the end of the retry loop'
+            raise RuntimeError(msg)
 
         return cast(Callable[..., Awaitable[T]], wrapper)
 
     return decorator
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/templates.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 
 @driver.on_startup
 async def init_templates() -> None:
     try:
         await create_subprocess_exec('git', '--version', stdout=PIPE)
     except FileNotFoundError as e:
-        raise RuntimeError(
-            '未找到 git, 请确保 git 已安装并在环境变量中\n安装步骤请参阅: https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git'
-        ) from e
+        msg = '未找到 git, 请确保 git 已安装并在环境变量中\n安装步骤请参阅: https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git'
+        raise RuntimeError(msg) from e
     if not templates_dir.exists():
         logger.info('模板仓库不存在, 正在尝试初始化...')
         proc = await create_subprocess_exec(
             'git',
             'clone',
             '-b',
             'gh-pages',
@@ -35,15 +34,16 @@
             stdout=PIPE,
             stderr=PIPE,
         )
         stdout, stderr = await proc.communicate()
         if proc.returncode != 0:
             for i in stderr.decode().splitlines():
                 logger.error(i)
-            raise RuntimeError('初始化模板仓库失败')
+            msg = '初始化模板仓库失败'
+            raise RuntimeError(msg)
         logger.success('模板仓库初始化成功')
         return
     proc = await create_subprocess_exec(
         'git', 'rev-parse', '--is-inside-work-tree', stdout=PIPE, stderr=PIPE, cwd=templates_dir
     )
     stdout, stderr = await proc.communicate()
     if proc.returncode != 0:
@@ -56,15 +56,16 @@
     logger.info('正在更新模板仓库...')
     proc = await create_subprocess_exec('git', 'pull', stdout=PIPE, stderr=PIPE, cwd=templates_dir)
     stdout, stderr = await proc.communicate()
     logger.info(stdout.decode().strip())
     if proc.returncode != 0:
         for i in stderr.decode().splitlines():
             logger.error(i)
-        raise RuntimeError('更新模板仓库失败')
+        msg = '更新模板仓库失败'
+        raise RuntimeError(msg)
     logger.success('模板仓库更新成功')
 
 
 @alc.handle()
 async def _():
     await init_templates()
     await alc.finish('模板仓库更新成功')
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.2.0/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.5/pyproject.toml` & `nonebot_plugin_tetris_stats-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.1.5'
+version = '1.2.0'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
 
 [tool.poetry.dependencies]
 python = '^3.10'
 nonebot2 = { extras = ["fastapi"], version = "^2.3.0" }
-lxml = '^5.1.0'
-pandas = '>=1.4.3,<3.0.0'
-playwright = '^1.41.2'
-ujson = '^5.9.0'
-aiofiles = "^23.2.1"
-nonebot-plugin-orm = ">=0.1.1,<0.8.0"
-nonebot-plugin-localstore = "^0.6.0"
-httpx = "^0.27.0"
 nonebot-plugin-alconna = ">=0.40"
 nonebot-plugin-apscheduler = "^0.4.0"
+nonebot-plugin-localstore = "^0.6.0"
+nonebot-plugin-orm = ">=0.1.1,<0.8.0"
+nonebot-plugin-session = "^0.3.1"
+nonebot-plugin-session-orm = "^0.2.0"
+nonebot-plugin-userinfo = "^0.2.4"
 aiocache = "^0.12.2"
-zstandard = "^0.22.0"
+aiofiles = "^23.2.1"
+httpx = "^0.27.0"
 jinja2 = "^3.1.3"
-nonebot-plugin-userinfo = "^0.2.4"
+lxml = '^5.1.0'
+pandas = '>=1.4.3,<3.0.0'
 pillow = "^10.3.0"
+playwright = '^1.41.2'
 rich = "^13.7.1"
+ujson = '^5.9.0'
+zstandard = "^0.22.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = '>=1.9'
-types-ujson = '^5.9.0'
-pandas-stubs = '>=1.5.2,<3.0.0'
 ruff = '>=0.3.0'
 types-aiofiles = "^23.2.0.20240106"
 types-lxml = "^2024.2.9"
+types-pillow = "^10.2.0.20240423"
+types-ujson = '^5.9.0'
+pandas-stubs = '>=1.5.2,<3.0.0'
 nonebot-plugin-orm = { extras = ["default"], version = ">=0.3,<0.8" }
+nonebot-adapter-discord = "^0.1.3"
+nonebot-adapter-kaiheila = "^0.3.4"
 nonebot-adapter-onebot = "^2.4.1"
+nonebot-adapter-qq = "^1.4.4"
 nonebot-adapter-satori = "^0.11.4"
-nonebot-adapter-kaiheila = "^0.3.4"
-nonebot-adapter-discord = "^0.1.3"
-types-pillow = "^10.2.0.20240423"
 
 [tool.poetry.group.debug.dependencies]
 objprint = '^0.2.2'
 viztracer = "^0.16.2"
 
 [build-system]
 requires = ['poetry-core>=1.0.0']
@@ -55,49 +58,64 @@
 target-version = "py310"
 
 [tool.ruff.lint]
 select = [
     'F',     # pyflakes
     'E',     # pycodestyle errors
     'W',     # pycodestyle warnings
+    'C90',   # mccabe
     'I',     # isort
     'N',     # PEP8-naming
     'UP',    # pyupgrade
     'YTT',   # flake8-2020
     'ANN',   # flake8-annotations
     'ASYNC', # flake8-async
     'S',     # flake8-bandit
     'BLE',   # flake8-blind-except
     'FBT',   # flake8-boolean-trap
     'B',     # flake8-bugbear
     'A',     # flake8-builtins
+    'COM',   # flake8-commas
     'C4',    # flake8-comprehensions
     'DTZ',   # flake8-datetimez
+    'T10',   # flake8-debugger
+    'EM',    # flake8-errmsg
     'FA',    # flake8-future-annotations
     'ISC',   # flake8-implicit-str-concat
+    'ICN',   # flake8-import-conventions
     'PIE',   # flake8-pie
     'T20',   # flake8-print
     'Q',     # flake8-quotes
     'RSE',   # flake8-raise
     'RET',   # flake8-return
+    'SLF',   # flake8-self
     'SIM',   # flake8-simplify
+    'TID',   # flake8-tidy-imports
+    'TCH',   # flake8-type-checking
+    'ARG',   # flake8-unused-arguments
     'PTH',   # flake8-use-pathlib
+    'ERA',   # eradicate
     'PD',    # pandas-vet
+    'PGH',   # pygrep-hooks
     'PL',    # pylint
     'TRY',   # tryceratops
     'FLY',   # flynt
     'PERF',  # Perflint
+    'FURB',  # refurb
     'RUF',   # Ruff-specific rules
 ]
 ignore = [
     'E501',   # 过长的行由 ruff format 处理, 剩余的都是字符串
     'ANN101', # 由 type checker 自动推断
     'ANN102', # 由 type checker 自动推断
     'ANN202', # 向 NoneBot 注册的函数
     'TRY003',
+    'COM812', # 强制尾随逗号
+    'TID252', # 相对导入
+    'ISC001', # format warning
 ]
 flake8-quotes = { inline-quotes = 'single', multiline-quotes = 'double' }
 
 [tool.ruff.lint.flake8-annotations]
 mypy-init-return = true
 
 [tool.ruff.lint.flake8-builtins]
```

### Comparing `nonebot_plugin_tetris_stats-1.1.5/PKG-INFO` & `nonebot_plugin_tetris_stats-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.1.5
+Version: 1.2.0
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -17,14 +17,16 @@
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: nonebot-plugin-alconna (>=0.40)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0)
 Requires-Dist: nonebot-plugin-localstore (>=0.6.0,<0.7.0)
 Requires-Dist: nonebot-plugin-orm (>=0.1.1,<0.8.0)
+Requires-Dist: nonebot-plugin-session (>=0.3.1,<0.4.0)
+Requires-Dist: nonebot-plugin-session-orm (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-userinfo (>=0.2.4,<0.3.0)
 Requires-Dist: nonebot2[fastapi] (>=2.3.0,<3.0.0)
 Requires-Dist: pandas (>=1.4.3,<3.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: playwright (>=1.41.2,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.0 Summary:
 ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸ææ°æ®çæä»¶ Home-
 page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats License:
 AGPL-3.0 Author: scdhh Author-email: wallfjjd@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiocache (>=0.12.2,<0.13.0) Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0) Requires-Dist: nonebot-plugin-alconna
 (>=0.40) Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0) Requires-
 Dist: nonebot-plugin-localstore (>=0.6.0,<0.7.0) Requires-Dist: nonebot-plugin-
-orm (>=0.1.1,<0.8.0) Requires-Dist: nonebot-plugin-userinfo (>=0.2.4,<0.3.0)
-Requires-Dist: nonebot2[fastapi] (>=2.3.0,<3.0.0) Requires-Dist: pandas
-(>=1.4.3,<3.0.0) Requires-Dist: pillow (>=10.3.0,<11.0.0) Requires-Dist:
-playwright (>=1.41.2,<2.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-
-Dist: ujson (>=5.9.0,<6.0.0) Requires-Dist: zstandard (>=0.22.0,<0.23.0)
-Project-URL: Repository, https://github.com/shoucandanghehe/nonebot-plugin-
-tetris-stats Description-Content-Type: text/markdown
+orm (>=0.1.1,<0.8.0) Requires-Dist: nonebot-plugin-session (>=0.3.1,<0.4.0)
+Requires-Dist: nonebot-plugin-session-orm (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot-plugin-userinfo (>=0.2.4,<0.3.0) Requires-Dist: nonebot2[fastapi]
+(>=2.3.0,<3.0.0) Requires-Dist: pandas (>=1.4.3,<3.0.0) Requires-Dist: pillow
+(>=10.3.0,<11.0.0) Requires-Dist: playwright (>=1.41.2,<2.0.0) Requires-Dist:
+rich (>=13.7.1,<14.0.0) Requires-Dist: ujson (>=5.9.0,<6.0.0) Requires-Dist:
+zstandard (>=0.22.0,<0.23.0) Project-URL: Repository, https://github.com/
+shoucandanghehe/nonebot-plugin-tetris-stats Description-Content-Type: text/
+markdown
                                     [logo]
 # Tetris Stats â¨ ä¸æ¬¾åºäº [NoneBot2](https://github.com/nonebot/nonebot2)
 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸æç©å®¶æ°æ®çæä»¶ â¨
                _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_]_[_P_y_P_i_]_[_R_u_f_f_]_[_G_i_t_m_o_j_i_]_[_w_a_k_a_t_i_m_e_]
 ## â¨ ç®åæ¯æçæ¸¸æ - [TETR.IO](https://tetr.io/) - [è¶æ](https://
 teatube.cn/tos/) - [TOP](http://tetrisonline.pl/) ## ð å®è£ - ä½¿ç¨ nb-
 cli ```bash nb plugin install nonebot-plugin-tetris-stats ``` - ä½¿ç¨ poetry
```


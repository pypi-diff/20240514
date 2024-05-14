# Comparing `tmp/shroudstone-0.1.2.tar.gz` & `tmp/shroudstone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroudstone-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shroudstone-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shroudstone-0.1.2.tar` & `shroudstone-0.1.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      957 2024-02-27 12:08:06.662709 shroudstone-0.1.2/.github/workflows/build-exe.yml
--rw-r--r--   0        0        0       45 2024-02-28 11:05:03.022804 shroudstone-0.1.2/.gitignore
--rw-r--r--   0        0        0    32422 2024-02-25 06:24:42.992531 shroudstone-0.1.2/LICENSE
--rw-r--r--   0        0        0     7244 2024-03-23 01:38:38.331578 shroudstone-0.1.2/README.md
--rwxr-xr-x   0        0        0      514 2024-02-29 02:05:53.988528 shroudstone-0.1.2/api-client-codegen.sh
--rwxr-xr-x   0        0        0      297 2024-02-25 06:24:42.992531 shroudstone-0.1.2/codegen.sh
--rw-r--r--   0        0        0    90765 2024-03-07 06:03:55.756412 shroudstone-0.1.2/docs/example-screenshot.png
--rw-r--r--   0        0        0      185 2024-03-23 01:38:38.331578 shroudstone-0.1.2/pyinstaller_build.bat
--rw-r--r--   0        0        0      873 2024-03-23 01:38:38.331578 shroudstone-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-11 03:07:01.984564 shroudstone-0.1.2/shroudstone/__init__.py
--rw-r--r--   0        0        0      373 2024-03-01 04:58:54.233893 shroudstone-0.1.2/shroudstone/__main__.py
--rw-r--r--   0        0        0     7858 2024-05-11 01:09:56.591517 shroudstone-0.1.2/shroudstone/cli.py
--rw-r--r--   0        0        0     2572 2024-03-23 01:38:38.331578 shroudstone-0.1.2/shroudstone/config.py
--rw-r--r--   0        0        0        0 2024-03-07 06:03:55.756412 shroudstone-0.1.2/shroudstone/gui/__init__.py
--rw-r--r--   0        0        0       43 2024-02-27 12:08:06.666709 shroudstone-0.1.2/shroudstone/gui/__main__.py
--rw-r--r--   0        0        0    15443 2024-05-11 01:09:56.591517 shroudstone-0.1.2/shroudstone/gui/app.py
--rw-r--r--   0        0        0    16958 2024-02-27 12:08:06.666709 shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.ico
--rw-r--r--   0        0        0     2821 2024-02-27 12:08:06.666709 shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.png
--rw-r--r--   0        0        0     6363 2024-02-27 12:08:06.666709 shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.svg
--rw-r--r--   0        0        0      569 2024-03-23 01:38:38.331578 shroudstone-0.1.2/shroudstone/gui/fonts.py
--rw-r--r--   0        0        0     2779 2024-03-07 04:57:52.650122 shroudstone-0.1.2/shroudstone/gui/jobs.py
--rw-r--r--   0        0        0     3002 2024-03-23 01:38:38.331578 shroudstone-0.1.2/shroudstone/gui/logview.py
--rw-r--r--   0        0        0      621 2024-03-23 01:38:38.331578 shroudstone-0.1.2/shroudstone/logging.py
--rwxr-xr-x   0        0        0    21707 2024-05-11 03:06:48.056450 shroudstone-0.1.2/shroudstone/renamer.py
--rwxr-xr-x   0        0        0    11462 2024-05-11 02:50:42.075928 shroudstone-0.1.2/shroudstone/replay.py
--rw-r--r--   0        0        0      353 2024-02-28 10:42:52.460560 shroudstone-0.1.2/shroudstone/sgw_api.py
--rw-r--r--   0        0        0     4463 2024-03-06 11:27:47.966810 shroudstone-0.1.2/shroudstone/stormgate_pb2.py
--rw-r--r--   0        0        0     5462 2024-03-06 11:27:47.966810 shroudstone-0.1.2/shroudstone/stormgate_pb2.pyi
--rw-r--r--   0        0        0     5374 2024-03-01 04:58:49.905816 shroudstone-0.1.2/shroudstone/stormgateworld/__init__.py
--rw-r--r--   0        0        0      417 2024-03-01 04:58:49.913816 shroudstone-0.1.2/shroudstone/stormgateworld/api/__init__.py
--rw-r--r--   0        0        0    12807 2024-03-01 04:58:49.917816 shroudstone-0.1.2/shroudstone/stormgateworld/api/leaderboard_entries_api.py
--rw-r--r--   0        0        0    22652 2024-03-01 04:58:49.925816 shroudstone-0.1.2/shroudstone/stormgateworld/api/leaderboards_api.py
--rw-r--r--   0        0        0    11844 2024-03-01 04:58:49.929816 shroudstone-0.1.2/shroudstone/stormgateworld/api/matches_api.py
--rw-r--r--   0        0        0    64249 2024-03-01 04:58:49.937816 shroudstone-0.1.2/shroudstone/stormgateworld/api/players_api.py
--rw-r--r--   0        0        0    43816 2024-03-01 04:58:49.941816 shroudstone-0.1.2/shroudstone/stormgateworld/api/statistics_api.py
--rw-r--r--   0        0        0    25859 2024-03-01 04:58:49.945817 shroudstone-0.1.2/shroudstone/stormgateworld/api_client.py
--rw-r--r--   0        0        0      652 2024-03-01 04:58:49.953817 shroudstone-0.1.2/shroudstone/stormgateworld/api_response.py
--rw-r--r--   0        0        0    15400 2024-03-01 04:58:49.957817 shroudstone-0.1.2/shroudstone/stormgateworld/configuration.py
--rw-r--r--   0        0        0     5968 2024-03-01 04:58:49.965817 shroudstone-0.1.2/shroudstone/stormgateworld/exceptions.py
--rw-r--r--   0        0        0     4353 2024-03-01 04:58:49.969817 shroudstone-0.1.2/shroudstone/stormgateworld/models/__init__.py
--rw-r--r--   0        0        0     3091 2024-03-01 04:58:49.977817 shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics.py
--rw-r--r--   0        0        0     3379 2024-03-01 04:58:49.981817 shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics_activity.py
--rw-r--r--   0        0        0     3113 2024-03-01 04:58:49.989817 shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics_entry.py
--rw-r--r--   0        0        0      770 2024-03-01 04:58:49.997818 shroudstone-0.1.2/shroudstone/stormgateworld/models/aggregation.py
--rw-r--r--   0        0        0     3263 2024-03-01 04:58:50.005818 shroudstone-0.1.2/shroudstone/stormgateworld/models/countries_statistics.py
--rw-r--r--   0        0        0     3090 2024-03-01 04:58:50.009818 shroudstone-0.1.2/shroudstone/stormgateworld/models/countries_statistics_entry.py
--rw-r--r--   0        0        0      731 2024-03-01 04:58:50.017818 shroudstone-0.1.2/shroudstone/stormgateworld/models/dump_format.py
--rw-r--r--   0        0        0     2956 2024-03-01 04:58:50.021818 shroudstone-0.1.2/shroudstone/stormgateworld/models/error_response.py
--rw-r--r--   0        0        0      784 2024-03-01 04:58:50.029818 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard.py
--rw-r--r--   0        0        0     3274 2024-03-01 04:58:50.033818 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_dump_response.py
--rw-r--r--   0        0        0     3459 2024-03-01 04:58:50.037818 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_history.py
--rw-r--r--   0        0        0     3172 2024-03-01 04:58:50.045818 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_history_row.py
--rw-r--r--   0        0        0     6683 2024-03-01 04:58:50.049818 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_response.py
--rw-r--r--   0        0        0      751 2024-03-01 04:58:50.053819 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_order.py
--rw-r--r--   0        0        0     3340 2024-03-01 04:58:50.061819 shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_response.py
--rw-r--r--   0        0        0      843 2024-03-01 04:58:50.065819 shroudstone-0.1.2/shroudstone/stormgateworld/models/league.py
--rw-r--r--   0        0        0     4124 2024-03-01 04:58:50.073819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_player_leaderboard_entry_response.py
--rw-r--r--   0        0        0     3287 2024-03-01 04:58:50.077819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_player_response.py
--rw-r--r--   0        0        0     6065 2024-03-01 04:58:50.081819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_response.py
--rw-r--r--   0        0        0     4510 2024-03-01 04:58:50.089819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_response.py
--rw-r--r--   0        0        0      760 2024-03-01 04:58:50.093819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_result.py
--rw-r--r--   0        0        0      745 2024-03-01 04:58:50.097819 shroudstone-0.1.2/shroudstone/stormgateworld/models/match_state.py
--rw-r--r--   0        0        0     3279 2024-03-01 04:58:50.105820 shroudstone-0.1.2/shroudstone/stormgateworld/models/matches_response.py
--rw-r--r--   0        0        0     4373 2024-03-01 04:58:50.109820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_activity_stats.py
--rw-r--r--   0        0        0     3575 2024-03-01 04:58:50.117820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_activity_stats_race.py
--rw-r--r--   0        0        0     3303 2024-03-01 04:58:50.121820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matches_response.py
--rw-r--r--   0        0        0     3129 2024-03-01 04:58:50.125820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats.py
--rw-r--r--   0        0        0     4181 2024-03-01 04:58:50.133820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats_entry.py
--rw-r--r--   0        0        0     3643 2024-03-01 04:58:50.137820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats_matchup.py
--rw-r--r--   0        0        0     3297 2024-03-01 04:58:50.145820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_opponents_stats.py
--rw-r--r--   0        0        0     4240 2024-03-01 04:58:50.149820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_opponents_stats_opponent.py
--rw-r--r--   0        0        0     5174 2024-03-01 04:58:50.153820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_response.py
--rw-r--r--   0        0        0     4858 2024-03-01 04:58:50.161821 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry.py
--rw-r--r--   0        0        0     4625 2024-03-01 04:58:50.165820 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry_aggregated.py
--rw-r--r--   0        0        0     3704 2024-03-01 04:58:50.173821 shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry_num_breakdown.py
--rw-r--r--   0        0        0      753 2024-03-01 04:58:50.177821 shroudstone-0.1.2/shroudstone/stormgateworld/models/profile_privacy.py
--rw-r--r--   0        0        0      731 2024-03-01 04:58:50.185821 shroudstone-0.1.2/shroudstone/stormgateworld/models/race.py
--rw-r--r--   0        0        0      769 2024-03-01 04:58:50.189821 shroudstone-0.1.2/shroudstone/stormgateworld/models/resolution.py
--rw-r--r--   0        0        0     3229 2024-03-01 04:58:50.193821 shroudstone-0.1.2/shroudstone/stormgateworld/models/servers_statistics.py
--rw-r--r--   0        0        0     2660 2024-03-01 04:58:50.197821 shroudstone-0.1.2/shroudstone/stormgateworld/models/servers_statistics_entry.py
--rw-r--r--   0        0        0     4183 2024-03-01 04:58:50.205821 shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time.py
--rw-r--r--   0        0        0     3457 2024-03-01 04:58:50.209821 shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_entry.py
--rw-r--r--   0        0        0     5499 2024-03-01 04:58:50.213822 shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_history_point.py
--rw-r--r--   0        0        0     3390 2024-03-01 04:58:50.217821 shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_match_length.py
--rw-r--r--   0        0        0     4227 2024-03-01 04:58:50.225822 shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_match_length_entry.py
--rw-r--r--   0        0        0        0 2024-02-29 02:04:14.863124 shroudstone-0.1.2/shroudstone/stormgateworld/py.typed
--rw-r--r--   0        0        0     9240 2024-03-01 04:58:50.229822 shroudstone-0.1.2/shroudstone/stormgateworld/rest.py
--rwxr-xr-x   0        0        0     2668 2024-03-06 11:27:47.970810 shroudstone-0.1.2/stormgate.proto
--rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 shroudstone-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1154 2024-05-14 01:34:18.440385 shroudstone-0.1.4/.github/workflows/build-exe.yml
+-rw-r--r--   0        0        0       45 2024-02-28 11:05:03.022804 shroudstone-0.1.4/.gitignore
+-rw-r--r--   0        0        0    32422 2024-02-25 06:24:42.992531 shroudstone-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7967 2024-05-14 01:34:18.440385 shroudstone-0.1.4/README.md
+-rw-r--r--   0        0        0      514 2024-05-14 02:08:42.269717 shroudstone-0.1.4/api-client-codegen.sh
+-rwxr-xr-x   0        0        0      297 2024-02-25 06:24:42.992531 shroudstone-0.1.4/codegen.sh
+-rw-r--r--   0        0        0    90765 2024-03-07 06:03:55.756412 shroudstone-0.1.4/docs/example-screenshot.png
+-rw-r--r--   0        0        0      185 2024-03-23 01:38:38.331578 shroudstone-0.1.4/pyinstaller_build.bat
+-rw-r--r--   0        0        0      873 2024-05-14 02:08:42.269717 shroudstone-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-14 01:34:18.440385 shroudstone-0.1.4/shroudstone/__init__.py
+-rw-r--r--   0        0        0      373 2024-05-13 08:26:21.715857 shroudstone-0.1.4/shroudstone/__main__.py
+-rw-r--r--   0        0        0     7858 2024-05-14 02:08:42.269717 shroudstone-0.1.4/shroudstone/cli.py
+-rw-r--r--   0        0        0     2626 2024-05-14 02:08:42.269717 shroudstone-0.1.4/shroudstone/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:03:55.756412 shroudstone-0.1.4/shroudstone/gui/__init__.py
+-rw-r--r--   0        0        0       43 2024-02-27 12:08:06.666709 shroudstone-0.1.4/shroudstone/gui/__main__.py
+-rw-r--r--   0        0        0    15780 2024-05-14 02:08:42.269717 shroudstone-0.1.4/shroudstone/gui/app.py
+-rw-r--r--   0        0        0    16958 2024-02-27 12:08:06.666709 shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.ico
+-rw-r--r--   0        0        0     2821 2024-02-27 12:08:06.666709 shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.png
+-rw-r--r--   0        0        0     6363 2024-02-27 12:08:06.666709 shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.svg
+-rw-r--r--   0        0        0      569 2024-05-13 08:26:21.739857 shroudstone-0.1.4/shroudstone/gui/fonts.py
+-rw-r--r--   0        0        0     2779 2024-03-07 04:57:52.650122 shroudstone-0.1.4/shroudstone/gui/jobs.py
+-rw-r--r--   0        0        0     3002 2024-03-23 01:38:38.331578 shroudstone-0.1.4/shroudstone/gui/logview.py
+-rw-r--r--   0        0        0      621 2024-05-13 08:26:21.743857 shroudstone-0.1.4/shroudstone/logging.py
+-rwxr-xr-x   0        0        0    21707 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/renamer.py
+-rwxr-xr-x   0        0        0    11462 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/replay.py
+-rw-r--r--   0        0        0      353 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/sgw_api.py
+-rw-r--r--   0        0        0     4463 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgate_pb2.py
+-rw-r--r--   0        0        0     5462 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgate_pb2.pyi
+-rw-r--r--   0        0        0     5374 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/__init__.py
+-rw-r--r--   0        0        0    12807 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/leaderboard_entries_api.py
+-rw-r--r--   0        0        0    22652 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/leaderboards_api.py
+-rw-r--r--   0        0        0    11844 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/matches_api.py
+-rw-r--r--   0        0        0    64249 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/players_api.py
+-rw-r--r--   0        0        0    43816 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api/statistics_api.py
+-rw-r--r--   0        0        0    25859 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/api_response.py
+-rw-r--r--   0        0        0    15400 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/configuration.py
+-rw-r--r--   0        0        0     5968 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/exceptions.py
+-rw-r--r--   0        0        0     4353 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/__init__.py
+-rw-r--r--   0        0        0     3091 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics.py
+-rw-r--r--   0        0        0     3379 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics_activity.py
+-rw-r--r--   0        0        0     3113 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics_entry.py
+-rw-r--r--   0        0        0      770 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/aggregation.py
+-rw-r--r--   0        0        0     3263 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/countries_statistics.py
+-rw-r--r--   0        0        0     3090 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/countries_statistics_entry.py
+-rw-r--r--   0        0        0      731 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/dump_format.py
+-rw-r--r--   0        0        0     2956 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/error_response.py
+-rw-r--r--   0        0        0      784 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard.py
+-rw-r--r--   0        0        0     3274 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_dump_response.py
+-rw-r--r--   0        0        0     3459 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_history.py
+-rw-r--r--   0        0        0     3172 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_history_row.py
+-rw-r--r--   0        0        0     6683 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_response.py
+-rw-r--r--   0        0        0      751 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_order.py
+-rw-r--r--   0        0        0     3340 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_response.py
+-rw-r--r--   0        0        0      843 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/league.py
+-rw-r--r--   0        0        0     4124 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_player_leaderboard_entry_response.py
+-rw-r--r--   0        0        0     3287 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_player_response.py
+-rw-r--r--   0        0        0     6065 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_response.py
+-rw-r--r--   0        0        0     4510 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_response.py
+-rw-r--r--   0        0        0      760 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_result.py
+-rw-r--r--   0        0        0      745 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/match_state.py
+-rw-r--r--   0        0        0     3279 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/matches_response.py
+-rw-r--r--   0        0        0     4373 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_activity_stats.py
+-rw-r--r--   0        0        0     3575 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_activity_stats_race.py
+-rw-r--r--   0        0        0     3303 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matches_response.py
+-rw-r--r--   0        0        0     3129 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats.py
+-rw-r--r--   0        0        0     4181 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats_entry.py
+-rw-r--r--   0        0        0     3643 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats_matchup.py
+-rw-r--r--   0        0        0     3297 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_opponents_stats.py
+-rw-r--r--   0        0        0     4240 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_opponents_stats_opponent.py
+-rw-r--r--   0        0        0     5174 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_response.py
+-rw-r--r--   0        0        0     4858 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry.py
+-rw-r--r--   0        0        0     4625 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry_aggregated.py
+-rw-r--r--   0        0        0     3704 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry_num_breakdown.py
+-rw-r--r--   0        0        0      753 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/profile_privacy.py
+-rw-r--r--   0        0        0      731 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/race.py
+-rw-r--r--   0        0        0      769 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/resolution.py
+-rw-r--r--   0        0        0     3229 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/servers_statistics.py
+-rw-r--r--   0        0        0     2660 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/servers_statistics_entry.py
+-rw-r--r--   0        0        0     4183 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time.py
+-rw-r--r--   0        0        0     3457 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_entry.py
+-rw-r--r--   0        0        0     5499 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_history_point.py
+-rw-r--r--   0        0        0     3390 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_match_length.py
+-rw-r--r--   0        0        0     4227 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_match_length_entry.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/py.typed
+-rw-r--r--   0        0        0     9240 2024-05-14 02:08:42.273717 shroudstone-0.1.4/shroudstone/stormgateworld/rest.py
+-rwxr-xr-x   0        0        0     2668 2024-05-14 02:08:42.273717 shroudstone-0.1.4/stormgate.proto
+-rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 shroudstone-0.1.4/PKG-INFO
```

### Comparing `shroudstone-0.1.2/.github/workflows/build-exe.yml` & `shroudstone-0.1.4/.github/workflows/build-exe.yml`

 * *Files 12% similar despite different names*

```diff
@@ -24,13 +24,20 @@
       run: pip install pyinstaller -e .
     - name: Sanity check
       run: shroudstone --help
     - name: Build shroudstone.exe
       run: ./pyinstaller_build.bat
     - name: Test .exe
       run: ./dist/shroudstone.exe --help
+    - name: Determine release type
+      shell: bash
+      id: check-tag
+      run: |
+        if [[ ${{ github.ref }} =~ [0-9](a|b|rc)[0-9]+$ ]]; then
+            echo "prerelease=true" >> $GITHUB_OUTPUT
+        fi
     - name: Create release
       uses: softprops/action-gh-release@v1
       if: startsWith(github.ref, 'refs/tags/v')
       with:
         files: dist/shroudstone.exe
-        prerelease: ${{ contains(github.ref, 'a') }} # flag alpha releases as pre-release
+        prerelease: ${{ steps.check-tag.outputs.prerelease == 'true' }}
```

### Comparing `shroudstone-0.1.2/LICENSE` & `shroudstone-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/README.md` & `shroudstone-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,24 @@
 accurate:
 
 - 1v1 match results are determined by who leaves the game first. In most ladder
   games this is the loser "gging out"; but if you e.g. win by destroying all
   your opponent's buildings and then leave the game before your opponent,
   Shroudstone will incorrectly mark your game as a loss.
 - Likewise, game durations are determined by the time at which the first player
-  leaves the game - this can also be incorrect in the case of a win by elimination.
+  leaves the game - this can also be incorrect in the case of a win by
+  elimination or in non-1v1 games.
 
 Previously, Shroudstone used data obtained from the Stormgate World API to fill
 these gaps (in the case of 1v1 ladder games). Unfortunately, Frost Giant are no
 longer providing access to this data to the community,  so this will no
 longer be possible going forward. See [Stormgate World's
 post](https://stormgateworld.com/api-restrictions/) on the matter for more
-information - I agree wholeheartedly with their disappointment. Thanks to the
-Stormgate World team (and contributors) for their great work.
+information. Thanks to the Stormgate World team (and contributors) for their
+great work, it was cool even if short-lived.
 
 ## Installation & Usage
 
 ### On Windows: .exe download
 
 Simply [download the latest standalone
 executable](https://github.com/acarapetis/shroudstone/releases/latest/download/shroudstone.exe)
@@ -160,7 +161,32 @@
 * `build_number` (int): Build number of Stormgate version on which the game was played (extracted from replay file)
 
 
 ## Contributing
 
 Contributions are welcome - feel free to open a PR, or message Pox on the
 Stormgate Discord if you want to discuss with me first.
+
+### Developing
+
+Assuming you have python 3.8+ and pip installed on your system, all you need to
+do to start working on shroudstone is to clone the repository and install the
+python package in *development mode*. [See
+here](https://setuptools.pypa.io/en/latest/userguide/development_mode.html) for
+more information, or follow this recipe to get started using a virtual
+environment:
+
+Create a working directory:
+```
+mkdir shroudstone-workspace
+cd shroudstone-workspace
+```
+Download the code and setup a python virtual environment:
+```
+python -m venv .venv
+git clone https://github.com/acarapetis/shroudstone.git
+```
+Finally, install and run the code:
+```
+.venv/bin/pip3 install -e shroudstone/
+.venv/bin/shroudstone
+```
```

### Comparing `shroudstone-0.1.2/api-client-codegen.sh` & `shroudstone-0.1.4/api-client-codegen.sh`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/docs/example-screenshot.png` & `shroudstone-0.1.4/docs/example-screenshot.png`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/pyproject.toml` & `shroudstone-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/cli.py` & `shroudstone-0.1.4/shroudstone/cli.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/config.py` & `shroudstone-0.1.4/shroudstone/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             with config_file.open("rt", encoding="utf-8") as f:
                 content = yaml.load(f, Loader=yaml.SafeLoader)
                 # Migrate old configs:
                 if "replay_name_format" in content:
                     content["replay_name_format_1v1"] = content["replay_name_format"]
                 return Config.model_validate(content)
         else:
-            return Config()
+            config = Config()
+            config.save()
+            return config
 
     def save(self):
         with config_file.open("wt", encoding="utf-8") as f:
             yaml.dump(self.model_dump(mode="json"), f, width=float("inf"))
 
     model_config = ConfigDict(extra="ignore")
```

### Comparing `shroudstone-0.1.2/shroudstone/gui/app.py` & `shroudstone-0.1.4/shroudstone/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from pystray import Icon, Menu, MenuItem
 from pystray._base import Icon as BaseIcon
 from PIL import Image
 import tkinter as tk
 from tkinter import ttk
 from tkinter.filedialog import askdirectory
 from tkinter.messagebox import showinfo, showwarning, askyesno
-from tkinter.font import Font, families, nametofont
 
-from shroudstone import config, renamer
+from shroudstone import config, renamer, __version__
 from shroudstone.gui.fonts import setup_style
 from shroudstone.gui.logview import LogView
 from shroudstone.logging import configure_logging
 from .jobs import TkWithJobs
 
 import logging
 
@@ -127,48 +126,55 @@
 
         logger.debug(f"icon.run() in thread {get_ident()}")
         icon.run()
         logger.debug("icon.run done")
         self.tray_quit_event.set()
 
 
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.vars = AppState()
         self.protocol("WM_DELETE_WINDOW", self.on_window_close)
         logger.debug(f"Main thread is {get_ident()}")
 
+        self.after(0, self.custom_startup)
+
+    def custom_startup(self):
+        """This method performs custom startup actions *after* the mainloop has started."""
+
         # The systray icon passes this message back from its thread when it's done:
         self.tray_quit_event = Event()
         def _check_quit_event():
             if self.tray_quit_event.is_set():
                 self.quit_app()
             self.after(10, _check_quit_event)
         _check_quit_event()
 
         self.setup_tray_icon()
 
 
+
+# TODO: Move the following methods inside our custom App class?
+# We currently have some root.after calls in here, and some in our
+# custom_startup method, so it's a bit of a mess. Definitely some kind of
+# tidyup needs to be done.
 def run():
     configure_logging()
     renamer.migrate()
     logger.info(
         "Keep this console open - it will show progress information during renaming."
     )
     cfg: config.Config = config.Config.load()
 
     root = App(className="Shroudstone")
     setup_style(root)
     setup_window_icon(root)
 
     if cfg.replay_dir is None:
-        configure_replay_dir(root, root.vars, cfg)
-        cfg.replay_dir = Path(root.vars.replay_dir.get())
-        cfg.save()
+        root.after(0, lambda: configure_replay_dir(root, root.vars, cfg))
 
     create_main_ui(root, cfg)
     root.mainloop()
 
 
 def setup_window_icon(root: tk.Tk):
     if platform.system() == "Windows":
@@ -193,14 +199,15 @@
     else:
         state.replay_dir.set(str(cfg.replay_dir))
         showinfo(
             title="Stormgate Replay Directory",
             message=f"Detected your replay directory as {cfg.replay_dir}."
             " If this is incorrect, please configure it manually on the next screen.",
         )
+    cfg.save()
     root.deiconify()
 
 
 def rename_replays_wrapper(*args, **kwargs):
     try:
         return renamer.rename_replays(*args, **kwargs)
     except Exception:
@@ -220,15 +227,15 @@
         state.replay_name_format_generic.set(cfg.replay_name_format_generic)
         state.minimize_to_tray.set(cfg.minimize_to_tray)
         state.show_log_on_autorename.set(cfg.show_log_on_autorename)
 
     def save_config():
         cfg.save()
 
-    root.title("Shroudstone - Stormgate Replay Renamer")
+    root.title(f"Shroudstone v{__version__} - Stormgate Replay Renamer")
 
     config_frame = ttk.LabelFrame(root, text="Configuration")
     config_frame.pack(fill="x", padx=5, pady=5)
 
     form = ttk.Frame(config_frame)
     form.pack(fill="x")
```

### Comparing `shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.ico` & `shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.ico`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.png` & `shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.png`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/gui/assets/shroudstone.svg` & `shroudstone-0.1.4/shroudstone/gui/assets/shroudstone.svg`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/gui/fonts.py` & `shroudstone-0.1.4/shroudstone/gui/fonts.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/gui/jobs.py` & `shroudstone-0.1.4/shroudstone/gui/jobs.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/gui/logview.py` & `shroudstone-0.1.4/shroudstone/gui/logview.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/logging.py` & `shroudstone-0.1.4/shroudstone/logging.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/renamer.py` & `shroudstone-0.1.4/shroudstone/renamer.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/replay.py` & `shroudstone-0.1.4/shroudstone/replay.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgate_pb2.py` & `shroudstone-0.1.4/shroudstone/stormgate_pb2.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgate_pb2.pyi` & `shroudstone-0.1.4/shroudstone/stormgate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/__init__.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/__init__.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api/leaderboard_entries_api.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api/leaderboard_entries_api.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api/leaderboards_api.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api/leaderboards_api.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api/matches_api.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api/matches_api.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api/players_api.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api/players_api.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api/statistics_api.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api/statistics_api.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api_client.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api_client.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/api_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/api_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/configuration.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/configuration.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/exceptions.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/exceptions.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/__init__.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics_activity.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics_activity.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/activity_statistics_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/activity_statistics_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/aggregation.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/countries_statistics.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/countries_statistics.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/countries_statistics_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/countries_statistics_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/dump_format.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/dump_format.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/error_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/error_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_dump_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_dump_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_history.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_history.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_history_row.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_history_row.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_entry_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_entry_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_order.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_order.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/leaderboard_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/leaderboard_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/league.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/league.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_player_leaderboard_entry_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_player_leaderboard_entry_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_player_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_player_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_participant_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_participant_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_result.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_result.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/match_state.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/match_state.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/matches_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/matches_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_activity_stats.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_activity_stats.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_activity_stats_race.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_activity_stats_race.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matches_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matches_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_matchups_stats_matchup.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_matchups_stats_matchup.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_opponents_stats.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_opponents_stats.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_opponents_stats_opponent.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_opponents_stats_opponent.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_response.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_response.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry_aggregated.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry_aggregated.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/player_stats_entry_num_breakdown.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/player_stats_entry_num_breakdown.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/profile_privacy.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/profile_privacy.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/race.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/race.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/resolution.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/resolution.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/servers_statistics.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/servers_statistics.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/servers_statistics_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/servers_statistics_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_history_point.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_history_point.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_match_length.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_match_length.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/models/stats_by_time_match_length_entry.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/models/stats_by_time_match_length_entry.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/shroudstone/stormgateworld/rest.py` & `shroudstone-0.1.4/shroudstone/stormgateworld/rest.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/stormgate.proto` & `shroudstone-0.1.4/stormgate.proto`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.2/PKG-INFO` & `shroudstone-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroudstone
-Version: 0.1.2
+Version: 0.1.4
 Summary: Python utilities for working with Stormgate replays
 Keywords: Stormgate
 Author-email: Anthony Carapetis <anthony.carapetis@gmail.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
@@ -47,23 +47,24 @@
 accurate:
 
 - 1v1 match results are determined by who leaves the game first. In most ladder
   games this is the loser "gging out"; but if you e.g. win by destroying all
   your opponent's buildings and then leave the game before your opponent,
   Shroudstone will incorrectly mark your game as a loss.
 - Likewise, game durations are determined by the time at which the first player
-  leaves the game - this can also be incorrect in the case of a win by elimination.
+  leaves the game - this can also be incorrect in the case of a win by
+  elimination or in non-1v1 games.
 
 Previously, Shroudstone used data obtained from the Stormgate World API to fill
 these gaps (in the case of 1v1 ladder games). Unfortunately, Frost Giant are no
 longer providing access to this data to the community,  so this will no
 longer be possible going forward. See [Stormgate World's
 post](https://stormgateworld.com/api-restrictions/) on the matter for more
-information - I agree wholeheartedly with their disappointment. Thanks to the
-Stormgate World team (and contributors) for their great work.
+information. Thanks to the Stormgate World team (and contributors) for their
+great work, it was cool even if short-lived.
 
 ## Installation & Usage
 
 ### On Windows: .exe download
 
 Simply [download the latest standalone
 executable](https://github.com/acarapetis/shroudstone/releases/latest/download/shroudstone.exe)
@@ -183,7 +184,32 @@
 
 
 ## Contributing
 
 Contributions are welcome - feel free to open a PR, or message Pox on the
 Stormgate Discord if you want to discuss with me first.
 
+### Developing
+
+Assuming you have python 3.8+ and pip installed on your system, all you need to
+do to start working on shroudstone is to clone the repository and install the
+python package in *development mode*. [See
+here](https://setuptools.pypa.io/en/latest/userguide/development_mode.html) for
+more information, or follow this recipe to get started using a virtual
+environment:
+
+Create a working directory:
+```
+mkdir shroudstone-workspace
+cd shroudstone-workspace
+```
+Download the code and setup a python virtual environment:
+```
+python -m venv .venv
+git clone https://github.com/acarapetis/shroudstone.git
+```
+Finally, install and run the code:
+```
+.venv/bin/pip3 install -e shroudstone/
+.venv/bin/shroudstone
+```
+
```


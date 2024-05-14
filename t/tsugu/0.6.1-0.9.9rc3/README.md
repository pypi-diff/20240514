# Comparing `tmp/tsugu-0.6.1.tar.gz` & `tmp/tsugu-0.9.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.6.1.tar", last modified: Sun May 12 11:45:39 2024, max compression
+gzip compressed data, was "tsugu-0.9.9rc3.tar", last modified: Tue May 14 07:25:01 2024, max compression
```

## Comparing `tsugu-0.6.1.tar` & `tsugu-0.9.9rc3.tar`

### file list

```diff
@@ -1,29 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.765472 tsugu-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 11:45:31.000000 tsugu-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-12 11:45:39.765472 tsugu-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-12 11:45:31.000000 tsugu-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:45:39.765472 tsugu-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-12 11:45:31.000000 tsugu-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-12 11:45:31.000000 tsugu-0.6.1/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/tsugu/local/
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/tsugu/local/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/local/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/tsugu/remote/
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.765472 tsugu-0.6.1/tsugu/remote/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/remote/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.765472 tsugu-0.6.1/tsugu/universal_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-12 11:45:31.000000 tsugu-0.6.1/tsugu/universal_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:45:39.761472 tsugu-0.6.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-12 11:45:39.000000 tsugu-0.6.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-12 11:45:39.000000 tsugu-0.6.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:45:39.000000 tsugu-0.6.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-12 11:45:39.000000 tsugu-0.6.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 11:45:39.000000 tsugu-0.6.1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.406106 tsugu-0.9.9rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 07:25:01.406106 tsugu-0.9.9rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:25:01.406106 tsugu-0.9.9rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu/local/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/local/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.398106 tsugu-0.9.9rc3/tsugu/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.398106 tsugu-0.9.9rc3/tsugu/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.398106 tsugu-0.9.9rc3/tsugu/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.398106 tsugu-0.9.9rc3/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.394106 tsugu-0.9.9rc3/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 07:25:01.000000 tsugu-0.9.9rc3/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-14 07:25:01.000000 tsugu-0.9.9rc3/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:25:01.000000 tsugu-0.9.9rc3/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 07:25:01.000000 tsugu-0.9.9rc3/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 07:25:01.000000 tsugu-0.9.9rc3/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.402106 tsugu-0.9.9rc3/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.402106 tsugu-0.9.9rc3/tsugu_async/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.402106 tsugu-0.9.9rc3/tsugu_async/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.402106 tsugu-0.9.9rc3/tsugu_async/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.402106 tsugu-0.9.9rc3/tsugu_async/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.406106 tsugu-0.9.9rc3/tsugu_async/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:25:01.406106 tsugu-0.9.9rc3/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 07:24:50.000000 tsugu-0.9.9rc3/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-0.6.1/LICENSE` & `tsugu-0.9.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.6.1/setup.py` & `tsugu-0.9.9rc3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.6.1',
+    version='0.9.9-rc3',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
+    url='https://github.com/kumoSleeping/tsugu-bot-py',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
-            "urllib3",
             "loguru",
+            "tsugu-api-python"
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-0.6.1/tsugu/config.py` & `tsugu-0.9.9rc3/tsugu/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,90 +2,63 @@
 import os
 
 from loguru import logger
 
 
 class Config:
     def __init__(self):
-        self._user_database_path = None
-        # 设置默认值
+        self.prefix = ['/', '']
+        self.allow_gap_less = True
         self.backend = "http://tsugubot.com:8080"
         self.user_data_backend = "http://tsugubot.com:8080"
+        self.car_room_backend = "http://tsugubot.com:8080"
+        self.get_remote_user_data_max_retry = 3
         self.backend_use_proxy = False
         self.user_data_backend_use_proxy = False
         self.submit_car_number_use_proxy = False
         self.verify_player_bind_use_proxy = False
         self.proxy_url = "http://localhost:7890"
         self.token_name = "Tsugu"
         self.bandori_station_token = "ZtV4EX2K9Onb"
-
         self.use_easy_bg = True
         self.compress = True
-
         self.ban_gacha_simulate_group_data = []
-
-        self._server_list = {0: "日服", 1: "国际服", 2: "台服", 3: "国服", 4: "韩服"}
-        self._server_name_to_index = {
-            "日服": "0",
-            "国际服": "1",
-            "台服": "2",
-            "国服": "3",
-            "韩服": "4",
-            "jp": "0",
-            "en": "1",
-            "tw": "2",
-            "cn": "3",
-            "kr": "4",
-        }
-
-        self._server_index_to_name = {
-            "0": "日服",
-            "1": "国际服",
-            "2": "台服",
-            "3": "国服",
-            "4": "韩服",
-        }
-
-        self._server_index_to_s_name = {
-            "0": "jp",
-            "1": "en",
-            "2": "tw",
-            "3": "cn",
-            "4": "kr",
-        }
-
-        self.features = {
-                "car_number_forwarding": True,
-                "change_main_server": True,
-                "switch_car_forwarding": True,
-                "bind_player": True,
-                "change_server_list": True,
-                "player_status": True,
-                "help": True,
-            }
-
         self.commands = [
-            {"api": "cardIllustration", "command_name": ["查插画", "查卡面"]},
-            {"api": "player", "command_name": ["查玩家", "查询玩家"]},
-            {"api": "gachaSimulate", "command_name": ["抽卡模拟", "卡池模拟"]},
-            {"api": "gacha", "command_name": ["查卡池"]},
-            {"api": "event", "command_name": ["查活动"]},
-            {"api": "song", "command_name": ["查歌曲", "查曲"]},
-            {"api": "songMeta", "command_name": ["查询分数表", "查分数表"]},
-            {"api": "character", "command_name": ["查角色"]},
-            {"api": "chart", "command_name": ["查铺面", "查谱面"]},
-            {"api": "ycxAll", "command_name": ["ycxall", "ycx all"]},
+            {"api": "get_card_illustration", "command_name": ["查插画", "查卡面"]},
+            {"api": "search_player", "command_name": ["查玩家", "查询玩家"]},
+            {"api": "gacha_simulate", "command_name": ["抽卡模拟", "卡池模拟"]},
+            {"api": "search_gacha", "command_name": ["查卡池"]},
+            {"api": "search_event", "command_name": ["查活动"]},
+            {"api": "search_song", "command_name": ["查歌曲", "查曲"]},
+            {"api": "song_meta", "command_name": ["查询分数表", "查分数表"]},
+            {"api": "search_character", "command_name": ["查角色"]},
+            {"api": "song_chart", "command_name": ["查铺面", "查谱面"]},
+            {"api": "ycx_all", "command_name": ["ycxall", "ycx all"]},
             {"api": "ycx", "command_name": ["ycx", "预测线"]},
             {"api": "lsycx", "command_name": ["lsycx"]},
-            {"api": "ycm", "command_name": ["ycm", "车来"]},
-            {"api": "card", "command_name": ["查卡"]},
-            {"api": "eventStage", "command_name": ["查试炼"]},
+            {"api": "room_list", "command_name": ["ycm", "车来"]},
+            {"api": "search_card", "command_name": ["查卡"]},
+            {"api": "event_stage", "command_name": ["查试炼"]},
+        ]
+        self.user_commands = [
+            {"api": "player_status", "command_name": ["玩家状态"]},
+            {"api": "switch_car_forwarding_off", "command_name": ['关闭车牌转发', '关闭个人车牌转发']},
+            {"api": "switch_car_forwarding_on", "command_name": ['开启车牌转发', '开启个人车牌转发']},
+            {"api": "bind_player", "command_name": ["绑定玩家"]},
+            {"api": "unbind_player", "command_name": ["解除绑定"]},
+            {"api": "change_server_mode", "command_name": ["主服务器"]},
+            {"api": "change_default_server", "command_name": ["设置默认服务器"]},
+            {"api": "bind_player_verification_off", "command_name": ["验证解绑"]},
+            {"api": "bind_player_verification_on", "command_name": ["验证绑定"]},
         ]
 
-        self.car_config = {
+        self._user_database_path = None
+        self._i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
+        self._s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
+        self._car_config = {
             "car": [
                 "q1",
                 "q2",
                 "q3",
                 "q4",
                 "Q1",
                 "Q2",
@@ -146,145 +119,145 @@
                 "疯狂星期四",
                 "离开了我们",
                 "日元",
                 "av",
                 "bv",
             ],
         }
-        self.help_doc_dict = {
+        self._help_doc_dict = {
             "玩家状态": """
-查询指定玩家的状态信息。
-使用示例：
-    玩家状态 : 查询你当前默认服务器的玩家状态
-    玩家状态  jp : 查询日服玩家状态
-    玩家状态 2 : 查询您的第二个绑定玩家的状态(*此功能需要BOT支持)
-        
-""",
+        查询指定玩家的状态信息。
+        使用示例：
+            玩家状态 : 查询你当前默认服务器的玩家状态
+            玩家状态  jp : 查询日服玩家状态
+            玩家状态 2 : 查询您的第二个绑定玩家的状态(*此功能需要BOT支持)
+
+        """,
             "开关车牌转发": """
-开启或关闭车牌转发功能，针对个人
-使用示例：
-    开启车牌转发 : 开启车牌转发功能
-    关闭车牌转发 : 关闭车牌转发功能
-""",
+        开启或关闭车牌转发功能，针对个人
+        使用示例：
+            开启车牌转发 : 开启车牌转发功能
+            关闭车牌转发 : 关闭车牌转发功能
+        """,
             "绑定玩家": """
-绑定玩家ID到当前账号
-使用示例：
-    绑定玩家 : 绑定玩家开始绑定玩家流程(*请根据BOT的提示进行操作)
-""",
+        绑定玩家ID到当前账号
+        使用示例：
+            绑定玩家 : 绑定玩家开始绑定玩家流程(*请根据BOT的提示进行操作)
+        """,
             "解除绑定": """
-解除绑定玩家ID
-使用示例：
-    解除绑定 : 解除绑定玩家开始解绑玩家流程(*请根据BOT的提示进行操作)
-""",
+        解除绑定玩家ID
+        使用示例：
+            解除绑定 : 解除绑定玩家开始解绑玩家流程(*请根据BOT的提示进行操作)
+        """,
             "切换主服务器": """
-切换主服务器
-使用示例：
-    主服务器 jp : 切换主服务器到日服
-    国服模式 : 切换主服务器到国服
-""",
+        切换主服务器
+        使用示例：
+            主服务器 jp : 切换主服务器到日服
+            国服模式 : 切换主服务器到国服
+        """,
             "设置默认服务器": """
-可以改变查询时的资源优先顺序
-设置默认服务器，使用空格分隔服务器列表
-使用示例：
-    设置默认服务器 国服 日服 : 将国服设置为第一服务器，日服设置为第二服务器
-""",
+        可以改变查询时的资源优先顺序
+        设置默认服务器，使用空格分隔服务器列表
+        使用示例：
+            设置默认服务器 国服 日服 : 将国服设置为第一服务器，日服设置为第二服务器
+        """,
             "查卡面": """
-根据卡片ID查询卡片插画
-使用示例：
-    查卡面 1399 :返回1399号卡牌的插画
-""",
+        根据卡片ID查询卡片插画
+        使用示例：
+            查卡面 1399 :返回1399号卡牌的插画
+        """,
             "查询玩家": """
-查询指定ID玩家的信息。省略服务器名时，默认从你当前的主服务器查询
-使用示例：
-    查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息
-    查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息
-""",
+        查询指定ID玩家的信息。省略服务器名时，默认从你当前的主服务器查询
+        使用示例：
+            查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息
+            查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息
+        """,
             "卡池模拟": """
-模拟抽卡，如果没有卡池ID的话，卡池为当前活动的卡池
-使用示例：
-    抽卡模拟:模拟抽卡10次
-    抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池
-""",
+        模拟抽卡，如果没有卡池ID的话，卡池为当前活动的卡池
+        使用示例：
+            抽卡模拟:模拟抽卡10次
+            抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池
+        """,
             "查卡池": """
-根据卡池ID查询卡池信息
-""",
+        根据卡池ID查询卡池信息
+        """,
             "查活动": """
-根据关键词或活动ID查询活动信息
-使用示例：
-    查活动 177 :返回177号活动的信息
-    查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
-    查活动 >255 :返回所有活动ID大于255的活动列表
-    查活动 255-256 :返回所有活动ID在255到256之间的活动列表
-    查活动 ppp :匹配到 PPP 乐队的活动信息
-""",
+        根据关键词或活动ID查询活动信息
+        使用示例：
+            查活动 177 :返回177号活动的信息
+            查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
+            查活动 >255 :返回所有活动ID大于255的活动列表
+            查活动 255-256 :返回所有活动ID在255到256之间的活动列表
+            查活动 ppp :匹配到 PPP 乐队的活动信息
+        """,
             "查曲": """
-根据关键词或曲目ID查询曲目信息
-使用示例：
-    查曲 1 :返回1号曲的信息
-    查曲 ag lv27 :返回所有难度为27的ag曲列表
-    查曲 1 ex :返回1号曲的expert难度曲目信息
-    查曲 滑滑蛋 :匹配到 ふわふわ時間 的曲目信息
-""",
+        根据关键词或曲目ID查询曲目信息
+        使用示例：
+            查曲 1 :返回1号曲的信息
+            查曲 ag lv27 :返回所有难度为27的ag曲列表
+            查曲 1 ex :返回1号曲的expert难度曲目信息
+            查曲 滑滑蛋 :匹配到 ふわふわ時間 的曲目信息
+        """,
             "查分数表": """
-查询指定服务器的歌曲分数表，如果没有服务器名的话，服务器为用户的默认服务器
-""",
+        查询指定服务器的歌曲分数表，如果没有服务器名的话，服务器为用户的默认服务器
+        """,
             "查角色": """
-根据关键词或角色ID查询角色信息
-使用示例：
-    查角色 10 :返回10号角色的信息
-    查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表
-""",
+        根据关键词或角色ID查询角色信息
+        使用示例：
+            查角色 10 :返回10号角色的信息
+            查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表
+        """,
             "查谱面": """
-根据曲目ID与难度查询铺面信息
-使用示例：
-    查谱面 1 :返回1号曲的所有铺面
-    查谱面 1 expert :返回1号曲的expert难度铺面
-""",
+        根据曲目ID与难度查询铺面信息
+        使用示例：
+            查谱面 1 :返回1号曲的所有铺面
+            查谱面 1 expert :返回1号曲的expert难度铺面
+        """,
             "ycxall": """
-查询所有档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
-可用档线:
-20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
-
-使用示例：
-    ycxall :返回默认服务器当前活动所有档位的档线与预测线
-    ycxall 177 jp:返回日服177号活动所有档位的档线与预测线
-""",
+        查询所有档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
+        可用档线:
+        20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
+
+        使用示例：
+            ycxall :返回默认服务器当前活动所有档位的档线与预测线
+            ycxall 177 jp:返回日服177号活动所有档位的档线与预测线
+        """,
             "ycx": """
-查询指定档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
-可用档线:
-20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
-使用示例：
-    ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线
-    ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线
-""",
+        查询指定档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
+        可用档线:
+        20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
+        使用示例：
+            ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线
+            ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线
+        """,
             "lsycx": """
-与ycx的区别是，lsycx会返回与最近的4期活动类型相同的活动的档线数据
-查询指定档位的预测线，与最近的4期活动类型相同的活动的档线数据，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
-可用档线:
-20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
-
-使用示例：
-    lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据
-    lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据
-""",
+        与ycx的区别是，lsycx会返回与最近的4期活动类型相同的活动的档线数据
+        查询指定档位的预测线，与最近的4期活动类型相同的活动的档线数据，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动
+        可用档线:
+        20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 
+
+        使用示例：
+            lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据
+            lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据
+        """,
             "ycm": """
-获取所有车牌车牌
-使用示例：
-    ycm : 获取所有车牌
-""",
+        获取所有车牌车牌
+        使用示例：
+            ycm : 获取所有车牌
+        """,
             "查卡": """
-根据关键词或卡牌ID查询卡片信息，请使用空格隔开所有参数
-使用示例：
-    查卡 1399 :返回1399号卡牌的信息
-    查卡 绿 tsugu :返回所有属性为pure的羽泽鸫的卡牌列表
-    查卡 kfes ars :返回所有为kfes的ars的卡牌列表
-""",
+        根据关键词或卡牌ID查询卡片信息，请使用空格隔开所有参数
+        使用示例：
+            查卡 1399 :返回1399号卡牌的信息
+            查卡 绿 tsugu :返回所有属性为pure的羽泽鸫的卡牌列表
+            查卡 kfes ars :返回所有为kfes的ars的卡牌列表
+        """,
             "查试炼": """
-查询当前服务器当前活动试炼信息\n可以自定义活动ID\n参数:-m 显示歌曲meta(相对效率)
-"""
+        查询当前服务器当前活动试炼信息\n可以自定义活动ID\n参数:-m 显示歌曲meta(相对效率)
+        """
         }
 
     def show_docs(self):
         logger.warning('此方法已经废弃')
         return None
 
     def output_config_json(self, path="./config.json"):
@@ -303,15 +276,15 @@
         '''
         通过配置文件重载配置
         配置文件不存在时自动生成默认配置文件
         :param path:
         :return:
         '''
         if not os.path.exists(path):
-            self.output_config_json(path="./config.json")
+            self.output_config_json(path=path)
             logger.error("配置文件不存在，已经生成默认配置文件")
 
         """Reloads configuration data from a JSON string or a JSON file path."""
         with open(path, "r", encoding="utf-8") as file:
             config_data = json.load(file)
         # Iterate over all keys in the input JSON and update the config attributes
         for key, value in config_data.items():
```

### Comparing `tsugu-0.6.1/tsugu/handler.py` & `tsugu-0.9.9rc3/tsugu_async/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,52 @@
 import base64
 from typing import List, Union, Dict
 
-from .universal_utils import *
-from .universal_utils import text_response
+from .utils import *
 from . import remote
-from . import local
-from .universal_utils import config
+from loguru import logger
 
 
-def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
+async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Union[bytes, str]]
     '''
-    data = handler_old(message, user_id, platform, channel_id)
+    data = await handler_raw(message, user_id, platform, channel_id)
     response = []
     if not data:
         return response
     for item in data:
-        if item['type'] == 'string':
-            response.append(item['string'])
-        elif item['type'] == 'base64':
-            bytes_data = base64.b64decode(item['string'].encode('utf-8'))
-            response.append(bytes_data)
+        response.append(item['string']) if item['type'] == 'string' else None
+        response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
     return response
 
 
-def handler_old(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
+async def handler_raw(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
     '''
-    old 除了返回的数据类型不同外，其他与 handler 函数一致
+    handler_raw 除了返回的数据类型不同外，其他与 handler 函数一致
     返回格式为 Tsugu 标准数据格式
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
-        def tsugu_handler(message: str, user_id: str, platform: str, channel_id: str):
-            message = message.strip()
-            # help
-            if config.features.get('help', True):
-                if message.startswith('帮助'):
-                    return help_command()
-                if message.startswith('help'):
-                    arg_text = message[4:].strip()
-                    return help_command(arg_text)
-                if message.endswith('-h'):
-                    arg_text = message[:-2].strip()
-                    return help_command(arg_text)
-            # 如果启用了本地数据库
-            if config._user_database_path:
-                return local.handler(message, user_id, platform, channel_id)
-            # 否则使用远程服务器
-            else:
-                return remote.handler(message, user_id, platform, channel_id)
-        data = tsugu_handler(message, user_id, platform, channel_id)
-        if not data:
+        # 使用远程服务器
+        res = await remote.handler(message, user_id, platform, channel_id)
+        if not res:
             return []
-        return data
+        return res
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
```


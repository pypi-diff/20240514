# Comparing `tmp/tsugu-0.9.9rc4.tar.gz` & `tmp/tsugu-0.9.9rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.9.9rc4.tar", last modified: Tue May 14 08:15:21 2024, max compression
+gzip compressed data, was "tsugu-0.9.9rc5.tar", last modified: Tue May 14 08:24:19 2024, max compression
```

## Comparing `tsugu-0.9.9rc4.tar` & `tsugu-0.9.9rc5.tar`

### file list

```diff
@@ -1,111 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.080087 tsugu-0.9.9rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 08:15:21.080087 tsugu-0.9.9rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:15:21.080087 tsugu-0.9.9rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.064087 tsugu-0.9.9rc4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.064087 tsugu-0.9.9rc4/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu/local/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/local/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu/universal/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.068086 tsugu-0.9.9rc4/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 08:15:20.000000 tsugu-0.9.9rc4/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-14 08:15:21.000000 tsugu-0.9.9rc4/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:15:20.000000 tsugu-0.9.9rc4/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 08:15:20.000000 tsugu-0.9.9rc4/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 08:15:20.000000 tsugu-0.9.9rc4/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.072087 tsugu-0.9.9rc4/tsugu_async/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.076087 tsugu-0.9.9rc4/tsugu_async/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.076087 tsugu-0.9.9rc4/tsugu_async/universal/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.076087 tsugu-0.9.9rc4/tsugu_async/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:15:21.076087 tsugu-0.9.9rc4/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:15:09.000000 tsugu-0.9.9rc4/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.072975 tsugu-0.9.9rc5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.072975 tsugu-0.9.9rc5/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.072975 tsugu-0.9.9rc5/tsugu/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.072975 tsugu-0.9.9rc5/tsugu/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/local/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/local/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/storage/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/storage/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/storage/remote_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/storage/remote_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.076975 tsugu-0.9.9rc5/tsugu/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.072975 tsugu-0.9.9rc5/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-14 08:24:18.000000 tsugu-0.9.9rc5/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-14 08:24:18.000000 tsugu-0.9.9rc5/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:24:18.000000 tsugu-0.9.9rc5/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 08:24:18.000000 tsugu-0.9.9rc5/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 08:24:18.000000 tsugu-0.9.9rc5/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu_async/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu_async/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.080975 tsugu-0.9.9rc5/tsugu_async/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/tsugu_async/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/tsugu_async/storage/remote_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/storage/remote_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/tsugu_async/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/tsugu_async/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:19.084975 tsugu-0.9.9rc5/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:24:06.000000 tsugu-0.9.9rc5/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-0.9.9rc4/LICENSE` & `tsugu-0.9.9rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/PKG-INFO` & `tsugu-0.9.9rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.9.9rc4
+Version: 0.9.9rc5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bot-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Bot Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc4 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc5 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/tsugu-bot-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ TTssuugguu BBoott PPyy[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 *** - `tsugu` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [x] æ¬å°æ°æ®åº -
 [x] è¿ç¨æ°æ®åº - `tsugu.async` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ -
 [x] è¿ç¨æ°æ®åº - [ ] æ¬å°æ°æ®åº ```shell pip install tsugu ``` >
```

### Comparing `tsugu-0.9.9rc4/README.md` & `tsugu-0.9.9rc5/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/setup.py` & `tsugu-0.9.9rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.9.9-rc4',
+    version='0.9.9-rc5',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bot-py',
```

### Comparing `tsugu-0.9.9rc4/test/test_async.py` & `tsugu-0.9.9rc5/test/test_async.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/command_matcher/__init__.py` & `tsugu-0.9.9rc5/tsugu/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/config.py` & `tsugu-0.9.9rc5/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/handler.py` & `tsugu-0.9.9rc5/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/__init__.py` & `tsugu-0.9.9rc5/tsugu/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/bind_player.py` & `tsugu-0.9.9rc5/tsugu/local/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/bind_player_verification_on.py` & `tsugu-0.9.9rc5/tsugu/local/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/change_default_server.py` & `tsugu-0.9.9rc5/tsugu/local/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/change_server_mode.py` & `tsugu-0.9.9rc5/tsugu/local/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/player_status.py` & `tsugu-0.9.9rc5/tsugu/local/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/local/router/unbind_player.py` & `tsugu-0.9.9rc5/tsugu/local/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/__init__.py` & `tsugu-0.9.9rc5/tsugu/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/bind_player.py` & `tsugu-0.9.9rc5/tsugu/remote/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/bind_player_verification_off.py` & `tsugu-0.9.9rc5/tsugu/remote/router/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/bind_player_verification_on.py` & `tsugu-0.9.9rc5/tsugu/remote/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/change_default_server.py` & `tsugu-0.9.9rc5/tsugu/remote/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/change_server_mode.py` & `tsugu-0.9.9rc5/tsugu/remote/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/player_status.py` & `tsugu-0.9.9rc5/tsugu/remote/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/remote/router/unbind_player.py` & `tsugu-0.9.9rc5/tsugu/remote/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/__init__.py` & `tsugu-0.9.9rc5/tsugu/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/help.py` & `tsugu-0.9.9rc5/tsugu/universal/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/rooms_forward.py` & `tsugu-0.9.9rc5/tsugu/universal/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/__init__.py` & `tsugu-0.9.9rc5/tsugu/universal/router/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/event_stage.py` & `tsugu-0.9.9rc5/tsugu/universal/router/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/gacha_simulate.py` & `tsugu-0.9.9rc5/tsugu/universal/router/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/lsycx.py` & `tsugu-0.9.9rc5/tsugu/universal/router/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/search_player.py` & `tsugu-0.9.9rc5/tsugu/universal/router/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/song_chart.py` & `tsugu-0.9.9rc5/tsugu/universal/router/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/ycx.py` & `tsugu-0.9.9rc5/tsugu/universal/router/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/universal/router/ycx_all.py` & `tsugu-0.9.9rc5/tsugu/universal/router/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu/utils/__init__.py` & `tsugu-0.9.9rc5/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu.egg-info/PKG-INFO` & `tsugu-0.9.9rc5/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.9.9rc4
+Version: 0.9.9rc5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bot-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Bot Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc4 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc5 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/tsugu-bot-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ TTssuugguu BBoott PPyy[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 *** - `tsugu` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [x] æ¬å°æ°æ®åº -
 [x] è¿ç¨æ°æ®åº - `tsugu.async` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ -
 [x] è¿ç¨æ°æ®åº - [ ] æ¬å°æ°æ®åº ```shell pip install tsugu ``` >
```

### Comparing `tsugu-0.9.9rc4/tsugu.egg-info/SOURCES.txt` & `tsugu-0.9.9rc5/tsugu.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 tsugu/remote/router/bind_player_verification_on.py
 tsugu/remote/router/change_default_server.py
 tsugu/remote/router/change_server_mode.py
 tsugu/remote/router/player_status.py
 tsugu/remote/router/switch_car_forwarding_off.py
 tsugu/remote/router/switch_car_forwarding_on.py
 tsugu/remote/router/unbind_player.py
+tsugu/storage/__init__.py
+tsugu/storage/db/__init__.py
+tsugu/storage/remote_db/__init__.py
 tsugu/universal/__init__.py
 tsugu/universal/help.py
 tsugu/universal/rooms_forward.py
 tsugu/universal/router/__init__.py
 tsugu/universal/router/event_stage.py
 tsugu/universal/router/gacha_simulate.py
 tsugu/universal/router/get_card_illustration.py
@@ -64,14 +67,16 @@
 tsugu_async/remote/router/bind_player_verification_on.py
 tsugu_async/remote/router/change_default_server.py
 tsugu_async/remote/router/change_server_mode.py
 tsugu_async/remote/router/player_status.py
 tsugu_async/remote/router/switch_car_forwarding_off.py
 tsugu_async/remote/router/switch_car_forwarding_on.py
 tsugu_async/remote/router/unbind_player.py
+tsugu_async/storage/__init__.py
+tsugu_async/storage/remote_db/__init__.py
 tsugu_async/universal/__init__.py
 tsugu_async/universal/help.py
 tsugu_async/universal/rooms_forward.py
 tsugu_async/universal/router/__init__.py
 tsugu_async/universal/router/event_stage.py
 tsugu_async/universal/router/gacha_simulate.py
 tsugu_async/universal/router/get_card_illustration.py
```

### Comparing `tsugu-0.9.9rc4/tsugu_async/command_matcher/__init__.py` & `tsugu-0.9.9rc5/tsugu_async/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/config.py` & `tsugu-0.9.9rc5/tsugu_async/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/handler.py` & `tsugu-0.9.9rc5/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/__init__.py` & `tsugu-0.9.9rc5/tsugu_async/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player_verification_off.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/bind_player_verification_on.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/change_default_server.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/change_server_mode.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/player_status.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/remote/router/unbind_player.py` & `tsugu-0.9.9rc5/tsugu_async/remote/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/__init__.py` & `tsugu-0.9.9rc5/tsugu_async/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/help.py` & `tsugu-0.9.9rc5/tsugu_async/universal/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/rooms_forward.py` & `tsugu-0.9.9rc5/tsugu_async/universal/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/__init__.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/event_stage.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/gacha_simulate.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/lsycx.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/search_player.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/song_chart.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/ycx.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/universal/router/ycx_all.py` & `tsugu-0.9.9rc5/tsugu_async/universal/router/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc4/tsugu_async/utils/__init__.py` & `tsugu-0.9.9rc5/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*


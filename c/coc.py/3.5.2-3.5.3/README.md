# Comparing `tmp/coc_py-3.5.2.tar.gz` & `tmp/coc_py-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc_py-3.5.2.tar", last modified: Sat Apr 27 17:31:55 2024, max compression
+gzip compressed data, was "coc_py-3.5.3.tar", last modified: Tue May 14 18:24:18 2024, max compression
```

## Comparing `coc_py-3.5.2.tar` & `coc_py-3.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 17:31:50.000000 coc_py-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 17:31:50.000000 coc_py-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 17:31:55.009181 coc_py-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-27 17:31:50.000000 coc_py-3.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (127)    83547 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.993182 coc_py-3.5.2/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (127)    30024 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/coc/static/
--rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/equipment.json
--rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/spell_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/troop_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-27 17:31:50.000000 coc_py-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 17:31:50.000000 coc_py-3.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:31:55.013182 coc_py-3.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 17:31:50.000000 coc_py-3.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_capitalraidseasons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_clash_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_troop_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 18:24:14.000000 coc_py-3.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 18:24:14.000000 coc_py-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-14 18:24:18.676546 coc_py-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-14 18:24:14.000000 coc_py-3.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.660546 coc_py-3.5.3/coc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83549 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.656546 coc_py-3.5.3/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30024 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.672546 coc_py-3.5.3/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/equipment.json
+-rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/spell_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/troop_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-14 18:24:14.000000 coc_py-3.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 18:24:14.000000 coc_py-3.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:24:18.676546 coc_py-3.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 18:24:14.000000 coc_py-3.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_capitalraidseasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_clash_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_troop_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_wars.py
```

### Comparing `coc_py-3.5.2/LICENSE` & `coc_py-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/PKG-INFO` & `coc_py-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.5.2
+Version: 3.5.3
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.5.2/README.rst` & `coc_py-3.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/__init__.py` & `coc_py-3.5.3/coc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "3.5.2"
+__version__ = "3.5.3"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
```

### Comparing `coc_py-3.5.2/coc/abc.py` & `coc_py-3.5.3/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/clans.py` & `coc_py-3.5.3/coc/clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/client.py` & `coc_py-3.5.3/coc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1894,31 +1894,31 @@
         Returns
         --------
         :class:`BaseLeague`
             The first league matching the league name. Could be ``None`` if not found.
         """
         return get(await self.search_capital_leagues(), name=league_name)
 
-    async def get_seasons(self, league_id: int = 29000021) -> List[str]:
+    async def get_seasons(self, league_id: int = 29000022) -> List[str]:
         """Get league seasons.
 
         .. note::
 
-            League season information is available only for Legend League, with a league ID 29000021.
+            League season information is available only for Legend League, with a league ID 29000022.
 
 
         Parameters
         -----------
         league_id : str
             The League ID to search for. Defaults to the only league you can get season information for, legends.
 
         Raises
         ------
         InvalidArgument
-            An invalid league_id was supplied. Currently the only league supported is legends.
+            An invalid league_id was supplied. Currently, the only league supported is legends.
 
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
@@ -1926,33 +1926,33 @@
         -------
         List[str]
             The legend season IDs, in the form ``YYYY-MM``, ie. ``2020-04``.
         """
         data = await self.http.get_league_seasons(league_id)
         return [entry["id"] for entry in data["items"]]
 
-    async def get_season_rankings(self, league_id: int, season_id: int) -> List[RankedPlayer]:
+    async def get_season_rankings(self, league_id: int, season_id: str) -> List[RankedPlayer]:
         """Get league season rankings.
 
         .. note::
 
-            League season information is available only for Legend League, with a league ID 29000021.
+            League season information is available only for Legend League, with a league ID 29000022.
 
 
         Parameters
         -----------
         league_id : str
             The League ID to search for.
         season_id : str
             The Season ID to search for.
 
         Raises
         ------
         InvalidArgument
-            An invalid league_id or season_id was supplied. Currently the only league supported is legends.
+            An invalid league_id or season_id was supplied. Currently, the only league supported is legends.
 
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
```

### Comparing `coc_py-3.5.2/coc/entry_logs.py` & `coc_py-3.5.3/coc/entry_logs.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/enums.py` & `coc_py-3.5.3/coc/enums.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/errors.py` & `coc_py-3.5.3/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/events.py` & `coc_py-3.5.3/coc/events.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/events.pyi` & `coc_py-3.5.3/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/ext/discordlinks/__init__.py` & `coc_py-3.5.3/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/ext/fullwarapi/__init__.py` & `coc_py-3.5.3/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/ext/triggers/cron.py` & `coc_py-3.5.3/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/ext/triggers/triggers.py` & `coc_py-3.5.3/coc/ext/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/hero.py` & `coc_py-3.5.3/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/http.py` & `coc_py-3.5.3/coc/http.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/iterators.py` & `coc_py-3.5.3/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/miscmodels.py` & `coc_py-3.5.3/coc/miscmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,16 +384,14 @@
     -----------
     small:
         :class:`str` - URL for a small sized badge (70x70).
     medium:
         :class:`str` - URL for a medium sized badge (200x200).
     large:
         :class:`str` - URL for a large sized badge (512x512).
-    url:
-        :class:`str` - Medium, the default URL badge size.
     """
 
     __slots__ = ("small", "medium", "large", "url", "_client")
 
     def __repr__(self):
         attrs = [
             ("url", self.url),
@@ -403,15 +401,19 @@
     def __init__(self, *, data, client):
         self._client = client
 
         self.small: str = data.get("small")
         self.medium: str = data.get("medium")
         self.large: str = data.get("large")
 
-        self.url: str = self.medium
+    @property
+    def url(self) -> str:
+        """:class:`str`: the default icon URL. Returns the medium-sized icon URL if available.
+        Falls back to small and large (in that order) if not"""
+        return self.medium or self.small or self.large
 
     async def save(self, filepath, size=None) -> int:
         """
         Save this badge as a file-like object.
 
         Parameters
         -----------
@@ -432,15 +434,15 @@
             The URL was not found.
         """
         sizes = {"small": self.small, "medium": self.medium, "large": self.large}
 
         if size and size in sizes.keys():
             url = sizes[size]
         else:
-            url = self.medium
+            url = self.url
 
         data = await self._client.http.get_data_from_url(url)
 
         with open(filepath, "wb") as file:
             return file.write(data)
 
 
@@ -451,16 +453,14 @@
     -----------
     tiny:
         :class:`str`: URL for a tiny sized icon (32x32).
     small:
         :class:`str`: URL for a small sized icon (72x72).
     medium:
         :class:`str`: URL for a medium sized icon (288x288).
-    url:
-        :class:`str`: ``small``, the default URL icon size
     """
 
     __slots__ = ("small", "medium", "tiny", "url", "_client")
 
     def __repr__(self):
         attrs = [
             ("url", self.url),
@@ -470,15 +470,19 @@
     def __init__(self, *, data, client):
         self._client = client
 
         self.tiny: str = data.get("tiny")
         self.small: str = data.get("small")
         self.medium: str = data.get("medium")
 
-        self.url: str = self.medium
+    @property
+    def url(self) -> str:
+        """:class:`str`: the default icon URL. Returns the medium-sized icon URL if available.
+        Falls back to small and tiny (in that order) if not"""
+        return self.medium or self.small or self.tiny
 
     async def save(self, filepath: str, size: Optional[str] = None) -> int:
         """
         Save this icon as a file-like object.
 
         Parameters
         -----------
@@ -499,15 +503,15 @@
             The URL was not found.
         """
         sizes = {"tiny": self.tiny, "small": self.small, "medium": self.medium}
 
         if size and size in sizes.keys():
             url = sizes[size]
         else:
-            url = self.medium
+            url = self.url
 
         data = await self._client.http.get_data_from_url(url)
 
         with open(filepath, "wb") as file:
             return file.write(data)
```

### Comparing `coc_py-3.5.2/coc/player_clan.py` & `coc_py-3.5.3/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/players.py` & `coc_py-3.5.3/coc/players.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/raid.py` & `coc_py-3.5.3/coc/raid.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/spell.py` & `coc_py-3.5.3/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/buildings.json` & `coc_py-3.5.3/coc/static/buildings.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/characters.json` & `coc_py-3.5.3/coc/static/characters.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/equipment.json` & `coc_py-3.5.3/coc/static/equipment.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/heroes.json` & `coc_py-3.5.3/coc/static/heroes.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/pets.json` & `coc_py-3.5.3/coc/static/pets.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/spells.json` & `coc_py-3.5.3/coc/static/spells.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/supers.json` & `coc_py-3.5.3/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/texts_EN.json` & `coc_py-3.5.3/coc/static/texts_EN.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/townhall_levels.json` & `coc_py-3.5.3/coc/static/townhall_levels.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/troop_ids.json` & `coc_py-3.5.3/coc/static/troop_ids.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/static/update_static.py` & `coc_py-3.5.3/coc/static/update_static.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/troop.py` & `coc_py-3.5.3/coc/troop.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/utils.py` & `coc_py-3.5.3/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/war_attack.py` & `coc_py-3.5.3/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/war_clans.py` & `coc_py-3.5.3/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/war_members.py` & `coc_py-3.5.3/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc/wars.py` & `coc_py-3.5.3/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/coc.py.egg-info/PKG-INFO` & `coc_py-3.5.3/coc.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.5.2
+Version: 3.5.3
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.5.2/coc.py.egg-info/SOURCES.txt` & `coc_py-3.5.3/coc.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/pyproject.toml` & `coc_py-3.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
 maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" },
     { name = "lukasthaler"}, { name = "doluk"}]
-version = "3.5.2"
+version = "3.5.3"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `coc_py-3.5.2/tests/test_capitalraidseasons.py` & `coc_py-3.5.3/tests/test_capitalraidseasons.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/tests/test_clans.py` & `coc_py-3.5.3/tests/test_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/tests/test_clash_meta.py` & `coc_py-3.5.3/tests/test_clash_meta.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/tests/test_players.py` & `coc_py-3.5.3/tests/test_players.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/tests/test_troop_levels.py` & `coc_py-3.5.3/tests/test_troop_levels.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.2/tests/test_wars.py` & `coc_py-3.5.3/tests/test_wars.py`

 * *Files identical despite different names*


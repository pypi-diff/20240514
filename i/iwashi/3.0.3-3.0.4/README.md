# Comparing `tmp/iwashi-3.0.3.tar.gz` & `tmp/iwashi-3.0.4.tar.gz`

## Comparing `iwashi-3.0.3.tar` & `iwashi-3.0.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 iwashi-3.0.3/.prettierignore
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-3.0.3/.python-version
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 iwashi-3.0.3/requirements-dev.lock
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.3/requirements.lock
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 iwashi-3.0.3/.github/scripts/report-failures.sh
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 iwashi-3.0.3/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 iwashi-3.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 iwashi-3.0.3/.vscode/settings.json
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iwashi-3.0.3/scripts/generate_version.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/__main__.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/helper.py
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/iwashi.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/throttle.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/version.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/visitor.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/bandcamp.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/booth.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/fanbox.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/github.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/instagram.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/itchio.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/kofi.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/linktree.py
--rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/litlink.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/mirrativ.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/nicovideo.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/note.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/patreon.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/pixiv.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/reddit.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/skeb.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/sketch.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/soundcloud.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/spotify.py
--rw-r--r--   0        0        0    92171 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/tiktok.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/twitcasting.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/twitch.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/twitter.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/__init__.py
--rw-r--r--   0        0        0     9162 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/youtube.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/types/__init__.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/types/about.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata2.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/service_tester.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_bandcamp.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_booth.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_error.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_fanbox.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_github.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_instagram.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_itchio.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_kofi.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_linktree.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_litlink.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_mirrativ.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_nicovideo.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_note.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_patreon.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_pixiv.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_reddit.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_skeb.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_sketch.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_soundcloud.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_spotify.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_tiktok.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_tree.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_twitcasting.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_twitch.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_twitter.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 iwashi-3.0.3/tests/test_youtube.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-3.0.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-3.0.3/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-3.0.3/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 iwashi-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 iwashi-3.0.4/.prettierignore
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-3.0.4/.python-version
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 iwashi-3.0.4/requirements-dev.lock
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.4/requirements.lock
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 iwashi-3.0.4/.github/scripts/report-failures.sh
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 iwashi-3.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 iwashi-3.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 iwashi-3.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iwashi-3.0.4/scripts/generate_version.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/__main__.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/helper.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/iwashi.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/throttle.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/version.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/visitor.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/bandcamp.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/booth.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/fanbox.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/github.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/instagram.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/itchio.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/kofi.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/linktree.py
+-rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/litlink.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/mirrativ.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/nicovideo.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/note.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/patreon.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/pixiv.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/reddit.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/skeb.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/sketch.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/soundcloud.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/spotify.py
+-rw-r--r--   0        0        0    92171 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/tiktok.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/twitcasting.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/twitch.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/twitter.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/__init__.py
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/youtube.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/types/__init__.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/types/about.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata2.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/service_tester.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_bandcamp.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_booth.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_error.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_fanbox.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_github.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_instagram.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_itchio.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_kofi.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_linktree.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_litlink.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_mirrativ.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_nicovideo.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_note.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_patreon.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_pixiv.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_reddit.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_skeb.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_sketch.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_soundcloud.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_spotify.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_tiktok.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_tree.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_twitcasting.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_twitch.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_twitter.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 iwashi-3.0.4/tests/test_youtube.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-3.0.4/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-3.0.4/LICENSE
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-3.0.4/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 iwashi-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-3.0.4/PKG-INFO
```

### Comparing `iwashi-3.0.3/requirements-dev.lock` & `iwashi-3.0.4/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -27,40 +27,40 @@
 click==8.1.7
     # via iwashi
 colorama==0.4.6
     # via build
     # via click
     # via loguru
     # via pytest
-coverage==7.4.3
+coverage==7.5.1
     # via pytest-cov
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
-idna==3.6
+idna==3.7
     # via requests
     # via yarl
 iniconfig==2.0.0
     # via pytest
 loguru==0.7.2
     # via iwashi
 multidict==6.0.5
     # via aiohttp
     # via yarl
 nodeenv==1.8.0
     # via pyright
-packaging==23.2
+packaging==24.0
     # via build
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via build
 pyright==1.1.362
-pytest==8.1.0
+pytest==8.2.0
     # via pytest-asyncio
     # via pytest-cov
 pytest-asyncio==0.23.6
 pytest-cov==5.0.0
 requests==2.31.0
 ruff==0.4.4
 setuptools==69.5.1
```

### Comparing `iwashi-3.0.3/requirements.lock` & `iwashi-3.0.4/requirements.lock`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # via iwashi
 colorama==0.4.6
     # via click
     # via loguru
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
-idna==3.6
+idna==3.7
     # via yarl
 loguru==0.7.2
     # via iwashi
 multidict==6.0.5
     # via aiohttp
     # via yarl
 soupsieve==2.5
```

### Comparing `iwashi-3.0.3/.github/workflows/pypi.yml` & `iwashi-3.0.4/.github/workflows/pypi.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 name: PyPI
 
-on: workflow_dispatch
+on:
+  workflow_dispatch:
+  push:
+    branches: [ master ]
 
 jobs:
   deploy:
+    if: startsWith(github.event.head_commit.message, 'publish')
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
```

### Comparing `iwashi-3.0.3/.github/workflows/test.yml` & `iwashi-3.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/.vscode/settings.json` & `iwashi-3.0.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/scripts/generate_version.py` & `iwashi-3.0.4/scripts/generate_version.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/helper.py` & `iwashi-3.0.4/src/iwashi/helper.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/iwashi.py` & `iwashi-3.0.4/src/iwashi/iwashi.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/throttle.py` & `iwashi-3.0.4/src/iwashi/throttle.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/visitor.py` & `iwashi-3.0.4/src/iwashi/visitor.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/__init__.py` & `iwashi-3.0.4/src/iwashi/service/__init__.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/bandcamp.py` & `iwashi-3.0.4/src/iwashi/service/bandcamp.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/booth.py` & `iwashi-3.0.4/src/iwashi/service/booth.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/fanbox.py` & `iwashi-3.0.4/src/iwashi/service/fanbox.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/github.py` & `iwashi-3.0.4/src/iwashi/service/github.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/instagram.py` & `iwashi-3.0.4/src/iwashi/service/instagram.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/itchio.py` & `iwashi-3.0.4/src/iwashi/service/itchio.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/kofi.py` & `iwashi-3.0.4/src/iwashi/service/kofi.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/linktree.py` & `iwashi-3.0.4/src/iwashi/service/linktree.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/litlink.py` & `iwashi-3.0.4/src/iwashi/service/litlink.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/mirrativ.py` & `iwashi-3.0.4/src/iwashi/service/mirrativ.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/nicovideo.py` & `iwashi-3.0.4/src/iwashi/service/nicovideo.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/note.py` & `iwashi-3.0.4/src/iwashi/service/note.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/patreon.py` & `iwashi-3.0.4/src/iwashi/service/patreon.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/pixiv.py` & `iwashi-3.0.4/src/iwashi/service/pixiv.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/reddit.py` & `iwashi-3.0.4/src/iwashi/service/reddit.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/skeb.py` & `iwashi-3.0.4/src/iwashi/service/skeb.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/sketch.py` & `iwashi-3.0.4/src/iwashi/service/sketch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/soundcloud.py` & `iwashi-3.0.4/src/iwashi/service/soundcloud.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/spotify.py` & `iwashi-3.0.4/src/iwashi/service/spotify.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/tiktok.py` & `iwashi-3.0.4/src/iwashi/service/tiktok.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/twitcasting.py` & `iwashi-3.0.4/src/iwashi/service/twitcasting.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/twitch.py` & `iwashi-3.0.4/src/iwashi/service/twitch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/twitter.py` & `iwashi-3.0.4/src/iwashi/service/twitter.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/youtube/youtube.py` & `iwashi-3.0.4/src/iwashi/service/youtube/youtube.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 from typing import Any
 from urllib import parse
 
 import bs4
 
-from iwashi.helper import HTTP_REGEX, normalize_url
+from iwashi.helper import HTTP_REGEX, normalize_url, traverse
 from iwashi.service.youtube.types.ytinitialdata2 import ProfileRes2
 from iwashi.service.youtube.types.ytinitialdata3 import ProfileRes3
 from iwashi.visitor import Context, Service
 
 from .types import thumbnails, ytinitialdata
 from .types.about import AboutRes
 
@@ -108,17 +108,22 @@
         if url is None:
             raise RuntimeError("Thumbnail not found")
         return url
 
     async def get_token(self, data: Any) -> str | None:
         data2: ProfileRes2 = data
         if "pageHeaderRenderer" in data2["header"]:
-            suffix = data2["header"]["pageHeaderRenderer"]["content"][
+            pageHeaderViewModel = data2["header"]["pageHeaderRenderer"]["content"][
                 "pageHeaderViewModel"
-            ]["attribution"]["attributionViewModel"]["suffix"]
+            ]
+            if "attribution" not in pageHeaderViewModel:
+                return None
+            suffix = pageHeaderViewModel["attribution"]["attributionViewModel"][
+                "suffix"
+            ]
             if not suffix:
                 return None
             for a in suffix["commandRuns"]:
                 for b in a["onTap"]["innertubeCommand"]["showEngagementPanelEndpoint"][
                     "engagementPanel"
                 ]["engagementPanelSectionListRenderer"]["content"][
                     "sectionListRenderer"
@@ -130,17 +135,20 @@
                         ].startswith("/youtubei/v1/browse"):
                             return endpoint["continuationCommand"]["token"]
         else:
             data3: ProfileRes3 = data
             c4TabbedHeaderRenderer = data3["header"]["c4TabbedHeaderRenderer"]
             if "headerLinks" not in c4TabbedHeaderRenderer:
                 return None
-            for a in c4TabbedHeaderRenderer["headerLinks"][
+            channelHeaderLinksViewModel = c4TabbedHeaderRenderer["headerLinks"][
                 "channelHeaderLinksViewModel"
-            ]["more"]["commandRuns"]:
+            ]
+            if "more" not in channelHeaderLinksViewModel:
+                return None
+            for a in channelHeaderLinksViewModel["more"]["commandRuns"]:
                 for b in a["onTap"]["innertubeCommand"]["showEngagementPanelEndpoint"][
                     "engagementPanel"
                 ]["engagementPanelSectionListRenderer"]["content"][
                     "sectionListRenderer"
                 ]["contents"]:
                     for c in b["itemSectionRenderer"]["contents"]:
                         endpoint = c["continuationItemRenderer"]["continuationEndpoint"]
```

### Comparing `iwashi-3.0.3/src/iwashi/service/youtube/types/about.py` & `iwashi-3.0.4/src/iwashi/service/youtube/types/about.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata.py` & `iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata2.py` & `iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict
+from typing import NotRequired, TypedDict
 
 
 class WebCommandMetadata(TypedDict):
     apiUrl: str
 
 
 class CommandMetadata(TypedDict):
@@ -76,35 +76,35 @@
 
 
 class Suffix(TypedDict):
     commandRuns: CommandRuns
 
 
 class AttributionViewModel(TypedDict):
-    suffix: Suffix
+    suffix: Suffix | None
 
 
 class Attribution(TypedDict):
     attributionViewModel: AttributionViewModel
 
 
 class PageHeaderViewModel(TypedDict):
-    attribution: Attribution
+    attribution: NotRequired[Attribution]
 
 
 class Content(TypedDict):
     pageHeaderViewModel: PageHeaderViewModel
 
 
 class PageHeaderRenderer(TypedDict):
     content: Content
 
 
 class Header(TypedDict):
-    pageHeaderRenderer: PageHeaderRenderer
+    pageHeaderRenderer: NotRequired[PageHeaderRenderer]
 
 
 class ProfileRes2(TypedDict):
     header: Header
 
 
 # data: ProfileRes = ...
```

### Comparing `iwashi-3.0.3/src/iwashi/service/youtube/types/ytinitialdata3.py` & `iwashi-3.0.4/src/iwashi/service/youtube/types/ytinitialdata3.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/service_tester.py` & `iwashi-3.0.4/tests/service_tester.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_bandcamp.py` & `iwashi-3.0.4/tests/test_bandcamp.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_booth.py` & `iwashi-3.0.4/tests/test_booth.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_fanbox.py` & `iwashi-3.0.4/tests/test_fanbox.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_github.py` & `iwashi-3.0.4/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_instagram.py` & `iwashi-3.0.4/tests/test_instagram.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_itchio.py` & `iwashi-3.0.4/tests/test_itchio.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_kofi.py` & `iwashi-3.0.4/tests/test_kofi.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_linktree.py` & `iwashi-3.0.4/tests/test_linktree.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_litlink.py` & `iwashi-3.0.4/tests/test_litlink.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_mirrativ.py` & `iwashi-3.0.4/tests/test_mirrativ.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_nicovideo.py` & `iwashi-3.0.4/tests/test_nicovideo.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_note.py` & `iwashi-3.0.4/tests/test_note.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_patreon.py` & `iwashi-3.0.4/tests/test_patreon.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_pixiv.py` & `iwashi-3.0.4/tests/test_pixiv.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_reddit.py` & `iwashi-3.0.4/tests/test_reddit.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_skeb.py` & `iwashi-3.0.4/tests/test_skeb.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_sketch.py` & `iwashi-3.0.4/tests/test_sketch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_soundcloud.py` & `iwashi-3.0.4/tests/test_soundcloud.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_spotify.py` & `iwashi-3.0.4/tests/test_spotify.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_tiktok.py` & `iwashi-3.0.4/tests/test_tiktok.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_twitcasting.py` & `iwashi-3.0.4/tests/test_twitcasting.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_twitch.py` & `iwashi-3.0.4/tests/test_twitch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_twitter.py` & `iwashi-3.0.4/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/tests/test_youtube.py` & `iwashi-3.0.4/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/LICENSE` & `iwashi-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.3/pyproject.toml` & `iwashi-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iwashi"
-version = "3.0.3"
+version = "3.0.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["aiohttp>=3.9.5", "bs4>=0.0.2", "loguru>=0.7.2", "click>=8.1.7"]
 readme = "README.md"
 requires-python = ">= 3.8"
```


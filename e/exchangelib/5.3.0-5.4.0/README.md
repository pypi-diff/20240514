# Comparing `tmp/exchangelib-5.3.0.tar.gz` & `tmp/exchangelib-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchangelib-5.3.0.tar", last modified: Thu Apr 25 11:16:36 2024, max compression
+gzip compressed data, was "exchangelib-5.4.0.tar", last modified: Tue May 14 20:23:01 2024, max compression
```

## Comparing `exchangelib-5.3.0.tar` & `exchangelib-5.4.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.745126 exchangelib-5.3.0/
--rw-r--r--   0 erik       (501) staff       (20)    38942 2024-04-25 11:13:46.000000 exchangelib-5.3.0/CHANGELOG.md
--rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.3.0/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)       91 2024-03-03 15:20:26.000000 exchangelib-5.3.0/MANIFEST.in
--rw-r--r--   0 erik       (501) staff       (20)     3597 2024-04-25 11:16:36.744902 exchangelib-5.3.0/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1978 2023-11-15 18:16:03.000000 exchangelib-5.3.0/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.735717 exchangelib-5.3.0/exchangelib/
--rw-r--r--   0 erik       (501) staff       (20)     2819 2024-04-25 11:14:07.000000 exchangelib-5.3.0/exchangelib/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    36054 2024-03-26 11:46:04.000000 exchangelib-5.3.0/exchangelib/account.py
--rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.3.0/exchangelib/attachments.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.736748 exchangelib-5.3.0/exchangelib/autodiscover/
--rw-r--r--   0 erik       (501) staff       (20)      499 2022-11-23 00:50:30.000000 exchangelib-5.3.0/exchangelib/autodiscover/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.3.0/exchangelib/autodiscover/cache.py
--rw-r--r--   0 erik       (501) staff       (20)    22636 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/autodiscover/discovery.py
--rw-r--r--   0 erik       (501) staff       (20)     2164 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/autodiscover/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)     4193 2022-10-10 07:45:39.000000 exchangelib-5.3.0/exchangelib/configuration.py
--rw-r--r--   0 erik       (501) staff       (20)    12159 2024-03-03 21:14:09.000000 exchangelib-5.3.0/exchangelib/credentials.py
--rw-r--r--   0 erik       (501) staff       (20)    31304 2024-03-03 21:14:09.000000 exchangelib-5.3.0/exchangelib/errors.py
--rw-r--r--   0 erik       (501) staff       (20)    11527 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/ewsdatetime.py
--rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.3.0/exchangelib/extended_properties.py
--rw-r--r--   0 erik       (501) staff       (20)    65275 2024-04-25 11:11:21.000000 exchangelib-5.3.0/exchangelib/fields.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.737488 exchangelib-5.3.0/exchangelib/folders/
--rw-r--r--   0 erik       (501) staff       (20)     5250 2024-03-18 11:34:30.000000 exchangelib-5.3.0/exchangelib/folders/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    39912 2024-04-23 17:43:38.000000 exchangelib-5.3.0/exchangelib/folders/base.py
--rw-r--r--   0 erik       (501) staff       (20)    23778 2024-03-17 10:08:54.000000 exchangelib-5.3.0/exchangelib/folders/collections.py
--rw-r--r--   0 erik       (501) staff       (20)    20228 2024-03-18 11:50:03.000000 exchangelib-5.3.0/exchangelib/folders/known_folders.py
--rw-r--r--   0 erik       (501) staff       (20)     7321 2024-04-16 18:03:25.000000 exchangelib-5.3.0/exchangelib/folders/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    16395 2024-04-23 17:45:53.000000 exchangelib-5.3.0/exchangelib/folders/roots.py
--rw-r--r--   0 erik       (501) staff       (20)     3339 2024-04-23 21:49:55.000000 exchangelib-5.3.0/exchangelib/indexed_properties.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.738555 exchangelib-5.3.0/exchangelib/items/
--rw-r--r--   0 erik       (501) staff       (20)     3381 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/items/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.3.0/exchangelib/items/base.py
--rw-r--r--   0 erik       (501) staff       (20)    20811 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/items/calendar_item.py
--rw-r--r--   0 erik       (501) staff       (20)    15117 2024-04-23 21:49:55.000000 exchangelib-5.3.0/exchangelib/items/contact.py
--rw-r--r--   0 erik       (501) staff       (20)    17951 2023-08-21 05:19:29.000000 exchangelib-5.3.0/exchangelib/items/item.py
--rw-r--r--   0 erik       (501) staff       (20)     9050 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/items/message.py
--rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.3.0/exchangelib/items/post.py
--rw-r--r--   0 erik       (501) staff       (20)     5876 2023-05-04 21:52:26.000000 exchangelib-5.3.0/exchangelib/items/task.py
--rw-r--r--   0 erik       (501) staff       (20)    90625 2024-04-23 17:41:31.000000 exchangelib-5.3.0/exchangelib/properties.py
--rw-r--r--   0 erik       (501) staff       (20)    35041 2024-03-07 10:53:09.000000 exchangelib-5.3.0/exchangelib/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)    29695 2024-03-18 13:00:51.000000 exchangelib-5.3.0/exchangelib/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.3.0/exchangelib/recurrence.py
--rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.3.0/exchangelib/restriction.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.744220 exchangelib-5.3.0/exchangelib/services/
--rw-r--r--   0 erik       (501) staff       (20)     3775 2024-03-03 21:14:09.000000 exchangelib-5.3.0/exchangelib/services/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/archive_item.py
--rw-r--r--   0 erik       (501) staff       (20)    46109 2024-04-16 18:04:04.000000 exchangelib-5.3.0/exchangelib/services/common.py
--rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.3.0/exchangelib/services/convert_id.py
--rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.3.0/exchangelib/services/copy_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/create_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1966 2024-04-16 17:56:41.000000 exchangelib-5.3.0/exchangelib/services/create_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/create_item.py
--rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.3.0/exchangelib/services/create_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/delete_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/delete_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/delete_item.py
--rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.3.0/exchangelib/services/delete_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/empty_folder.py
--rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/expand_dl.py
--rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/export_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3621 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/services/find_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.3.0/exchangelib/services/find_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.3.0/exchangelib/services/find_people.py
--rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_delegate.py
--rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2598 2024-04-16 17:56:41.000000 exchangelib-5.3.0/exchangelib/services/get_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_mail_tips.py
--rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_persona.py
--rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_room_lists.py
--rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_rooms.py
--rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_searchable_mailboxes.py
--rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_server_time_zones.py
--rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_streaming_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_user_availability.py
--rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/get_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/get_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     4131 2024-04-11 18:51:38.000000 exchangelib-5.3.0/exchangelib/services/get_user_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     4647 2024-03-26 09:33:46.000000 exchangelib-5.3.0/exchangelib/services/inbox_rules.py
--rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/mark_as_junk.py
--rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/move_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/move_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.3.0/exchangelib/services/resolve_names.py
--rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/send_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.3.0/exchangelib/services/send_notification.py
--rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/set_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     5139 2024-03-03 21:14:09.000000 exchangelib-5.3.0/exchangelib/services/subscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     3734 2024-04-16 17:56:41.000000 exchangelib-5.3.0/exchangelib/services/sync_folder_hierarchy.py
--rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.3.0/exchangelib/services/sync_folder_items.py
--rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/services/unsubscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     7593 2024-04-16 17:56:41.000000 exchangelib-5.3.0/exchangelib/services/update_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4788 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/services/update_item.py
--rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/update_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.3.0/exchangelib/services/upload_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.3.0/exchangelib/settings.py
--rw-r--r--   0 erik       (501) staff       (20)     7956 2023-05-03 11:21:13.000000 exchangelib-5.3.0/exchangelib/transport.py
--rw-r--r--   0 erik       (501) staff       (20)    33704 2024-04-25 11:11:21.000000 exchangelib-5.3.0/exchangelib/util.py
--rw-r--r--   0 erik       (501) staff       (20)    13974 2023-11-15 18:16:03.000000 exchangelib-5.3.0/exchangelib/version.py
--rw-r--r--   0 erik       (501) staff       (20)    37550 2024-03-03 21:14:09.000000 exchangelib-5.3.0/exchangelib/winzone.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-04-25 11:16:36.744386 exchangelib-5.3.0/exchangelib.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     3597 2024-04-25 11:16:36.000000 exchangelib-5.3.0/exchangelib.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     3294 2024-04-25 11:16:36.000000 exchangelib-5.3.0/exchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2024-04-25 11:16:36.000000 exchangelib-5.3.0/exchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)      315 2024-04-25 11:16:36.000000 exchangelib-5.3.0/exchangelib.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       12 2024-04-25 11:16:36.000000 exchangelib-5.3.0/exchangelib.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)     2187 2024-04-25 11:16:04.000000 exchangelib-5.3.0/pyproject.toml
--rw-r--r--   0 erik       (501) staff       (20)       38 2024-04-25 11:16:36.745167 exchangelib-5.3.0/setup.cfg
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.067085 exchangelib-5.4.0/
+-rw-r--r--   0 erik       (501) staff       (20)    39156 2024-05-14 19:59:22.000000 exchangelib-5.4.0/CHANGELOG.md
+-rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.4.0/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)       91 2024-03-03 15:20:26.000000 exchangelib-5.4.0/MANIFEST.in
+-rw-r--r--   0 erik       (501) staff       (20)     3696 2024-05-14 20:23:01.066893 exchangelib-5.4.0/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1978 2023-11-15 18:16:03.000000 exchangelib-5.4.0/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.057008 exchangelib-5.4.0/exchangelib/
+-rw-r--r--   0 erik       (501) staff       (20)     2885 2024-05-14 20:00:03.000000 exchangelib-5.4.0/exchangelib/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    36054 2024-03-26 11:46:04.000000 exchangelib-5.4.0/exchangelib/account.py
+-rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.4.0/exchangelib/attachments.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.058035 exchangelib-5.4.0/exchangelib/autodiscover/
+-rw-r--r--   0 erik       (501) staff       (20)      499 2024-05-13 21:25:48.000000 exchangelib-5.4.0/exchangelib/autodiscover/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.4.0/exchangelib/autodiscover/cache.py
+-rw-r--r--   0 erik       (501) staff       (20)    22636 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/autodiscover/discovery.py
+-rw-r--r--   0 erik       (501) staff       (20)     2164 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/autodiscover/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)     4534 2024-05-14 19:57:13.000000 exchangelib-5.4.0/exchangelib/configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)    12720 2024-05-14 19:57:13.000000 exchangelib-5.4.0/exchangelib/credentials.py
+-rw-r--r--   0 erik       (501) staff       (20)    31304 2024-03-03 21:14:09.000000 exchangelib-5.4.0/exchangelib/errors.py
+-rw-r--r--   0 erik       (501) staff       (20)    11527 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/ewsdatetime.py
+-rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.4.0/exchangelib/extended_properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    65275 2024-04-25 11:11:21.000000 exchangelib-5.4.0/exchangelib/fields.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.058794 exchangelib-5.4.0/exchangelib/folders/
+-rw-r--r--   0 erik       (501) staff       (20)     5344 2024-05-13 21:19:30.000000 exchangelib-5.4.0/exchangelib/folders/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    40332 2024-05-13 22:04:41.000000 exchangelib-5.4.0/exchangelib/folders/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    23778 2024-03-17 10:08:54.000000 exchangelib-5.4.0/exchangelib/folders/collections.py
+-rw-r--r--   0 erik       (501) staff       (20)    20652 2024-05-13 21:50:18.000000 exchangelib-5.4.0/exchangelib/folders/known_folders.py
+-rw-r--r--   0 erik       (501) staff       (20)     7321 2024-04-16 18:03:25.000000 exchangelib-5.4.0/exchangelib/folders/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    16395 2024-04-23 17:45:53.000000 exchangelib-5.4.0/exchangelib/folders/roots.py
+-rw-r--r--   0 erik       (501) staff       (20)     3339 2024-04-23 21:49:55.000000 exchangelib-5.4.0/exchangelib/indexed_properties.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.060334 exchangelib-5.4.0/exchangelib/items/
+-rw-r--r--   0 erik       (501) staff       (20)     3628 2024-05-13 21:46:48.000000 exchangelib-5.4.0/exchangelib/items/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.4.0/exchangelib/items/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    20811 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/items/calendar_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    15117 2024-04-23 21:49:55.000000 exchangelib-5.4.0/exchangelib/items/contact.py
+-rw-r--r--   0 erik       (501) staff       (20)    17951 2023-08-21 05:19:29.000000 exchangelib-5.4.0/exchangelib/items/item.py
+-rw-r--r--   0 erik       (501) staff       (20)     9050 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/items/message.py
+-rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.4.0/exchangelib/items/post.py
+-rw-r--r--   0 erik       (501) staff       (20)     5876 2023-05-04 21:52:26.000000 exchangelib-5.4.0/exchangelib/items/task.py
+-rw-r--r--   0 erik       (501) staff       (20)    90914 2024-05-13 19:22:15.000000 exchangelib-5.4.0/exchangelib/properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    35041 2024-03-07 10:53:09.000000 exchangelib-5.4.0/exchangelib/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)    29695 2024-03-18 13:00:51.000000 exchangelib-5.4.0/exchangelib/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.4.0/exchangelib/recurrence.py
+-rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.4.0/exchangelib/restriction.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.066231 exchangelib-5.4.0/exchangelib/services/
+-rw-r--r--   0 erik       (501) staff       (20)     3775 2024-05-13 21:25:48.000000 exchangelib-5.4.0/exchangelib/services/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/archive_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    46348 2024-05-13 22:04:41.000000 exchangelib-5.4.0/exchangelib/services/common.py
+-rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.4.0/exchangelib/services/convert_id.py
+-rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.4.0/exchangelib/services/copy_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/create_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1966 2024-04-16 17:56:41.000000 exchangelib-5.4.0/exchangelib/services/create_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/create_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.4.0/exchangelib/services/create_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/delete_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/delete_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/delete_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.4.0/exchangelib/services/delete_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/empty_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/expand_dl.py
+-rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/export_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3621 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/services/find_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.4.0/exchangelib/services/find_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.4.0/exchangelib/services/find_people.py
+-rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_delegate.py
+-rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2598 2024-04-16 17:56:41.000000 exchangelib-5.4.0/exchangelib/services/get_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_mail_tips.py
+-rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_persona.py
+-rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_room_lists.py
+-rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_rooms.py
+-rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_searchable_mailboxes.py
+-rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_server_time_zones.py
+-rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_streaming_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_user_availability.py
+-rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/get_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/get_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4131 2024-04-11 18:51:38.000000 exchangelib-5.4.0/exchangelib/services/get_user_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4647 2024-03-26 09:33:46.000000 exchangelib-5.4.0/exchangelib/services/inbox_rules.py
+-rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/mark_as_junk.py
+-rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/move_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/move_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.4.0/exchangelib/services/resolve_names.py
+-rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/send_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.4.0/exchangelib/services/send_notification.py
+-rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/set_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     5139 2024-03-03 21:14:09.000000 exchangelib-5.4.0/exchangelib/services/subscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     3734 2024-04-16 17:56:41.000000 exchangelib-5.4.0/exchangelib/services/sync_folder_hierarchy.py
+-rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.4.0/exchangelib/services/sync_folder_items.py
+-rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/services/unsubscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     7593 2024-04-16 17:56:41.000000 exchangelib-5.4.0/exchangelib/services/update_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4788 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/services/update_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/update_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.4.0/exchangelib/services/upload_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.4.0/exchangelib/settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     7956 2023-05-03 11:21:13.000000 exchangelib-5.4.0/exchangelib/transport.py
+-rw-r--r--   0 erik       (501) staff       (20)    33704 2024-04-25 11:11:21.000000 exchangelib-5.4.0/exchangelib/util.py
+-rw-r--r--   0 erik       (501) staff       (20)    13974 2023-11-15 18:16:03.000000 exchangelib-5.4.0/exchangelib/version.py
+-rw-r--r--   0 erik       (501) staff       (20)    37550 2024-03-03 21:14:09.000000 exchangelib-5.4.0/exchangelib/winzone.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-05-14 20:23:01.066376 exchangelib-5.4.0/exchangelib.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     3696 2024-05-14 20:23:01.000000 exchangelib-5.4.0/exchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     3294 2024-05-14 20:23:01.000000 exchangelib-5.4.0/exchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2024-05-14 20:23:01.000000 exchangelib-5.4.0/exchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)      333 2024-05-14 20:23:01.000000 exchangelib-5.4.0/exchangelib.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       12 2024-05-14 20:23:01.000000 exchangelib-5.4.0/exchangelib.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)     2235 2024-05-14 20:22:38.000000 exchangelib-5.4.0/pyproject.toml
+-rw-r--r--   0 erik       (501) staff       (20)       38 2024-05-14 20:23:01.067119 exchangelib-5.4.0/setup.cfg
```

### Comparing `exchangelib-5.3.0/CHANGELOG.md` & `exchangelib-5.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Change Log
 ==========
 
 HEAD
 ----
 
 
+5.4.0
+-----
+- Add `O365InteractiveConfiguration` helper class to set up MSAL auth for O365.
+- Add `exchangelib[msal]` installation flavor to match the above.
+- Various bug fixes related to distinguished folders.
+
+
 5.3.0
 -----
 - Fix various issues related to public folders and archive folders
 - Support read-write for ``Contact.im_addresses`
 - Improve reporting of inbox rule validation errors
```

### Comparing `exchangelib-5.3.0/LICENSE` & `exchangelib-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/PKG-INFO` & `exchangelib-5.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.3.0
+Version: 5.4.0
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Author-email: Erik Cederstrand <erik@cederstrand.dk>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/ecederstrand/exchangelib
 Project-URL: Issues, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
 Project-URL: Repository, https://github.com/ecederstrand/exchangelib.git
@@ -28,18 +28,21 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests_ntlm>=0.2.0
 Requires-Dist: requests_oauthlib
 Requires-Dist: tzdata
 Requires-Dist: tzlocal
 Provides-Extra: kerberos
 Requires-Dist: requests_gssapi; extra == "kerberos"
+Provides-Extra: msal
+Requires-Dist: msal; extra == "msal"
 Provides-Extra: sspi
 Requires-Dist: requests_negotiate_sspi; extra == "sspi"
 Provides-Extra: complete
 Requires-Dist: requests_gssapi; extra == "complete"
+Requires-Dist: msal; extra == "complete"
 Requires-Dist: requests_negotiate_sspi; extra == "complete"
 
 Exchange Web Services client library
 ====================================
 
 This module is an ORM for your Exchange mailbox, providing Django-style access to all your data. It is a
 platform-independent, well-performing, well-behaving, well-documented, well-tested and simple interface for
```

### Comparing `exchangelib-5.3.0/README.md` & `exchangelib-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/__init__.py` & `exchangelib-5.4.0/exchangelib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .account import Account, Identity
 from .attachments import FileAttachment, ItemAttachment
 from .autodiscover import discover
-from .configuration import Configuration
+from .configuration import Configuration, O365InteractiveConfiguration
 from .credentials import (
     DELEGATE,
     IMPERSONATION,
     Credentials,
     OAuth2AuthorizationCodeCredentials,
     OAuth2Credentials,
     OAuth2LegacyCredentials,
@@ -32,18 +32,17 @@
 from .properties import UID, Attendee, Body, DLMailbox, HTMLBody, ItemId, Mailbox, Room, RoomList
 from .protocol import BaseProtocol, FailFast, FaultTolerance, NoVerifyHTTPAdapter, TLSClientAuth
 from .restriction import Q
 from .settings import OofSettings
 from .transport import BASIC, CBA, DIGEST, GSSAPI, NTLM, OAUTH2, SSPI
 from .version import Build, Version
 
-__version__ = "5.3.0"
+__version__ = "5.4.0"
 
 __all__ = [
-    "__version__",
     "AcceptItem",
     "Account",
     "Attendee",
     "BASIC",
     "BaseProtocol",
     "Body",
     "Build",
@@ -75,14 +74,15 @@
     "Identity",
     "ItemAttachment",
     "ItemId",
     "Mailbox",
     "Message",
     "NTLM",
     "NoVerifyHTTPAdapter",
+    "O365InteractiveConfiguration",
     "OAUTH2",
     "OAuth2AuthorizationCodeCredentials",
     "OAuth2Credentials",
     "OAuth2LegacyCredentials",
     "OofSettings",
     "PostItem",
     "PostReplyItem",
@@ -97,14 +97,15 @@
     "TLSClientAuth",
     "Task",
     "TentativelyAcceptItem",
     "UID",
     "UTC",
     "UTC_NOW",
     "Version",
+    "__version__",
     "close_connections",
     "discover",
 ]
 
 # Set a default user agent, e.g. "exchangelib/3.1.1 (python-requests/2.22.0)"
 import requests.utils
```

### Comparing `exchangelib-5.3.0/exchangelib/account.py` & `exchangelib-5.4.0/exchangelib/account.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/attachments.py` & `exchangelib-5.4.0/exchangelib/attachments.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/autodiscover/cache.py` & `exchangelib-5.4.0/exchangelib/autodiscover/cache.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/autodiscover/discovery.py` & `exchangelib-5.4.0/exchangelib/autodiscover/discovery.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/autodiscover/protocol.py` & `exchangelib-5.4.0/exchangelib/autodiscover/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/configuration.py` & `exchangelib-5.4.0/exchangelib/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from cached_property import threaded_cached_property
 
-from .credentials import BaseCredentials, BaseOAuth2Credentials
+from .credentials import BaseCredentials, BaseOAuth2Credentials, O365InteractiveCredentials
 from .errors import InvalidEnumValue, InvalidTypeError
 from .protocol import FailFast, RetryPolicy
 from .transport import AUTH_TYPE_MAP, CREDENTIALS_REQUIRED, OAUTH2
 from .util import split_url
 from .version import Version
 
 log = logging.getLogger(__name__)
@@ -92,7 +92,15 @@
 
     def __repr__(self):
         args_str = ", ".join(
             f"{k}={getattr(self, k)!r}"
             for k in ("credentials", "service_endpoint", "auth_type", "version", "retry_policy")
         )
         return f"{self.__class__.__name__}({args_str})"
+
+
+class O365InteractiveConfiguration(Configuration):
+    SERVER = "outlook.office365.com"
+
+    def __init__(self, client_id, username):
+        credentials = O365InteractiveCredentials(client_id=client_id, username=username)
+        super().__init__(server=self.SERVER, auth_type=OAUTH2, credentials=credentials)
```

### Comparing `exchangelib-5.3.0/exchangelib/credentials.py` & `exchangelib-5.4.0/exchangelib/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,7 +303,20 @@
         credential = (
             "[access_token]"
             if self.access_token is not None
             else ("[authorization_code]" if self.authorization_code is not None else None)
         )
         description = " ".join(filter(None, [client_id, credential]))
         return description or "[underspecified credentials]"
+
+
+class O365InteractiveCredentials(OAuth2AuthorizationCodeCredentials):
+    AUTHORITY = "https://login.microsoftonline.com/organizations"
+    SCOPE = ["EWS.AccessAsUser.All"]
+
+    def __init__(self, client_id, username):
+        import msal
+
+        app = msal.PublicClientApplication(client_id=client_id, authority=self.AUTHORITY)
+        print("A local browser window will be open for you to sign in. CTRL+C to cancel.")
+        access_token = app.acquire_token_interactive(self.SCOPE, login_hint=username)
+        super().__init__(access_token=access_token)
```

### Comparing `exchangelib-5.3.0/exchangelib/errors.py` & `exchangelib-5.4.0/exchangelib/errors.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/ewsdatetime.py` & `exchangelib-5.4.0/exchangelib/ewsdatetime.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/extended_properties.py` & `exchangelib-5.4.0/exchangelib/extended_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/fields.py` & `exchangelib-5.4.0/exchangelib/fields.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/folders/__init__.py` & `exchangelib-5.4.0/exchangelib/folders/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ArchiveRecoverableItemsPurges,
     ArchiveRecoverableItemsRoot,
     ArchiveRecoverableItemsVersions,
     Audits,
     Birthdays,
     Calendar,
     CalendarLogging,
+    CalendarSearchCache,
     CommonViews,
     Companies,
     Conflicts,
     Contacts,
     ConversationHistory,
     ConversationSettings,
     CrawlerData,
@@ -64,14 +65,15 @@
     OrganizationalContacts,
     Outbox,
     ParkedMessages,
     PassThroughSearchResults,
     PdpProfileV2Secured,
     PeopleCentricConversationBuddies,
     PeopleConnect,
+    PersonMetadata,
     QedcDefaultRetention,
     QedcLongRetention,
     QedcMediumRetention,
     QedcShortRetention,
     QuarantinedEmail,
     QuarantinedEmailDefaultCategory,
     QuickContacts,
@@ -130,14 +132,15 @@
     "ArchiveRecoverableItemsVersions",
     "ArchiveRoot",
     "Audits",
     "BaseFolder",
     "Birthdays",
     "Calendar",
     "CalendarLogging",
+    "CalendarSearchCache",
     "CommonViews",
     "Companies",
     "Conflicts",
     "Contacts",
     "ConversationHistory",
     "ConversationSettings",
     "CrawlerData",
@@ -185,21 +188,22 @@
     "OrganizationalContacts",
     "Outbox",
     "ParkedMessages",
     "PassThroughSearchResults",
     "PdpProfileV2Secured",
     "PeopleCentricConversationBuddies",
     "PeopleConnect",
+    "PersonMetadata",
+    "PublicFoldersRoot",
     "QedcDefaultRetention",
-    "QedcMediumRetention",
     "QedcLongRetention",
+    "QedcMediumRetention",
     "QedcShortRetention",
     "QuarantinedEmail",
     "QuarantinedEmailDefaultCategory",
-    "PublicFoldersRoot",
     "QuickContacts",
     "RSSFeeds",
     "RecipientCache",
     "RecoverableItemsDeletions",
     "RecoverableItemsPurges",
     "RecoverableItemsRoot",
     "RecoverableItemsSubstrateHolds",
@@ -213,16 +217,16 @@
     "SOFT_DELETED",
     "Schedule",
     "SearchFolders",
     "SentItems",
     "ServerFailures",
     "SharePointNotifications",
     "Sharing",
-    "Shortcuts",
     "ShortNotes",
+    "Shortcuts",
     "Signal",
     "SingleFolderQuerySet",
     "SkypeTeamsMessages",
     "SmsAndChatsSync",
     "SpoolerQueue",
     "SwssItems",
     "SyncIssues",
```

### Comparing `exchangelib-5.3.0/exchangelib/folders/base.py` & `exchangelib-5.4.0/exchangelib/folders/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ParentFolderId,
     UserConfiguration,
     UserConfigurationName,
     UserConfigurationNameMNS,
 )
 from ..queryset import DoesNotExist, SearchableMixIn
 from ..util import TNS, is_iterable, require_id
-from ..version import EXCHANGE_2007_SP1, EXCHANGE_2010, SupportedVersionClassMixIn
+from ..version import EXCHANGE_2007_SP1, EXCHANGE_2010, EXCHANGE_2016, SupportedVersionClassMixIn
 from .collections import FolderCollection, PullSubscription, PushSubscription, StreamingSubscription, SyncCompleted
 from .queryset import DEEP as DEEP_FOLDERS
 from .queryset import MISSING_FOLDER_ERRORS
 from .queryset import SHALLOW as SHALLOW_FOLDERS
 from .queryset import SingleFolderQuerySet
 
 log = logging.getLogger(__name__)
@@ -73,15 +73,17 @@
     DEFAULT_FOLDER_TRAVERSAL_DEPTH = DEEP_FOLDERS
     DEFAULT_ITEM_TRAVERSAL_DEPTH = SHALLOW_ITEMS
     LOCALIZED_NAMES = {}  # A map of (str)locale: (tuple)localized_folder_names
     ITEM_MODEL_MAP = {cls.response_tag(): cls for cls in ITEM_CLASSES}
     ID_ELEMENT_CLS = FolderId
 
     _id = IdElementField(field_uri="folder:FolderId", value_cls=ID_ELEMENT_CLS)
-    _distinguished_id = IdElementField(field_uri="folder:DistinguishedFolderId", value_cls=DistinguishedFolderId)
+    _distinguished_id = IdElementField(
+        field_uri="folder:DistinguishedFolderId", value_cls=DistinguishedFolderId, supported_from=EXCHANGE_2016
+    )
     parent_folder_id = EWSElementField(field_uri="folder:ParentFolderId", value_cls=ParentFolderId, is_read_only=True)
     folder_class = CharField(field_uri="folder:FolderClass", is_required_after_save=True)
     name = CharField(field_uri="folder:DisplayName")
     total_count = IntegerField(field_uri="folder:TotalCount", is_read_only=True)
     child_folder_count = IntegerField(field_uri="folder:ChildFolderCount", is_read_only=True)
     unread_count = IntegerField(field_uri="folder:UnreadCount", is_read_only=True)
 
@@ -940,8 +942,12 @@
                 with suppress(KeyError):
                     folder_cls = cls.folder_cls_from_container_class(container_class=folder.folder_class)
                     log.debug(
                         "Folder class %s matches container class %s (%s)", folder_cls, folder.folder_class, folder.name
                     )
             if folder_cls == Folder:
                 log.debug("Fallback to class Folder (folder_class %s, name %s)", folder.folder_class, folder.name)
+        # Some servers return folders in a FindFolder result that have a DistinguishedFolderId element that the same
+        # server cannot handle in a GetFolder request. Only set the DistinguishedFolderId field if we recognize the ID.
+        if folder._distinguished_id and not folder_cls.DISTINGUISHED_FOLDER_ID:
+            folder._distinguished_id = None
         return folder_cls(root=root, **{f.name: getattr(folder, f.name) for f in folder.FIELDS})
```

### Comparing `exchangelib-5.3.0/exchangelib/folders/collections.py` & `exchangelib-5.4.0/exchangelib/folders/collections.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/folders/known_folders.py` & `exchangelib-5.4.0/exchangelib/folders/known_folders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from ..items import (
     ASSOCIATED,
+    CONTACT_ITEM_CLASSES,
     ITEM_CLASSES,
+    MESSAGE_ITEM_CLASSES,
+    TASK_ITEM_CLASSES,
     CalendarItem,
-    Contact,
-    DistributionList,
-    MeetingCancellation,
-    MeetingRequest,
-    MeetingResponse,
-    Message,
-    Task,
 )
 from ..properties import EWSMeta
-from ..version import EXCHANGE_2010_SP1, EXCHANGE_2013, EXCHANGE_2013_SP1
+from ..version import EXCHANGE_2010_SP1, EXCHANGE_2013, EXCHANGE_2013_SP1, EXCHANGE_O365
 from .base import Folder
 from .collections import FolderCollection
 
 
 class Birthdays(Folder):
     CONTAINER_CLASS = "IPF.Appointment.Birthday"
     LOCALIZED_NAMES = {
@@ -52,188 +48,36 @@
 
 class WellknownFolder(Folder, metaclass=EWSMeta):
     """Base class to use until we have a more specific folder implementation for this folder."""
 
     supported_item_models = ITEM_CLASSES
 
 
-class Messages(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Note"
-    supported_item_models = (Message, MeetingRequest, MeetingResponse, MeetingCancellation)
-
-
-class Calendar(WellknownFolder):
-    """An interface for the Exchange calendar."""
-
-    DISTINGUISHED_FOLDER_ID = "calendar"
-    CONTAINER_CLASS = "IPF.Appointment"
-    supported_item_models = (CalendarItem,)
-    LOCALIZED_NAMES = {
-        "da_DK": ("Kalender",),
-        "de_DE": ("Kalender",),
-        "en_US": ("Calendar",),
-        "es_ES": ("Calendario",),
-        "fr_CA": ("Calendrier",),
-        "nl_NL": ("Agenda",),
-        "ru_RU": ("Календарь",),
-        "sv_SE": ("Kalender",),
-        "zh_CN": ("日历",),
-    }
-
-    def view(self, *args, **kwargs):
-        return FolderCollection(account=self.account, folders=[self]).view(*args, **kwargs)
-
-
-class Contacts(WellknownFolder):
-    DISTINGUISHED_FOLDER_ID = "contacts"
-    CONTAINER_CLASS = "IPF.Contact"
-    supported_item_models = (Contact, DistributionList)
-    LOCALIZED_NAMES = {
-        "da_DK": ("Kontaktpersoner",),
-        "de_DE": ("Kontakte",),
-        "en_US": ("Contacts",),
-        "es_ES": ("Contactos",),
-        "fr_CA": ("Contacts",),
-        "nl_NL": ("Contactpersonen",),
-        "ru_RU": ("Контакты",),
-        "sv_SE": ("Kontakter",),
-        "zh_CN": ("联系人",),
-    }
-
-
-class DeletedItems(WellknownFolder):
-    DISTINGUISHED_FOLDER_ID = "deleteditems"
-    CONTAINER_CLASS = "IPF.Note"
-    supported_item_models = ITEM_CLASSES
-    LOCALIZED_NAMES = {
-        "da_DK": ("Slettet post",),
-        "de_DE": ("Gelöschte Elemente",),
-        "en_US": ("Deleted Items",),
-        "es_ES": ("Elementos eliminados",),
-        "fr_CA": ("Éléments supprimés",),
-        "nl_NL": ("Verwijderde items",),
-        "ru_RU": ("Удаленные",),
-        "sv_SE": ("Borttaget",),
-        "zh_CN": ("已删除邮件",),
-    }
-
-
-class Drafts(Messages):
-    DISTINGUISHED_FOLDER_ID = "drafts"
-    LOCALIZED_NAMES = {
-        "da_DK": ("Kladder",),
-        "de_DE": ("Entwürfe",),
-        "en_US": ("Drafts",),
-        "es_ES": ("Borradores",),
-        "fr_CA": ("Brouillons",),
-        "nl_NL": ("Concepten",),
-        "ru_RU": ("Черновики",),
-        "sv_SE": ("Utkast",),
-        "zh_CN": ("草稿",),
-    }
-
-
-class Inbox(Messages):
-    DISTINGUISHED_FOLDER_ID = "inbox"
-    LOCALIZED_NAMES = {
-        "da_DK": ("Indbakke",),
-        "de_DE": ("Posteingang",),
-        "en_US": ("Inbox",),
-        "es_ES": ("Bandeja de entrada",),
-        "fr_CA": ("Boîte de réception",),
-        "nl_NL": ("Postvak IN",),
-        "ru_RU": ("Входящие",),
-        "sv_SE": ("Inkorgen",),
-        "zh_CN": ("收件箱",),
-    }
-
-
-class JunkEmail(Messages):
-    DISTINGUISHED_FOLDER_ID = "junkemail"
-    LOCALIZED_NAMES = {
-        "da_DK": ("Uønsket e-mail",),
-        "de_DE": ("Junk-E-Mail",),
-        "en_US": ("Junk E-mail",),
-        "es_ES": ("Correo no deseado",),
-        "fr_CA": ("Courrier indésirables",),
-        "nl_NL": ("Ongewenste e-mail",),
-        "ru_RU": ("Нежелательная почта",),
-        "sv_SE": ("Skräppost",),
-        "zh_CN": ("垃圾邮件",),
-    }
-
-
-class Outbox(Messages):
-    DISTINGUISHED_FOLDER_ID = "outbox"
-    LOCALIZED_NAMES = {
-        "da_DK": ("Udbakke",),
-        "de_DE": ("Postausgang",),
-        "en_US": ("Outbox",),
-        "es_ES": ("Bandeja de salida",),
-        "fr_CA": ("Boîte d'envoi",),
-        "nl_NL": ("Postvak UIT",),
-        "ru_RU": ("Исходящие",),
-        "sv_SE": ("Utkorgen",),
-        "zh_CN": ("发件箱",),
-    }
-
-
-class SentItems(Messages):
-    DISTINGUISHED_FOLDER_ID = "sentitems"
-    LOCALIZED_NAMES = {
-        "da_DK": ("Sendt post",),
-        "de_DE": ("Gesendete Elemente",),
-        "en_US": ("Sent Items",),
-        "es_ES": ("Elementos enviados",),
-        "fr_CA": ("Éléments envoyés",),
-        "nl_NL": ("Verzonden items",),
-        "ru_RU": ("Отправленные",),
-        "sv_SE": ("Skickat",),
-        "zh_CN": ("已发送邮件",),
-    }
-
-
-class Tasks(WellknownFolder):
-    DISTINGUISHED_FOLDER_ID = "tasks"
-    CONTAINER_CLASS = "IPF.Task"
-    supported_item_models = (Task,)
-    LOCALIZED_NAMES = {
-        "da_DK": ("Opgaver",),
-        "de_DE": ("Aufgaben",),
-        "en_US": ("Tasks",),
-        "es_ES": ("Tareas",),
-        "fr_CA": ("Tâches",),
-        "nl_NL": ("Taken",),
-        "ru_RU": ("Задачи",),
-        "sv_SE": ("Uppgifter",),
-        "zh_CN": ("任务",),
-    }
-
-
 class AdminAuditLogs(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "adminauditlogs"
     supported_from = EXCHANGE_2013
     get_folder_allowed = False
 
 
+class AllCategorizedItems(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "allcategorizeditems"
+    CONTAINER_CLASS = "IPF.Note"
+    supported_from = EXCHANGE_O365
+
+
 class AllContacts(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "allcontacts"
     CONTAINER_CLASS = "IPF.Note"
 
 
 class AllItems(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "allitems"
     CONTAINER_CLASS = "IPF"
 
 
-class AllCategorizedItems(WellknownFolder):
-    DISTINGUISHED_FOLDER_ID = "allcategorizeditems"
-    CONTAINER_CLASS = "IPF.Note"
-
-
 class AllPersonMetadata(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "allpersonmetadata"
     CONTAINER_CLASS = "IPF.Note"
 
 
 class ArchiveDeletedItems(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "archivedeleteditems"
@@ -266,84 +110,197 @@
 
 
 class ArchiveRecoverableItemsVersions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "archiverecoverableitemsversions"
     supported_from = EXCHANGE_2010_SP1
 
 
+class Calendar(WellknownFolder):
+    """An interface for the Exchange calendar."""
+
+    DISTINGUISHED_FOLDER_ID = "calendar"
+    CONTAINER_CLASS = "IPF.Appointment"
+    supported_item_models = (CalendarItem,)
+    LOCALIZED_NAMES = {
+        "da_DK": ("Kalender",),
+        "de_DE": ("Kalender",),
+        "en_US": ("Calendar",),
+        "es_ES": ("Calendario",),
+        "fr_CA": ("Calendrier",),
+        "nl_NL": ("Agenda",),
+        "ru_RU": ("Календарь",),
+        "sv_SE": ("Kalender",),
+        "zh_CN": ("日历",),
+    }
+
+    def view(self, *args, **kwargs):
+        return FolderCollection(account=self.account, folders=[self]).view(*args, **kwargs)
+
+
 class Companies(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "companycontacts"
     CONTAINER_CLASS = "IPF.Contact.Company"
-    supported_item_models = (Contact, DistributionList)
+    supported_item_models = CONTACT_ITEM_CLASSES
     LOCALIZED_NAMES = {
         "da_DK": ("Firmaer",),
     }
 
 
 class Conflicts(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "conflicts"
     supported_from = EXCHANGE_2013
 
 
+class Contacts(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "contacts"
+    CONTAINER_CLASS = "IPF.Contact"
+    supported_item_models = CONTACT_ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Kontaktpersoner",),
+        "de_DE": ("Kontakte",),
+        "en_US": ("Contacts",),
+        "es_ES": ("Contactos",),
+        "fr_CA": ("Contacts",),
+        "nl_NL": ("Contactpersonen",),
+        "ru_RU": ("Контакты",),
+        "sv_SE": ("Kontakter",),
+        "zh_CN": ("联系人",),
+    }
+
+
 class ConversationHistory(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "conversationhistory"
     supported_from = EXCHANGE_2013
 
 
+class DeletedItems(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "deleteditems"
+    CONTAINER_CLASS = "IPF.Note"
+    supported_item_models = ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Slettet post",),
+        "de_DE": ("Gelöschte Elemente",),
+        "en_US": ("Deleted Items",),
+        "es_ES": ("Elementos eliminados",),
+        "fr_CA": ("Éléments supprimés",),
+        "nl_NL": ("Verwijderde items",),
+        "ru_RU": ("Удаленные",),
+        "sv_SE": ("Borttaget",),
+        "zh_CN": ("已删除邮件",),
+    }
+
+
 class Directory(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "directory"
     supported_from = EXCHANGE_2013_SP1
 
 
 class DlpPolicyEvaluation(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "dlppolicyevaluation"
     CONTAINER_CLASS = "IPF.StoreItem.DlpPolicyEvaluation"
+    supported_from = EXCHANGE_O365
 
 
-class Favorites(WellknownFolder):
+class Drafts(WellknownFolder):
     CONTAINER_CLASS = "IPF.Note"
+    DISTINGUISHED_FOLDER_ID = "drafts"
+    supported_item_models = MESSAGE_ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Kladder",),
+        "de_DE": ("Entwürfe",),
+        "en_US": ("Drafts",),
+        "es_ES": ("Borradores",),
+        "fr_CA": ("Brouillons",),
+        "nl_NL": ("Concepten",),
+        "ru_RU": ("Черновики",),
+        "sv_SE": ("Utkast",),
+        "zh_CN": ("草稿",),
+    }
+
+
+class Favorites(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "favorites"
+    CONTAINER_CLASS = "IPF.Note"
     supported_from = EXCHANGE_2013
 
 
 class FolderMemberships(Folder):
     CONTAINER_CLASS = "IPF.Task"
     LOCALIZED_NAMES = {
         None: ("Folder Memberships",),
     }
 
 
 class FromFavoriteSenders(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Note"
     DISTINGUISHED_FOLDER_ID = "fromfavoritesenders"
+    CONTAINER_CLASS = "IPF.Note"
     LOCALIZED_NAMES = {
         "da_DK": ("Personer jeg kender",),
     }
 
 
 class IMContactList(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Contact.MOC.ImContactList"
     DISTINGUISHED_FOLDER_ID = "imcontactlist"
+    CONTAINER_CLASS = "IPF.Contact.MOC.ImContactList"
     supported_from = EXCHANGE_2013
 
 
+class Inbox(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    DISTINGUISHED_FOLDER_ID = "inbox"
+    supported_item_models = MESSAGE_ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Indbakke",),
+        "de_DE": ("Posteingang",),
+        "en_US": ("Inbox",),
+        "es_ES": ("Bandeja de entrada",),
+        "fr_CA": ("Boîte de réception",),
+        "nl_NL": ("Postvak IN",),
+        "ru_RU": ("Входящие",),
+        "sv_SE": ("Inkorgen",),
+        "zh_CN": ("收件箱",),
+    }
+
+
 class Inference(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "inference"
 
 
 class Journal(WellknownFolder):
     CONTAINER_CLASS = "IPF.Journal"
     DISTINGUISHED_FOLDER_ID = "journal"
 
 
+class JunkEmail(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    DISTINGUISHED_FOLDER_ID = "junkemail"
+    supported_item_models = MESSAGE_ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Uønsket e-mail",),
+        "de_DE": ("Junk-E-Mail",),
+        "en_US": ("Junk E-mail",),
+        "es_ES": ("Correo no deseado",),
+        "fr_CA": ("Courrier indésirables",),
+        "nl_NL": ("Ongewenste e-mail",),
+        "ru_RU": ("Нежелательная почта",),
+        "sv_SE": ("Skräppost",),
+        "zh_CN": ("垃圾邮件",),
+    }
+
+
 class LocalFailures(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "localfailures"
     supported_from = EXCHANGE_2013
 
 
+class Messages(WellknownFolder):
+    CONTAINER_CLASS = "IPF.Note"
+    supported_item_models = MESSAGE_ITEM_CLASSES
+
+
 class MsgFolderRoot(WellknownFolder):
     """Also known as the 'Top of Information Store' folder."""
 
     DISTINGUISHED_FOLDER_ID = "msgfolderroot"
     LOCALIZED_NAMES = {
         None: ("Top of Information Store",),
         "da_DK": ("Informationslagerets øverste niveau",),
@@ -363,14 +320,30 @@
     LOCALIZED_NAMES = {
         "da_DK": ("Noter",),
     }
 
 
 class OneNotePagePreviews(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "onenotepagepreviews"
+    supported_from = EXCHANGE_O365
+
+
+class Outbox(Messages):
+    DISTINGUISHED_FOLDER_ID = "outbox"
+    LOCALIZED_NAMES = {
+        "da_DK": ("Udbakke",),
+        "de_DE": ("Postausgang",),
+        "en_US": ("Outbox",),
+        "es_ES": ("Bandeja de salida",),
+        "fr_CA": ("Boîte d'envoi",),
+        "nl_NL": ("Postvak UIT",),
+        "ru_RU": ("Исходящие",),
+        "sv_SE": ("Utkorgen",),
+        "zh_CN": ("发件箱",),
+    }
 
 
 class PeopleCentricConversationBuddies(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "peoplecentricconversationbuddies"
     CONTAINER_CLASS = "IPF.Contact.PeopleCentricConversationBuddies"
     LOCALIZED_NAMES = {
         None: ("PeopleCentricConversation Buddies",),
@@ -380,57 +353,57 @@
 class PeopleConnect(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "peopleconnect"
     supported_from = EXCHANGE_2013
 
 
 class QedcDefaultRetention(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "qedcdefaultretention"
+    supported_from = EXCHANGE_O365
 
 
 class QedcLongRetention(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "qedclongretention"
+    supported_from = EXCHANGE_O365
 
 
 class QedcMediumRetention(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "qedcmediumretention"
+    supported_from = EXCHANGE_O365
 
 
 class QedcShortRetention(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "qedcshortretention"
+    supported_from = EXCHANGE_O365
 
 
 class QuarantinedEmail(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "quarantinedemail"
+    supported_from = EXCHANGE_O365
 
 
 class QuarantinedEmailDefaultCategory(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "quarantinedemaildefaultcategory"
+    supported_from = EXCHANGE_O365
 
 
 class QuickContacts(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Contact.MOC.QuickContacts"
     DISTINGUISHED_FOLDER_ID = "quickcontacts"
+    CONTAINER_CLASS = "IPF.Contact.MOC.QuickContacts"
     supported_from = EXCHANGE_2013
 
 
 class RecipientCache(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recipientcache"
     CONTAINER_CLASS = "IPF.Contact.RecipientCache"
     supported_from = EXCHANGE_2013
-    LOCALIZED_NAMES = {
-        None: ("RecipientCache",),
-    }
 
 
 class RelevantContacts(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "relevantcontacts"
     CONTAINER_CLASS = "IPF.Note"
-    LOCALIZED_NAMES = {
-        None: ("RelevantContacts",),
-    }
 
 
 class RecoverableItemsDeletions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsdeletions"
     supported_from = EXCHANGE_2010_SP1
 
 
@@ -442,64 +415,98 @@
 class RecoverableItemsRoot(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsroot"
     supported_from = EXCHANGE_2010_SP1
 
 
 class RecoverableItemsSubstrateHolds(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemssubstrateholds"
-    supported_from = EXCHANGE_2010_SP1
+    supported_from = EXCHANGE_O365
     LOCALIZED_NAMES = {
         None: ("SubstrateHolds",),
     }
 
 
 class RecoverableItemsVersions(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "recoverableitemsversions"
     supported_from = EXCHANGE_2010_SP1
 
 
 class SearchFolders(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "searchfolders"
 
 
+class SentItems(Messages):
+    DISTINGUISHED_FOLDER_ID = "sentitems"
+    LOCALIZED_NAMES = {
+        "da_DK": ("Sendt post",),
+        "de_DE": ("Gesendete Elemente",),
+        "en_US": ("Sent Items",),
+        "es_ES": ("Elementos enviados",),
+        "fr_CA": ("Éléments envoyés",),
+        "nl_NL": ("Verzonden items",),
+        "ru_RU": ("Отправленные",),
+        "sv_SE": ("Skickat",),
+        "zh_CN": ("已发送邮件",),
+    }
+
+
 class ServerFailures(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "serverfailures"
     supported_from = EXCHANGE_2013
 
 
 class SharePointNotifications(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "sharepointnotifications"
 
 
 class ShortNotes(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "shortnotes"
+    supported_from = EXCHANGE_O365
 
 
 class SyncIssues(WellknownFolder):
     CONTAINER_CLASS = "IPF.Note"
     DISTINGUISHED_FOLDER_ID = "syncissues"
     supported_from = EXCHANGE_2013
 
 
+class Tasks(WellknownFolder):
+    DISTINGUISHED_FOLDER_ID = "tasks"
+    CONTAINER_CLASS = "IPF.Task"
+    supported_item_models = TASK_ITEM_CLASSES
+    LOCALIZED_NAMES = {
+        "da_DK": ("Opgaver",),
+        "de_DE": ("Aufgaben",),
+        "en_US": ("Tasks",),
+        "es_ES": ("Tareas",),
+        "fr_CA": ("Tâches",),
+        "nl_NL": ("Taken",),
+        "ru_RU": ("Задачи",),
+        "sv_SE": ("Uppgifter",),
+        "zh_CN": ("任务",),
+    }
+
+
 class TemporarySaves(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "temporarysaves"
 
 
 class ToDoSearch(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Task"
     DISTINGUISHED_FOLDER_ID = "todosearch"
+    CONTAINER_CLASS = "IPF.Task"
     supported_from = EXCHANGE_2013
     LOCALIZED_NAMES = {
         None: ("To-Do Search",),
     }
 
 
 class UserCuratedContacts(WellknownFolder):
-    CONTAINER_CLASS = "IPF.Note"
     DISTINGUISHED_FOLDER_ID = "usercuratedcontacts"
+    CONTAINER_CLASS = "IPF.Note"
+    supported_from = EXCHANGE_O365
 
 
 class VoiceMail(WellknownFolder):
     DISTINGUISHED_FOLDER_ID = "voicemail"
     CONTAINER_CLASS = "IPF.Note.Microsoft.Voicemail"
     LOCALIZED_NAMES = {
         None: ("Voice Mail",),
@@ -510,30 +517,17 @@
     """A mixin for non-wellknown folders than that are not deletable."""
 
     @property
     def is_deletable(self):
         return False
 
 
-class ExternalContacts(NonDeletableFolder):
-    DISTINGUISHED_FOLDER_ID = None
-    CONTAINER_CLASS = "IPF.Contact"
-    supported_item_models = (Contact, DistributionList)
-    LOCALIZED_NAMES = {
-        None: ("ExternalContacts",),
-    }
-
-
 class AllTodoTasks(NonDeletableFolder):
-    DISTINGUISHED_FOLDER_ID = None
     CONTAINER_CLASS = "IPF.Task"
-    supported_item_models = (Task,)
-    LOCALIZED_NAMES = {
-        None: ("AllTodoTasks",),
-    }
+    supported_item_models = TASK_ITEM_CLASSES
 
 
 class ApplicationData(NonDeletableFolder):
     CONTAINER_CLASS = "IPM.ApplicationData"
 
 
 class Audits(NonDeletableFolder):
@@ -542,14 +536,18 @@
 
 class CalendarLogging(NonDeletableFolder):
     LOCALIZED_NAMES = {
         None: ("Calendar Logging",),
     }
 
 
+class CalendarSearchCache(NonDeletableFolder):
+    CONTAINER_CLASS = "IPF.Appointment"
+
+
 class CommonViews(NonDeletableFolder):
     DEFAULT_ITEM_TRAVERSAL_DEPTH = ASSOCIATED
     LOCALIZED_NAMES = {
         None: ("Common Views",),
     }
 
 
@@ -570,14 +568,19 @@
     }
 
 
 class ExchangeSyncData(NonDeletableFolder):
     pass
 
 
+class ExternalContacts(NonDeletableFolder):
+    CONTAINER_CLASS = "IPF.Contact"
+    supported_item_models = CONTACT_ITEM_CLASSES
+
+
 class Files(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Files"
     LOCALIZED_NAMES = {
         "da_DK": ("Filer",),
     }
 
 
@@ -585,23 +588,23 @@
     LOCALIZED_NAMES = {
         None: ("Freebusy Data",),
     }
 
 
 class Friends(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note"
-    supported_item_models = (Contact, DistributionList)
+    supported_item_models = CONTACT_ITEM_CLASSES
     LOCALIZED_NAMES = {
         "de_DE": ("Bekannte",),
     }
 
 
 class GALContacts(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Contact.GalContacts"
-    supported_item_models = (Contact, DistributionList)
+    supported_item_models = CONTACT_ITEM_CLASSES
     LOCALIZED_NAMES = {
         None: ("GAL Contacts",),
     }
 
 
 class GraphAnalytics(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.GraphAnalytics"
@@ -613,20 +616,20 @@
 
 class MailboxAssociations(NonDeletableFolder):
     pass
 
 
 class MyContactsExtended(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Note"
-    supported_item_models = (Contact, DistributionList)
+    supported_item_models = CONTACT_ITEM_CLASSES
 
 
 class OrganizationalContacts(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.Contact.OrganizationalContacts"
-    supported_item_models = (Contact, DistributionList)
+    supported_item_models = CONTACT_ITEM_CLASSES
     LOCALIZED_NAMES = {
         None: ("Organizational Contacts",),
     }
 
 
 class ParkedMessages(NonDeletableFolder):
     CONTAINER_CLASS = None
@@ -635,14 +638,18 @@
 class PassThroughSearchResults(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.PassThroughSearchResults"
     LOCALIZED_NAMES = {
         None: ("Pass-Through Search Results",),
     }
 
 
+class PersonMetadata(NonDeletableFolder):
+    CONTAINER_CLASS = "IPF.Contact"
+
+
 class PdpProfileV2Secured(NonDeletableFolder):
     CONTAINER_CLASS = "IPF.StoreItem.PdpProfileSecured"
 
 
 class Reminders(NonDeletableFolder):
     CONTAINER_CLASS = "Outlook.Reminder"
     LOCALIZED_NAMES = {
@@ -700,38 +707,40 @@
         None: ("Working Set",),
     }
 
 
 # Folders that do not have a distinguished folder ID but return 'ErrorDeleteDistinguishedFolder' or
 # 'ErrorCannotDeleteObject' when we try to delete them. I can't find any official docs listing these folders.
 NON_DELETABLE_FOLDERS = [
-    ApplicationData,
     AllTodoTasks,
+    ApplicationData,
     Audits,
     CalendarLogging,
+    CalendarSearchCache,
     CommonViews,
     ConversationSettings,
     DefaultFoldersChangeHistory,
     DeferredAction,
     ExchangeSyncData,
     ExternalContacts,
-    FreebusyData,
     Files,
+    FreebusyData,
     Friends,
     GALContacts,
     GraphAnalytics,
     Location,
     MailboxAssociations,
     MyContactsExtended,
     OrganizationalContacts,
     ParkedMessages,
     PassThroughSearchResults,
     PdpProfileV2Secured,
-    Reminders,
+    PersonMetadata,
     RSSFeeds,
+    Reminders,
     Schedule,
     Sharing,
     Shortcuts,
     Signal,
     SmsAndChatsSync,
     SpoolerQueue,
     System,
@@ -755,16 +764,16 @@
     DeletedItems,
     Directory,
     DlpPolicyEvaluation,
     Drafts,
     Favorites,
     FromFavoriteSenders,
     IMContactList,
-    Inference,
     Inbox,
+    Inference,
     Journal,
     JunkEmail,
     LocalFailures,
     MsgFolderRoot,
     MyContacts,
     Notes,
     OneNotePagePreviews,
@@ -775,20 +784,20 @@
     QedcLongRetention,
     QedcMediumRetention,
     QedcShortRetention,
     QuarantinedEmail,
     QuarantinedEmailDefaultCategory,
     QuickContacts,
     RecipientCache,
-    RelevantContacts,
     RecoverableItemsDeletions,
     RecoverableItemsPurges,
     RecoverableItemsRoot,
     RecoverableItemsSubstrateHolds,
     RecoverableItemsVersions,
+    RelevantContacts,
     SearchFolders,
     SentItems,
     ServerFailures,
     SharePointNotifications,
     ShortNotes,
     SyncIssues,
     Tasks,
@@ -807,16 +816,16 @@
     ArchiveRecoverableItemsPurges,
     ArchiveRecoverableItemsRoot,
     ArchiveRecoverableItemsVersions,
 ]
 
 # Folders that do not have a distinguished ID but have their own container class
 MISC_FOLDERS = [
+    Birthdays,
     CrawlerData,
     EventCheckPoints,
     FolderMemberships,
     FreeBusyCache,
     RecoveryPoints,
-    SwssItems,
     SkypeTeamsMessages,
-    Birthdays,
+    SwssItems,
 ]
```

### Comparing `exchangelib-5.3.0/exchangelib/folders/queryset.py` & `exchangelib-5.4.0/exchangelib/folders/queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/folders/roots.py` & `exchangelib-5.4.0/exchangelib/folders/roots.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/indexed_properties.py` & `exchangelib-5.4.0/exchangelib/indexed_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/__init__.py` & `exchangelib-5.4.0/exchangelib/items/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,70 +72,76 @@
     MeetingMessage,
     MeetingRequest,
     MeetingResponse,
     MeetingCancellation,
     PostItem,
     Task,
 )
+TASK_ITEM_CLASSES = (Task,)
+CONTACT_ITEM_CLASSES = (Contact, DistributionList)
+MESSAGE_ITEM_CLASSES = (Message, MeetingRequest, MeetingResponse, MeetingCancellation)
 
 __all__ = [
-    "RegisterMixIn",
-    "MESSAGE_DISPOSITION_CHOICES",
-    "SAVE_ONLY",
-    "SEND_ONLY",
-    "SEND_AND_SAVE_COPY",
-    "CalendarItem",
-    "AcceptItem",
-    "TentativelyAcceptItem",
-    "DeclineItem",
-    "CancelCalendarItem",
-    "MeetingRequest",
-    "MeetingResponse",
-    "MeetingCancellation",
-    "CONFERENCE_TYPES",
-    "Contact",
-    "Persona",
-    "DistributionList",
-    "SEND_MEETING_INVITATIONS_CHOICES",
-    "SEND_TO_NONE",
-    "SEND_ONLY_TO_ALL",
-    "SEND_TO_ALL_AND_SAVE_COPY",
-    "SEND_MEETING_INVITATIONS_AND_CANCELLATIONS_CHOICES",
-    "SEND_ONLY_TO_CHANGED",
-    "SEND_TO_CHANGED_AND_SAVE_COPY",
-    "SEND_MEETING_CANCELLATIONS_CHOICES",
+    "ACTIVE_DIRECTORY",
+    "ACTIVE_DIRECTORY_CONTACTS",
     "AFFECTED_TASK_OCCURRENCES_CHOICES",
     "ALL_OCCURRENCES",
-    "SPECIFIED_OCCURRENCE_ONLY",
-    "CONFLICT_RESOLUTION_CHOICES",
-    "NEVER_OVERWRITE",
-    "AUTO_RESOLVE",
+    "ALL_PROPERTIES",
     "ALWAYS_OVERWRITE",
+    "ASSOCIATED",
+    "AUTO_RESOLVE",
+    "AcceptItem",
+    "BaseItem",
+    "BulkCreateResult",
+    "CONFERENCE_TYPES",
+    "CONFLICT_RESOLUTION_CHOICES",
+    "CONTACT_ITEM_CLASSES",
+    "CONTACTS",
+    "CONTACTS_ACTIVE_DIRECTORY",
+    "CalendarItem",
+    "CancelCalendarItem",
+    "Contact",
+    "DEFAULT",
     "DELETE_TYPE_CHOICES",
+    "DeclineItem",
+    "DistributionList",
+    "ForwardItem",
     "HARD_DELETE",
-    "SOFT_DELETE",
-    "MOVE_TO_DELETED_ITEMS",
-    "BaseItem",
+    "ID_ONLY",
+    "ITEM_CLASSES",
+    "ITEM_TRAVERSAL_CHOICES",
     "Item",
-    "BulkCreateResult",
+    "MESSAGE_DISPOSITION_CHOICES",
+    "MESSAGE_ITEM_CLASSES",
+    "MOVE_TO_DELETED_ITEMS",
+    "TASK_ITEM_CLASSES",
+    "MeetingCancellation",
+    "MeetingRequest",
+    "MeetingResponse",
     "Message",
-    "ReplyToItem",
-    "ReplyAllToItem",
-    "ForwardItem",
+    "NEVER_OVERWRITE",
+    "Persona",
     "PostItem",
     "PostReplyItem",
-    "Task",
-    "ITEM_TRAVERSAL_CHOICES",
+    "RegisterMixIn",
+    "ReplyAllToItem",
+    "ReplyToItem",
+    "SAVE_ONLY",
+    "SEARCH_SCOPE_CHOICES",
+    "SEND_AND_SAVE_COPY",
+    "SEND_MEETING_CANCELLATIONS_CHOICES",
+    "SEND_MEETING_INVITATIONS_AND_CANCELLATIONS_CHOICES",
+    "SEND_MEETING_INVITATIONS_CHOICES",
+    "SEND_ONLY",
+    "SEND_ONLY_TO_ALL",
+    "SEND_ONLY_TO_CHANGED",
+    "SEND_TO_ALL_AND_SAVE_COPY",
+    "SEND_TO_CHANGED_AND_SAVE_COPY",
+    "SEND_TO_NONE",
     "SHALLOW",
-    "SOFT_DELETED",
-    "ASSOCIATED",
     "SHAPE_CHOICES",
-    "ID_ONLY",
-    "DEFAULT",
-    "ALL_PROPERTIES",
-    "SEARCH_SCOPE_CHOICES",
-    "ACTIVE_DIRECTORY",
-    "ACTIVE_DIRECTORY_CONTACTS",
-    "CONTACTS",
-    "CONTACTS_ACTIVE_DIRECTORY",
-    "ITEM_CLASSES",
+    "SOFT_DELETE",
+    "SOFT_DELETED",
+    "SPECIFIED_OCCURRENCE_ONLY",
+    "Task",
+    "TentativelyAcceptItem",
 ]
```

### Comparing `exchangelib-5.3.0/exchangelib/items/base.py` & `exchangelib-5.4.0/exchangelib/items/base.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/calendar_item.py` & `exchangelib-5.4.0/exchangelib/items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/contact.py` & `exchangelib-5.4.0/exchangelib/items/contact.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/item.py` & `exchangelib-5.4.0/exchangelib/items/item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/message.py` & `exchangelib-5.4.0/exchangelib/items/message.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/post.py` & `exchangelib-5.4.0/exchangelib/items/post.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/items/task.py` & `exchangelib-5.4.0/exchangelib/items/task.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/properties.py` & `exchangelib-5.4.0/exchangelib/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -2298,16 +2298,21 @@
             self.account.create_rule(self)
         else:
             self.account.set_rule(self)
         return self
 
     def delete(self):
         if self.is_enabled is False:
-            # Cannot delete a disabled rule - server throws 'ErrorItemNotFound'
+            # Cannot delete a disabled rule - the server throws 'ErrorItemNotFound'. We need to enable it first.
             self.is_enabled = True
+            # Make sure we can save the rule by wiping all possibly-misconfigured fields
+            self.priority = 10**6
+            self.conditions = None
+            self.exceptions = None
+            self.actions = Actions(stop_processing_rules=True)
             self.save()
         self.account.delete_rule(self)
 
 
 class InboxRules(EWSElement):
     """MSDN: https://docs.microsoft.com/en-us/exchange/client-developer/web-service-reference/inboxrules"""
```

### Comparing `exchangelib-5.3.0/exchangelib/protocol.py` & `exchangelib-5.4.0/exchangelib/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/queryset.py` & `exchangelib-5.4.0/exchangelib/queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/recurrence.py` & `exchangelib-5.4.0/exchangelib/recurrence.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/restriction.py` & `exchangelib-5.4.0/exchangelib/restriction.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/__init__.py` & `exchangelib-5.4.0/exchangelib/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,31 +60,34 @@
 
 __all__ = [
     "ArchiveItem",
     "ConvertId",
     "CopyItem",
     "CreateAttachment",
     "CreateFolder",
+    "CreateInboxRule",
     "CreateItem",
     "CreateUserConfiguration",
     "DeleteAttachment",
     "DeleteFolder",
-    "DeleteUserConfiguration",
+    "DeleteInboxRule",
     "DeleteItem",
-    "EmptyFolder",
+    "DeleteUserConfiguration",
     "EWSService",
+    "EmptyFolder",
     "ExpandDL",
     "ExportItems",
     "FindFolder",
     "FindItem",
     "FindPeople",
     "GetAttachment",
     "GetDelegate",
     "GetEvents",
     "GetFolder",
+    "GetInboxRules",
     "GetItem",
     "GetMailTips",
     "GetPersona",
     "GetRoomLists",
     "GetRooms",
     "GetSearchableMailboxes",
     "GetServerTimeZones",
@@ -95,23 +98,20 @@
     "GetUserSettings",
     "MarkAsJunk",
     "MoveFolder",
     "MoveItem",
     "ResolveNames",
     "SendItem",
     "SendNotification",
+    "SetInboxRule",
     "SetUserOofSettings",
     "SubscribeToPull",
     "SubscribeToPush",
     "SubscribeToStreaming",
     "SyncFolderHierarchy",
     "SyncFolderItems",
     "Unsubscribe",
     "UpdateFolder",
     "UpdateItem",
     "UpdateUserConfiguration",
     "UploadItems",
-    "GetInboxRules",
-    "CreateInboxRule",
-    "SetInboxRule",
-    "DeleteInboxRule",
 ]
```

### Comparing `exchangelib-5.3.0/exchangelib/services/archive_item.py` & `exchangelib-5.4.0/exchangelib/services/archive_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/common.py` & `exchangelib-5.4.0/exchangelib/services/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,11 +967,16 @@
 
 def attachment_ids_element(items, version, tag="m:AttachmentIds"):
     return _ids_element(items, AttachmentId, version, tag)
 
 
 def parse_folder_elem(elem, folder):
     if isinstance(folder, RootOfHierarchy):
-        return folder.from_xml(elem=elem, account=folder.account)
-    if isinstance(folder, Folder):
-        return folder.from_xml_with_root(elem=elem, root=folder.root)
-    raise ValueError(f"Unsupported folder class: {folder}")
+        res = folder.from_xml(elem=elem, account=folder.account)
+    elif isinstance(folder, Folder):
+        res = folder.from_xml_with_root(elem=elem, root=folder.root)
+    else:
+        raise ValueError(f"Unsupported folder class: {folder}")
+    # Not all servers support fetching the DistinguishedFolderId field. Add it back here.
+    if folder._distinguished_id and not res._distinguished_id:
+        res._distinguished_id = folder._distinguished_id
+    return res
```

### Comparing `exchangelib-5.3.0/exchangelib/services/convert_id.py` & `exchangelib-5.4.0/exchangelib/services/convert_id.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/create_attachment.py` & `exchangelib-5.4.0/exchangelib/services/create_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/create_folder.py` & `exchangelib-5.4.0/exchangelib/services/create_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/create_item.py` & `exchangelib-5.4.0/exchangelib/services/create_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/create_user_configuration.py` & `exchangelib-5.4.0/exchangelib/services/create_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/delete_attachment.py` & `exchangelib-5.4.0/exchangelib/services/delete_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/delete_folder.py` & `exchangelib-5.4.0/exchangelib/services/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/delete_item.py` & `exchangelib-5.4.0/exchangelib/services/delete_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/delete_user_configuration.py` & `exchangelib-5.4.0/exchangelib/services/delete_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/empty_folder.py` & `exchangelib-5.4.0/exchangelib/services/empty_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/expand_dl.py` & `exchangelib-5.4.0/exchangelib/services/expand_dl.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/export_items.py` & `exchangelib-5.4.0/exchangelib/services/export_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/find_folder.py` & `exchangelib-5.4.0/exchangelib/services/find_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/find_item.py` & `exchangelib-5.4.0/exchangelib/services/find_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/find_people.py` & `exchangelib-5.4.0/exchangelib/services/find_people.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_attachment.py` & `exchangelib-5.4.0/exchangelib/services/get_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_delegate.py` & `exchangelib-5.4.0/exchangelib/services/get_delegate.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_events.py` & `exchangelib-5.4.0/exchangelib/services/get_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_folder.py` & `exchangelib-5.4.0/exchangelib/services/get_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_item.py` & `exchangelib-5.4.0/exchangelib/services/get_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_mail_tips.py` & `exchangelib-5.4.0/exchangelib/services/get_mail_tips.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_persona.py` & `exchangelib-5.4.0/exchangelib/services/get_persona.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_room_lists.py` & `exchangelib-5.4.0/exchangelib/services/get_room_lists.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_rooms.py` & `exchangelib-5.4.0/exchangelib/services/get_rooms.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_searchable_mailboxes.py` & `exchangelib-5.4.0/exchangelib/services/get_searchable_mailboxes.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_server_time_zones.py` & `exchangelib-5.4.0/exchangelib/services/get_server_time_zones.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_streaming_events.py` & `exchangelib-5.4.0/exchangelib/services/get_streaming_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_user_availability.py` & `exchangelib-5.4.0/exchangelib/services/get_user_availability.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_user_configuration.py` & `exchangelib-5.4.0/exchangelib/services/get_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_user_oof_settings.py` & `exchangelib-5.4.0/exchangelib/services/get_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/get_user_settings.py` & `exchangelib-5.4.0/exchangelib/services/get_user_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/inbox_rules.py` & `exchangelib-5.4.0/exchangelib/services/inbox_rules.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/mark_as_junk.py` & `exchangelib-5.4.0/exchangelib/services/mark_as_junk.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/move_folder.py` & `exchangelib-5.4.0/exchangelib/services/move_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/move_item.py` & `exchangelib-5.4.0/exchangelib/services/move_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/resolve_names.py` & `exchangelib-5.4.0/exchangelib/services/resolve_names.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/send_item.py` & `exchangelib-5.4.0/exchangelib/services/send_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/send_notification.py` & `exchangelib-5.4.0/exchangelib/services/send_notification.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/set_user_oof_settings.py` & `exchangelib-5.4.0/exchangelib/services/set_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/subscribe.py` & `exchangelib-5.4.0/exchangelib/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/sync_folder_hierarchy.py` & `exchangelib-5.4.0/exchangelib/services/sync_folder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/sync_folder_items.py` & `exchangelib-5.4.0/exchangelib/services/sync_folder_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/unsubscribe.py` & `exchangelib-5.4.0/exchangelib/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/update_folder.py` & `exchangelib-5.4.0/exchangelib/services/update_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/update_item.py` & `exchangelib-5.4.0/exchangelib/services/update_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/update_user_configuration.py` & `exchangelib-5.4.0/exchangelib/services/update_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/services/upload_items.py` & `exchangelib-5.4.0/exchangelib/services/upload_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/settings.py` & `exchangelib-5.4.0/exchangelib/settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/transport.py` & `exchangelib-5.4.0/exchangelib/transport.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/util.py` & `exchangelib-5.4.0/exchangelib/util.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/version.py` & `exchangelib-5.4.0/exchangelib/version.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib/winzone.py` & `exchangelib-5.4.0/exchangelib/winzone.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/exchangelib.egg-info/PKG-INFO` & `exchangelib-5.4.0/exchangelib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.3.0
+Version: 5.4.0
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Author-email: Erik Cederstrand <erik@cederstrand.dk>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/ecederstrand/exchangelib
 Project-URL: Issues, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
 Project-URL: Repository, https://github.com/ecederstrand/exchangelib.git
@@ -28,18 +28,21 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests_ntlm>=0.2.0
 Requires-Dist: requests_oauthlib
 Requires-Dist: tzdata
 Requires-Dist: tzlocal
 Provides-Extra: kerberos
 Requires-Dist: requests_gssapi; extra == "kerberos"
+Provides-Extra: msal
+Requires-Dist: msal; extra == "msal"
 Provides-Extra: sspi
 Requires-Dist: requests_negotiate_sspi; extra == "sspi"
 Provides-Extra: complete
 Requires-Dist: requests_gssapi; extra == "complete"
+Requires-Dist: msal; extra == "complete"
 Requires-Dist: requests_negotiate_sspi; extra == "complete"
 
 Exchange Web Services client library
 ====================================
 
 This module is an ORM for your Exchange mailbox, providing Django-style access to all your data. It is a
 platform-independent, well-performing, well-behaving, well-documented, well-tested and simple interface for
```

### Comparing `exchangelib-5.3.0/exchangelib.egg-info/SOURCES.txt` & `exchangelib-5.4.0/exchangelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchangelib-5.3.0/pyproject.toml` & `exchangelib-5.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Release notes:
-# *  Install pdoc3, wheel, twine
+# *  Install pdoc3, wheel, twine, build
 # * Bump version in exchangelib/__init__.py
 # * Bump version in CHANGELOG.md
 # * Generate documentation:
-#     rm -r docs/exchangelib && pdoc3 --html exchangelib -o docs --force && git add docs && pre-commit run end-of-file-fixer
+#     rm -r docs/exchangelib && pdoc3 --html exchangelib -o docs --force  && git add docs && pre-commit run end-of-file-fixer || git add docs
 # * Commit and push changes
 # * Build package:
 #     rm -rf build dist exchangelib.egg-info && python -m build
 # * Push to PyPI:
 #     twine upload dist/*
 # * Create release on GitHub
 
@@ -58,16 +58,17 @@
 Issues = "https://github.com/ecederstrand/exchangelib/issues"
 Documentation = "https://ecederstrand.github.io/exchangelib/"
 Repository = "https://github.com/ecederstrand/exchangelib.git"
 Changelog = "https://github.com/ecederstrand/exchangelib/blob/master/CHANGELOG.md"
 
 [project.optional-dependencies]
 kerberos = ["requests_gssapi"]
+msal = ["msal"]
 sspi = ["requests_negotiate_sspi"]
-complete = ["requests_gssapi", "requests_negotiate_sspi"]
+complete = ["requests_gssapi", "msal", "requests_negotiate_sspi"]
 
 [tool.setuptools.dynamic]
 version = {attr = "exchangelib.__version__"}
 
 [bdist_wheel]
 universal = 1
```


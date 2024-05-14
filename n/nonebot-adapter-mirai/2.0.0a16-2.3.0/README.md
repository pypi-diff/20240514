# Comparing `tmp/nonebot-adapter-mirai-2.0.0a16.tar.gz` & `tmp/nonebot_adapter_mirai-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-adapter-mirai-2.0.0a16.tar", max compression
+gzip compressed data, was "nonebot_adapter_mirai-2.3.0.tar", last modified: Tue May 14 16:55:11 2024, max compression
```

## Comparing `nonebot-adapter-mirai-2.0.0a16.tar` & `nonebot_adapter_mirai-2.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0    34523 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/LICENSE
--rw-r--r--   0        0        0      298 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/README.md
--rw-r--r--   0        0        0      915 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/__init__.py
--rw-r--r--   0        0        0    24340 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/bot.py
--rw-r--r--   0        0        0      639 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/config.py
--rw-r--r--   0        0        0     1322 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/__init__.py
--rw-r--r--   0        0        0     4066 2021-10-02 16:34:15.496918 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/base.py
--rw-r--r--   0        0        0     2008 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/message.py
--rw-r--r--   0        0        0      498 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/meta.py
--rw-r--r--   0        0        0     3636 2021-10-02 16:34:15.496918 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/notice.py
--rw-r--r--   0        0        0     5729 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/event/request.py
--rw-r--r--   0        0        0     8273 2021-10-02 16:34:15.496918 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/message.py
--rw-r--r--   0        0        0     5354 2021-09-23 03:27:32.091699 nonebot-adapter-mirai-2.0.0a16/nonebot/adapters/mirai/utils.py
--rw-r--r--   0        0        0     1130 2021-10-02 18:03:04.029416 nonebot-adapter-mirai-2.0.0a16/pyproject.toml
--rw-r--r--   0        0        0     1045 2021-10-02 18:05:26.163890 nonebot-adapter-mirai-2.0.0a16/setup.py
--rw-r--r--   0        0        0     1257 2021-10-02 18:05:26.164117 nonebot-adapter-mirai-2.0.0a16/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1300 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/README.md
+-rw-r--r--   0        0        0      244 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/__init__.py
+-rw-r--r--   0        0        0    11812 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/adapter.py
+-rw-r--r--   0        0        0    55508 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/bot.py
+-rw-r--r--   0        0        0     1463 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/compat.py
+-rw-r--r--   0        0        0      923 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/config.py
+-rw-r--r--   0        0        0    30053 2024-05-14 16:54:46.947192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/event.py
+-rw-r--r--   0        0        0     3117 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/exception.py
+-rw-r--r--   0        0        0    19490 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/message.py
+-rw-r--r--   0        0        0      601 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/base.py
+-rw-r--r--   0        0        0     2762 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/common.py
+-rw-r--r--   0        0        0     8816 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/model/relationship.py
+-rw-r--r--   0        0        0     2559 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/nonebot/adapters/mirai/utils.py
+-rw-r--r--   0        0        0     2263 2024-05-14 16:55:11.223346 nonebot_adapter_mirai-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 16:54:46.951192 nonebot_adapter_mirai-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 nonebot_adapter_mirai-2.3.0/PKG-INFO
```

### Comparing `nonebot-adapter-mirai-2.0.0a16/LICENSE` & `nonebot_adapter_mirai-2.3.0/LICENSE`

 * *Files identical despite different names*


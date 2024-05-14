# Comparing `tmp/nonebot-plugin-overbracket-0.1.2.tar.gz` & `tmp/nonebot_plugin_overbracket-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-overbracket-0.1.2.tar", last modified: Mon Jun 19 08:06:31 2023, max compression
+gzip compressed data, was "nonebot_plugin_overbracket-0.2.0.tar", last modified: Tue May 14 10:52:53 2024, max compression
```

## Comparing `nonebot-plugin-overbracket-0.1.2.tar` & `nonebot_plugin_overbracket-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:06:31.983712 nonebot-plugin-overbracket-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 08:06:21.000000 nonebot-plugin-overbracket-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-19 08:06:31.983712 nonebot-plugin-overbracket-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-19 08:06:21.000000 nonebot-plugin-overbracket-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:06:31.983712 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-19 08:06:21.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-19 08:06:21.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:06:31.983712 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-19 08:06:31.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-19 08:06:31.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:06:31.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:06:31.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 08:06:31.000000 nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-19 08:06:21.000000 nonebot-plugin-overbracket-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:06:31.983712 nonebot-plugin-overbracket-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:52:53.116793 nonebot_plugin_overbracket-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 10:52:47.000000 nonebot_plugin_overbracket-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 10:52:53.116793 nonebot_plugin_overbracket-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-14 10:52:47.000000 nonebot_plugin_overbracket-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:52:53.116793 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 10:52:47.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 10:52:47.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:52:53.116793 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 10:52:53.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 10:52:53.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:52:53.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 10:52:53.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 10:52:53.000000 nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 10:52:47.000000 nonebot_plugin_overbracket-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:52:53.116793 nonebot_plugin_overbracket-0.2.0/setup.cfg
```

### Comparing `nonebot-plugin-overbracket-0.1.2/LICENSE` & `nonebot_plugin_overbracket-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-overbracket-0.1.2/PKG-INFO` & `nonebot_plugin_overbracket-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-overbracket
-Version: 0.1.2
+Version: 0.2.0
 Summary: NoneBot2 插件 通括膨胀——泛滥的括号
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-overbracket
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-overbracket
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-overbracket
 
 _✨ 通括膨胀——泛滥的括号 ✨_
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.2.0 Summary:
 NoneBot2 æä»¶ éæ¬è¨èââæ³æ»¥çæ¬å· Author-email: HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-overbracket Project-URL: Repository, https://github.com/NCBM/nonebot-
 plugin-overbracket Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE
+markdown License-File: LICENSE Requires-Dist: nonebot2>=2.2.0
    # nonebot-plugin-overbracket _â¨ éæ¬è¨èââæ³æ»¥çæ¬å· â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» è®©ä½ çæºå¨äººéæºåæ¬å·ã ## ð¿ å®è£ éè¿ `nb-
 cli`: ```console nb plugin install nonebot-plugin-overbracket ``` ## âï¸
 éç½® æ¬æä»¶å¢å äºä¸åå¯ééç½®é¡¹ï¼æéè¦çç¨æ·è¯·èªè¡å¨
 `.env` ä¸­éç½®ï¼ ```python # ä¸åéç½®é¡¹è¯·æéè§£é¤æ³¨éå¹¶éç½® #
 æ¬éç½®æä»¶ä¸­çæææ¦çåå¨ 0~1 ä¹é´ #
```

### Comparing `nonebot-plugin-overbracket-0.1.2/README.md` & `nonebot_plugin_overbracket-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket/__init__.py` & `nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 import random
-from nonebot import on_message, get_driver, __version__ as nbver
+
+from nonebot import get_plugin_config, on_message
 from nonebot.adapters import Event
 from nonebot.plugin import PluginMetadata
-from .config import Config
 
-_extra_meta_source = {
-    "type": "application",
-    "homepage": "https://github.com/NCBM/nonebot-plugin-overbracket"
-}
-
-if (
-    not nbver
-    or not nbver.startswith("2.0.0")
-    or not (_suf := nbver[5:])
-    or _suf[0] not in "abr"
-    or (_suf.startswith("rc") and int(_suf[2:]) > 4)
-):
-    _extra_meta = _extra_meta_source
-else:
-    _extra_meta = {"extra": _extra_meta_source}
+from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     name="通括膨胀",
     description="让你的机器人随机发括号",
     usage="[请查阅插件介绍文档]",
-    config=Config,
-    **_extra_meta
+    type="application",
+    homepage="https://github.com/NCBM/nonebot-plugin-overbracket",
+    config=Config
 )
 
-global_config = get_driver().config
-parsed_config = Config.parse_obj(global_config)
+parsed_config = get_plugin_config(Config)
 
 obr = on_message(priority=25, block=False)
 
 
 @obr.handle()
 async def make_lbracket(event: Event):
     msg = event.get_message().extract_plain_text()
```

### Comparing `nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket/config.py` & `nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
 
 
-class Config(BaseModel, extra=Extra.ignore):
+class Config(BaseModel, extra="ignore"):
     """Plugin Config Here"""
 
     overbracket_base_chance: float = 0.12
     """收到任意消息时发送括号的概率"""
 
     overbracket_purpose_chance: float = 0.42
     """收到末尾带括号消息时发送括号的概率"""
```

### Comparing `nonebot-plugin-overbracket-0.1.2/nonebot_plugin_overbracket.egg-info/PKG-INFO` & `nonebot_plugin_overbracket-0.2.0/nonebot_plugin_overbracket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-overbracket
-Version: 0.1.2
+Version: 0.2.0
 Summary: NoneBot2 插件 通括膨胀——泛滥的括号
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-overbracket
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-overbracket
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-overbracket
 
 _✨ 通括膨胀——泛滥的括号 ✨_
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.2.0 Summary:
 NoneBot2 æä»¶ éæ¬è¨èââæ³æ»¥çæ¬å· Author-email: HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-overbracket Project-URL: Repository, https://github.com/NCBM/nonebot-
 plugin-overbracket Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE
+markdown License-File: LICENSE Requires-Dist: nonebot2>=2.2.0
    # nonebot-plugin-overbracket _â¨ éæ¬è¨èââæ³æ»¥çæ¬å· â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» è®©ä½ çæºå¨äººéæºåæ¬å·ã ## ð¿ å®è£ éè¿ `nb-
 cli`: ```console nb plugin install nonebot-plugin-overbracket ``` ## âï¸
 éç½® æ¬æä»¶å¢å äºä¸åå¯ééç½®é¡¹ï¼æéè¦çç¨æ·è¯·èªè¡å¨
 `.env` ä¸­éç½®ï¼ ```python # ä¸åéç½®é¡¹è¯·æéè§£é¤æ³¨éå¹¶éç½® #
 æ¬éç½®æä»¶ä¸­çæææ¦çåå¨ 0~1 ä¹é´ #
```


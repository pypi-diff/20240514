# Comparing `tmp/nonebot-plugin-mixin-0.1.2.tar.gz` & `tmp/nonebot_plugin_mixin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mixin-0.1.2.tar", last modified: Mon Jun 19 08:05:10 2023, max compression
+gzip compressed data, was "nonebot_plugin_mixin-0.2.0.tar", last modified: Tue May 14 10:32:28 2024, max compression
```

## Comparing `nonebot-plugin-mixin-0.1.2.tar` & `nonebot_plugin_mixin-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.389717 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.389717 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:28.462506 nonebot_plugin_mixin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 10:32:22.000000 nonebot_plugin_mixin-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-14 10:32:28.462506 nonebot_plugin_mixin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-14 10:32:22.000000 nonebot_plugin_mixin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:28.462506 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-14 10:32:22.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-14 10:32:22.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:32:28.462506 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-14 10:32:28.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-14 10:32:28.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:32:28.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 10:32:28.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 10:32:28.000000 nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 10:32:22.000000 nonebot_plugin_mixin-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:32:28.462506 nonebot_plugin_mixin-0.2.0/setup.cfg
```

### Comparing `nonebot-plugin-mixin-0.1.2/LICENSE` & `nonebot_plugin_mixin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mixin-0.1.2/PKG-INFO` & `nonebot_plugin_mixin-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.2
+Version: 0.2.0
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-mixin
 
 _✨ 通过代码或非代码方式外部介入 NoneBot2 插件行为 ✨_
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.2.0 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE
+File: LICENSE Requires-Dist: nonebot2>=2.2.0
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
                    æä»¶è¡ä¸º â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» æ¬æä»¶åè®¸éè¿ä»£ç /éä»£ç æ¹å¼ä»å¥æä»¶åé¨
 Matcher çè¡ä¸ºã ## ð¿ å®è£ éè¿ `nb-cli`: ```console nb plugin
 install nonebot-plugin-mixin ``` ## âï¸ éç½®
 æ¬æä»¶å¢å äºä¸åå¯ééç½®é¡¹ï¼æéè¦çç¨æ·è¯·èªè¡å¨ `.env`
 ä¸­éç½®ï¼ ```python # ä¸åéç½®é¡¹è¯·æéè§£é¤æ³¨éå¹¶éç½® # Mixin
```

### Comparing `nonebot-plugin-mixin-0.1.2/README.md` & `nonebot_plugin_mixin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/__init__.py` & `nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 """
 通过 mixin 调整特定 Matcher 的行为
 
 注意：本插件并不保证更改会被稳定应用，部分插件可能会在运行时修改自身部分行为。
 """
 
-from functools import partial, reduce
 import json
+from functools import partial, reduce
 from operator import and_
 from pathlib import Path
 from typing import Any, Iterable, List, Optional, Tuple, Type, Union
-from nonebot import get_driver, logger, __version__ as nbver
+
+from nonebot import get_driver, get_plugin_config, logger
 from nonebot.internal.matcher import Matcher, matchers
 from nonebot.internal.rule import Rule
+from nonebot.plugin import PluginMetadata
 from nonebot.rule import (
-    StartswithRule, EndswithRule, FullmatchRule,
-    KeywordsRule, CommandRule, RegexRule, ToMeRule,
-    command
+    CommandRule,
+    EndswithRule,
+    FullmatchRule,
+    KeywordsRule,
+    RegexRule,
+    StartswithRule,
+    ToMeRule,
+    command,
 )
-from nonebot.plugin import PluginMetadata
 from pydantic import BaseModel, Field
 
 from .config import Config
 
-global_config = get_driver().config
-config_ = Config.parse_obj(global_config)
-
-_extra_meta_source = {
-    "type": "library",
-    "homepage": "https://github.com/NCBM/nonebot-plugin-mixin"
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
+config_ = get_plugin_config(Config)
 
 __plugin_meta__ = PluginMetadata(
     name="Mixin",
     description="通过代码或非代码方式外部介入 NoneBot2 插件行为",
     usage="[请查阅插件介绍文档]",
-    config=Config,
-    **_extra_meta
+    type="library",
+    homepage="https://github.com/NCBM/nonebot-plugin-mixin",
+    config=Config
 )
 
 driver = get_driver()
 
 
 class CaseMatch(BaseModel):
     msg: Tuple[str, ...]
@@ -132,23 +122,23 @@
                     )
                 ):
                     rule.checkers.add(sub)
                     continue
                 tmp.append(sub.call)
         for loc, obj in complex_rules:
             if loc is not None:
-                rule &= obj(**loc.dict())
+                rule &= obj(**loc.model_dump())
             else:
-                rule: Rule = reduce(
+                rule = reduce(
                     and_, filter(lambda x: isinstance(x, obj), tmp), rule
                 )
         if self.keywords is not None:
             rule &= KeywordsRule(*self.keywords)
         else:
-            rule: Rule = reduce(
+            rule = reduce(
                 and_, filter(lambda x: isinstance(x, KeywordsRule), tmp), rule
             )
         if self.command is not None:
             rule &= command(*self.command)
         else:
             rule: Rule = reduce(
                 and_, filter(lambda x: isinstance(x, CommandRule), tmp), rule
@@ -258,15 +248,15 @@
         else:
             logger.warning(f"尚未支持 {fp!r} 的数据格式")
     return
 
 
 def parse_mixin(*rules: Any):
     for r in rules:
-        mixins.append(Mixin.parse_obj(r))
+        mixins.append(Mixin.model_validate(r))
 
 
 @driver.on_startup
 async def load_mixin_files():
     for obj in read_mixin(*config_.mixin_source):
         parse_mixin(*obj)
     multi_mixin()
```

### Comparing `nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/PKG-INFO` & `nonebot_plugin_mixin-0.2.0/nonebot_plugin_mixin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.2
+Version: 0.2.0
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-mixin
 
 _✨ 通过代码或非代码方式外部介入 NoneBot2 插件行为 ✨_
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.2.0 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE
+File: LICENSE Requires-Dist: nonebot2>=2.2.0
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
                    æä»¶è¡ä¸º â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» æ¬æä»¶åè®¸éè¿ä»£ç /éä»£ç æ¹å¼ä»å¥æä»¶åé¨
 Matcher çè¡ä¸ºã ## ð¿ å®è£ éè¿ `nb-cli`: ```console nb plugin
 install nonebot-plugin-mixin ``` ## âï¸ éç½®
 æ¬æä»¶å¢å äºä¸åå¯ééç½®é¡¹ï¼æéè¦çç¨æ·è¯·èªè¡å¨ `.env`
 ä¸­éç½®ï¼ ```python # ä¸åéç½®é¡¹è¯·æéè§£é¤æ³¨éå¹¶éç½® # Mixin
```


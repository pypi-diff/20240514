# Comparing `tmp/nonebot-plugin-tempfile-0.1.0.tar.gz` & `tmp/nonebot_plugin_tempfile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-tempfile-0.1.0.tar", last modified: Fri Jul 21 08:40:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_tempfile-0.2.0.tar", last modified: Tue May 14 10:44:33 2024, max compression
```

## Comparing `nonebot-plugin-tempfile-0.1.0.tar` & `nonebot_plugin_tempfile-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:39.203451 nonebot-plugin-tempfile-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-21 08:40:28.000000 nonebot-plugin-tempfile-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-21 08:40:39.203451 nonebot-plugin-tempfile-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 08:40:28.000000 nonebot-plugin-tempfile-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:39.203451 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-21 08:40:28.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 08:40:28.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:39.203451 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-21 08:40:39.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 08:40:39.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:40:39.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:40:39.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 08:40:39.000000 nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-21 08:40:28.000000 nonebot-plugin-tempfile-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:40:39.203451 nonebot-plugin-tempfile-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:44:33.786068 nonebot_plugin_tempfile-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 10:44:28.000000 nonebot_plugin_tempfile-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 10:44:33.786068 nonebot_plugin_tempfile-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-14 10:44:28.000000 nonebot_plugin_tempfile-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:44:33.786068 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-14 10:44:28.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 10:44:28.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:44:33.786068 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 10:44:33.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 10:44:33.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:44:33.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 10:44:33.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 10:44:33.000000 nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 10:44:28.000000 nonebot_plugin_tempfile-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:44:33.786068 nonebot_plugin_tempfile-0.2.0/setup.cfg
```

### Comparing `nonebot-plugin-tempfile-0.1.0/LICENSE` & `nonebot_plugin_tempfile-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-tempfile-0.1.0/PKG-INFO` & `nonebot_plugin_tempfile-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tempfile
-Version: 0.1.0
+Version: 0.2.0
 Summary: 适用于 NoneBot2 插件的临时文件/IO 依赖注入支持
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-tempfile
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-tempfile
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-tempfile
 
 _✨ 适用于 NoneBot2 插件的临时文件/IO 依赖注入支持 ✨_
```

### Comparing `nonebot-plugin-tempfile-0.1.0/README.md` & `nonebot_plugin_tempfile-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile/__init__.py` & `nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+import os
 from functools import wraps
 from io import BytesIO, StringIO
-import os
 from pathlib import Path
-from tempfile import TemporaryDirectory as _TemporaryDirectory, mkstemp
+from tempfile import TemporaryDirectory as _TemporaryDirectory
+from tempfile import mkstemp
 from typing import Callable, Generator, Optional, TypeVar
-from typing_extensions import Annotated, ParamSpec
 
-from nonebot import get_driver, logger
+from nonebot import get_plugin_config, logger
 from nonebot.params import Depends
 from nonebot.plugin import PluginMetadata
+from typing_extensions import Annotated, ParamSpec
 
 from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     "方寸狭间",
     "临时文件/IO 依赖注入支持",
     "[详见插件主页]",
     "library",
     "https://github.com/NCBM/nonebot-plugin-tempfile",
     Config
 )
 
-_config = Config.parse_obj(get_driver().config)
+_config = get_plugin_config(Config)
 
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 
 
 def TempDir(
     suffix: str = "",
```

### Comparing `nonebot-plugin-tempfile-0.1.0/nonebot_plugin_tempfile.egg-info/PKG-INFO` & `nonebot_plugin_tempfile-0.2.0/nonebot_plugin_tempfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tempfile
-Version: 0.1.0
+Version: 0.2.0
 Summary: 适用于 NoneBot2 插件的临时文件/IO 依赖注入支持
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-tempfile
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-tempfile
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2>=2.2.0
 
 <div align="center">
 
 # nonebot-plugin-tempfile
 
 _✨ 适用于 NoneBot2 插件的临时文件/IO 依赖注入支持 ✨_
```


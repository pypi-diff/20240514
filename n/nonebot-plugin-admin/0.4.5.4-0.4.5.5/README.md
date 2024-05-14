# Comparing `tmp/nonebot-plugin-admin-0.4.5.4.tar.gz` & `tmp/nonebot_plugin_admin-0.4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-admin-0.4.5.4.tar", last modified: Thu Feb 29 03:41:11 2024, max compression
+gzip compressed data, was "nonebot_plugin_admin-0.4.5.5.tar", last modified: Tue May 14 20:39:54 2024, max compression
```

## Comparing `nonebot-plugin-admin-0.4.5.4.tar` & `nonebot_plugin_admin-0.4.5.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 03:41:11.300491 nonebot-plugin-admin-0.4.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-29 03:41:11.300491 nonebot-plugin-admin-0.4.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 03:41:11.300491 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/admin_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/approve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/auto_ban.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/auto_ban_.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/func_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/img_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/kick_member_by_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/notice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/particular_e_notice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/request_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/switcher.html
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/switcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/word_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/wordcloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 03:41:11.300491 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-29 03:41:11.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-29 03:41:11.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 03:41:11.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 03:41:11.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-29 03:41:11.000000 nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 03:41:11.300491 nonebot-plugin-admin-0.4.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-29 03:41:00.000000 nonebot-plugin-admin-0.4.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:54.142583 nonebot_plugin_admin-0.4.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-05-14 20:39:54.142583 nonebot_plugin_admin-0.4.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:54.142583 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/approve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/auto_ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/auto_ban_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/func_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/img_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/kick_member_by_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/particular_e_notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/request_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/switcher.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/switcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/word_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/wordcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:54.142583 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-05-14 20:39:54.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 20:39:54.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:39:54.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 20:39:54.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 20:39:54.000000 nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:39:54.142583 nonebot_plugin_admin-0.4.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 20:39:47.000000 nonebot_plugin_admin-0.4.5.5/setup.py
```

### Comparing `nonebot-plugin-admin-0.4.5.4/LICENSE` & `nonebot_plugin_admin-0.4.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/PKG-INFO` & `nonebot_plugin_admin-0.4.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-admin
-Version: 0.4.5.4
+Version: 0.4.5.5
 Summary: nonebot2 plugin for group administration
 Home-page: https://github.com/yzyyz1387/nonebot_plugin_admin
 Author: yzyyz1387
 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,admin,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-admin Version: 0.4.5.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-admin Version: 0.4.5.5 Summary:
 nonebot2 plugin for group administration Home-page: https://github.com/
 yzyyz1387/nonebot_plugin_admin Author: yzyyz1387 Author-email:
 youzyyz1384@qq.com Keywords: pip,nonebot2,nonebot,admin,nonebot_plugin
 Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 or later
 (AGPLv3+) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: fuzzyfinder Requires-
```

### Comparing `nonebot-plugin-admin-0.4.5.4/README.md` & `nonebot_plugin_admin-0.4.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/__init__.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/admin.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/admin.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/admin_role.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/admin_role.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/approve.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/approve.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/auto_ban.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/auto_ban.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/auto_ban_.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/auto_ban_.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/broadcast.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/broadcast.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/config.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # from typing import Optional
 from nonebot import get_driver
 from pydantic import BaseModel, Extra
-
+from nonebot import get_plugin_config
 
 class Config(BaseModel, extra=Extra.ignore):
     tenid: str = 'xxxxxx'  # 腾讯云图片安全，开通地址： https://console.cloud.tencent.com/cms
     tenkeys: str = 'xxxxxx'  # 文档： https://cloud.tencent.com/document/product/1125
     callback_notice: bool = True  # 是否在操作完成后在 QQ 返回提示
     ban_rand_time_min: int = 60  # 随机禁言最短时间(s) default: 1分钟
     ban_rand_time_max: int = 2591999  # 随机禁言最长时间(s) default: 30天: 60*60*24*30
 
 
 driver = get_driver()
 global_config = driver.config
-plugin_config = Config.parse_obj(global_config)
+# plugin_config = Config.parse_obj(global_config)
+plugin_config = get_plugin_config(Config)
```

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/func_hook.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/func_hook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_msg.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_msg.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_recall.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_recall.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/group_request_verify.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/group_request_verify.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/img_check.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/img_check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/kick_member_by_rule.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/kick_member_by_rule.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/notice.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/particular_e_notice.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/particular_e_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/path.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/path.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/request_manual.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/request_manual.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/requests.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/requests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/switcher.html` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/switcher.html`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/switcher.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/switcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/utils.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/word_analyze.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/word_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin/wordcloud.py` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/PKG-INFO` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-admin
-Version: 0.4.5.4
+Version: 0.4.5.5
 Summary: nonebot2 plugin for group administration
 Home-page: https://github.com/yzyyz1387/nonebot_plugin_admin
 Author: yzyyz1387
 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,admin,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-admin Version: 0.4.5.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-admin Version: 0.4.5.5 Summary:
 nonebot2 plugin for group administration Home-page: https://github.com/
 yzyyz1387/nonebot_plugin_admin Author: yzyyz1387 Author-email:
 youzyyz1384@qq.com Keywords: pip,nonebot2,nonebot,admin,nonebot_plugin
 Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 or later
 (AGPLv3+) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: fuzzyfinder Requires-
```

### Comparing `nonebot-plugin-admin-0.4.5.4/nonebot_plugin_admin.egg-info/SOURCES.txt` & `nonebot_plugin_admin-0.4.5.5/nonebot_plugin_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-admin-0.4.5.4/setup.py` & `nonebot_plugin_admin-0.4.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-admin",
-    version="0.4.5.4",
+    version="0.4.5.5",
     author="yzyyz1387",
     author_email="youzyyz1384@qq.com",
     keywords=("pip", "nonebot2", "nonebot", "admin", "nonebot_plugin"),
     description="""nonebot2 plugin for group administration""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yzyyz1387/nonebot_plugin_admin",
```


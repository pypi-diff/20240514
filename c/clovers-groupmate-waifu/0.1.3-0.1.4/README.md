# Comparing `tmp/clovers_groupmate_waifu-0.1.3.tar.gz` & `tmp/clovers_groupmate_waifu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_groupmate_waifu-0.1.3.tar", max compression
+gzip compressed data, was "clovers_groupmate_waifu-0.1.4.tar", max compression
```

## Comparing `clovers_groupmate_waifu-0.1.3.tar` & `clovers_groupmate_waifu-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    15054 2024-04-28 09:06:20.918901 clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/clovers.py
--rw-r--r--   0        0        0     2642 2024-04-27 15:28:58.471177 clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/config.py
--rw-r--r--   0        0        0     1973 2024-04-28 09:06:20.919901 clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/data.py
--rw-r--r--   0        0        0      627 2024-04-27 15:12:59.042886 clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/utils.py
--rw-r--r--   0        0        0     1086 2024-04-27 15:12:59.040886 clovers_groupmate_waifu-0.1.3/LICENSE
--rw-r--r--   0        0        0      389 2024-04-28 09:21:04.973556 clovers_groupmate_waifu-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4818 2024-04-27 15:59:04.794098 clovers_groupmate_waifu-0.1.3/README.md
--rw-r--r--   0        0        0     5019 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    15531 2024-05-14 02:07:03.135249 clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/clovers.py
+-rw-r--r--   0        0        0     2642 2024-04-27 15:28:58.471177 clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/config.py
+-rw-r--r--   0        0        0     1973 2024-04-28 09:06:20.919901 clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/data.py
+-rw-r--r--   0        0        0      627 2024-04-27 15:12:59.042886 clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/utils.py
+-rw-r--r--   0        0        0     1086 2024-04-27 15:12:59.040886 clovers_groupmate_waifu-0.1.4/LICENSE
+-rw-r--r--   0        0        0      390 2024-05-14 02:08:09.437866 clovers_groupmate_waifu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4818 2024-04-27 15:59:04.794098 clovers_groupmate_waifu-0.1.4/README.md
+-rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.4/PKG-INFO
```

### Comparing `clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/__init__.py` & `clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,26 +63,24 @@
 async def _(event: Event):
     if event.permission != 3:
         return
     reset_data()
     return "娶群友记录已重置"
 
 
-@plugin.handle({"设置娶群友保护"}, {"permission", "nickname", "user_id", "at"}, {"group_member_list"})
+@plugin.handle({"设置娶群友保护"}, {"permission", "user_id", "at"})
 async def _(event: Event):
     if not event.at:
         protect_uids.add(event.user_id)
-        namelist = event.nickname
     elif event.permission != 3:
         return "保护失败。你无法为其他人设置保护。"
     else:
         waifu_data.protect_uids = protect_uids | set(event.at)
-        namelist = "\n".join(user.nickname for user in await event.group_member_list())
     waifu_data.save(waifu_data_file)
-    return f"保护成功！\n保护名单为：\n{namelist}"
+    return "保护成功！"
 
 
 @plugin.handle({"解除娶群友保护"}, {"permission", "nickname", "user_id", "at"})
 async def _(event: Event):
     if not event.at:
         if event.user_id in protect_uids:
             protect_uids.remove(event.user_id)
@@ -150,72 +148,79 @@
     record_couple = group_record.record_couple
     record_lock = group_record.record_lock
     couple_id = record_couple.get(user_id)
     if couple_id == user_id:
         return [Result("at", user_id), f"{random.choice(bad_end_tips)}\n你没有娶到群友。"]
     if event.at:
         waifu_id = event.at[0]
-        if couple_id:
+        if couple_id:  # 判断自己是否有 CP
             waifu = user_data[couple_id]
-            if couple_id == waifu_id:
+            if couple_id == waifu_id:  # 如果 at 到自己的 CP
                 tips = random.choice(happy_end_tips) + "\n你的CP："
                 record_lock[user_id] = couple_id
                 waifu_data.save(waifu_data_file)
-            elif user_id not in record_lock and random.randint(1, 100) <= waifu_he:
+            elif user_id not in record_lock and random.randint(1, 100) <= waifu_he:  # 如果自己未主动锁定对方
                 if couple_id in record_lock:
                     del record_lock[couple_id]
                 del record_couple[couple_id]
                 waifu_data.update_nickname(await event.group_member_list(), group_id)
                 waifu = user_data[waifu_id]
                 avatar = await download_url(waifu.avatar)
                 record_lock[user_id] = waifu_id
                 record_couple[user_id] = waifu_id
                 record_couple[waifu_id] = user_id
                 waifu_data.save(waifu_data_file)
                 tips = "恭喜你娶到了群友！"
             else:
                 tips = "你已经有CP了，不许花心哦~\n你的CP："
             tips += waifu.group_nickname(group_id)
-        elif waifu_id in waifu_data.protect_uids:
+        elif waifu_id in waifu_data.protect_uids:  # 如果对方在保护列表
             return
-        elif waifus_waifu_id := record_couple.get(waifu_id):
-            waifu = user_data[waifus_waifu_id]
-            tips = f"ta已经名花有主了~\nta的CP：{waifu.group_nickname(group_id)}"
-            if not locked_check(record_lock, waifus_waifu_id, waifu_id):
-                randvalue = random.randint(1, 100)
-                if randvalue <= waifu_ntr:
-                    waifu = user_data[waifu_id]
-                    tips += f"\n但是...\n恭喜你抢到了群友{waifu.group_nickname(group_id)}"
-                    if waifus_waifu_id in record_lock:
-                        del record_lock[waifus_waifu_id]
-                    del record_couple[waifus_waifu_id]
-                    record_lock[user_id] = waifu_id
-                    record_couple[user_id] = waifu_id
-                    record_couple[waifu_id] = user_id
-                    waifu_data.save(waifu_data_file)
-                elif randvalue <= waifu_ntr_be:
-                    record_couple[user_id] = user_id
-                    waifu_data.save(waifu_data_file)
-                    if user_id in user_data:
-                        waifu = user_data[user_id]
-                    else:
-                        waifu = user_data[user_id] = User(user_id=user_id, nickname=event.nickname, card="", avatar=event.avatar)
-                    tips += "不过好消息是...\n你娶到了你自己！"
+        elif waifus_waifu_id := record_couple.get(waifu_id):  # 如果对方有 CP 记录
+            if waifus_waifu_id == waifu_id:  # 判断是否对方被锁定单身
+                record_lock[user_id] = waifu_id
+                record_couple[user_id] = waifu_id
+                record_couple[waifu_id] = user_id
+                waifu_data.save(waifu_data_file)
+                tips = "恭喜你娶到了群友！"
+            else:
+                tips = f"ta已经名花有主了~\nta的CP：{waifu.group_nickname(group_id)}"
+                waifu = user_data[waifus_waifu_id]
+                if not locked_check(record_lock, waifus_waifu_id, waifu_id):  # 判断对方 CP 是否无锁定
+                    randvalue = random.randint(1, 100)  # ntr及 BE 检定
+                    if randvalue <= waifu_ntr:
+                        waifu = user_data[waifu_id]
+                        tips += f"\n但是...\n恭喜你抢到了群友{waifu.group_nickname(group_id)}"
+                        if waifus_waifu_id in record_lock:
+                            del record_lock[waifus_waifu_id]
+                        del record_couple[waifus_waifu_id]
+                        record_lock[user_id] = waifu_id
+                        record_couple[user_id] = waifu_id
+                        record_couple[waifu_id] = user_id
+                        waifu_data.save(waifu_data_file)
+                    elif randvalue <= waifu_ntr_be:
+                        record_couple[user_id] = user_id
+                        waifu_data.save(waifu_data_file)
+                        if user_id in user_data:
+                            waifu = user_data[user_id]
+                        else:
+                            waifu = user_data[user_id] = User(user_id=user_id, nickname=event.nickname, card="", avatar=event.avatar)
+                        tips += "不过好消息是...\n你娶到了你自己！"
         else:
             randvalue = random.randint(1, 100)
             waifu_data.update_nickname(await event.group_member_list(), group_id)
             if randvalue <= waifu_he:
                 waifu = user_data[waifu_id]
                 avatar = await download_url(waifu.avatar)
                 record_lock[user_id] = waifu_id
                 record_couple[user_id] = waifu_id
                 record_couple[waifu_id] = user_id
                 waifu_data.save(waifu_data_file)
                 tips = f"恭喜你娶到了群友：{waifu.group_nickname(group_id)}"
-            elif randvalue <= waifu_be:
+            elif randvalue <= waifu_be:  # 锁定单身
                 record_couple[user_id] = user_id
                 waifu = user_data[user_id]
                 waifu_data.save(waifu_data_file)
                 tips = f"{random.choice(bad_end_tips)}\n恭喜你娶到了你自己。"
             else:
                 return [Result("at", user_id), f"{random.choice(bad_end_tips)}\n你没有娶到群友。"]
     else:
```

### Comparing `clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/clovers.py` & `clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/config.py` & `clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/config.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/data.py` & `clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/data.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/clovers_groupmate_waifu/utils.py` & `clovers_groupmate_waifu-0.1.4/clovers_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/LICENSE` & `clovers_groupmate_waifu-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/README.md` & `clovers_groupmate_waifu-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.3/PKG-INFO` & `clovers_groupmate_waifu-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: clovers-groupmate-waifu
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: clovers-apscheduler (>=0.1.4,<0.2.0)
-Requires-Dist: clovers[linecard,tools] (>=0.1.8,<0.2.0)
+Requires-Dist: clovers[linecard,tools] (>=0.1.10,<0.2.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # clovers-groupmate-waifu
 
 _✨ 娶群友 ✨_
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.4 Summary:
 Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
 apscheduler (>=0.1.4,<0.2.0) Requires-Dist: clovers[linecard,tools]
-(>=0.1.8,<0.2.0) Description-Content-Type: text/markdown
+(>=0.1.10,<0.2.0) Description-Content-Type: text/markdown
    # clovers-groupmate-waifu _â¨ å¨¶ç¾¤å â¨_[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i
                                    _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```bash pip install clovers_groupmate_waifu ``` ## âï¸ éç½®
 å¨ clovers éç½®æä»¶åæéæ·»å ä¸é¢çéç½®é¡¹ ```toml
 [clovers_groupmate_waifu] # é»è®¤æ¾ç¤ºå­ä½ fontname = "simsun" #
 é»è®¤å¤ç¨å­ä½ fallback_fonts = [ "Arial", "Tahoma", "Microsoft YaHei",
 "Segoe UI", "Segoe UI Emoji", "Segoe UI Symbol", "Helvetica Neue", "PingFang
```


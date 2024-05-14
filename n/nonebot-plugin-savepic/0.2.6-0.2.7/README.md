# Comparing `tmp/nonebot_plugin_savepic-0.2.6.tar.gz` & `tmp/nonebot_plugin_savepic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_savepic-0.2.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_savepic-0.2.7.tar", max compression
```

## Comparing `nonebot_plugin_savepic-0.2.6.tar` & `nonebot_plugin_savepic-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1060 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/LICENSE
--rw-r--r--   0        0        0     2770 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/README.md
--rw-r--r--   0        0        0    10921 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/__init__.py
--rw-r--r--   0        0        0     1726 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/ai_utils.py
--rw-r--r--   0        0        0      850 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/config.py
--rw-r--r--   0        0        0      786 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/countpic.py
--rw-r--r--   0        0        0      662 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/error.py
--rw-r--r--   0        0        0      906 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/ext_listener.py
--rw-r--r--   0        0        0     3868 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/model.py
--rw-r--r--   0        0        0     4259 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/mvpic.py
--rw-r--r--   0        0        0        0 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/networks/__init__.py
--rw-r--r--   0        0        0     8015 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/networks/resnet_big.py
--rw-r--r--   0        0        0    13267 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/pic_sql.py
--rw-r--r--   0        0        0     2250 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/picture.py
--rw-r--r--   0        0        0     1391 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/randpic.py
--rw-r--r--   0        0        0     1471 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/rule.py
--rw-r--r--   0        0        0      691 2024-05-11 11:39:49.436268 nonebot_plugin_savepic-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2770 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/README.md
+-rw-r--r--   0        0        0    10921 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/__init__.py
+-rw-r--r--   0        0        0     1726 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/ai_utils.py
+-rw-r--r--   0        0        0      952 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/config.py
+-rw-r--r--   0        0        0      786 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/countpic.py
+-rw-r--r--   0        0        0      662 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/error.py
+-rw-r--r--   0        0        0      906 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/ext_listener.py
+-rw-r--r--   0        0        0     3868 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/model.py
+-rw-r--r--   0        0        0     4522 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/mvpic.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/networks/__init__.py
+-rw-r--r--   0        0        0     8015 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/networks/resnet_big.py
+-rw-r--r--   0        0        0    13182 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/pic_sql.py
+-rw-r--r--   0        0        0     2250 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/picture.py
+-rw-r--r--   0        0        0     1391 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/randpic.py
+-rw-r--r--   0        0        0     1471 2024-05-14 04:54:37.957213 nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/rule.py
+-rw-r--r--   0        0        0      691 2024-05-14 04:54:37.961213 nonebot_plugin_savepic-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_savepic-0.2.6/LICENSE` & `nonebot_plugin_savepic-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/README.md` & `nonebot_plugin_savepic-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/__init__.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/ai_utils.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/ai_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/config.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,7 +29,10 @@
 
     p_model_path: str = "networks/ckpt_epoch_100_rein.pth"
     q_model_path: str = "networks/ckpt_epoch_100_rein.pth.qt.pth"
     # 基于模型的相似度判断
 
     embedding_sqlurl: str
     black_group: list[str]
+
+    notfound_with_jpg: bool = True
+    """ randpic 的时候，尝试带 .jpg 再度检索向量 """
```

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/countpic.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/countpic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/error.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/ext_listener.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/ext_listener.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/model.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/mvpic.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/mvpic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import re
 from nonebot import on_command
+from nonebot.params import CommandArg
 from nonebot.internal.adapter import Bot
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent as V11GME
 from .rule import BLACK_GROUP
 from .rule import PIC_AMDIN
 from .rule import GROUP_ADMIN
 from .config import WORDS
 from .pic_sql import rename
@@ -22,24 +23,21 @@
 # mvpic -g -l name
 # mvpic -gl name
 # mvpic -lg name
 # mvpic name name
 
 
 @s_mvpic.handle()
-async def _(
-    bot: Bot,
-    event: V11GME,
-):
+async def _(bot: Bot, event: V11GME, args=CommandArg()):
     if not (await PIC_AMDIN(bot, event) or await GROUP_ADMIN(bot, event)):
         await s_mvpic.finish(
             random.choice(WORDS.get("permission denied", ["没有权限"]))
         )
 
-    cmd = event.message.extract_plain_text().strip()
+    cmd = args.extract_plain_text().strip()
     name = []
     options = []
 
     def parser():
         pos = 0
         nonlocal cmd, name, options
 
@@ -100,15 +98,14 @@
             elif cmd[pos] == '"':
                 name.append(_str('"'))
             else:
                 pos -= 1
                 name.append(_str(""))
 
     parser()
-
     if not name:
         await s_mvpic.finish("文件名呢？")
     if not options:
         options = ["l"]
 
     if (not await PIC_AMDIN(bot, event)) and await GROUP_ADMIN(bot, event):
         if "g" in options:
@@ -120,16 +117,20 @@
         sname = sname.replace(c, "-")
         dname = dname.replace(c, "-")
     if not sname.endswith((".jpg", ".png", ".gif")):
         sname += ".jpg"
     if not dname.endswith((".jpg", ".png", ".gif")):
         dname += ".jpg"
 
-    sg = options[0]
-    dg = options[1] if len(options) > 1 else sg
+    sg = "globe" if options[0] == "g" else f"qq_group:{event.group_id}"
+    dg = options[1] if len(options) > 1 else options[0]
+    dg = "globe" if dg == "g" else f"qq_group:{event.group_id}"
+
+    if sname == dname and sg == dg:
+        await s_mvpic.finish("嗯，什么都没有变化嘛。")
 
     try:
         await rename(sname, dname, sg, dg)
     except NoPictureException as ex:
         await s_mvpic.finish(
             random.choice(WORDS.get("not found", [ex.name + " 没有找到哦"]))
             + f"\n{ex.name} 没有找到哦"
```

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/networks/resnet_big.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/networks/resnet_big.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/pic_sql.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/pic_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,22 +26,39 @@
 
 def AsyncDatabase():
     if not _async_database:
         raise RuntimeError("Database is not initialized")
     return _async_database
 
 
+async def update_vec(pic: PicData):
+    if pic is None:
+        return
+    if not pic.u_vec_text:
+        return
+
+    async with AsyncSession(_async_database) as db_session:
+        if pic.u_vec_text:
+            pic.u_vec_text = False
+            await _async_embedding_database.execute(
+                "UPDATE savepic_word2vec SET embedding = $1 WHERE id = $2",
+                str(word2vec(pic.name)),
+                pic.id,
+            )
+        db_session.merge(pic)
+        db_session.commit()
+
+
 async def select_pic(filename: str, group: str):
     async with AsyncSession(_async_database) as db_session:
-        pic = await db_session.scalar(
+        if pic := await db_session.scalar(
             select(PicData)
             .where(PicData.name == filename)
             .where(PicData.group == group)
-        )
-        if pic:
+        ):
             await update_vec(pic)
             return pic
         return await db_session.scalar(
             select(PicData)
             .where(PicData.name == filename)
             .where(PicData.group == "globe")
         )
@@ -93,36 +110,22 @@
             select(PicData)
             .where(PicData.name == filename)
             .where(PicData.group == group_id)
         )
         if despic:
             raise SameNameException(despic.name)
 
-        # if not collision_allow:
-        #     ret = _pincone_index.query(img_vec, top_k=25)["matches"]
-        #     for i in ret:
-        #         if i["score"] and i["score"] < 0.98:
-        #             break
-        #         despic = await db_session.scalar(
-        #             select(PicData)
-        #             .where(PicData.id == int(ret[0]["id"]))
-        #             .where(sa.or_(PicData.group == group_id, PicData.group == "globe"))
-        #         )
-        #         if despic:
-        #             raise SimilarPictureException(despic.name, i["score"], despic.url)
-
         empty = await db_session.scalar(select(PicData).where(PicData.name == ""))
         if empty:
             pic.id = empty.id
             await db_session.merge(pic)
         else:
             db_session.add(pic)
         await db_session.flush()
 
-        # _pincone_index.upsert([(str(pic.id), img_vec)])
         await _async_embedding_database.execute(
             (
                 "INSERT INTO savepic_word2vec (id, embedding) VALUES ($1, $2) "
                 "ON CONFLICT (id) DO UPDATE SET embedding = $2"
             ),
             pic.id,
             str(word2vec(filename)),
@@ -141,17 +144,17 @@
             raise NoPictureException(ori)
 
         despic = await db_session.scalar(
             select(PicData).where(PicData.name == des).where(PicData.group == d_group)
         )
         if despic:
             raise SameNameException(despic.name)
+
         pic.name = des
         pic.group = d_group
-
         pic.u_vec_text = False
         await _async_embedding_database.execute(
             "UPDATE savepic_word2vec SET embedding = $1 WHERE id = $2",
             str(word2vec(des)),
             pic.id,
         )
         await db_session.merge(pic)
@@ -214,14 +217,15 @@
             select(PicData)
             .where(sa.or_(PicData.group == group, PicData.group == "globe"))
             .where(PicData.name.ilike(f"%{name}%"))
             .order_by(sa.func.random())
         ):
             await update_vec(pic)
             return pic, ""
+
         if not vector:
             return None, ""
 
         datas = await _async_embedding_database.fetch(
             (
                 "SELECT id FROM savepic_word2vec "
                 "WHERE embedding IS NOT NULL and embedding <=> $1 <= 0.45 "
@@ -233,14 +237,33 @@
             select(PicData)
             .where(sa.or_(PicData.group == group, PicData.group == "globe"))
             .where(PicData.id.in_([i["id"] for i in datas]))
             .where(PicData.name != "")
             .order_by(sa.func.random())
         ):
             return pic, "（语义向量相似度检索）"
+
+        if p_config.notfound_with_jpg:
+            datas = await _async_embedding_database.fetch(
+                (
+                    "SELECT id FROM savepic_word2vec "
+                    "WHERE embedding IS NOT NULL and embedding <=> $1 <= 0.45 "
+                    "ORDER BY embedding <#> $1 LIMIT 8;"
+                ),
+                str(word2vec(name + ".jpg")),
+            )
+            if pic := await db_session.scalar(
+                select(PicData)
+                .where(sa.or_(PicData.group == group, PicData.group == "globe"))
+                .where(PicData.id.in_([i["id"] for i in datas]))
+                .where(PicData.name != "")
+                .order_by(sa.func.random())
+            ):
+                return pic, "（语义向量相似度检索）"
+
         return None, False
 
 
 async def countpic(reg: str, group: str = "globe") -> int:
     reg = reg.strip()
     if not reg:
         reg = ".*"
@@ -254,37 +277,14 @@
             )
         )
         if pics:
             return pics
         return 0
 
 
-async def update_vec(pic: PicData):
-    if not pic:
-        return
-    if not pic.u_vec_text:  # and not pic.u_vec_img:
-        return
-    if pic.u_vec_text:
-        pic.u_vec_text = False
-        await _async_embedding_database.execute(
-            "UPDATE savepic_word2vec SET embedding = $1 WHERE id = $2",
-            str(word2vec(pic.name)),
-            pic.id,
-        )
-    # if pic.u_vec_img:
-    #     pic.u_vec_img = False
-    #     _pincone_index.upsert(
-    #         [(str(pic.id), file2vec(pathlib.Path(pic.url), pic.name))]
-    #     )
-    async with AsyncSession(_async_database) as db_session:
-        db_session.merge(pic)
-        await db_session.flush()
-        db_session.commit()
-
-
 async def listpic(reg: str, group: str = "globe", pages: int = 0) -> list[str]:
     reg = reg.strip()
     if not reg:
         reg = ".*"
     pages -= 1
     async with AsyncSession(_async_database) as db_session:
         pics = await db_session.scalars(
```

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/picture.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/picture.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/randpic.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/randpic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/nonebot_plugin_savepic/rule.py` & `nonebot_plugin_savepic-0.2.7/nonebot_plugin_savepic/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.6/pyproject.toml` & `nonebot_plugin_savepic-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-savepic"
-version = "0.2.6"
+version = "0.2.7"
 description = "保存表情包（语录）与随机出图"
 authors = ["Yan <1964649083@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_savepic"}]
 homepage = "https://github.com/Yan-Zero/nonebot-plugin-savepic"
```

### Comparing `nonebot_plugin_savepic-0.2.6/PKG-INFO` & `nonebot_plugin_savepic-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-savepic
-Version: 0.2.6
+Version: 0.2.7
 Summary: 保存表情包（语录）与随机出图
 Home-page: https://github.com/Yan-Zero/nonebot-plugin-savepic
 License: MIT
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.2.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.2.7 Summary:
 ä¿å­è¡¨æåï¼è¯­å½ï¼ä¸éæºåºå¾ Home-page: https://github.com/Yan-
 Zero/nonebot-plugin-savepic License: MIT Author: Yan Author-email:
 1964649083@qq.com Requires-Python: >=3.10,<3.13 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0) Requires-Dist: asyncpg
```


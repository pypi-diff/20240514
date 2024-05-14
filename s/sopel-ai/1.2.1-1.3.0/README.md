# Comparing `tmp/sopel_ai-1.2.1-py3-none-any.whl.zip` & `tmp/sopel_ai-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11506 bytes, number of entries: 11
+Zip file size: 11535 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     2531 b- defN 24-Mar-08 16:08 sopel_ai/__init__.py
 -rw-r--r--  2.0 unx      867 b- defN 24-Mar-08 16:08 sopel_ai/config.py
--rw-r--r--  2.0 unx     7240 b- defN 24-Mar-08 16:08 sopel_ai/core.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-14 05:15 sopel_ai/core.py
 -rw-r--r--  2.0 unx      192 b- defN 24-Mar-08 16:08 sopel_ai/errors.py
 -rw-r--r--  2.0 unx     6800 b- defN 24-Mar-08 16:08 sopel_ai/plugin.py
--rw-r--r--  2.0 unx     1531 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6200 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 24-May-05 02:48 sopel_ai-1.2.1.dist-info/RECORD
-11 files, 26368 bytes uncompressed, 10050 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx     1531 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6200 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 24-May-14 05:19 sopel_ai-1.3.0.dist-info/RECORD
+11 files, 26405 bytes uncompressed, 10079 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: sopel_ai/errors.py
 Comment: 
 
 Filename: sopel_ai/plugin.py
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/LICENSE.txt
+Filename: sopel_ai-1.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/METADATA
+Filename: sopel_ai-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/WHEEL
+Filename: sopel_ai-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/entry_points.txt
+Filename: sopel_ai-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/top_level.txt
+Filename: sopel_ai-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sopel_ai-1.2.1.dist-info/RECORD
+Filename: sopel_ai-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sopel_ai/core.py

```diff
@@ -50,14 +50,15 @@
 
 def _checkDB(fileName: str) -> TinyDB:
     # Checks if DB exists; if not, it creates it
     global _database
 
     if not _database:
         _database = TinyDB(fileName)
+        _database.table('_default', cache_size = 0)
 
     return _database
 
 
 def _checkClientInstance(key: str) -> None:
     global _client
 
@@ -197,18 +198,18 @@
     ---
     """
     _checkDB(fileNameDB)
     models= modelsList(key)
     if modelID not in range(len(models)):
         raise SopelAIError('modelID outside of available models index range')
 
-    Preference = Query()
+    query = Query()
 
-    if _database.search(Preference.nick == nick):
-        _database.update({ 'model': models[modelID], }, Preference.nick == nick)
+    if _database.search(query.nick == nick):
+        _database.update({ 'model': models[modelID], }, query.nick == nick)
     else:
         _database.insert({ 'nick': nick, 'model': models[modelID], })
 
     return models[modelID]
 
 
 def getModelForUser(nick: str, fileNameDB: str, key = None) -> str:
```

## Comparing `sopel_ai-1.2.1.dist-info/LICENSE.txt` & `sopel_ai-1.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `sopel_ai-1.2.1.dist-info/METADATA` & `sopel_ai-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-ai
-Version: 1.2.1
+Version: 1.3.0
 Summary: Sopel AI - an LLM enhanced chat bot plug-in
 Author-email: The SopelAI team <sopel_ai@cime.net>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pr3d4t0r/sopel_ai
 Project-URL: Bug Tracker, https://github.com/pr3d4t0r/sopel_ai/issues
 Keywords: ai,bot,irc,llm,plugin,sopel
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: perplexipy
 Requires-Dist: sopel (>=7.1)
 Requires-Dist: tinydb
 
-% sopel_ai(1) Version 1.2.1 chatbot plugin
+% sopel_ai(1) Version 1.3.0 chatbot plugin
 
 Name
 ====
 
 **Sopel AI** - AI query/response plugin
```


# Comparing `tmp/omuchatprovider-0.3.1.tar.gz` & `tmp/omuchatprovider-0.3.2.tar.gz`

## Comparing `omuchatprovider-0.3.1.tar` & `omuchatprovider-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/__main__.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/chatprovider.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/errors.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/helper.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/tasks.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/throttle.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/version.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/service.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/__init__.py
--rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/chat.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/const.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/youtube.py
--rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/youtubeapi.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/accessibility.py
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/chatactions.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/contents.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/continuations.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/frameworkupdates.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/image.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/live_chat.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/metadataactions.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/responsecontext.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/runs.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/simpletext.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/updated_metadata.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/urlendpoint.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/youtuberesponse.py
--rw-r--r--   0        0        0    40280 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/ytcfg.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/ytinitialdata.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/__main__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/chatprovider.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/errors.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/helper.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/tasks.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/throttle.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/version.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/service.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/__init__.py
+-rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/chat.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/const.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/youtube.py
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/youtubeapi.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/accessibility.py
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/chatactions.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/contents.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/continuations.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/frameworkupdates.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/image.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/live_chat.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/metadataactions.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/responsecontext.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/runs.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/simpletext.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/updated_metadata.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/urlendpoint.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/youtuberesponse.py
+-rw-r--r--   0        0        0    40280 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/ytcfg.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.3.2/PKG-INFO
```

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/chatprovider.py` & `omuchatprovider-0.3.2/src/omuchatprovider/chatprovider.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/helper.py` & `omuchatprovider-0.3.2/src/omuchatprovider/helper.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/tasks.py` & `omuchatprovider-0.3.2/src/omuchatprovider/tasks.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/throttle.py` & `omuchatprovider-0.3.2/src/omuchatprovider/throttle.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/service.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/service.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/chat.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/chat.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/const.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/const.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/youtube.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/youtube.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/youtubeapi.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/youtubeapi.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/chatactions.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/chatactions.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/contents.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/contents.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/continuations.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/continuations.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/frameworkupdates.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/frameworkupdates.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/metadataactions.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/metadataactions.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/responsecontext.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/responsecontext.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/runs.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/runs.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/urlendpoint.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/urlendpoint.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/src/omuchatprovider/services/youtube/types/ytcfg.py` & `omuchatprovider-0.3.2/src/omuchatprovider/services/youtube/types/ytcfg.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.3.1/pyproject.toml` & `omuchatprovider-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuchatprovider"
-version = "0.3.1"
+version = "0.3.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "loguru>=0.7.2",
     "aiohttp>=3.9.1",
```


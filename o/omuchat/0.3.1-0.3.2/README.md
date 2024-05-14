# Comparing `tmp/omuchat-0.3.1.tar.gz` & `tmp/omuchat-0.3.2.tar.gz`

## Comparing `omuchat-0.3.1.tar` & `omuchat-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/__init__.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/chat.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/client.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/const.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/permissions.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/version.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/event/__init__.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/event/event.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/event/event_types.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/__init__.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/author.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/channel.py
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/content.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/gift.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/paid.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/provider.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/role.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 omuchat-0.3.1/src/omuchat/model/room.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchat-0.3.1/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.3.1/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/__init__.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/chat.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/client.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/const.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/permissions.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/version.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/event/__init__.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/event/event.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/event/event_types.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/author.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/channel.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/content.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/gift.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/paid.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/provider.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/role.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 omuchat-0.3.2/src/omuchat/model/room.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchat-0.3.2/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.3.2/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.3.2/PKG-INFO
```

### Comparing `omuchat-0.3.1/src/omuchat/chat.py` & `omuchat-0.3.2/src/omuchat/chat.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/client.py` & `omuchat-0.3.2/src/omuchat/client.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/event/event.py` & `omuchat-0.3.2/src/omuchat/event/event.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/event/event_types.py` & `omuchat-0.3.2/src/omuchat/event/event_types.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/__init__.py` & `omuchat-0.3.2/src/omuchat/model/__init__.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/author.py` & `omuchat-0.3.2/src/omuchat/model/author.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/channel.py` & `omuchat-0.3.2/src/omuchat/model/channel.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/content.py` & `omuchat-0.3.2/src/omuchat/model/content.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/gift.py` & `omuchat-0.3.2/src/omuchat/model/gift.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/message.py` & `omuchat-0.3.2/src/omuchat/model/message.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/paid.py` & `omuchat-0.3.2/src/omuchat/model/paid.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/provider.py` & `omuchat-0.3.2/src/omuchat/model/provider.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/role.py` & `omuchat-0.3.2/src/omuchat/model/role.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.3.1/src/omuchat/model/room.py` & `omuchat-0.3.2/src/omuchat/model/room.py`

 * *Files identical despite different names*


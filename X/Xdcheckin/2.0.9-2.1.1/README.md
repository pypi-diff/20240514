# Comparing `tmp/xdcheckin-2.0.9.tar.gz` & `tmp/xdcheckin-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcheckin-2.0.9.tar", last modified: Sat Apr 27 01:02:54 2024, max compression
+gzip compressed data, was "xdcheckin-2.1.1.tar", last modified: Tue May 14 09:35:49 2024, max compression
```

## Comparing `xdcheckin-2.0.9.tar` & `xdcheckin-2.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.827584 xdcheckin-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33622 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/chaoxing_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.502866 xdcheckin-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 09:35:49.000000 xdcheckin-2.1.1/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.502866 xdcheckin-2.1.1/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.502866 xdcheckin-2.1.1/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33125 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:49.506866 xdcheckin-2.1.1/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/util/chaoxing_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/util/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-14 09:35:43.000000 xdcheckin-2.1.1/src/xdcheckin/util/types.py
```

### Comparing `xdcheckin-2.0.9/LICENSE` & `xdcheckin-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/PKG-INFO` & `xdcheckin-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.9
+Version: 2.1.1
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.9/README.md` & `xdcheckin-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/pyproject.toml` & `xdcheckin-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Xdcheckin"
-version = "2.0.9"
+version = "2.1.1"
 authors = [
 	{name = "Pairman", email = "pairmanxlr@gmail.com"}
 ]
 readme = "README.md"
 description = "Chaoxing Checkin Tool for XDU."
 license = {text = "GNU General Public License v3 (GPLv3)"}
 keywords = ["xdu", "xidian", "chaoxing", "livestream"]
```

### Comparing `xdcheckin-2.0.9/src/Xdcheckin.egg-info/PKG-INFO` & `xdcheckin-2.1.1/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.9
+Version: 2.1.1
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.9/src/Xdcheckin.egg-info/SOURCES.txt` & `xdcheckin-2.1.1/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 src/xdcheckin/server/static/misc.js
 src/xdcheckin/server/static/player.js
 src/xdcheckin/server/static/style.css
 src/xdcheckin/server/static/util.js
 src/xdcheckin/server/templates/index.html
 src/xdcheckin/util/__init__.py
 src/xdcheckin/util/chaoxing_captcha.py
-src/xdcheckin/util/encryption.py
+src/xdcheckin/util/encryption.py
+src/xdcheckin/util/types.py
```

### Comparing `xdcheckin-2.0.9/src/xdcheckin/core/chaoxing.py` & `xdcheckin-2.1.1/src/xdcheckin/core/chaoxing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from ast import literal_eval as _literal_eval
 from datetime import datetime as _datetime
 from json import dumps as _dumps
 from random import choice as _choice, uniform as _uniform
-from re import findall as _findall, search as _search, DOTALL as _DOTALL
+from re import findall as _findall, search as _search, split as _split, DOTALL as _DOTALL
 from threading import Thread as _Thread
 from requests import Response as _Response
 from requests.adapters import HTTPAdapter as _HTTPAdapter
 from requests.exceptions import RequestException as _RequestException
 from requests_cache.session import CachedSession as _CachedSession
 from xdcheckin.util.chaoxing_captcha import generate_secrets as _generate_secrets
 from xdcheckin.util.encryption import encrypt_aes as _encrypt_aes
@@ -299,26 +299,26 @@
 		"""Log into Chaoxing account with username and password 
 		via Fanya API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v3().
 		"""
 		url = "https://passport2.chaoxing.com/fanyalogin"
 		data = {
-				"uname": _encrypt_aes(
-					msg = account["username"],
-					key = b"u2oh6Vu^HWe4_AES",
-					iv = b"u2oh6Vu^HWe4_AES"
-				),
-				"password": _encrypt_aes(
-					msg = account["password"],
-					key = b"u2oh6Vu^HWe4_AES",
-					iv = b"u2oh6Vu^HWe4_AES"
-				),
-				"t": True
-			}
+			"uname": _encrypt_aes(
+				msg = account["username"],
+				key = b"u2oh6Vu^HWe4_AES",
+				iv = b"u2oh6Vu^HWe4_AES"
+			),
+			"password": _encrypt_aes(
+				msg = account["password"],
+				key = b"u2oh6Vu^HWe4_AES",
+				iv = b"u2oh6Vu^HWe4_AES"
+			),
+			"t": True
+		}
 		ret = {
 			"name": "",
 			"cookies": None,
 			"logined": False
 		}
 		res = self.post(url = url, data = data)
 		if res.status_code == 200 and res.cookies.get("p_auth_token"):
@@ -356,14 +356,15 @@
 		:return: Dictionary of curriculum details and lessons 
 		containing course IDs, names, classroom locations, teachers 
 		and time.
 		"""
 		def _add_lesson(lesson: dict = {}):
 			lesson_class_id = str(lesson["classId"])
 			lesson = {
+				"class_id": lesson_class_id,
 				"course_id": str(lesson["courseId"]),
 				"name": lesson["name"],
 				"locations": [lesson["location"]],
 				"invite_code": lesson["meetCode"],
 				"teachers": [lesson["teacherName"]],
 				"times": [{
 					"day": str(lesson["dayOfWeek"]),
@@ -409,36 +410,41 @@
 		return curriculum
 
 	def course_get_courses(self):
 		"""Get all courses in the root folder.
 		:return: Dictionary of class IDs to course containing 
 		course IDs, names, teachers, status, start and end time.
 		"""
-		url = "https://mooc1-1.chaoxing.com/visit/courselistdata"
+		def _fill_courses(matches, status):
+			nonlocal courses
+			courses.update({
+				match[2]: {
+					"class_id": match[2],
+					"course_id": match[0],
+					"name": match[1],
+					"teachers": _split(r", |,|，|、", match[3]),
+					"status": status,
+					"time_start": match[4],
+					"time_end": match[5]
+				} for match in matches
+			})
+		url = "https://mooc2-ans.chaoxing.com/visit/courselistdata"
 		params = {
 			"courseType": 1
 		}
 		res = self.get(url = url, params = params, expire_after = 86400)
-		matches = _findall(
-			r"course_(\d+)_(\d+).*?(?:(not-open).*?)?title="
-			r"\"(.*?)\".*?title.*?title=\"(.*?)\""
-			r"(?:.*?(\d+-\d+-\d+)～(\d+-\d+-\d+))?",
-			res.text, _DOTALL
-		)
-		return {
-			match[1]: {
-				"class_id": match[1],
-				"course_id": match[0],
-				"name": match[3],
-				"teacher": match[4].split("，"),
-				"status": int(not bool(match[2])),
-				"time_start": match[5],
-				"time_end": match[6]
-			} for match in matches
-		}
+		active, ended = res.text.split("isState")
+		reg = r"Client\('(\d+)','(.*?)','(\d+).*?color3\" " \
+			r"title=\"(.*?)\".*?\n(?:[^\n]*?(\d+-\d+-\d+)～(\d+-\d+-\d+))?"
+		matches_active = _findall(reg, active, _DOTALL)
+		matches_ended = _findall(reg, ended, _DOTALL)
+		courses = {}
+		_fill_courses(matches_active, 1)
+		_fill_courses(matches_ended, 0)
+		return courses
 
 	def course_get_course_id(
 		self, course: dict = {"course_id": "", "class_id": ""}
 	):
 		"""Get course ID of a course.
 		:param course: Course ID (will be filled if not given) and 
 		clsss ID in dictionary.
@@ -620,15 +626,15 @@
 		:param location: Address, latitude and longitude in dictionary. 
 		Used for address override for checkin location.
 		:param location_new: Address, latitude and longitude 
 		in dictionary. The checkin location to upload.
 		:return: Checkin location containing address, latitude, 
 		longitude, range and ranged option.
 		"""
-		def _randomness(x: int | float = 0):
+		def _randomness(x: float = 0):
 			return round(x + _choice((-1, 1)) * _uniform(1, 5) * 0.0001, 6)
 		location_new = {
 			"ranged": 0,
 			"range": 0,
 			**location_new
 		}
 		if self.config["chaoxing_checkin_location_randomness"]:
@@ -636,37 +642,14 @@
 				"latitude": _randomness(location_new["latitude"]),
 				"longitude": _randomness(location_new["longitude"])
 			})
 		if len(location_new["address"]) < self.config["chaoxing_checkin_location_address_override_maxlen"]:
 			location_new["address"] = location["address"]
 		return location_new
 
-	def checkin_get_location_log(self, activity: dict = {"active_id": ""}):
-		"""Get checkin locations submitted by up to 100 students.
-		:param activity: Activity ID in dictionary.
-		:return: List of checkin locations containing address, 
-		latitude, longitude, range (placeholder) and 
-		ranged (placeholder) option.
-		"""
-		url = "https://mobilelearn.chaoxing.com/pptSign/autoRefeashSignList4Json2"
-		params = {
-			"activeId": activity["active_id"]
-		}
-		res = self.get(url = url, params = params)
-		data = res.json()["list"]
-		return [
-			{
-				"latitude": location.get("latitude"),
-				"longitude": location.get("longitude"),
-				"address": location.get("title"),
-				"ranged": int(not location.get("latitude") is None),
-				"range": 0
-			} for location in data
-		]
-
 	def checkin_get_location(
 		self, activity: dict = {"active_id": ""},
 		course: dict ={"course_id": "", "class_id": ""}
 	):
 		"""Get checkin location from the location log of its 
 		corresponding course.
 		:param activity: Activity ID in dictionary.
```

### Comparing `xdcheckin-2.0.9/src/xdcheckin/core/locations.py` & `xdcheckin-2.1.1/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/core/xidian.py` & `xdcheckin-2.1.1/src/xdcheckin/core/xidian.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/server.py` & `xdcheckin-2.1.1/src/xdcheckin/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import version as _version
 from io import BytesIO as _BytesIO
 from json import loads as _loads, dumps as _dumps
-from uuid import uuid4
+from uuid import uuid4 as _uuid4
 from flask import Flask as _Flask, render_template as _render_template, \
 	make_response as _make_response, request as _request, session as _session
 from flask_session import Session as _Session
 from PIL.Image import open as _open
 from pyzbar.pyzbar import decode as _decode, ZBarSymbol as _ZBarSymbol
 from requests import get as _get
 from xdcheckin.core.chaoxing import Chaoxing as _Chaoxing
@@ -66,15 +66,15 @@
 			return res
 
 	@server.route("/ids/login_prepare", methods = ["POST"])
 	def ids_login_prepare():
 		try:
 			ids = _IDSSession(service = "https://learning.xidian.edu.cn/cassso/xidian")
 			if not _session.get("xdcheckin_uuid"):
-				_session["xdcheckin_uuid"] = str(uuid4())
+				_session["xdcheckin_uuid"] = str(_uuid4())
 			if not server.config["XDCHECKIN_SESSION"].get(_session["xdcheckin_uuid"]):
 				server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]] = {}
 			server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["ids"] = ids
 			res = _make_response(_dumps(ids.login_username_prepare()))
 		except Exception as e:
 			res = _make_response(_dumps({"err": str(e)}))
 		finally:
@@ -122,15 +122,15 @@
 					"chaoxing_course_get_activities_courses_limit": 36,
 					"chaoxing_checkin_location_address_override_maxlen": 13
 				}
 			)
 			assert chaoxing.logined, "Chaoxing login failed."
 			newesxidian = _Newesxidian(chaoxing = chaoxing)
 			if not _session.get("xdcheckin_uuid"):
-				_session["xdcheckin_uuid"] = str(uuid4())
+				_session["xdcheckin_uuid"] = str(_uuid4())
 			if not server.config["XDCHECKIN_SESSION"].get(_session["xdcheckin_uuid"]):
 				server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]] = {}
 			server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]].update({
 				"chaoxing": chaoxing,
 				"newesxidian": newesxidian
 			})
 			ret = {
@@ -302,36 +302,55 @@
 	return server
 
 def start_server(host: str = "127.0.0.1", port: int = 5001):
 	"""Run a Xdcheckin server.
 	:param host: IP address.
 	:param port: Port.
 	"""
+	from datetime import datetime
 	from os import listdir, remove, makedirs
-	from os.path import exists, join
+	from os.path import join, getmtime
 	from tempfile import gettempdir
+	from time import sleep
+	from threading import Thread
 	from urllib3 import disable_warnings
 	from waitress import serve
+	from xdcheckin.util.types import TimestampDict
 	config = {
 		"SESSION_PERMANENT": False,
 		"SESSION_TYPE": "filesystem",
 		"SESSION_FILE_DIR": join(gettempdir(), "xdcheckin"),
-		"XDCHECKIN_SESSION": {}
+		"XDCHECKIN_SESSION_VACUUM_DAY": 1,
+		"XDCHECKIN_SESSION": TimestampDict()
 	}
-	if not exists(config["SESSION_FILE_DIR"]):
-		makedirs(config["SESSION_FILE_DIR"])
-	else:
-		for i in listdir(config["SESSION_FILE_DIR"]):
-				remove(join(config["SESSION_FILE_DIR"], i))
+	session_file_dir = config["SESSION_FILE_DIR"]
+	makedirs(session_file_dir, exist_ok = True)
+	def _vacuum_sessions():
+		nonlocal config, session_file_dir
+		vacuum_day = config["XDCHECKIN_SESSION_VACUUM_DAY"]
+		vacuum_seconds = vacuum_day * 86400
+		xdcheckin_session = config["XDCHECKIN_SESSION"]
+		while True:
+			now = datetime.now()
+			now_ts = now.timestamp()
+			for fname in listdir(session_file_dir):
+				fpath = join(session_file_dir, fname)
+				if now_ts > getmtime(fpath) + vacuum_seconds:
+					remove(fpath)
+			then = now.replace(
+				day = now.day + vacuum_day, hour = 3, minute = 0
+			)
+			sleep((then - now).total_seconds())
+			xdcheckin_session.vacuum(seconds = vacuum_seconds)
+	Thread(target = _vacuum_sessions, daemon = True).start()
 	disable_warnings()
 	serve(app = create_server(config = config), host = host, port = port)
 
 def main():
 	from sys import argv
-
 	if not len(argv) in (1, 3):
 		print(f"xdcheckin-server - Xdcheckin Server Commandline Tool {_version('Xdcheckin')}")
 		print(f"Usage: {argv[0]} <ip> <port>")
 		print(f"  or:  {argv[0]}")
 		return 1
 	ip, port = "0.0.0.0", 5001
 	if len(argv) == 3:
```

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/activity.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/classroom.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/curriculum.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/curriculum.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/g_classroom_urls.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/location.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/login.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/misc.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/player.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/style.css` & `xdcheckin-2.1.1/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/static/util.js` & `xdcheckin-2.1.1/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/server/templates/index.html` & `xdcheckin-2.1.1/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.9/src/xdcheckin/util/chaoxing_captcha.py` & `xdcheckin-2.1.1/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 	x_r -= border
 	y_b -= border
 	with small_img.crop((x_l, y_t, x_r, y_b)) as crop:
 		with crop.convert("L") as grayscale:
 			template = grayscale.getdata()
 	mean_tmp = sum(template) / len(template)
 	template = [v - mean_tmp for v in template]
-	maxncc = 0
-	maxx = 0
+	ncc_max = 0
+	x_max = 0
 	with big_img.crop(
 		(x_l + 1, y_t, big_img.width - small_img.width + x_r, y_b)
 	) as img:
 		with img.convert("L") as grayscale:
 			for x in range(0, grayscale.width - x_r + x_l, 2):
 				with grayscale.crop(
 					(x, 0, x + x_r - x_l, grayscale.height)
 				) as crop:
 					window = crop.getdata()
 				mean_wd = sum(window) / len(window)
 				window = [w - mean_wd for w in window]
 				ncc = sum(
 					w * t for w, t in zip(window, template)
 				) / sum(w * w for w in window)
-				if ncc > maxncc:
-					maxncc = ncc
-					maxx = x
-	return maxx
+				if ncc > ncc_max:
+					ncc_max = ncc
+					x_max = x
+	return x_max
```

### Comparing `xdcheckin-2.0.9/src/xdcheckin/util/encryption.py` & `xdcheckin-2.1.1/src/xdcheckin/util/encryption.py`

 * *Files identical despite different names*


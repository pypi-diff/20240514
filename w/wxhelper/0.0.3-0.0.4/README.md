# Comparing `tmp/wxhelper-0.0.3.tar.gz` & `tmp/wxhelper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhelper-0.0.3.tar", last modified: Sun May 12 11:36:25 2024, max compression
+gzip compressed data, was "wxhelper-0.0.4.tar", last modified: Tue May 14 10:21:13 2024, max compression
```

## Comparing `wxhelper-0.0.3.tar` & `wxhelper-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:36:25.441379 wxhelper-0.0.3/
--rw-rw-rw-   0        0        0     1077 2024-05-12 03:43:34.000000 wxhelper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-12 03:43:34.000000 wxhelper-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3652 2024-05-12 11:36:25.438938 wxhelper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2904 2024-05-12 05:57:53.000000 wxhelper-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 11:36:25.441379 wxhelper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3932 2024-05-12 11:36:05.000000 wxhelper-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:36:25.420903 wxhelper-0.0.3/wxhelper/
--rw-rw-rw-   0        0        0       44 2024-05-12 11:36:05.000000 wxhelper-0.0.3/wxhelper/__init__.py
--rw-rw-rw-   0        0        0    20724 2024-05-12 05:49:21.000000 wxhelper-0.0.3/wxhelper/core.py
--rw-rw-rw-   0        0        0      630 2024-05-12 03:43:35.000000 wxhelper-0.0.3/wxhelper/events.py
--rw-rw-rw-   0        0        0      314 2024-05-12 03:43:35.000000 wxhelper-0.0.3/wxhelper/logger.py
--rw-rw-rw-   0        0        0     2693 2024-05-12 04:58:55.000000 wxhelper-0.0.3/wxhelper/model.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:36:25.435908 wxhelper-0.0.3/wxhelper/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-12 03:43:35.000000 wxhelper-0.0.3/wxhelper/tools/faker.exe
--rwxrwxrwx   0        0        0   888832 2024-05-12 09:24:46.000000 wxhelper-0.0.3/wxhelper/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   489984 2024-05-12 03:43:35.000000 wxhelper-0.0.3/wxhelper/tools/wxhelper.dll
--rw-rw-rw-   0        0        0     3789 2024-05-12 11:34:55.000000 wxhelper-0.0.3/wxhelper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:36:25.428880 wxhelper-0.0.3/wxhelper.egg-info/
--rw-rw-rw-   0        0        0     3652 2024-05-12 11:36:25.000000 wxhelper-0.0.3/wxhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-12 11:36:25.000000 wxhelper-0.0.3/wxhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:36:25.000000 wxhelper-0.0.3/wxhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 11:36:25.000000 wxhelper-0.0.3/wxhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 11:36:25.000000 wxhelper-0.0.3/wxhelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:13.768830 wxhelper-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2024-05-14 05:57:33.000000 wxhelper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-14 05:57:33.000000 wxhelper-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3652 2024-05-14 10:21:13.767843 wxhelper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2904 2024-05-14 05:57:33.000000 wxhelper-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:21:13.768830 wxhelper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3932 2024-05-14 10:01:04.000000 wxhelper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:13.758829 wxhelper-0.0.4/wxhelper/
+-rw-rw-rw-   0        0        0       44 2024-05-14 10:01:04.000000 wxhelper-0.0.4/wxhelper/__init__.py
+-rw-rw-rw-   0        0        0    20732 2024-05-14 09:20:21.000000 wxhelper-0.0.4/wxhelper/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/events.py
+-rw-rw-rw-   0        0        0      314 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/logger.py
+-rw-rw-rw-   0        0        0     2693 2024-05-14 09:19:20.000000 wxhelper-0.0.4/wxhelper/model.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:13.766829 wxhelper-0.0.4/wxhelper/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/tools/faker.exe
+-rwxrwxrwx   0        0        0   888832 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   489984 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/tools/wxhelper.dll
+-rw-rw-rw-   0        0        0     3789 2024-05-14 05:57:33.000000 wxhelper-0.0.4/wxhelper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:21:13.763829 wxhelper-0.0.4/wxhelper.egg-info/
+-rw-rw-rw-   0        0        0     3652 2024-05-14 10:21:13.000000 wxhelper-0.0.4/wxhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-14 10:21:13.000000 wxhelper-0.0.4/wxhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:21:13.000000 wxhelper-0.0.4/wxhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-14 10:21:13.000000 wxhelper-0.0.4/wxhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 10:21:13.000000 wxhelper-0.0.4/wxhelper.egg-info/top_level.txt
```

### Comparing `wxhelper-0.0.3/LICENSE` & `wxhelper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/PKG-INFO` & `wxhelper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.3
+Version: 0.0.4
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wxhelper-0.0.3/README.md` & `wxhelper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/setup.py` & `wxhelper-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhelper'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhelper'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhelper-0.0.3/wxhelper/core.py` & `wxhelper-0.0.4/wxhelper/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         """获取群详情"""
         params = {
             "type": "47"
         }
         data = {
             "chatRoomId": room_id
         }
-        return Room(**self.call_api(params=params, json=data))
+        return Room(**self.call_api(params=params, json=data)["data"])
 
     def get_room_members(self, room_id: str) -> RoomMembers:
         """获取群成员列表"""
         params = {
             "type": "25"
         }
         data = {
```

### Comparing `wxhelper-0.0.3/wxhelper/events.py` & `wxhelper-0.0.4/wxhelper/events.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper/model.py` & `wxhelper-0.0.4/wxhelper/model.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper/tools/faker.exe` & `wxhelper-0.0.4/wxhelper/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper/tools/start-wechat.exe` & `wxhelper-0.0.4/wxhelper/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper/tools/wxhelper.dll` & `wxhelper-0.0.4/wxhelper/tools/wxhelper.dll`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper/utils.py` & `wxhelper-0.0.4/wxhelper/utils.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.3/wxhelper.egg-info/PKG-INFO` & `wxhelper-0.0.4/wxhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.3
+Version: 0.0.4
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```


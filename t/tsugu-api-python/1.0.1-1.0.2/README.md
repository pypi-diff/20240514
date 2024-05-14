# Comparing `tmp/tsugu-api-python-1.0.1.tar.gz` & `tmp/tsugu-api-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.0.1.tar", last modified: Mon May 13 02:52:41 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.0.2.tar", last modified: Mon May 13 09:10:12 2024, max compression
```

## Comparing `tsugu-api-python-1.0.1.tar` & `tsugu-api-python-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 02:52:41.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.0.1/LICENSE` & `tsugu-api-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/PKG-INFO` & `tsugu-api-python-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.1/README.md` & `tsugu-api-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/setup.py` & `tsugu-api-python-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.0.1',
+    version='1.0.2',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api/__init__.py` & `tsugu-api-python-1.0.2/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.0.2/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_network.py` & `tsugu-api-python-1.0.2/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_station.py` & `tsugu-api-python-1.0.2/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_tsugu.py` & `tsugu-api-python-1.0.2/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_typing.py` & `tsugu-api-python-1.0.2/tsugu_api/_typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 _DifficultyText: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
 '''难度名'''
 
 class _Player(TypedDict):
     id: int
     server: _Server
 
-_Status: TypeAlias = Literal['success', 'failure']
+_Status: TypeAlias = Literal['success', 'failed']
 '''响应状态'''
 
 class _SubmitResponse(TypedDict):
     '''`/station/submitRoomNumber` 响应结果'''
     status: _Status
     data: str
 
@@ -86,39 +86,39 @@
     user_id: str
     platform: str
     server_mode: _Server
     default_server: list[_Server]
     car: bool
     server_list: list[_TsuguUserServer]
 
-class _UserDataResponse(TypedDict):
+class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
 
 class _Update(TypedDict):
     '''更新数据'''
     user_id: NotRequired[str]
     platform: NotRequired[str]
     server_mode: NotRequired[_ServerId]
     default_server: NotRequired[list[_ServerId]]
     car: NotRequired[bool]
     server_list: NotRequired[list[_TsuguUserServer]]
 
-class _UpdateResponse(TypedDict):
+class _ChangeUserDataResponse(TypedDict):
     '''`/user/changeUserData` 响应结果'''
     status: _Status
     data: NotRequired[str]
 
 class _VerifyCode(TypedDict):
     '''验证码'''
     verifyCode: int
 
-class _BindResponse(TypedDict):
+class _BindPlayerRequestResponse(TypedDict):
     '''`/user/bindPlayerRequest` 绑定响应'''
     status: _Status
     data: Union[str, _VerifyCode]
 
-class _VerificationResponse(TypedDict):
+class _BindPlayerVerificationResponse(TypedDict):
     '''`/user/bindPlayerVerification` 响应结果'''
     status: _Status
     data: str
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api/_user.py` & `tsugu-api-python-1.0.2/tsugu_api/_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import Union
 
 from tsugu_api import settings
 from tsugu_api._network import Api
 from tsugu_api._typing import (
     _Update,
-    _Response,
     _ServerId,
-    _BindResponse,
-    _UpdateResponse,
-    _UserDataResponse,
-    _VerificationResponse
+    _GetUserDataResponse,
+    _ChangeUserDataResponse,
+    _BindPlayerRequestResponse,
+    _BindPlayerVerificationResponse
 )
 
-def get_user_data(platform: str, user_id: str) -> Union[_Response, _UserDataResponse]:
+def get_user_data(platform: str, user_id: str) -> _GetUserDataResponse:
     '''获取用户数据
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
 
     返回:
-        _UserDataResult: 用户数据
-        _Response: 当请求失败时返回的数据
+        _GetUserDataResponse: API 返回响应
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/getUserData'
     
     # 构建数据
     data = {
@@ -35,25 +33,24 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.userdata_backend_proxy
     ).post(data).json()
 
-def change_user_data(platform: str, user_id: str, update: _Update) -> Union[_Response, _UpdateResponse]:
+def change_user_data(platform: str, user_id: str, update: _Update) -> _ChangeUserDataResponse:
     '''修改用户数据
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         update (_Update): 更新数据
 
     返回:
-        _UpdateResult: 更新结果
-        _Response: 当请求失败时返回的数据
+        _ChangeUserDataResponse: API 返回响应
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/changeUserData'
     
     # 构建数据
     data = {
@@ -69,26 +66,25 @@
     ).post(data).json()
 
 def bind_player_request(
     platform: str,
     user_id: str,
     server: _ServerId,
     bind_type: bool
-) -> Union[_Response, _BindResponse]:
+) -> _BindPlayerRequestResponse:
     '''绑定玩家请求
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         server (_ServerId): 服务器编号 0 - 日服 1 - 国际服 2 - 台服 3 - 国服 4 - 韩服
         bind_type (bool): 绑定类型， `true` 为绑定， `false` 为解绑
 
     返回:
-        _BindResponse: 请求返回数据
-        _Response: 当请求失败时返回的数据
+        _BindPlayerRequestResponse: 请求返回数据
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/bindPlayerRequest'
     
     # 构建数据
     data = {
@@ -106,27 +102,26 @@
 
 def bind_player_verification(
     platform: str,
     user_id: str,
     server: _ServerId,
     player_id: int,
     bind_type: bool
-) -> Union[_Response, _VerificationResponse]:
+) -> _BindPlayerVerificationResponse:
     '''绑定玩家验证
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         server (_ServerId): 服务器编号 0 - 日服 1 - 国际服 2 - 台服 3 - 国服 4 - 韩服
         player_id (int): 玩家 ID
         bind_type (bool): 绑定类型， `true` 为绑定， `false` 为解绑
 
     返回:
-        _VerificationResponse: 验证返回数据
-        _Response: 当请求失败时返回的数据
+        _BindPlayerVerificationResponse: 验证返回数据
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/bindPlayerVerification'
     
     # 构建数据
     data = {
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api/settings.py` & `tsugu-api-python-1.0.2/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api/utils.py` & `tsugu-api-python-1.0.2/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/__init__.py` & `tsugu-api-python-1.0.2/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_network.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_station.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_typing.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 _DifficultyText: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
 '''难度名'''
 
 class _Player(TypedDict):
     id: int
     server: _Server
 
-_Status: TypeAlias = Literal['success', 'failure']
+_Status: TypeAlias = Literal['success', 'failed']
 '''响应状态'''
 
 class _SubmitResponse(TypedDict):
     '''`/station/submitRoomNumber` 响应结果'''
     status: _Status
     data: str
 
@@ -91,39 +91,39 @@
     user_id: str
     platform: str
     server_mode: _Server
     default_server: list[_Server]
     car: bool
     server_list: list[_TsuguUserServer]
 
-class _UserDataResponse(TypedDict):
+class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
 
 class _Update(TypedDict):
     '''更新数据'''
     user_id: NotRequired[str]
     platform: NotRequired[str]
     server_mode: NotRequired[_ServerId]
     default_server: NotRequired[list[_ServerId]]
     car: NotRequired[bool]
     server_list: NotRequired[list[_TsuguUserServer]]
 
-class _UpdateResponse(TypedDict):
+class _ChangeUserDataResponse(TypedDict):
     '''`/user/changeUserData` 响应结果'''
     status: _Status
     data: NotRequired[str]
 
 class _VerifyCode(TypedDict):
     '''验证码'''
     verifyCode: int
 
-class _BindResponse(TypedDict):
+class _BindPlayerRequestResponse(TypedDict):
     '''`/user/bindPlayerRequest` 绑定响应'''
     status: _Status
     data: Union[str, _VerifyCode]
 
-class _VerificationResponse(TypedDict):
+class _BindPlayerVerificationResponse(TypedDict):
     '''`/user/bindPlayerVerification` 响应结果'''
     status: _Status
     data: str
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/_user.py` & `tsugu-api-python-1.0.2/tsugu_api_async/_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import (
     _Update,
-    _Response,
     _ServerId,
-    _BindResponse,
-    _UpdateResponse,
-    _UserDataResponse,
-    _VerificationResponse
+    _GetUserDataResponse,
+    _ChangeUserDataResponse,
+    _BindPlayerRequestResponse,
+    _BindPlayerVerificationResponse
 )
 
-async def get_user_data(platform: str, user_id: str) -> Union[_Response, _UserDataResponse]:
+async def get_user_data(platform: str, user_id: str) -> _GetUserDataResponse:
     '''获取用户数据
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
 
     返回:
-        _UserDataResult: 用户数据
-        _Response: 当请求失败时返回的数据
+        _GetUserDataResponse: API 返回响应
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/getUserData'
     
     # 构建数据
     data = {
@@ -39,25 +37,24 @@
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def change_user_data(platform: str, user_id: str, update: _Update) -> Union[_Response, _UpdateResponse]:
+async def change_user_data(platform: str, user_id: str, update: _Update) -> _ChangeUserDataResponse:
     '''修改用户数据
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         update (_Update): 更新数据
 
     返回:
-        _UpdateResult: 更新结果
-        _Response: 当请求失败时返回的数据
+        _ChangeUserDataResponse: API 返回响应
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/changeUserData'
     
     # 构建数据
     data = {
@@ -75,26 +72,25 @@
     return await response.json()
 
 async def bind_player_request(
     platform: str,
     user_id: str,
     server: _ServerId,
     bind_type: bool
-) -> Union[_Response, _BindResponse]:
+) -> _BindPlayerRequestResponse:
     '''绑定玩家请求
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         server (_ServerId): 服务器编号 0 - 日服 1 - 国际服 2 - 台服 3 - 国服 4 - 韩服
         bind_type (bool): 绑定类型， `true` 为绑定， `false` 为解绑
 
     返回:
-        _BindResponse: 请求返回数据
-        _Response: 当请求失败时返回的数据
+        _BindPlayerRequestResponse: 请求返回数据
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/bindPlayerRequest'
     
     # 构建数据
     data = {
@@ -114,27 +110,26 @@
 
 async def bind_player_verification(
     platform: str,
     user_id: str,
     server: _ServerId,
     player_id: int,
     bind_type: bool
-) -> Union[_Response, _VerificationResponse]:
+) -> _BindPlayerVerificationResponse:
     '''绑定玩家验证
 
     参数:
         platform (str): 平台名称
         user_id (str): 用户 ID
         server (_ServerId): 服务器编号 0 - 日服 1 - 国际服 2 - 台服 3 - 国服 4 - 韩服
         player_id (int): 玩家 ID
         bind_type (bool): 绑定类型， `true` 为绑定， `false` 为解绑
 
     返回:
-        _VerificationResponse: 验证返回数据
-        _Response: 当请求失败时返回的数据
+        _BindPlayerVerificationResponse: 验证返回数据
     '''
     
     # 构建 URL
     url = settings.userdata_backend_url + '/user/bindPlayerVerification'
     
     # 构建数据
     data = {
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/settings.py` & `tsugu-api-python-1.0.2/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_async/utils.py` & `tsugu-api-python-1.0.2/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.1/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.0.2/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.1/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.0.2/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


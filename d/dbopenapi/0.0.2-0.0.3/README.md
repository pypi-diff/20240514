# Comparing `tmp/dbopenapi-0.0.2.tar.gz` & `tmp/dbopenapi-0.0.3.tar.gz`

## Comparing `dbopenapi-0.0.2.tar` & `dbopenapi-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/dbopenapi.pyproj
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/OpenApi.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/code_realtime_account.py
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/LICENSE
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/dbopenapi.pyproj
+-rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/src/dbopenapi/OpenApi.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/src/dbopenapi/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/src/dbopenapi/code_realtime_account.py
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/src/dbopenapi/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/LICENSE
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dbopenapi-0.0.3/PKG-INFO
```

### Comparing `dbopenapi-0.0.2/dbopenapi.pyproj` & `dbopenapi-0.0.3/dbopenapi.pyproj`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.2/src/dbopenapi/OpenApi.py` & `dbopenapi-0.0.3/src/dbopenapi/OpenApi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ﻿import asyncio
 import aiohttp
 import json
 from dbopenapi.tr_code_to_path import tr_code_to_path
 from dbopenapi.code_realtime_account import code_realtime_account
 
 BASE_URL = "https://openapi.db-fi.com:8443"
-WSS_URL_REAL = "wss://openapi.db-fi.com:7070"
-WSS_URL_SIMULATION = "wss://openapi.db-fi.com:17070"
+WSS_URL_REAL = "wss://openapi.db-fi.com:7070/websocket"
+WSS_URL_SIMULATION = "wss://openapi.db-fi.com:17070/websocket"
 
 #해외선물옵션
-WSS_URL_REAL_overseas_future = "wss://openapi.db-fi.com:7071"
+WSS_URL_REAL_overseas_future = "wss://openapi.db-fi.com:7071/websocket"
 
 class ResponseValue:
     def __init__(
         self,
         cont_yn: str,
         cont_key: str,
         body: dict,
@@ -110,23 +110,21 @@
         if self._websocket and not self._websocket.closed:
             await self._websocket.close()
         if self._http and not self._http.closed:
             await self._http.close()
 
     async def login(self, appkey:str, appsecretkey:str
                     ,*
-                    , enable_wss:bool=True
                     , wss_domain:str=None
                     , access_token:str=None) -> bool:
         '''
         로그인 요청
         appkey: 앱키
         appsecretkey: 앱시크릿키
         *
-        enable_wss: 웹소켓 연결허용(기본값: True), False로 설정하면 웹소켓 연결을 하지 않음
         wss_domain: 웹소켓 도메인(해외선물옵션인 경우에만 설정, wss://openapi.db-fi.com:7071 으로 설정)
         access_token: 토큰(기본값: ''), 토큰이 있는 경우에는 토큰을 사용하고, 없는 경우에는 새로 토큰을 가져옴
         return: True: 성공, False: 실패, 실패시 last_message에 실패사유가 저장됨
         '''
         if self._connected :
             self._last_message = "aleady connected";
             return True;
@@ -169,31 +167,30 @@
             return False;
     
         rsp_msg:str = response.body["rsp_msg"];
         if rsp_msg.__contains__("모의투자"):
             self._is_simulation = True;
 
         # 웹소켓 연결
-        if enable_wss:
-            if not wss_domain:
-                wss_domain = WSS_URL_SIMULATION if self._is_simulation else WSS_URL_REAL;
-            self._connected = False;
-            try:
-                websocket = await  httpclient.ws_connect(wss_domain)
-                self._connected = not websocket.closed;
-            except :
-                pass
+        if not wss_domain:
+            wss_domain = WSS_URL_SIMULATION if self._is_simulation else WSS_URL_REAL;
+        self._connected = False;
+        try:
+            websocket = await  httpclient.ws_connect(wss_domain)
+            self._connected = not websocket.closed;
+        except :
+            pass
     
-            if not self._connected:
-                await httpclient.close();
-                self._last_message = "websocket connection failed.";
-                return False;
+        if not self._connected:
+            await httpclient.close();
+            self._last_message = "websocket connection failed.";
+            return False;
     
-            self._websocket = websocket;
-            asyncio.create_task(self._websocket_listen());
+        self._websocket = websocket;
+        asyncio.create_task(self._websocket_listen());
         
         return True;
 
     async def request(self, tr_cd:str, data:dict
                              ,*
                              , path:str=None
                              , cont_yn:str="N"
```

### Comparing `dbopenapi-0.0.2/src/dbopenapi/tr_code_to_path.py` & `dbopenapi-0.0.3/src/dbopenapi/tr_code_to_path.py`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.2/.gitignore` & `dbopenapi-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.2/LICENSE` & `dbopenapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.2/README.md` & `dbopenapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.2/pyproject.toml` & `dbopenapi-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbopenapi"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for db openapi"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dbopenapi-0.0.2/PKG-INFO` & `dbopenapi-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbopenapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: package for db openapi
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/dbopenapi
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


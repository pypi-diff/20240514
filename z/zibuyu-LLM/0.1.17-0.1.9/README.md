# Comparing `tmp/zibuyu_LLM-0.1.17-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 70172 bytes, number of entries: 18
+Zip file size: 67284 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
 -rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
 -rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
 -rw-rw-rw-  2.0 fat     7376 b- defN 24-May-11 14:22 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7104 b- defN 24-May-12 05:31 zibuyu_llm_web/base.py
 -rw-rw-rw-  2.0 fat    14789 b- defN 24-May-11 14:25 zibuyu_llm_web/deepseek.py
--rw-rw-rw-  2.0 fat      807 b- defN 24-May-12 10:11 zibuyu_llm_web/errors.py
+-rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
 -rw-rw-rw-  2.0 fat     9962 b- defN 24-May-11 14:22 zibuyu_llm_web/kimi.py
--rw-rw-rw-  2.0 fat    48418 b- defN 24-May-14 08:26 zibuyu_llm_web/minmax.py
+-rw-rw-rw-  2.0 fat    37747 b- defN 24-May-12 02:39 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37730 b- defN 24-May-11 13:49 zibuyu_llm_web/qwen.py
 -rw-rw-rw-  2.0 fat     5308 b- defN 24-May-12 03:43 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14705 b- defN 24-May-11 14:25 zibuyu_llm_web/xinchen.py
--rw-rw-rw-  2.0 fat    59762 b- defN 24-May-12 16:58 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1572 b- defN 24-May-14 08:30 zibuyu_LLM-0.1.17.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 08:30 zibuyu_LLM-0.1.17.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-14 08:30 zibuyu_LLM-0.1.17.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1459 b- defN 24-May-14 08:30 zibuyu_LLM-0.1.17.dist-info/RECORD
-18 files, 250151 bytes uncompressed, 67806 bytes compressed:  72.9%
+-rw-rw-rw-  2.0 fat    55663 b- defN 24-May-12 05:50 zibuyu_llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1621 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/RECORD
+18 files, 235351 bytes uncompressed, 64926 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.1.17.dist-info/METADATA
+Filename: zibuyu_LLM-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.1.17.dist-info/WHEEL
+Filename: zibuyu_LLM-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.1.17.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.1.17.dist-info/RECORD
+Filename: zibuyu_LLM-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/errors.py

```diff
@@ -29,11 +29,7 @@
 
 class APIConnectionError(Exception):
     message = "网络连接错误"
 
 
 class SpiderHasToChangeError(Exception):
     message = "网页出现新逻辑，爬虫需要更换"
-
-
-class UnexpectResponseError(Exception):
-    message = "响应异常"
```

## zibuyu_llm_web/minmax.py

```diff
@@ -2,44 +2,28 @@
 
 """
 --------------------------------------------
 project: zibuyu_LLM
 author: 子不语
 date: 2024/5/4
 contact: 【公众号】思维兵工厂
-description: 海螺问问Web逆向。
-
-该平台使用是在请求头中通过Token（JWT）进行鉴权的；cookies无关鉴权。
-
-JWT的载荷部分:
-
-{
-  "exp": 1718232417,
-  "user": {
-    "id": "242935160332279815",
-    "name": "小螺帽9815",
-    "avatar": "https://cdn.yingshi-ai.com/prod/user_avatar/1706267544389820801-173194570668965896oversize.png",
-    "deviceID": "242935159979966466",
-    "isAnonymous": false
-  }
-}
+description: 海螺问问Web逆向
 --------------------------------------------
 """
-
 import base64
 import os
 import re
 import uuid
 import time
 import json
 import hashlib
 import logging
 import asyncio
 import traceback
-from typing import Dict, Optional, Literal
+from typing import Dict, Optional
 from urllib.parse import urlencode, quote_plus
 
 import aiohttp
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from .base import LLMBase
@@ -59,44 +43,38 @@
     def __init__(
             self,
             login_phone: str = None,
             token_str: str = None,
             logger_obj: logging.Logger = None,
             error_dir: str = None
     ):
-        """
-        :param login_phone: 登录手机号
-        :param token_str: 登录token
-        :param logger_obj: 日志对象
-        :param error_dir: 错误日志保存目录
-        """
 
         self.logger = logger_obj
         self.login_phone = login_phone
         self.error_dir = error_dir
         self.token_str = token_str
 
         super().__init__()
 
         self.chat_id: str = ''  # 会话ID
-        self.user_msg_id: str = ''  # 用户所发送的消息的id，目前无作用
-        self.system_msg_id: str = ''  # 系统回复的消息的id，主要用于获取音频
+        self.user_msg_id: str = ''  # 用户所发送的消息的id
+        self.system_msg_id: str = ''  # 系统回复的消息的id
 
         self.__single_uuid: str = ''  # 单次会话标识ID
         self.__user_id: str = ''  # 用户标识ID
         self.__device_id: str = ''  # 设备标识ID
         self.__device_info_expire: int = 0  # 设备ID过期时间
 
         self.__voice_info_dict: Optional[dict] = None
 
         # 语音相关_请求参数
         self.__voice_user_data = {
             'msgID': "",  # 消息ID
             'timbre': "",  # 配音音色
-            'device_platform': "web",
+            'device_platform': "zibuyu_llm_web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
@@ -107,15 +85,15 @@
             'screen_width': 1920,
             'screen_height': 1080,
             'unix': '',  # 时间戳，待填充
         }
 
         # 公用请求参数
         self.__user_data = {
-            'device_platform': "web",
+            'device_platform': "zibuyu_llm_web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
@@ -140,46 +118,33 @@
             "Sec-Ch-Ua": '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"',
             "Sec-Ch-Ua-Mobile": "?0",
             "Sec-Ch-Ua-Platform": '"Windows"',
             "User-Agent": super().user_agent,
             "Token": self.token_str,
         }
 
-        self.is_anonymous: bool = True  # 是否是匿名用户；默认为匿名用户
         self.single_answer: str = ''
-        self.single_answer_obj: AiAnswer = AiAnswer()
+        self.single_answer_obj: Optional[AiAnswer] = None
         self.single_padding: str = ''  # 流式输出时，每次接收到的回答中的增量部分
-        self.single_answer_audio_url_list: Optional[list] = None  # 单次回复时，音频文件的url列表
-
-        if self.token_str:
-            self.parse_token_str()
-        elif self.anonymity_login():
-            self.logger.info(f'未传入Token，进行匿名登录，成功获取token_str')
-        else:
-            self.logger.error(f'未传入Token，且匿名登录失败')
+        self.single_answer_audio_url_list: list = []  # 单次回复时，音频文件的url列表
 
     @property
     def device_id(self):
         """ 获取设备id，该值存在有效期 """
 
-        now = int(time.time()) * 1000
+        now = int(time.time())
 
         if self.__device_id and self.__device_info_expire > now:
             return self.__device_id
 
         self.update_device_id()
 
         return self.__device_id
 
     @property
-    def device_info_expire(self):
-        """ 获取设备id的过期时间 """
-        return self.__device_info_expire
-
-    @property
     def user_id(self):
         """ 获取user_id """
 
         if self.__user_id:
             return self.__user_id
 
         self.update_device_id()
@@ -395,263 +360,40 @@
 
     @staticmethod
     def get_timestamp():
         """ 获取时间戳 """
 
         return str(int(time.time()) * 1000)
 
-    @staticmethod
-    def add_padding_to_base64(s):
-        missing_padding = 4 - (len(s) % 4)
-        if missing_padding == 4:
-            return s  # 已经是4的倍数，不需要添加填充
-        return s + '=' * missing_padding  # 添加缺失的填充字符
-
-    def parse_token_str(self) -> bool:
-        """海螺使用的Token是JWT格式，可以解析后获取基本信息"""
-
-        if not self.token_str:
-            return False
-
-        try:
-
-            first_data = self.token_str.split('.')[1]
-            padded_payload = self.add_padding_to_base64(first_data)
-
-            data = json.loads(base64.b64decode(padded_payload).decode())
-            device_id = data.get('user', {}).get('deviceID', '')
-            self.is_anonymous = data.get('user', {}).get('isAnonymous', True)
-            self.__device_id = device_id
-            self.logger.info(f'成功解析JWT\n\n设备ID：【{device_id}】\n用户类型：isAnonymous【{self.is_anonymous}】\n')
-            return True
-        except:
-            self.logger.error(f'解析JWT失败', exc_info=True)
-            return False
-
-    def renew_token_str(self) -> bool:
-
-        uri = '/v1/api/user/renewal'
-        unix = self.get_timestamp()
-
-        user_data = self.__user_data.copy()
-        user_data['device_id'] = self.device_id
-        user_data['uuid'] = self.single_uuid
-        user_data['unix'] = unix
-
-        headers = self.__headers.copy()
-
-        yy = self.get_yy(
-            uri=uri,
-            unix=unix,
-            data=user_data,
-            user_data=user_data,
-            jsonfy=True,
-        )
-
-        headers["Yy"] = yy
-        try:
-            response = self.request_session.post(
-                self.base_host + uri,
-                headers=headers,
-                json=user_data
-            )
-
-            resp_data = response.json()
-            request_status = resp_data.get('statusInfo', {}).get('code', )
-            if request_status != 200:
-                self.logger.error(f'token_str更新失败，错误码：{request_status}')
-                return False
-
-            token = resp_data.get('data', {}).get('token')
-            if not token:
-                self.logger.error(f'token_str更新失败，token为空')
-                return False
-
-            self.token_str = token
-        except:
-            self.logger.error(f'token_str更新失败', exc_info=True)
-            return False
-
-    def anonymity_login(self) -> bool:
-        """ 匿名登录，获取token_str """
-
-        uri = '/v1/api/user/login/phone'
-
-        unix = self.get_timestamp()
-
-        user_data = self.__user_data.copy()
-        user_data['device_id'] = self.device_id
-        user_data['uuid'] = self.single_uuid
-        user_data['unix'] = unix
-
-        headers = self.__headers.copy()
-
-        data = {
-            "loginType": "3",
-            "adInfo": {}
-        }
-
-        yy = self.get_yy(
-            uri=uri,
-            unix=unix,
-            data=data,
-            user_data=user_data,
-            jsonfy=True,
-        )
-
-        headers["Yy"] = yy
-        headers["server_version"] = ''
-
-        query_str = self.build_query_string(user_data)
-
-        response = self.request_session.post(
-            self.base_host + uri + f'?{query_str}',
-            headers=headers,
-            json=data
-        )
-
-        resp_data = response.json()
-
-        token_str = resp_data.get('data', {}).get('token')
-        device_id = resp_data.get('data', {}).get('deviceID')
-        user_id = resp_data.get('data', {}).get('userID')
-
-        if token_str:
-            self.chat_id = None
-
-            self.token_str = token_str
-            self.__headers['Token'] = token_str
-            self.__device_id = device_id
-            self.__user_id = user_id
-            self.__device_info_expire = (int(time.time()) + 10800) * 1000
-
-            self.logger.info(f'成功获取到token_str：{token_str}')
-            return True
-
-        return False
-
-    def post(
-            self,
-            url: str,
-            headers: dict,
-            data: dict,
-            stream: bool = False,
-            multipart_encode: bool = False,
-    ) -> Optional[requests.Response]:
-        """
-        发送post请求，如果失败，则重新登录后再尝试，尝试两次
-        :param url: 请求url
-        :param headers: 请求头
-        :param data: 请求体
-        :param stream: 是否流式传输
-        :param multipart_encode: 是否使用multipart/form-data格式
-        :return:
-        """
-
-        for i in range(3):
-
-            if multipart_encode:
-                self.logger.info(f"使用multipart/form-data格式发送POST请求")
-
-                multipart_data = MultipartEncoder(data)
-                headers["Content-Type"] = multipart_data.content_type
-                headers["Token"] = self.token_str
-                response = self.request_session.post(
-                    url,
-                    headers=headers,
-                    data=multipart_data,
-                    stream=stream
-                )
-            else:
-                self.logger.info(f"使用json格式发送POST请求")
-
-                headers["Token"] = self.token_str
-                response = self.request_session.post(
-                    url,
-                    headers=headers,
-                    data=data,
-                    stream=stream
-                )
-
-            if response.status_code == 200:
-                self.logger.info(f"POST请求成功")
-                return response
-
-            self.logger.error(f"POST请求失败，状态码：{response.status_code}")
-            self.logger.error(f"POST请求失败，响应内容：{response.text}")
-
-            if not self.is_anonymous:
-                self.logger.info(f"并非匿名用户，不进行自动登录")
-                return
-
-            result = self.re_login_by_anonymous(data)
-            if not result:
-                self.logger.error(f"重新匿名登录失败，不再尝试发送POST请求")
-                return
-            self.logger.info(f"重新匿名登录成功，即将重新发送请求")
-
-        self.logger.error(f"请求3次仍然失败，退出")
-
-    def get(self, url: str, headers: dict, params: dict, stream: bool = False) -> Optional[requests.Response]:
-        pass
-
-    def update_device_id(
-            self,
-            request_uuid: str = None,
-            request_device_id: str = None,
-    ):
+    def update_device_id(self):
         """ 更新设备id """
 
-        uri = "/v1/api/user/device/register"
+        path = self.base_host + "/v1/api/user/device/register"
 
-        unix = self.get_timestamp()
+        data = self.__user_data.copy()
 
-        user_data = self.__user_data.copy()
-
-        user_data['uuid'] = request_uuid or self.single_uuid
-        user_data['device_id'] = request_device_id or self.__device_id
-        data = {"uuid": request_uuid or self.single_uuid}
-
-        user_data['unix'] = unix
-
-        headers = self.__headers.copy()
-
-        yy = self.get_yy(
-            user_data=user_data,
-            uri=uri,
-            data=data,
-            unix=unix,
-            jsonfy=True
-        )
-
-        headers["Yy"] = yy
-
-        query_str = self.build_query_string(user_data)
-        response = self.request_session.post(
-            self.base_host + uri + f'?{query_str}',
-            json=data,
-            headers=headers
-        )
+        data['uuid'] = self.single_uuid
 
+        response = requests.post(path, json=data, headers=self.__headers)
         resp_json = response.json()
-
         status_code = resp_json.get('statusInfo', {}).get('code')
 
         if status_code != 0:
             self.logger.error(f'获取设备信息出错')
             self.logger.info(f'响应数据: {resp_json}')
             raise RequestsError(resp_json)
 
         self.__device_id = resp_json.get('data', {}).get('deviceIDStr')
         self.__user_id = resp_json.get('data', {}).get('userID')
 
         if self.__device_id:
             self.logger.info(f'成功更新设备ID: 【{self.__device_id}】')
 
-            self.__device_info_expire = (int(time.time()) + 10800) * 1000
+            now = int(time.time())
+            self.__device_info_expire = now + 10800
 
             self.logger.info(f'成功更新设备过期时间: 【{self.__device_info_expire}】')
 
         if self.__user_id:
             self.logger.info(f'成功更新用户ID: 【{self.__user_id}】')
 
         # 响应数据示例
@@ -733,87 +475,57 @@
 
         full_uri = f"{uri}{uri.find('?') != -1 and '&' or '?'}{query_str}"
 
         yy = self.md5(f"{quote_plus(full_uri)}_{data_json}{self.md5(unix)}ooui")
 
         return yy
 
-    def check_request_info(
-            self, request_uuid: str = None,
-            request_device_id: str = None,
-            device_info_expire: int = 0,
-    ) -> bool:
-
-        """MinMax似乎并不检查请求时携带的device_id；但这里仍然带上"""
-
-        if not request_uuid or not request_device_id or not device_info_expire:
-            return False
-
-        now = int(time.time()) * 1000
-
-        if device_info_expire < now:
-            return False
-
-        self.__device_info_expire = device_info_expire
-        self.__device_id = request_device_id
-        self.__single_uuid = request_uuid
-        return True
-
     def ask(
             self,
             question: str,
             chat_id: str = None,
             callback_func=None,
             character_id: str = '1',
-            search_mode: Literal['0', '1'] = '0',
-            audio_output_dir: str = None,
+            search_mode: str = '0',
+            audio_output_dir: str = '',
             voice_id: str = 'male-botong',
-            request_uuid: str = None,
-            request_device_id: str = None,
-            device_info_expire: int = None,
     ) -> AiAnswer:
         """
         提问
         :param question: 问题
         :param chat_id: 会话ID
         :param callback_func: 回调函数，处理每一次回答的增量文本
         :param character_id: 角色id，目前固定为1
         :param search_mode: 搜索模式：1表示关闭；0表示开启
         :param audio_output_dir: 音频文件输出目录；不为空时将在AI交互之后生成音频
         :param voice_id: 配音音色ID
-        :param request_uuid: 配音音色ID
-        :param request_device_id: 配音音色ID
-        :param device_info_expire: 配音音色ID
-        :return: AiAnswer
+        :return:
         """
 
         if search_mode not in ['0', '1']:
             raise ValueError("search_mode参数错误，请传入0或1")
 
-        self.check_request_info(request_uuid, request_device_id, device_info_expire)
-
-        if chat_id:
-            self.logger.info(f'使用传入的会话ID: 【{chat_id}】')
-            self.chat_id = chat_id
+        self.chat_id = chat_id
 
         uri = "/v4/api/chat/msg"
 
         unix = self.get_timestamp()
 
         # 1. 处理请求参数
         user_data = self.__user_data.copy()
-
         user_data["uuid"] = self.single_uuid
         user_data["device_id"] = self.device_id
         user_data["unix"] = unix
 
         # 2. 处理请求体数据
         headers = self.__headers.copy()
-        referer = f'https://hailuoai.com/?chat={self.chat_id}' if self.chat_id else 'https://hailuoai.com/'
-        headers["Referer"] = referer
+
+        headers[
+            "Referer"] = f'https://hailuoai.com/?chat={self.chat_id}' if self.chat_id else 'https://hailuoai.com/'
+
         headers["Accept"] = 'text/event-stream'
 
         data = {
             "characterID": character_id,
             "msgContent": question,
             "chatID": self.chat_id if self.chat_id else '0',  # 为0时将新建对话
             "searchMode": search_mode,
@@ -824,85 +536,35 @@
             uri=uri,
             data=data,
             unix=unix
         )
 
         headers["Yy"] = yy
 
-        query_str = self.build_query_string(user_data)
-
-        for i in range(3):
-
-            try:
-                response = self.post(
-                    self.base_host + uri + f'?{query_str}',
-                    headers=headers,
-                    data=data,
-                    stream=True,
-                    multipart_encode=True,
-                )
-
-                # 请求失败，返回空对象
-                if not response:
-                    return AiAnswer()
-
-                self.parse_ask_result(
-                    response=response,
-                    callback_func=callback_func,
-                    audio_output_dir=audio_output_dir,
-                    voice_id=voice_id
-                )
-
-                return self.single_answer_obj
-            except NeedLoginError:
-
-                if not self.is_anonymous:
-                    self.logger.info('该用户并非匿名用户，不进行自动登录')
-                    return AiAnswer()
-
-                result = self.re_login_by_anonymous(data)
-                if not result:
-                    self.logger.error(f"重新匿名登录失败，AI回答获取失败，返回空对象")
-                    return AiAnswer()
-
-        self.logger.error(f"多次获取AI回答都失败，返回空对象")
-        return AiAnswer()
-
-    def re_login_by_anonymous(self, data: dict) -> bool:
-        """重新进行匿名登录"""
-
-        self.logger.info(f"尝试重新匿名登录...")
-        result = self.anonymity_login()
-
-        if not result:
-            self.logger.error(f"重新匿名登录失败")
-            return False
-
-        self.logger.info(f"重新匿名登录成功")
-        self.__headers["Token"] = self.token_str
-
-        # 匿名登录后，就没法保持原来的会话了
-        if 'chatID' in data:
-            data['chatID'] = '0'
-            self.chat_id = None
-            self.logger.info(f"原会话ID失效，已清除")
+        # 3. 将data转换为FormData格式
+        multipart_data = MultipartEncoder(data)
+        headers['Content-Type'] = multipart_data.content_type
 
-        return True
+        # 4. 发起请求
+        query_str = self.build_query_string(user_data)
+        response = requests.post(
+            self.base_host + uri + f'?{query_str}',
+            headers=headers,
+            data=multipart_data,
+            stream=True
+        )
 
-    def parse_ask_result(
-            self,
-            response: requests.Response,
-            callback_func,
-            audio_output_dir,
-            voice_id
-    ):
         index = 0
         pending = ""
         event = ""
 
+        if response.status_code != 200:
+            self.logger.error(f"请求失败，状态码：{response.status_code}")
+            raise NeedLoginError('请检查Token是否过期')
+
         for chunk in response.iter_lines():
 
             if not chunk:
                 continue
 
             index += 1
             chunk = chunk.decode("utf-8")
@@ -923,41 +585,60 @@
             # Incomplete chunk
             if not pending.endswith("}"):
                 self.logger.debug("The chunk is incomplete.")
                 continue
 
             self.logger.debug(f"The chunk is complete.")
 
-            # Remove the 'data:' prefix, convert JSON to dict
-            pending = pending[5:]
-            resp_json = json.loads(pending)
-            pending = ""
-
-            message_type = resp_json.get('type')
-            status_code = resp_json.get('statusInfo', {}).get('code')
-            error_message = resp_json.get('statusInfo', {}).get('message')
+            try:
 
-            if status_code == 0:
-                pass
-            else:
-                self.logger.error(f"解析请求数据时发送错误，状态码：【{status_code}】，消息：【{error_message}】")
-                raise NeedLoginError('error_message')
+                # Remove the 'data:' prefix, convert JSON to dict
+                pending = pending[5:]
+                resp_json = json.loads(pending)
+                pending = ""
 
-            if event == "send_result" and message_type == 1:
-                self.handle_send_result(resp_json)
-                continue
-            elif event == "message_result" and message_type == 2:
-                self.handle_message_result(resp_json, callback_func)
-                continue
-            elif event == "follow_up_question_result" and message_type == 4:
-                self.handle_follow_up_question_result(resp_json)
+                message_type = resp_json.get('type')
+                status_code = resp_json.get('statusInfo', {}).get('code')
+                error_message = resp_json.get('statusInfo', {}).get('message')
+
+                if status_code != 0:
+                    self.logger.error(f"请求失败，状态码：{status_code}，消息：{error_message}")
+                    continue
+
+                if event == "send_result" and message_type == 1:
+                    self.handle_send_result(resp_json)
+                    continue
+                elif event == "message_result" and message_type == 2:
+                    self.handle_message_result(resp_json, callback_func)
+                    continue
+                elif event == "follow_up_question_result" and message_type == 4:
+                    self.handle_follow_up_question_result(resp_json)
+                    continue
+                else:
+                    self.logger.error(f"MinMax响应出现未知数据，可能需要重新逆向，数据类型：{event}")
+                    self.logger.info(f"MinMax响应数据：{pending}")
+
+            except Exception:
+
+                request_url = self.base_host + uri
+
+                request_data = json.dumps(data)
+                request_response = pending
+                traceback_info = f"\n--- Error Log Entry ---\n{traceback.format_exc()}\n--- End of Entry ---\n"
+
+                all_data = (f"请求URL：\n{request_url}\n\n"
+                            f"请求头数据：\n{headers}\n\n"
+                            f"请求体数据：\n{request_data}\n\n"
+                            f"回信数据：\n{request_response}\n\n"
+                            f"调用栈信息：\n{traceback_info}")
+
+                file_path = self.save_bad_request_data('MinMax交互-出现未知错误', all_data)
+
+                self.logger.error(f"MinMax交互-出现未知错误，相关数据已写入【{file_path}】", exc_info=True)
                 continue
-            else:
-                self.logger.error(f"MinMax响应出现未知数据，可能需要重新逆向，数据类型：{event}")
-                self.logger.info(f"MinMax响应数据：{pending}")
 
         # 检查是否收到任何响应
         if index == 0:
             self.logger.error("MinMax请求没有收到任何响应")
 
         if audio_output_dir:
             audio_path_list = self.download_audios(output_dir=audio_output_dir, voice_id=voice_id)
@@ -967,55 +648,48 @@
                 return self.single_answer_obj
 
             self.logger.info(f"已将文本转为音频，存放到【{audio_output_dir}】，共计{len(audio_path_list)}条音频")
 
             self.single_answer_obj.audio_url_list = audio_path_list
             return self.single_answer_obj
 
+        return self.single_answer_obj
+
     def handle_follow_up_question_result(self, data: dict):
         """服务端返回最后总结信息"""
 
         self.single_answer = data.get('data', {}).get('messageResult', {}).get('content')
 
         reference_link_list = data.get('data', {}).get('extra', {}).get('netSearchStatus', {}).get('linkDetail', [])
 
-        self.single_answer_obj.is_success = True
-        self.single_answer_obj.content = self.single_answer
-        self.single_answer_obj.conversation_id = self.chat_id
-        self.single_answer_obj.reference_link_list = [ReferenceLink(
-            title=item['detail'],
-            url=item['url'],
-        ) for item in reference_link_list]
+        answer_obj = AiAnswer(
+            is_success=True,
+            content=self.single_answer,
+            conversation_id=self.chat_id,
+            reference_link_list=[ReferenceLink(
+                title=item['detail'],
+                url=item['url'],
+            ) for item in reference_link_list]
+        )
+
+        self.single_answer_obj = answer_obj
 
     def handle_message_result(self, data: dict, callback_func: callable = None):
         """服务端返回响应文本"""
 
         content = data.get('data', {}).get('messageResult', {}).get('content')
         self.single_padding = content.replace(self.single_answer, '')
         self.single_answer = content
 
-        if callable(callback_func):
+        if callback_func:
             try:
                 callback_func(self.single_padding)
             except:
                 self.logger.error("回调函数执行失败")
 
-        is_end = data.get('data', {}).get('messageResult', {}).get('isEnd')
-
-        if is_end == 0:
-            self.single_answer_obj.is_success = True
-            self.single_answer_obj.content = self.single_answer
-            self.single_answer_obj.conversation_id = self.chat_id
-
-        if is_end == 0 and callable(callback_func):
-            try:
-                callback_func(self.end_signal)
-            except:
-                self.logger.error("回调函数执行失败")
-
     def handle_send_result(self, data: dict):
         """服务端接收到用户文本，返回chatID等信息"""
 
         self.user_msg_id = data.get('data', {}).get('sendResult', {}).get('userMsgID')
         self.chat_id = data.get('data', {}).get('sendResult', {}).get('chatID')
         self.system_msg_id = data.get('data', {}).get('sendResult', {}).get('systemMsgID')
 
@@ -1254,15 +928,15 @@
 
     def login(
             self,
             phone: str,
             sms_code: str,
     ) -> bool:
         """
-        账号登录
+        登录
         :param phone: 手机号
         :param sms_code: 手机验证码
         :return: 登录成功时返回获取到的Token
         """
 
         if len(sms_code) != 6:
             self.logger.error(f"验证码长度错误")
@@ -1314,38 +988,34 @@
             return True
 
         except:
             self.logger.error(f"登录失败")
             return False
 
     def test(self):
-        unix = '1715584452000'
+        unix = '1715264091000'
 
         user_data = {
-            'device_platform': "web",
+            'msgID': 244977956405796869,
+            'timbre': "male-botong",
+            'device_platform': "zibuyu_llm_web",
             'app_id': "3001",
-            'uuid': 'e63d7053-82b5-4bca-b188-8c21d12b644a',  # uuid，待填充
-            'device_id': '246324378819584000',  # 设备ID，待填充
+            'uuid': '7c251825-9626-4e8a-81df-d8a3cbf58c50',  # uuid，待填充
+            'device_id': '244976245380423685',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
-            'server_version': "",
+            'server_version': "101",
             'device_memory': 8,
             'cpu_core_num': 8,
             'browser_language': "zh-CN",
             'browser_platform': "Win32",
             'screen_width': 1920,
             'screen_height': 1080,
             'unix': unix,  # 时间戳，待填充
         }
 
-        data = {"loginType": "3", "adInfo": {}}
+        data = {}
 
-        uri = '/v1/api/user/login/phone'
-        yy = self.get_yy(
-            uri=uri,
-            unix=unix,
-            user_data=user_data,
-            data=data,
-            jsonfy=True,
-        )
+        uri = '/v1/api/chat/msg_tts'
+        yy = self.get_yy(user_data=user_data, uri=uri, data=data, unix=unix, jsonfy=True)
         print(yy)
```

## zibuyu_llm_web/xunfei.py

```diff
@@ -2,21 +2,19 @@
 
 """
 --------------------------------------------
 project: zibuyu_LLM
 author: 子不语
 date: 2024/5/10
 contact: 【公众号】思维兵工厂
-description: 讯飞星火Web端。
-
-但出现因Token失效而导致的访问失败，会自动尝试重新登录。
+description: 
 --------------------------------------------
 """
 
-from typing import Optional, Union
+from typing import List, Optional
 from pathlib import Path
 import logging
 import base64
 import random
 import time
 import json
 import sys
@@ -27,21 +25,23 @@
 import numpy as np
 import requests
 import ddddocr
 import execjs
 
 from .base import LLMBase
 from .types import AiAnswer
-from .errors import LoginFailError, NeedLoginError, UnexpectResponseError
+from .errors import LoginFailError, APIConnectionError, NeedLoginError
 
 BASE_DIR = Path(__file__).parent
 STATIC_DIR = BASE_DIR / 'static_data'
 if not STATIC_DIR.exists():
     STATIC_DIR.mkdir(parents=True)
 
+JS_FILE_PATH = STATIC_DIR / 'generate_w.js'
+
 
 class GTrace(object):
     def __init__(self):
         self.__pos_x = []
         self.__pos_y = []
         self.__pos_z = []
 
@@ -172,30 +172,30 @@
         for idx in range(len(x)):
             result.append([int(x[idx]), int(y[idx]), int(z[idx])])
 
         return int(_distance), result
 
 
 class WebLogin(object):
-    """该类用于讯飞网页版登录，获取登录token"""
+    """
+    该类用于讯飞网页版登录，获取登录token
+    """
 
     def __init__(
             self,
             account_name: str,
             password: str,
             logger: logging.Logger = None,
-            generate_w_js_file_path: str = None,
     ):
         """
 
         :param account_name: 账号
         :param password: 密码
         """
 
-        self.generate_w_js_file_path = generate_w_js_file_path
         self.account_name = account_name
         self.password = password
         self.logger = logger or logging.getLogger(__name__)
 
         self.gt = ''
         self.challenge = ''
         self.c = ''
@@ -612,15 +612,15 @@
 
     def generate_w(self, target_bytes, background_bytes):
 
         res = self.get_slice_res(target_bytes, background_bytes)
         self.logger.info(f'【generate_w】识别结果：{res}')
 
         # 读取slide.js执行get_w()方法
-        with open(self.generate_w_js_file_path, 'r', encoding='utf-8') as f:
+        with open(JS_FILE_PATH, 'r', encoding='utf-8') as f:
             js = f.read()
 
         ctx = execjs.compile(js)
 
         gtrace = GTrace()
 
         # -10，图片不是从头部开始的
@@ -774,18 +774,14 @@
         self.logger.info(f'【get_cookie】请求响应数据：{response.text}')
 
         for k, v in self.session.cookies.items():
             print(f'{k}: {v}')
 
     def run(self):
 
-        if not self.generate_w_js_file_path:
-            print('缺少js解密文件')
-            return
-
         self.if_captcha()
         print(f"第一次请求，if_captcha")
 
         print('-'.center(50, '-'))
 
         self.get_gt_and_challenge()
         print(f"第二次请求，获取gt和challenge")
@@ -838,20 +834,15 @@
         self.login()
         print('-'.center(50, '-'))
 
         if self.sso_session_id:
             print(f"第十一次请求，获取cookie")
             self.get_cookie()
 
-    def get_session_id(self, generate_w_js_file_path: str = None):
-
-        self.generate_w_js_file_path = generate_w_js_file_path
-
-        if not self.generate_w_js_file_path:
-            raise Exception('缺少js解密文件')
+    def get_session_id(self):
 
         for i in range(3):
 
             self.if_captcha()
 
             self.get_gt_and_challenge()
 
@@ -885,49 +876,37 @@
 
 class XunFeiWeb(LLMBase):
     model_name = 'XunFeiWeb'
     base_url = 'https://xinghuo.xfyun.cn'
 
     def __init__(
             self,
-            cookie: str = None,
             account: str = None,
             password: str = None,
-            error_dir: str = None,
+            cookie: str = None,
             sso_session_id: str = None,
             logger_obj: logging.Logger = None,
-            generate_w_js_file_path: str = None,
+            error_dir: str = None,
             *args,
             **kwargs
     ):
-        """
-        :param generate_w_js_file_path: js解密文件
-        :param account: 账号
-        :param password: 密码
-        :param cookie: cookie
-        :param sso_session_id: ssoSessionId
-        :param logger_obj: 日志对象
-        :param error_dir: 错误保存目录
-        """
-
         self.logger = logger_obj
         self.account = account
         self.password = password
         self.cookie = cookie
         self._sso_session_id = sso_session_id
         self._account_id: str = ''
         self.__gt_token = ''
         self.error_dir = error_dir
-        self.generate_w_js_file_path = generate_w_js_file_path
 
         super().__init__()
         self.request_session.cookies.update(self.cookies_dict)
 
         if self._sso_session_id:
-            self.request_session.cookies.update('ssoSessionId', self._sso_session_id)
+            self.request_session.cookies.set('ssoSessionId', self._sso_session_id)
 
         self.__headers = {
             'Accept': "*/*",
             "Accept-Encoding": "gzip, deflate, br, zstd",
             "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
 
             "Cache-Control": "no-cache",
@@ -946,27 +925,25 @@
         self.chat_id: str = ''
         self.single_answer: str = ''
         self.single_answer_obj: Optional[AiAnswer] = None
         self.single_answer_padding: str = ''
 
     @property
     def account_id(self) -> str:
-        """ 获取cookie中的账号id """
 
         if self._account_id:
             return self._account_id
 
         result = self.login()
         if result:
             return self._account_id
         raise LoginFailError(f'{self.model_name} login failed')
 
     @property
     def sso_session_id(self) -> str:
-        """ 获取ssoSessionId """
 
         if self._sso_session_id:
             return self._sso_session_id
 
         result = self.login()
         if result:
             return self._sso_session_id
@@ -983,163 +960,96 @@
     def decode(text):
         try:
             decoded_data = base64.b64decode(text).decode('utf-8')
             return decoded_data
         except Exception as e:
             return ''
 
-    def check_response_status(self, response: requests.Response, jsonfy: bool, function_name: str = None):
-
-        result = {
-            'is_success': True,
-            'response': response,
-            'continue': True
-        }
-
-        if response.status_code == 200:
-            if jsonfy:
-                result['response'] = self.parse_data(response, function_name=function_name)
-
-        elif response.status_code == 401:
-            self.logger.error(f'The response status_code is 401, need to login again.')
-
-            self.logger.info('即将尝试重新登录...')
-            login_result = self.login()
-            if login_result:
-                self.logger.info('重新登录成功，即将重新请求...')
-                result['is_success'] = False
-
-            self.logger.error('重新登录失败，即将退出程序...')
-            result['continue'] = False
-
-        else:
-            self.logger.error(f'【{self.model_name}】 get failed, status_code: 【{response.status_code}】')
-            result['continue'] = False
-
-        return result
-
     def get(
             self,
             url: str,
             headers: dict = None,
             params: Optional[dict] = None,
-            function_name: str = None,
-            jsonfy: bool = False,
-    ) -> Optional[Union[requests.Response, dict]]:
+    ) -> Optional[requests.Response]:
 
         for i in range(3):
             try:
                 if not headers:
                     headers = self.__headers
-
                 response = self.request_session.get(
                     url,
                     headers=headers,
                     params=params,
                     verify=False,
                 )
 
-                check_result = self.check_response_status(response, jsonfy=jsonfy, function_name=function_name)
-
-                if check_result['is_success']:
-                    return check_result['response']
-                elif check_result['continue']:
-                    continue
+                if response.status_code == 200:
+                    return response
                 else:
-                    return
-
-            except NeedLoginError:
-
-                self.logger.info('即将尝试重新登录...')
-                result = self.login()
-
-                # 如果成功重新登录，则重新请求
-                if result:
-                    self.logger.info('重新登录成功，即将重新请求...')
-                    continue
-
-                # 如果登录失败，则跳出循环，直接返回
-                self.logger.error('重新登录失败，即将退出程序...')
-                break
-            except UnexpectResponseError:
-                # TODO 这里暂时留空，后续补充
-                pass
-
+                    self.logger.error(f'【{self.model_name}】 get failed, status_code: 【{response.status_code}】')
             except:
                 self.logger.error(f'【{self.model_name}】 get request got an unexpected error.', exc_info=True)
+        raise APIConnectionError(f'【{self.model_name}】 get request failed. URL: 【{url}】')
 
     def post(
             self,
             url: str,
             headers: dict = None,
             params: Optional[dict] = None,
-            _json: Optional[dict] = None,
+            json: Optional[dict] = None,
             data: [dict, str] = None,
-            stream=False,
-            function_name: str = None,
-            jsonfy: bool = False,
-    ) -> Optional[Union[requests.Response, dict]]:
+            stream=False
+    ) -> Optional[requests.Response]:
 
         # 防止网络错误，设置重试次数
         for i in range(3):
 
             try:
                 if not headers:
                     headers = self.__headers
 
                 response = self.request_session.post(
                     url,
                     headers=headers,
                     params=params,
-                    json=_json,
+                    json=json,
                     data=data,
                     stream=stream,
                     verify=False
                 )
 
-                check_result = self.check_response_status(response, jsonfy=jsonfy, function_name=function_name)
-
-                if check_result['is_success']:
-                    return check_result['response']
-                elif check_result['continue']:
-                    continue
+                if response.status_code == 200:
+                    return response
+                elif response.status_code == 401:
+                    self.logger.error(f'【{self.model_name}】 post failed, status_code: 【{response.status_code}】')
+                    self.logger.info('即将尝试重新登录...')
+                    result = self.login()
+                    if result:
+                        self.logger.info('重新登录成功，即将重新请求...')
+                        continue
+                    self.logger.error('重新登录失败，即将退出程序...')
+                    break
                 else:
-                    return
-
-            except NeedLoginError:
-
-                self.logger.info('即将尝试重新登录...')
-                result = self.login()
-
-                # 如果成功重新登录，则重新请求
-                if result:
-                    self.logger.info('重新登录成功，即将重新请求...')
-                    continue
-
-                # 如果登录失败，则跳出循环，直接返回
-                self.logger.error('重新登录失败，即将退出程序...')
-                break
-            except UnexpectResponseError:
-                # TODO 这里暂时留空，后续补充
-                self.logger.error('出现了预期外的回应数据...')
+                    self.logger.error(f'【{self.model_name}】 post failed, status_code: 【{response.status_code}】')
             except:
                 self.logger.error(f'【{self.model_name}】 post request got an unexpected error.', exc_info=True)
 
+        raise APIConnectionError(f'【{self.model_name}】 post request failed. URL: 【{url}】')
+
     def login(self) -> bool:
         """登录新方法，添加极验滑块的逆向"""
 
         try:
             handler = WebLogin(
                 account_name=self.account,
                 password=self.password,
             )
-            session_id = handler.get_session_id(self.generate_w_js_file_path)
+            session_id = handler.get_session_id()
 
             if session_id:
-                self.request_session.cookies.update({'ssoSessionId': session_id})
                 self.request_session.headers.update({'Cookie': f'ssoSessionId={session_id}'})
                 self._sso_session_id = session_id
                 return True
         except:
             self.logger.error(f'【{self.model_name}】 login failed', exc_info=True)
 
         return False
@@ -1168,156 +1078,137 @@
                 self.logger.error(
                     f'【{self.model_name}】 login failed, code: 【{code}】, message: 【{resp_json.get("desc")}】')
                 return False
 
             self.logger.info(f'【{self.model_name}】 login success')
 
             self._sso_session_id = data['ssoSessionId']
-            self._account_id = data['account_id']
-            self.request_session.cookies.update('ssoSessionId', data['ssoSessionId'])
-            self.request_session.cookies.update('account_id', data['account_id'])
+            self.request_session.cookies.set('ssoSessionId', data['ssoSessionId'])
+            self.request_session.cookies.set('account_id', data['account_id'])
 
             return True
         except:
             self.logger.error(f'【{self.model_name}】 login request got an unexpected error.', exc_info=True)
             return False
 
-    def get_chat_list(self) -> dict:
+    def get_chat_list(self) -> List[dict]:
         """获取会话列表"""
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/chat-list'
 
-        return self.get(url=url, function_name='get_chat_list', jsonfy=True)
+        response = self.get(url=url)
+        return self.parse_data(response.json(), 'get_chat_list')
 
     def get_prompt_list(self) -> dict:
         """
         获取提示列表
         :return：提示列表
         """
 
         url = self.base_url + '/iflygpt/u/prompt/getPromptList'
 
-        return self.get(url=url, function_name='get_prompt_list', jsonfy=True)
+        response = self.get(url)
+        return self.parse_data(response.json(), 'get_prompt_list')
 
     def get_chat_history(self, chat_id: [int, str]) -> dict:
         """
         获取会话记录
         :param chat_id：会话 ID
         :return：会话记录
         """
 
         url = self.base_url + f'/iflygpt/u/chat_history/all/{chat_id}'
 
-        data = self.get(url=url, function_name='get_chat_history', jsonfy=True)
-        return data.get('data', {})
+        response = self.get(url)
+
+        return self.parse_data(response.json(), 'get_chat_history')
 
-    def create_new_chat(self, chat_name: str = None, bot_id: str = None) -> str:
+    def create_new_chat(self, bot_id: str = None) -> str:
         """
         创建新的会话，注意，在新的会话窗口未被使用前，重复创建返回的chat_id是一样的
-        :return：成功时返回新建的chat_id；失败时返回空字符串
+        :return：chat_id
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/create-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
         if bot_id:
             data = json.dumps({"botId": bot_id})
         else:
             data = "{}"
 
-        data = self.post(url=url, headers=headers, data=data, function_name='create_new_chat', jsonfy=True)
-
-        if not data:
-            return ''
-
-        chat_id = data.get('data', {}).get('id')
+        response = self.post(url=url, headers=headers, data=data)
+        data = self.parse_data(response.json(), 'create_new_chat')
+        chat_id = data.get('id')
 
         if chat_id:
-
-            if chat_name:
-                self.rename_chat(chat_id, chat_name)
-
             self.chat_id = chat_id
             return chat_id
 
-    def rename_chat(self, chat_id: int, chat_name: str) -> dict:
+    def rename_chat(self, chat_id: int, name: str) -> bool:
         """
         重命名会话
         :param chat_id：会话 ID
-        :param chat_name：新的会话名
+        :param name：新的会话名
         :return：bool
         """
 
-        # 名称长度存在限制，截取前15个字符
-        chat_name = chat_name[:15]
-
         url = self.base_url + '/iflygpt/u/chat-list/v1/rename-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
-        _json = {'chatListId': chat_id, 'chatListName': chat_name}
+        _json = {'chatListId': chat_id, 'chatListName': name}
 
-        return self.post(url=url, headers=headers, _json=_json, function_name='rename_chat', jsonfy=True)
+        response = self.post(url=url, headers=headers, json=_json)
+        return self.parse_data(response.json(), 'rename_chat') or False
 
-    def delete_chat(self, chat_id: int) -> dict:
+    def delete_chat(self, chat_id: int) -> bool:
         """
         删除会话
         :param chat_id：会话 ID
         :return：bool
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/del-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
         _json = {'chatListId': chat_id}
 
-        return self.post(url=url, headers=headers, _json=_json, function_name='delete_chat', jsonfy=True)
+        response = self.post(url=url, headers=headers, json=_json)
+        return self.parse_data(response.json(), 'delete_chat') or False
 
     def get_chat_sid(self, chat_id: str) -> str:
         """
         通过会话id获取最新的机器人消息的sid；
         该值与chat_id一起确保了会话的上下文记忆
         新会话没有消息时，返回空字符串；
         """
 
         try:
             history_list = self.get_chat_history(chat_id)
             return history_list[-1]["historyList"][-1]["sid"]
         except:
             self.logger.error(f'【{self.model_name}】 get_chat_sid failed, chat_id: 【{chat_id}】')
 
-    def parse_data(self, response: Optional[requests.Response], function_name: str = None) -> dict:
-
-        if not response:
-            self.logger.error(f'【{self.model_name}】 search_bot failed.')
-            return {}
+    def parse_data(self, resp_json, function_name):
 
-        resp_json = response.json()
         code = resp_json.get('code')
         if code != 0:
             self.logger.error(
                 f'【{self.model_name}】 {function_name} failed, code: 【{code}】, message: 【{resp_json.get("desc")}】')
 
-            # 判断是否需要重新登录：80000错误表示token过期，需要重新登录
             if code == 80000:
-                msg = (f'【{self.model_name}】 {function_name} failed! Need re-login!\n\n'
-                       f'code: 【{code}】, message: 【{resp_json.get("desc")}】')
-                self.logger.error(msg)
-
-                raise NeedLoginError(msg)
-
-            # 非预期响应
-            msg = (f'【{self.model_name}】 {function_name} got an unexpected response.\n\n'
-                   f'code: 【{code}】, message: 【{resp_json.get("desc")}】\n\n'
-                   f'full data: 【{response.text}】\n\n')
-            self.logger.error(msg)
-            raise UnexpectResponseError(msg)
+                raise NeedLoginError(
+                    f'【{self.model_name}】 {function_name} failed!\n\ncode: 【{code}】, message: 【{resp_json.get("desc")}】')
 
-        return resp_json
+            raise Exception(
+                f'【{self.model_name}】 {function_name} got an unexpected error.\n\ncode: 【{code}】, message: 【{resp_json.get("desc")}】')
+
+        return resp_json.get('data')
 
     def ask(
             self,
             question: str,
             gt_token: str = None,
             chat_id: str = None,
             callback_func=None,
@@ -1360,15 +1251,15 @@
             'sid': self.get_chat_sid(chat_id),
             'GtToken': gt_token or self.gt_token,
             'clientType': client_type
         }
 
         response = self.post(url=url, headers=headers, data=data, stream=True)
 
-        if not response:
+        if response.status_code != 200:
             self.logger.error(f'【{self.model_name}】 ask failed, status_code: 【{response.status_code}】')
             return AiAnswer()
 
         self.single_answer = ''
         for line in response.iter_lines():
 
             if not line:
@@ -1380,16 +1271,15 @@
             if missing_padding != 0:
                 encoded_data += b'=' * (4 - missing_padding)
 
             if self.decode(encoded_data) != 'zw':
                 answer = self.decode(encoded_data).replace('\n\n', '\n')
 
                 if answer.startswith('```') and answer.endswith('```'):
-                    answer = ''
-                    # answer = '【任务执行中】'
+                    answer = '【任务执行中】'
 
                 self.single_answer_padding = answer
 
                 # 执行回调函数，如果有的话
                 if callable(callback_func):
                     try:
                         self.logger.debug(f"执行回调函数：内容【{answer}】")
@@ -1413,42 +1303,42 @@
             content=self.single_answer,
             is_success=True,
             conversation_id=chat_id,
         )
 
         return self.single_answer_obj
 
-    def search_bot(self, bot_name: str) -> dict:
+    def search_bot(self, bot_name: str):
         """根据名称搜索助手"""
 
         url = self.base_url + '/iflygpt/bot/search'
 
         data = {
             "searchValue": bot_name,
             "pageIndex": 1,
             "pageSize": 45,
             "botType": ""
         }
 
-        return self.post(url=url, _json=data, function_name='search_bot', jsonfy=True)
+        response = self.post(url=url, json=data)
+        return self.parse_data(response.json(), 'search_bot')
 
     def reset_bot(self, bot_id: str, chat_id: str):
         """
         【待完成】
         助手2.0重置话题
         """
         url = 'https://xinghuo.xfyun.cn/iflygpt/u/bot/v2/restart'
 
         params = {
             'botId': bot_id,
             'chatId': chat_id
         }
 
-        response = self.get(url=url, params=params, function_name='reset_bot')
-
+        response = self.get(url=url, params=params)
         return response.text
 
     def get_gt_token(self):
         """
         【待完成】
         对于gt_token，经分析是极验的风控，定时将旧的gt_token更换
         但讯飞似乎并没有进行验证
```

## Comparing `zibuyu_LLM-0.1.17.dist-info/METADATA` & `zibuyu_LLM-0.1.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.1.17
+Version: 0.1.9
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -37,24 +37,26 @@
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
 
 # 版本记录
 
-`0.1.16`：海螺问问添加鉴权出错重试机制
+`0.1.9`：讯飞星火部分添加自动鉴权
 
-`0.1.12`：讯飞星火添加请求出错重试机制
+`0.0.9`：修复由于类型注解引起的版本不兼容问题
 
-`0.1.11`：修改讯飞星火请求出错判断
+`0.0.8`：修复由于类型注解引起的版本不兼容问题
 
-`0.1.10`：修改bug
+`0.0.7`：统一各模型交互输出类型
 
-`0.1.9`：讯飞星火部分添加自动鉴权
+`0.0.6`：修改讯飞星火调用的传值
 
-`0.0.9`：修复由于类型注解引起的版本不兼容问题
+`0.0.5`：增加error与types模块
+
+`0.0.4`：修复导包路径问题
 
 `0.0.3`：修复导包路径问题
 
 `0.0.2`：无变化，增加Readme文件
 
 `0.0.1`：第一次上传
```

## Comparing `zibuyu_LLM-0.1.17.dist-info/RECORD` & `zibuyu_LLM-0.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 zibuyu_llm_api/__init__.py,sha256=Ox3V8_X8l52LqJ_ATAWv0xpxBZxq5o1xn16TcEvSUl4,305
 zibuyu_llm_api/minmax_api.py,sha256=6gZMHkmSfwsmbFtjkJF2W9uUX35zmdk1vLwIlcUuOJo,31879
 zibuyu_llm_web/__init__.py,sha256=1YEBJuq9b5XG8jUOtgdrMNDiSiHZ9_OCT6PxH_xDoiY,735
 zibuyu_llm_web/baichuan.py,sha256=lFq8jX7VwTBqB9EP31-H1Zj-WIiDWD4JScVMiq9yxUA,7376
 zibuyu_llm_web/base.py,sha256=C2BF_5tdCYt4XzWiWpQBlA3Gc3HfQS7suDl5yOVwGCU,7104
 zibuyu_llm_web/deepseek.py,sha256=b7buJU59WMri4qqulb_T2HuBEqsTtkoulI9M4aPRzpc,14789
-zibuyu_llm_web/errors.py,sha256=EPjEXZJTWyhUz-LLnTra7Rg6Qu2EjpdYog2_QE-iEs8,807
+zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
 zibuyu_llm_web/kimi.py,sha256=kWj7tUqTOyFsbe60bFhg6dcNdzNKtDQ0kAIxEvSFvdU,9962
-zibuyu_llm_web/minmax.py,sha256=5txD-su-rKH0dQzDuLYMIfZeqq6ZdN4ru9Or3_a_jjY,48418
+zibuyu_llm_web/minmax.py,sha256=TUbX4Dzn3JP9vNYdYdeYzcZIJgBK-tySdypHQF12URc,37747
 zibuyu_llm_web/qwen.py,sha256=ja3fyFtY6bQmjCWNtcOtgMIRt6RSgtuYmNxDCQBk5oU,37730
 zibuyu_llm_web/types.py,sha256=a_kIEwO3gK8tHgHqfYOi7ug2qNK9s54PDjEdm1Z5ZKg,5308
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
 zibuyu_llm_web/xinchen.py,sha256=PTkPhh-S8gsWr6ULAvJV2E2kwBtO95lKohyxQiGA_hE,14705
-zibuyu_llm_web/xunfei.py,sha256=s2DChDtksCVxlFLwqcei87rvAfvvmaBZuWig_yUdNno,59762
-zibuyu_LLM-0.1.17.dist-info/METADATA,sha256=WPDWrzCL3DRKuu7qv1DHHD827q4pBPfiUNaVlGFw4BM,1572
-zibuyu_LLM-0.1.17.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.1.17.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.1.17.dist-info/RECORD,,
+zibuyu_llm_web/xunfei.py,sha256=3PtnE7Tv9Hs1r4AAUfPkGXnVmJIlEWB28h1JQ1_1sPo,55663
+zibuyu_LLM-0.1.9.dist-info/METADATA,sha256=4RikLUzMc_jtRXXy8MfEQ7W0a5aPZkASb55eRVJqOYU,1621
+zibuyu_LLM-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.1.9.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.1.9.dist-info/RECORD,,
```


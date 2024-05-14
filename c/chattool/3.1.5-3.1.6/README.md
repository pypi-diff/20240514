# Comparing `tmp/chattool-3.1.5.tar.gz` & `tmp/chattool-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattool-3.1.5.tar", last modified: Fri Apr  5 16:35:38 2024, max compression
+gzip compressed data, was "chattool-3.1.6.tar", last modified: Tue May 14 15:58:42 2024, max compression
```

## Comparing `chattool-3.1.5.tar` & `chattool-3.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 16:35:27.000000 chattool-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-05 16:35:38.230668 chattool-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-05 16:35:27.000000 chattool-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/chattool/
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/asynctool.py
--rw-r--r--   0 runner    (1001) docker     (127)    20497 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/chattype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/functioncall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/tokencalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/chattool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:35:38.230668 chattool-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 16:35:27.000000 chattool-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 15:58:34.000000 chattool-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-14 15:58:42.293391 chattool-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-14 15:58:34.000000 chattool-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/chattool/
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/asynctool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20511 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/chattype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/functioncall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/tokencalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/chattool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:58:42.293391 chattool-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 15:58:34.000000 chattool-3.1.6/setup.py
```

### Comparing `chattool-3.1.5/LICENSE` & `chattool-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/PKG-INFO` & `chattool-3.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.5
+Version: 3.1.6
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
@@ -23,15 +23,15 @@
         
         <div align="center">
             <img src="https://qiniu.wzhecnu.cn/PicBed6/picgo/chattool.jpeg" alt="ChatAPI Toolkit" width="360", style="border-radius: 20px;">
         
         [English](README_en.md) | [简体中文](README.md)
         </div>
         
-        基于 API 的简单封装，支持多轮对话，代理，以及异步处理数据等。
+        基于 OpenAI API 的 `Chat` 对象，支持多轮对话，代理，以及异步处理数据等。
         
         ## 安装方法
         
         ```bash
         pip install chattool --upgrade
         ```
         
@@ -43,21 +43,27 @@
         
         ```bash
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         export OPENAI_API_BASE="https://api.example.com/v1"
         export OPENAI_API_BASE_URL="https://api.example.com" # 可选
         ```
         
-        Win 在系统中设置环境变量。
+        或者在代码中设置：
         
-        注：环境变量中，`OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
+        ```py
+        import chattool
+        chattool.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        chattool.api_base = "https://api.example.com/v1"
+        ```
+        
+        注：环境变量 `OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
         
         ### 示例
         
-        示例1，模拟多轮对话：
+        示例1，多轮对话：
         
         ```python
         # 初次对话
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse()
         
         # 继续对话
@@ -71,15 +77,15 @@
         # 保存对话内容
         chat.save("chat.json", mode="w") # 默认为 "a"
         
         # 打印对话历史
         chat.print_log()
         ```
         
-        示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
+        示例2，批量处理数据（串行），并使用缓存文件 `chat.jsonl`：
         
         ```python
         # 编写处理函数
         def data2chat(msg):
             chat = Chat()
             chat.system("你是一个熟练的数字翻译家。")
             chat.user(f"请将该数字翻译为罗马数字：{msg}")
@@ -105,15 +111,15 @@
             # 注意，这里不需要 getresponse 而交给异步处理
             return chat
         
         async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
         chats = load_chats("async_chat.jsonl")
         ```
         
-        在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+        在 Jupyter Notebook 中运行，因其[特殊机制](https://stackoverflow.com/questions/47518874/how-do-i-run-python-asyncio-code-in-a-jupyter-notebook)，需使用 `await` 关键字和 `wait=True` 参数：
         
         ```python
         await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
         ```
         
         示例4，使用工具（自定义函数）：
         
@@ -141,26 +147,24 @@
         
         ## 开源协议
         
         这个项目使用 MIT 协议开源。
         
         ## 更新日志
         
-        当前版本为 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能。
-        
-        ### 测试版本
-        - 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
+        - 版本 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能
+        - 版本 `2.0.0` 开始，更名为 `chattool`
+        - 版本 `1.0.0` 开始，支持异步处理数据
+        - 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
+        - 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
+        - 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
         - 版本 `0.3.0` 开始不依赖模块 `openai.py` ，而是直接使用 `requests` 发送请求
             - 支持对每个 `Chat` 使用不同 API 密钥
             - 支持使用代理链接
-        - 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
-        - 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
-        - 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
-        - 版本 `1.0.0` 开始，支持异步处理数据
-        - 版本 `2.0.0` 开始，模块更名为 `chattool`
+        - 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
 Keywords: chattool
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chattool-3.1.5/README.md` & `chattool-3.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 <div align="center">
     <img src="https://qiniu.wzhecnu.cn/PicBed6/picgo/chattool.jpeg" alt="ChatAPI Toolkit" width="360", style="border-radius: 20px;">
 
 [English](README_en.md) | [简体中文](README.md)
 </div>
 
-基于 API 的简单封装，支持多轮对话，代理，以及异步处理数据等。
+基于 OpenAI API 的 `Chat` 对象，支持多轮对话，代理，以及异步处理数据等。
 
 ## 安装方法
 
 ```bash
 pip install chattool --upgrade
 ```
 
@@ -35,21 +35,27 @@
 
 ```bash
 export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
 export OPENAI_API_BASE="https://api.example.com/v1"
 export OPENAI_API_BASE_URL="https://api.example.com" # 可选
 ```
 
-Win 在系统中设置环境变量。
+或者在代码中设置：
 
-注：环境变量中，`OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
+```py
+import chattool
+chattool.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+chattool.api_base = "https://api.example.com/v1"
+```
+
+注：环境变量 `OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
 
 ### 示例
 
-示例1，模拟多轮对话：
+示例1，多轮对话：
 
 ```python
 # 初次对话
 chat = Chat("Hello, GPT-3.5!")
 resp = chat.getresponse()
 
 # 继续对话
@@ -63,15 +69,15 @@
 # 保存对话内容
 chat.save("chat.json", mode="w") # 默认为 "a"
 
 # 打印对话历史
 chat.print_log()
 ```
 
-示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
+示例2，批量处理数据（串行），并使用缓存文件 `chat.jsonl`：
 
 ```python
 # 编写处理函数
 def data2chat(msg):
     chat = Chat()
     chat.system("你是一个熟练的数字翻译家。")
     chat.user(f"请将该数字翻译为罗马数字：{msg}")
@@ -97,15 +103,15 @@
     # 注意，这里不需要 getresponse 而交给异步处理
     return chat
 
 async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
 chats = load_chats("async_chat.jsonl")
 ```
 
-在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+在 Jupyter Notebook 中运行，因其[特殊机制](https://stackoverflow.com/questions/47518874/how-do-i-run-python-asyncio-code-in-a-jupyter-notebook)，需使用 `await` 关键字和 `wait=True` 参数：
 
 ```python
 await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
 ```
 
 示例4，使用工具（自定义函数）：
 
@@ -133,19 +139,17 @@
 
 ## 开源协议
 
 这个项目使用 MIT 协议开源。
 
 ## 更新日志
 
-当前版本为 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能。
-
-### 测试版本
-- 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
+- 版本 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能
+- 版本 `2.0.0` 开始，更名为 `chattool`
+- 版本 `1.0.0` 开始，支持异步处理数据
+- 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
+- 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
+- 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
 - 版本 `0.3.0` 开始不依赖模块 `openai.py` ，而是直接使用 `requests` 发送请求
     - 支持对每个 `Chat` 使用不同 API 密钥
     - 支持使用代理链接
-- 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
-- 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
-- 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
-- 版本 `1.0.0` 开始，支持异步处理数据
-- 版本 `2.0.0` 开始，模块更名为 `chattool`
+- 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
```

### Comparing `chattool-3.1.5/chattool/asynctool.py` & `chattool-3.1.6/chattool/asynctool.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/chattype.py` & `chattool-3.1.6/chattool/chattype.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def add(self, role:str, **kwargs):
         """Add a message to the chat log"""
         assert role in ['user', 'assistant', 'system', 'function'],\
             f"role should be one of ['user', 'assistant', 'system', 'function'], but got {role}"
         self._chat_log.append({'role':role, **kwargs})
         return self
 
-    def user(self, content:str):
+    def user(self, content: Union[List, str]):
         """User message"""
         return self.add('user', content=content)
     
     def assistant(self, content:Union[None, str], function_call:Union[None, Dict]=None):
         """Assistant message"""
         if function_call is not None:
             assert isinstance(function_call, dict), "function_call should be a dict"
@@ -507,15 +507,15 @@
                 if strline == '[DONE]': break
                 # skip empty line
                 if not strline: continue
                 # read the json string
                 try:
                     # wrap the response
                     resp = Resp(json.loads(strline))
-                    # stop if the response is finished
-                    if resp.finish_reason == 'stop': break
                     # deal with the message
                     if 'content' not in resp.delta: continue
                     yield resp
+                    # stop if the response is finished
+                    if resp.finish_reason == 'stop': break
                 except Exception as e:
                     print(f"Error: {e}, line: {strline}")
                     break
```

### Comparing `chattool-3.1.5/chattool/checkpoint.py` & `chattool-3.1.6/chattool/checkpoint.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/finetune.py` & `chattool-3.1.6/chattool/finetune.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/functioncall.py` & `chattool-3.1.6/chattool/functioncall.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/proxy.py` & `chattool-3.1.6/chattool/proxy.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/request.py` & `chattool-3.1.6/chattool/request.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/response.py` & `chattool-3.1.6/chattool/response.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool/tokencalc.py` & `chattool-3.1.6/chattool/tokencalc.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.5/chattool.egg-info/PKG-INFO` & `chattool-3.1.6/chattool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.5
+Version: 3.1.6
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
@@ -23,15 +23,15 @@
         
         <div align="center">
             <img src="https://qiniu.wzhecnu.cn/PicBed6/picgo/chattool.jpeg" alt="ChatAPI Toolkit" width="360", style="border-radius: 20px;">
         
         [English](README_en.md) | [简体中文](README.md)
         </div>
         
-        基于 API 的简单封装，支持多轮对话，代理，以及异步处理数据等。
+        基于 OpenAI API 的 `Chat` 对象，支持多轮对话，代理，以及异步处理数据等。
         
         ## 安装方法
         
         ```bash
         pip install chattool --upgrade
         ```
         
@@ -43,21 +43,27 @@
         
         ```bash
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         export OPENAI_API_BASE="https://api.example.com/v1"
         export OPENAI_API_BASE_URL="https://api.example.com" # 可选
         ```
         
-        Win 在系统中设置环境变量。
+        或者在代码中设置：
         
-        注：环境变量中，`OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
+        ```py
+        import chattool
+        chattool.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        chattool.api_base = "https://api.example.com/v1"
+        ```
+        
+        注：环境变量 `OPENAI_API_BASE` 优先于 `OPENAI_API_BASE_URL`，二者选其一即可。
         
         ### 示例
         
-        示例1，模拟多轮对话：
+        示例1，多轮对话：
         
         ```python
         # 初次对话
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse()
         
         # 继续对话
@@ -71,15 +77,15 @@
         # 保存对话内容
         chat.save("chat.json", mode="w") # 默认为 "a"
         
         # 打印对话历史
         chat.print_log()
         ```
         
-        示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
+        示例2，批量处理数据（串行），并使用缓存文件 `chat.jsonl`：
         
         ```python
         # 编写处理函数
         def data2chat(msg):
             chat = Chat()
             chat.system("你是一个熟练的数字翻译家。")
             chat.user(f"请将该数字翻译为罗马数字：{msg}")
@@ -105,15 +111,15 @@
             # 注意，这里不需要 getresponse 而交给异步处理
             return chat
         
         async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
         chats = load_chats("async_chat.jsonl")
         ```
         
-        在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+        在 Jupyter Notebook 中运行，因其[特殊机制](https://stackoverflow.com/questions/47518874/how-do-i-run-python-asyncio-code-in-a-jupyter-notebook)，需使用 `await` 关键字和 `wait=True` 参数：
         
         ```python
         await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
         ```
         
         示例4，使用工具（自定义函数）：
         
@@ -141,26 +147,24 @@
         
         ## 开源协议
         
         这个项目使用 MIT 协议开源。
         
         ## 更新日志
         
-        当前版本为 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能。
-        
-        ### 测试版本
-        - 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
+        - 版本 `2.3.0`，支持调用外部工具，异步处理数据，以及模型微调功能
+        - 版本 `2.0.0` 开始，更名为 `chattool`
+        - 版本 `1.0.0` 开始，支持异步处理数据
+        - 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
+        - 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
+        - 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
         - 版本 `0.3.0` 开始不依赖模块 `openai.py` ，而是直接使用 `requests` 发送请求
             - 支持对每个 `Chat` 使用不同 API 密钥
             - 支持使用代理链接
-        - 版本 `0.4.0` 开始，工具维护转至 [CubeNLP](https://github.com/cubenlp) 组织账号
-        - 版本 `0.5.0` 开始，支持使用 `process_chats` 处理数据，借助 `msg2chat` 函数以及 `checkpoint` 文件
-        - 版本 `0.6.0` 开始，支持 [function call](https://platform.openai.com/docs/guides/gpt/function-calling) 功能
-        - 版本 `1.0.0` 开始，支持异步处理数据
-        - 版本 `2.0.0` 开始，模块更名为 `chattool`
+        - 版本 `0.2.0` 改用 `Chat` 类型作为中心交互对象
 Keywords: chattool
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chattool-3.1.5/setup.py` & `chattool-3.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '3.1.5'
+VERSION = '3.1.6'
 
 requirements = [
     'Click>=7.0', 'requests>=2.20', "responses>=0.23", 'aiohttp>=3.8',
     'tqdm>=4.60', 'docstring_parser>=0.10', "python-dotenv>=0.17.0"]
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
```


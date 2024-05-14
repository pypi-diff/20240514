# Comparing `tmp/xiaogpt-2.70.tar.gz` & `tmp/xiaogpt-2.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.70.tar", last modified: Fri May  3 05:30:50 2024, max compression
+gzip compressed data, was "xiaogpt-2.71.tar", last modified: Tue May 14 03:27:27 2024, max compression
```

## Comparing `xiaogpt-2.70.tar` & `xiaogpt-2.71.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-03 05:30:43.428077 xiaogpt-2.70/LICENSE
--rw-r--r--   0        0        0    22452 2024-05-03 05:30:43.428077 xiaogpt-2.70/README.md
--rw-r--r--   0        0        0     3987 2024-05-03 05:30:50.091982 xiaogpt-2.70/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1252 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0      708 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/llama_bot.py
--rw-r--r--   0        0        0      822 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/moonshot_bot.py
--rw-r--r--   0        0        0     2289 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0      784 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/yi_bot.py
--rw-r--r--   0        0        0     5899 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/cli.py
--rw-r--r--   0        0        0     7006 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/utils.py
--rw-r--r--   0        0        0    16525 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    28501 1970-01-01 00:00:00.000000 xiaogpt-2.70/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-14 03:27:23.184762 xiaogpt-2.71/LICENSE
+-rw-r--r--   0        0        0    23909 2024-05-14 03:27:23.184762 xiaogpt-2.71/README.md
+-rw-r--r--   0        0        0     3829 2024-05-14 03:27:27.328760 xiaogpt-2.71/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1160 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3660 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5711 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6734 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16525 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 xiaogpt-2.71/PKG-INFO
```

### Comparing `xiaogpt-2.70/LICENSE` & `xiaogpt-2.71/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/README.md` & `xiaogpt-2.71/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 - [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
 - [01](https://platform.lingyiwanwu.com/apikeys)
 - [Llama3](https://console.groq.com/docs/quickstart)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
 
-| 系统和Shell  | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
-|------------|------------------------------------------------|----------------------------------------|------------------------------------------------|
+| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
 | 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
 | 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
 | 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
 | 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
@@ -131,88 +131,81 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
-## config.json
+## config.yaml
 
-如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
+如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 Yaml 或 JSON 格式
 参数优先级
 
 - cli args > default > config
 
 ```shell
-python3 xiaogpt.py --config xiao_config.json
+python3 xiaogpt.py --config xiao_config.yaml
 # or
-xiaogpt --config xiao_config.json
+xiaogpt --config xiao_config.yaml
 ```
 
 或者
 
 ```shell
-cp xiao_config.json.example xiao_config.json
+cp xiao_config.yaml.example xiao_config.yaml
 python3 xiaogpt.py
 ```
 
-若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在config.json中指定：
+若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在 config.yaml 中指定：
 
-```json
-{
-    ...
-    "gpt_options": {
-        "temperature": 0.9,
-        "top_p": 0.9,
-    }
-}
+```yaml
+gpt_options:
+  temperature: 0.9
+  top_p: 0.9
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数             | 说明                                                                                                       | 默认值 | 可选值 |
-|------------------|-----------------------------------------------------------------------------------------------------------|--------|--------|
-| hardware         | 设备型号                                                                                                   |        |        |
-| account          | 小爱账户                                                                                                   |        |        |
-| password         | 小爱账户密码                                                                                               |        |        |
-| openai_key       | openai的apikey                                                                                             |        |        |
-| moonshot_api_key | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |        |        |
-| yi_api_key       | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |        |        |
-| llama_api_key       | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                             |        |        |
-| serpapi_api_key  | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |        |        |
-| glm_key          | chatglm 的 apikey                                                                                          |        |        |
-| gemini_key       | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |        |        |
-| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
-| mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
-| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
-| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
-| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                  |
-| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
-| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                                  |
-| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                  |
-| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                  |
-| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                  |
-| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                  |
-| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                  |
-| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                  |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                  |
-| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
-| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-[这里]: <https://github.com/acheong08/EdgeGPT#getting-authentication-required>
+| 参数                  | 说明                                                                                                       | 默认值                                                                                                    | 可选值                                                           |
+| --------------------- | ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
+| hardware              | 设备型号                                                                                                   |                                                                                                           |                                                                  |
+| account               | 小爱账户                                                                                                   |                                                                                                           |                                                                  |
+| password              | 小爱账户密码                                                                                               |                                                                                                           |                                                                  |
+| openai_key            | openai的apikey                                                                                             |                                                                                                           |                                                                  |
+| moonshot_api_key      | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |                                                                                                           |                                                                  |
+| yi_api_key            | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |                                                                                                           |                                                                  |
+| llama_api_key         | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                          |                                                                                                           |                                                                  |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |                                                                                                           |                                                                  |
+| glm_key               | chatglm 的 apikey                                                                                          |                                                                                                           |                                                                  |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |                                                                                                           |                                                                  |
+| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                |                                                                                                           |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)                |                                                                                                           |                                                                  |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                                              |                                                                                                           |                                                                  |
+| mi_did                | 设备did                                                                                                    |                                                                                                           |                                                                  |
+| use_command           | 使用 MI command 与小爱交互                                                                                 | `false`                                                                                                   |                                                                  |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                                     | `true`                                                                                                    |                                                                  |
+| verbose               | 是否打印详细日志                                                                                           | `false`                                                                                                   |                                                                  |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                                 | `chatgptapi`                                                                                              |                                                                  |
+| tts                   | 使用的 TTS 类型                                                                                            | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                                |                                                                                                           |                                                                  |
+| prompt                | 自定义prompt                                                                                               | `请用100字以内回答`                                                                                       |                                                                  |
+| keyword               | 自定义请求词列表                                                                                           | `["请"]`                                                                                                  |                                                                  |
+| change_prompt_keyword | 更改提示词触发列表                                                                                         | `["更改提示词"]`                                                                                          |                                                                  |
+| start_conversation    | 开始持续对话关键词                                                                                         | `开始持续对话`                                                                                            |                                                                  |
+| end_conversation      | 结束持续对话关键词                                                                                         | `结束持续对话`                                                                                            |                                                                  |
+| stream                | 使用流式响应，获得更快的响应                                                                               | `true`                                                                                                    |                                                                  |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                                        | ""                                                                                                        |                                                                  |
+| gpt_options           | OpenAI API 的参数字典                                                                                      | `{}`                                                                                                      |                                                                  |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                                          | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                                            | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取                        |                                                                                                           |                                                                  |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取                        |                                                                                                           |
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
 4. 在wsl使用时, 需要设置代理为 <http://wls的ip:port(vpn的代理端口)>, 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
@@ -250,21 +243,21 @@
 ```
 
 ### 使用配置文件
 
 xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
 
 ```shell
-docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 ### 网络使用 host 模型
 
 ```shell
-docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 ### 本地编译Docker Image
 
 ```shell
  docker build -t xiaogpt .
 ```
@@ -289,32 +282,30 @@
 [azure-tts](https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/9-more-realistic-ai-voices-for-conversations-now-generally/ba-p/4099471) 提供了微软 azure tts 的能力
 [openai-tts](https://platform.openai.com/docs/guides/text-to-speech) 提供了类似 openai tts 的能力
 
 #### Usage
 
 你可以通过参数 `tts`, 来启用它
 
-```json
-{
-  "tts": "edge",
-}
+```yaml
+tts: edge
 ```
 
 For edge 查看更多语言支持, 从中选择一个
 
 ```shell
 edge-tts --list-voices
 ```
 
 #### 在容器中使用 edge-tts/azure-tts/openai-tts/volc/google/baidu
 
 由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
 
 ```shell
-docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
 ## 推荐的 fork
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
```

### Comparing `xiaogpt-2.70/pyproject.toml` & `xiaogpt-2.71/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 dependencies = [
     "miservice_fork",
     "openai>=1",
     "aiohttp",
     "rich",
     "zhipuai>=2.0.1",
     "httpx[socks]",
-    "EdgeGPT==0.1.26",
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
     "groq>=0.5.0",
+    "pyyaml>=6.0.1",
 ]
 dynamic = []
-version = "2.70"
+version = "2.71"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -46,94 +46,88 @@
     "aiosignal==1.3.1",
     "annotated-types==0.6.0",
     "anyio==4.3.0",
     "async-timeout==4.0.3 ; python_version < \"3.11\"",
     "attrs==23.2.0",
     "azure-cognitiveservices-speech==1.37.0",
     "beautifulsoup4==4.12.3",
-    "bingimagecreator==0.5.0",
     "cachetools==5.3.2",
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
     "click==8.1.7",
     "colorama==0.4.6 ; platform_system == \"Windows\"",
-    "dashscope==1.18.0",
+    "dashscope==1.19.0",
     "dataclasses-json==0.6.3",
     "distro==1.9.0",
     "edge-tts==6.1.10",
-    "edgegpt==0.1.26",
     "exceptiongroup==1.2.0 ; python_version < \"3.11\"",
     "frozenlist==1.4.1",
-    "google-ai-generativelanguage==0.6.2",
+    "google-ai-generativelanguage==0.6.3",
     "google-api-core==2.15.0",
     "google-api-core[grpc]==2.15.0",
     "google-api-python-client==2.125.0",
     "google-auth==2.26.1",
     "google-auth-httplib2==0.2.0",
     "google-cloud-texttospeech==2.16.3",
-    "google-generativeai==0.5.2",
+    "google-generativeai==0.5.3",
     "google-search-results==2.4.2",
     "googleapis-common-protos==1.62.0",
     "greenlet==3.0.3 ; platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\"",
     "groq==0.5.0",
     "grpcio==1.60.0",
     "grpcio-status==1.60.0",
     "h11==0.14.0",
     "httpcore==1.0.5",
     "httplib2==0.22.0",
     "httpx==0.27.0",
     "httpx[socks]==0.27.0",
     "idna==3.7",
     "jsonpatch==1.33",
     "jsonpointer==2.4",
-    "langchain==0.1.17",
-    "langchain-community==0.0.36",
-    "langchain-core==0.1.50",
+    "langchain==0.1.20",
+    "langchain-community==0.0.38",
+    "langchain-core==0.1.52",
     "langchain-text-splitters==0.0.1",
     "langsmith==0.1.45",
     "markdown-it-py==3.0.0",
     "marshmallow==3.20.1",
     "mdurl==0.1.2",
     "miservice-fork==2.4.3",
     "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
     "numexpr==2.10.0",
     "numpy==1.26.3",
-    "openai==1.25.1",
+    "openai==1.29.0",
     "orjson==3.10.0",
     "packaging==23.2",
-    "prompt-toolkit==3.0.43",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
     "pyasn1==0.5.1",
     "pyasn1-modules==0.3.0",
     "pydantic==2.5.3",
     "pydantic-core==2.14.6",
     "pygments==2.17.2",
     "pyjwt==2.8.0",
     "pyparsing==3.1.2 ; python_version > \"3.0\"",
     "pyyaml==6.0.1",
-    "regex==2023.12.25",
     "requests==2.31.0",
     "rich==13.7.1",
     "rsa==4.9",
     "sniffio==1.3.0",
     "socksio==1.0.0",
     "soupsieve==2.5",
     "sqlalchemy==2.0.25",
     "tenacity==8.2.3",
     "tetos==0.2.1",
     "tqdm==4.66.1",
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
-    "wcwidth==0.2.13",
-    "websockets==12.0",
     "yarl==1.9.4",
     "zhipuai==2.0.1.20240423.1",
 ]
 
 [tool.pdm]
 plugins = [
     "pdm-autoexport",
```

### Comparing `xiaogpt-2.70/xiaogpt/bot/__init__.py` & `xiaogpt-2.71/xiaogpt/bot/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.bot.chatgptapi_bot import ChatGPTBot
 from xiaogpt.bot.doubao_bot import DoubaoBot
 from xiaogpt.bot.gemini_bot import GeminiBot
 from xiaogpt.bot.glm_bot import GLMBot
 from xiaogpt.bot.langchain_bot import LangChainBot
-from xiaogpt.bot.newbing_bot import NewBingBot
-from xiaogpt.bot.qwen_bot import QwenBot
+from xiaogpt.bot.llama_bot import LlamaBot
 from xiaogpt.bot.moonshot_bot import MoonshotBot
+from xiaogpt.bot.qwen_bot import QwenBot
 from xiaogpt.bot.yi_bot import YiBot
-from xiaogpt.bot.llama_bot import LlamaBot
 from xiaogpt.config import Config
 
 BOTS: dict[str, type[BaseBot]] = {
-    "newbing": NewBingBot,
     "chatgptapi": ChatGPTBot,
     "glm": GLMBot,
     "gemini": GeminiBot,
     "qwen": QwenBot,
     "langchain": LangChainBot,
     "doubao": DoubaoBot,
     "moonshot": MoonshotBot,
@@ -32,15 +30,14 @@
         return BOTS[config.bot].from_config(config)
     except KeyError:
         raise ValueError(f"Unsupported bot {config.bot}, must be one of {list(BOTS)}")
 
 
 __all__ = [
     "ChatGPTBot",
-    "NewBingBot",
     "GLMBot",
     "GeminiBot",
     "MoonshotBot",
     "QwenBot",
     "get_bot",
     "LangChainBot",
     "DoubaoBot",
```

### Comparing `xiaogpt-2.70/xiaogpt/bot/base_bot.py` & `xiaogpt-2.71/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.71/xiaogpt/bot/chatgptapi_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 if TYPE_CHECKING:
     import openai
 
 
 @dataclasses.dataclass
 class ChatGPTBot(ChatHistoryMixin, BaseBot):
     name: ClassVar[str] = "ChatGPT"
-    default_options: ClassVar[dict[str, str]] = {"model": "gpt-3.5-turbo"}
+    default_options: ClassVar[dict[str, str]] = {"model": "gpt-4o-2024-05-13"}
     openai_key: str
     api_base: str | None = None
     proxy: str | None = None
     deployment_id: str | None = None
     history: list[tuple[str, str]] = dataclasses.field(default_factory=list, init=False)
 
     def _make_openai_client(self, sess: httpx.AsyncClient) -> openai.AsyncOpenAI:
```

### Comparing `xiaogpt-2.70/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.71/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.71/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.71/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.71/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/llama_bot.py` & `xiaogpt-2.71/xiaogpt/bot/llama_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/moonshot_bot.py` & `xiaogpt-2.71/xiaogpt/bot/moonshot_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.71/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/bot/yi_bot.py` & `xiaogpt-2.71/xiaogpt/bot/yi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/cli.py` & `xiaogpt-2.71/xiaogpt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,14 @@
         "--use_langchain",
         dest="bot",
         action="store_const",
         const="langchain",
         help="if use langchain",
     )
     bot_group.add_argument(
-        "--use_newbing",
-        dest="bot",
-        action="store_const",
-        const="newbing",
-        help="if use newbing",
-    )
-    bot_group.add_argument(
         "--use_glm",
         dest="bot",
         action="store_const",
         const="glm",
         help="if use chatglm",
     )
     bot_group.add_argument(
@@ -194,15 +187,14 @@
     )
     bot_group.add_argument(
         "--bot",
         dest="bot",
         help="bot type",
         choices=[
             "chatgptapi",
-            "newbing",
             "glm",
             "gemini",
             "langchain",
             "qwen",
             "doubao",
             "moonshot",
             "yi",
```

### Comparing `xiaogpt-2.70/xiaogpt/config.py` & `xiaogpt-2.71/xiaogpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import argparse
 import json
 import os
 from dataclasses import dataclass, field
 from typing import Any, Iterable, Literal
 
+import yaml
+
 from xiaogpt.utils import validate_proxy
 
 LATEST_ASK_API = "https://userprofile.mina.mi.com/device_profile/v2/conversation?source=dialogu&hardware={hardware}&timestamp={timestamp}&limit=2"
 COOKIE_TEMPLATE = "deviceId={device_id}; serviceToken={service_token}; userId={user_id}"
 WAKEUP_KEYWORD = "小爱同学"
 
 HARDWARE_COMMAND_DICT = {
@@ -80,26 +82,18 @@
     end_conversation: str = "结束持续对话"
     stream: bool = False
     tts: Literal[
         "mi", "edge", "azure", "openai", "baidu", "google", "volc", "minimax"
     ] = "mi"
     tts_options: dict[str, Any] = field(default_factory=dict)
     gpt_options: dict[str, Any] = field(default_factory=dict)
-    bing_cookie_path: str = ""
-    bing_cookies: dict | None = None
 
     def __post_init__(self) -> None:
         if self.proxy:
             validate_proxy(self.proxy)
-        if self.bot == "newbing":
-            if not (self.bing_cookie_path or self.bing_cookies):
-                raise Exception(
-                    "New bing bot needs bing_cookie_path or bing_cookies, read this: "
-                    "https://github.com/acheong08/EdgeGPT#getting-authentication-required"
-                )
         if (
             self.api_base
             and self.api_base.endswith(("openai.azure.com", "openai.azure.com/"))
             and not self.deployment_id
         ):
             raise Exception(
                 "Using Azure OpenAI needs deployment_id, read this: "
@@ -136,15 +130,18 @@
             )
         return cls(**config)
 
     @classmethod
     def read_from_file(cls, config_path: str) -> dict:
         result = {}
         with open(config_path, "rb") as f:
-            config = json.load(f)
+            if config_path.endswith(".json"):
+                config = json.load(f)
+            else:
+                config = yaml.safe_load(f)
             for key, value in config.items():
                 if value is None:
                     continue
                 if key == "keyword":
                     if not isinstance(value, list):
                         value = [value]
                     value = [kw for kw in value if kw]
```

### Comparing `xiaogpt-2.70/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.71/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/langchain/chain.py` & `xiaogpt-2.71/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/tts/base.py` & `xiaogpt-2.71/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/tts/mi.py` & `xiaogpt-2.71/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/tts/tetos.py` & `xiaogpt-2.71/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/utils.py` & `xiaogpt-2.71/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/xiaogpt/xiaogpt.py` & `xiaogpt-2.71/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.70/PKG-INFO` & `xiaogpt-2.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,121 +1,115 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.70
+Version: 2.71
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
 Requires-Python: >=3.9
 Requires-Dist: miservice_fork
 Requires-Dist: openai>=1
 Requires-Dist: aiohttp
 Requires-Dist: rich
 Requires-Dist: zhipuai>=2.0.1
 Requires-Dist: httpx[socks]
-Requires-Dist: EdgeGPT==0.1.26
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
 Requires-Dist: tetos>=0.2.1
 Requires-Dist: groq>=0.5.0
+Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
 Requires-Dist: beautifulsoup4==4.12.3; extra == "locked"
-Requires-Dist: bingimagecreator==0.5.0; extra == "locked"
 Requires-Dist: cachetools==5.3.2; extra == "locked"
 Requires-Dist: certifi==2024.2.2; extra == "locked"
 Requires-Dist: charset-normalizer==3.3.2; extra == "locked"
 Requires-Dist: click==8.1.7; extra == "locked"
 Requires-Dist: colorama==0.4.6; platform_system == "Windows" and extra == "locked"
-Requires-Dist: dashscope==1.18.0; extra == "locked"
+Requires-Dist: dashscope==1.19.0; extra == "locked"
 Requires-Dist: dataclasses-json==0.6.3; extra == "locked"
 Requires-Dist: distro==1.9.0; extra == "locked"
 Requires-Dist: edge-tts==6.1.10; extra == "locked"
-Requires-Dist: edgegpt==0.1.26; extra == "locked"
 Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11" and extra == "locked"
 Requires-Dist: frozenlist==1.4.1; extra == "locked"
-Requires-Dist: google-ai-generativelanguage==0.6.2; extra == "locked"
+Requires-Dist: google-ai-generativelanguage==0.6.3; extra == "locked"
 Requires-Dist: google-api-core==2.15.0; extra == "locked"
 Requires-Dist: google-api-core[grpc]==2.15.0; extra == "locked"
 Requires-Dist: google-api-python-client==2.125.0; extra == "locked"
 Requires-Dist: google-auth==2.26.1; extra == "locked"
 Requires-Dist: google-auth-httplib2==0.2.0; extra == "locked"
 Requires-Dist: google-cloud-texttospeech==2.16.3; extra == "locked"
-Requires-Dist: google-generativeai==0.5.2; extra == "locked"
+Requires-Dist: google-generativeai==0.5.3; extra == "locked"
 Requires-Dist: google-search-results==2.4.2; extra == "locked"
 Requires-Dist: googleapis-common-protos==1.62.0; extra == "locked"
 Requires-Dist: greenlet==3.0.3; (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64") and extra == "locked"
 Requires-Dist: groq==0.5.0; extra == "locked"
 Requires-Dist: grpcio==1.60.0; extra == "locked"
 Requires-Dist: grpcio-status==1.60.0; extra == "locked"
 Requires-Dist: h11==0.14.0; extra == "locked"
 Requires-Dist: httpcore==1.0.5; extra == "locked"
 Requires-Dist: httplib2==0.22.0; extra == "locked"
 Requires-Dist: httpx==0.27.0; extra == "locked"
 Requires-Dist: httpx[socks]==0.27.0; extra == "locked"
 Requires-Dist: idna==3.7; extra == "locked"
 Requires-Dist: jsonpatch==1.33; extra == "locked"
 Requires-Dist: jsonpointer==2.4; extra == "locked"
-Requires-Dist: langchain==0.1.17; extra == "locked"
-Requires-Dist: langchain-community==0.0.36; extra == "locked"
-Requires-Dist: langchain-core==0.1.50; extra == "locked"
+Requires-Dist: langchain==0.1.20; extra == "locked"
+Requires-Dist: langchain-community==0.0.38; extra == "locked"
+Requires-Dist: langchain-core==0.1.52; extra == "locked"
 Requires-Dist: langchain-text-splitters==0.0.1; extra == "locked"
 Requires-Dist: langsmith==0.1.45; extra == "locked"
 Requires-Dist: markdown-it-py==3.0.0; extra == "locked"
 Requires-Dist: marshmallow==3.20.1; extra == "locked"
 Requires-Dist: mdurl==0.1.2; extra == "locked"
 Requires-Dist: miservice-fork==2.4.3; extra == "locked"
 Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
 Requires-Dist: numexpr==2.10.0; extra == "locked"
 Requires-Dist: numpy==1.26.3; extra == "locked"
-Requires-Dist: openai==1.25.1; extra == "locked"
+Requires-Dist: openai==1.29.0; extra == "locked"
 Requires-Dist: orjson==3.10.0; extra == "locked"
 Requires-Dist: packaging==23.2; extra == "locked"
-Requires-Dist: prompt-toolkit==3.0.43; extra == "locked"
 Requires-Dist: proto-plus==1.23.0; extra == "locked"
 Requires-Dist: protobuf==4.25.1; extra == "locked"
 Requires-Dist: pyasn1==0.5.1; extra == "locked"
 Requires-Dist: pyasn1-modules==0.3.0; extra == "locked"
 Requires-Dist: pydantic==2.5.3; extra == "locked"
 Requires-Dist: pydantic-core==2.14.6; extra == "locked"
 Requires-Dist: pygments==2.17.2; extra == "locked"
 Requires-Dist: pyjwt==2.8.0; extra == "locked"
 Requires-Dist: pyparsing==3.1.2; python_version > "3.0" and extra == "locked"
 Requires-Dist: pyyaml==6.0.1; extra == "locked"
-Requires-Dist: regex==2023.12.25; extra == "locked"
 Requires-Dist: requests==2.31.0; extra == "locked"
 Requires-Dist: rich==13.7.1; extra == "locked"
 Requires-Dist: rsa==4.9; extra == "locked"
 Requires-Dist: sniffio==1.3.0; extra == "locked"
 Requires-Dist: socksio==1.0.0; extra == "locked"
 Requires-Dist: soupsieve==2.5; extra == "locked"
 Requires-Dist: sqlalchemy==2.0.25; extra == "locked"
 Requires-Dist: tenacity==8.2.3; extra == "locked"
 Requires-Dist: tetos==0.2.1; extra == "locked"
 Requires-Dist: tqdm==4.66.1; extra == "locked"
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
-Requires-Dist: wcwidth==0.2.13; extra == "locked"
-Requires-Dist: websockets==12.0; extra == "locked"
 Requires-Dist: yarl==1.9.4; extra == "locked"
 Requires-Dist: zhipuai==2.0.1.20240423.1; extra == "locked"
 Provides-Extra: locked
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
@@ -139,16 +133,16 @@
 - [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
 - [01](https://platform.lingyiwanwu.com/apikeys)
 - [Llama3](https://console.groq.com/docs/quickstart)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
 
-| 系统和Shell  | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
-|------------|------------------------------------------------|----------------------------------------|------------------------------------------------|
+| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
 | 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
 | 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
 | 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
 | 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
@@ -250,88 +244,81 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
-## config.json
+## config.yaml
 
-如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
+如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 Yaml 或 JSON 格式
 参数优先级
 
 - cli args > default > config
 
 ```shell
-python3 xiaogpt.py --config xiao_config.json
+python3 xiaogpt.py --config xiao_config.yaml
 # or
-xiaogpt --config xiao_config.json
+xiaogpt --config xiao_config.yaml
 ```
 
 或者
 
 ```shell
-cp xiao_config.json.example xiao_config.json
+cp xiao_config.yaml.example xiao_config.yaml
 python3 xiaogpt.py
 ```
 
-若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在config.json中指定：
+若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在 config.yaml 中指定：
 
-```json
-{
-    ...
-    "gpt_options": {
-        "temperature": 0.9,
-        "top_p": 0.9,
-    }
-}
+```yaml
+gpt_options:
+  temperature: 0.9
+  top_p: 0.9
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数             | 说明                                                                                                       | 默认值 | 可选值 |
-|------------------|-----------------------------------------------------------------------------------------------------------|--------|--------|
-| hardware         | 设备型号                                                                                                   |        |        |
-| account          | 小爱账户                                                                                                   |        |        |
-| password         | 小爱账户密码                                                                                               |        |        |
-| openai_key       | openai的apikey                                                                                             |        |        |
-| moonshot_api_key | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |        |        |
-| yi_api_key       | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |        |        |
-| llama_api_key       | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                             |        |        |
-| serpapi_api_key  | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |        |        |
-| glm_key          | chatglm 的 apikey                                                                                          |        |        |
-| gemini_key       | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |        |        |
-| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
-| mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
-| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
-| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
-| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                  |
-| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
-| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                                  |
-| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                  |
-| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                  |
-| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                  |
-| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                  |
-| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                  |
-| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                  |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                  |
-| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
-| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-[这里]: <https://github.com/acheong08/EdgeGPT#getting-authentication-required>
+| 参数                  | 说明                                                                                                       | 默认值                                                                                                    | 可选值                                                           |
+| --------------------- | ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
+| hardware              | 设备型号                                                                                                   |                                                                                                           |                                                                  |
+| account               | 小爱账户                                                                                                   |                                                                                                           |                                                                  |
+| password              | 小爱账户密码                                                                                               |                                                                                                           |                                                                  |
+| openai_key            | openai的apikey                                                                                             |                                                                                                           |                                                                  |
+| moonshot_api_key      | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |                                                                                                           |                                                                  |
+| yi_api_key            | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |                                                                                                           |                                                                  |
+| llama_api_key         | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                          |                                                                                                           |                                                                  |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |                                                                                                           |                                                                  |
+| glm_key               | chatglm 的 apikey                                                                                          |                                                                                                           |                                                                  |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |                                                                                                           |                                                                  |
+| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                |                                                                                                           |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)                |                                                                                                           |                                                                  |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                                              |                                                                                                           |                                                                  |
+| mi_did                | 设备did                                                                                                    |                                                                                                           |                                                                  |
+| use_command           | 使用 MI command 与小爱交互                                                                                 | `false`                                                                                                   |                                                                  |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                                     | `true`                                                                                                    |                                                                  |
+| verbose               | 是否打印详细日志                                                                                           | `false`                                                                                                   |                                                                  |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                                 | `chatgptapi`                                                                                              |                                                                  |
+| tts                   | 使用的 TTS 类型                                                                                            | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                                |                                                                                                           |                                                                  |
+| prompt                | 自定义prompt                                                                                               | `请用100字以内回答`                                                                                       |                                                                  |
+| keyword               | 自定义请求词列表                                                                                           | `["请"]`                                                                                                  |                                                                  |
+| change_prompt_keyword | 更改提示词触发列表                                                                                         | `["更改提示词"]`                                                                                          |                                                                  |
+| start_conversation    | 开始持续对话关键词                                                                                         | `开始持续对话`                                                                                            |                                                                  |
+| end_conversation      | 结束持续对话关键词                                                                                         | `结束持续对话`                                                                                            |                                                                  |
+| stream                | 使用流式响应，获得更快的响应                                                                               | `true`                                                                                                    |                                                                  |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                                        | ""                                                                                                        |                                                                  |
+| gpt_options           | OpenAI API 的参数字典                                                                                      | `{}`                                                                                                      |                                                                  |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                                          | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                                            | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取                        |                                                                                                           |                                                                  |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取                        |                                                                                                           |
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
 4. 在wsl使用时, 需要设置代理为 <http://wls的ip:port(vpn的代理端口)>, 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
@@ -369,21 +356,21 @@
 ```
 
 ### 使用配置文件
 
 xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
 
 ```shell
-docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 ### 网络使用 host 模型
 
 ```shell
-docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 ### 本地编译Docker Image
 
 ```shell
  docker build -t xiaogpt .
 ```
@@ -408,32 +395,30 @@
 [azure-tts](https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/9-more-realistic-ai-voices-for-conversations-now-generally/ba-p/4099471) 提供了微软 azure tts 的能力
 [openai-tts](https://platform.openai.com/docs/guides/text-to-speech) 提供了类似 openai tts 的能力
 
 #### Usage
 
 你可以通过参数 `tts`, 来启用它
 
-```json
-{
-  "tts": "edge",
-}
+```yaml
+tts: edge
 ```
 
 For edge 查看更多语言支持, 从中选择一个
 
 ```shell
 edge-tts --list-voices
 ```
 
 #### 在容器中使用 edge-tts/azure-tts/openai-tts/volc/google/baidu
 
 由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
 
 ```shell
-docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.json
+docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.yaml
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
 ## 推荐的 fork
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
```


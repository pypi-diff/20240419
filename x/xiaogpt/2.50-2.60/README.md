# Comparing `tmp/xiaogpt-2.50.tar.gz` & `tmp/xiaogpt-2.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.50.tar", last modified: Thu Apr 18 03:33:53 2024, max compression
+gzip compressed data, was "xiaogpt-2.60.tar", last modified: Thu Apr 18 13:20:09 2024, max compression
```

## Comparing `xiaogpt-2.50.tar` & `xiaogpt-2.60.tar`

### file list

```diff
@@ -1,29 +1,26 @@
--rw-r--r--   0        0        0     1063 2024-04-18 03:33:49.898299 xiaogpt-2.50/LICENSE
--rw-r--r--   0        0        0    23992 2024-04-18 03:33:49.898299 xiaogpt-2.50/README.md
--rw-r--r--   0        0        0     4133 2024-04-18 03:33:53.230314 xiaogpt-2.50/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/__main__.py
--rw-r--r--   0        0        0      919 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4738 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/cli.py
--rw-r--r--   0        0        0     6726 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      279 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     3979 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/azure.py
--rw-r--r--   0        0        0     4660 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     3984 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/volc.py
--rw-r--r--   0        0        0     2072 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/utils.py
--rw-r--r--   0        0        0    15513 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    30311 1970-01-01 00:00:00.000000 xiaogpt-2.50/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-18 13:20:05.908612 xiaogpt-2.60/LICENSE
+-rw-r--r--   0        0        0    20871 2024-04-18 13:20:05.912612 xiaogpt-2.60/README.md
+-rw-r--r--   0        0        0     3938 2024-04-18 13:20:09.456638 xiaogpt-2.60/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      919 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4409 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5896 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1903 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15821 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    26836 1970-01-01 00:00:00.000000 xiaogpt-2.60/PKG-INFO
```

### Comparing `xiaogpt-2.50/LICENSE` & `xiaogpt-2.60/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/README.md` & `xiaogpt-2.60/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-系统和Shell|Linux *sh|Windows CMD用户|Windows PowerShell用户
--|-|-|-
-1、安装包|`pip install miservice_fork`|`pip install miservice_fork`|`pip install miservice_fork`
-2、设置变量|`export MI_USER=xxx` <br> `export MI_PASS=xxx`|`set MI_USER=xxx`<br>`set MI_PASS=xxx`|`$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"`
-3、取得MI_DID|`micli list` |`micli list` |`micli list` 
-4、设置MI_DID|`export MI_DID=xxx`| `set MI_DID=xxx`| `$env:MI_DID="xxx"`
+| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
+| 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
+| 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
+| 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
+| 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
@@ -142,50 +142,44 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                     | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                                                                                     |
-| ------------------------ | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
-| hardware                 | 设备型号                                                                                    |                                                                                                           |                                                                                                                            |
-| account                  | 小爱账户                                                                                    |                                                                                                           |                                                                                                                            |
-| password                 | 小爱账户密码                                                                                |                                                                                                           |                                                                                                                            |
-| openai_key               | openai的apikey                                                                              |                                                                                                           |                                                                                                                            |
-| serpapi_api_key          | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                                                                            |
-| glm_key                  | chatglm 的 apikey                                                                           |                                                                                                           |                                                                                                                            |
-| gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
-| qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
-| cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
-| mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
-| use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
-| mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
-| verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
-| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                           | `chatgptapi`                                                                                              |                                                                                                                            |
-| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`                                                                                                 |
-| tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
-| prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
-| keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
-| change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
-| start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
-| end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
-| stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
-| proxy                    | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                                                                            |
-| gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
-| bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
-| bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
-| deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
-| api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
-| azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
-| azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
-| volc_accesskey | 火山引擎accesskey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 |  |
-| volc_secretkey | 火山引擎secretkey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 | |
-| volc_tts_app | 火山引擎  TTS app 服务   [参考]( https://console.volcengine.com/sami/)                          |                                  |  |
-| volc_tts_speaker | 火山引擎 TTS speaker   [参考]( https://www.volcengine.com/docs/6489/93478)                          |   `zh_female_qingxin`                               |  |
+| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                |
+| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
+| hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
+| account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
+| password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
+| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
+| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
+| mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
+| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
+| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
+| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                       |
+| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                       |
+| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                       |
+| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                       |
+| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                       |
+| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
+| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
+| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
+| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
+| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                       |
 
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
@@ -296,14 +290,15 @@
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
+- [Tetos](https://github.com/frostming/tetos) TTS 云服务支持
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
 - @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
 - @[frostming](https://github.com/frostming) 重构了一些代码，支持了`持续会话功能`
 
 ## 赞赏
 
 谢谢就够了
```

### Comparing `xiaogpt-2.50/pyproject.toml` & `xiaogpt-2.60/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,69 +14,66 @@
 dependencies = [
     "miservice_fork",
     "openai>=1",
     "aiohttp",
     "rich",
     "zhipuai>=2.0.1",
     "httpx[socks]",
-    "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
-    "azure-cognitiveservices-speech>=1.37.0",
-    "multidict>=6.0.5",
-    "volcengine>=1.0.136",
+    "tetos>=0.1.0",
 ]
 dynamic = []
-version = "2.50"
+version = "2.60"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
 [project.scripts]
 xiaogpt = "xiaogpt.cli:main"
 
 [project.optional-dependencies]
 locked = [
-    "aiohttp==3.9.4",
+    "aiohttp==3.9.5",
     "aiosignal==1.3.1",
     "annotated-types==0.6.0",
-    "anyio==3.7.1",
+    "anyio==4.3.0",
     "async-timeout==4.0.3 ; python_version < \"3.11\"",
     "attrs==23.2.0",
     "azure-cognitiveservices-speech==1.37.0",
     "beautifulsoup4==4.12.3",
     "bingimagecreator==0.5.0",
     "cachetools==5.3.2",
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
+    "click==8.1.7",
     "colorama==0.4.6 ; platform_system == \"Windows\"",
-    "dashscope==1.10.0",
+    "dashscope==1.17.0",
     "dataclasses-json==0.6.3",
-    "decorator==5.1.1",
     "distro==1.9.0",
     "edge-tts==6.1.10",
     "edgegpt==0.1.26",
     "exceptiongroup==1.2.0 ; python_version < \"3.11\"",
     "frozenlist==1.4.1",
-    "google==3.0.0",
-    "google-ai-generativelanguage==0.6.1",
+    "google-ai-generativelanguage==0.6.2",
     "google-api-core==2.15.0",
     "google-api-core[grpc]==2.15.0",
     "google-api-python-client==2.125.0",
     "google-auth==2.26.1",
     "google-auth-httplib2==0.2.0",
-    "google-generativeai==0.5.0",
+    "google-cloud-texttospeech==2.16.3",
+    "google-generativeai==0.5.1",
     "google-search-results==2.4.2",
     "googleapis-common-protos==1.62.0",
     "greenlet==3.0.3 ; platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\"",
     "grpcio==1.60.0",
     "grpcio-status==1.60.0",
     "h11==0.14.0",
     "httpcore==1.0.5",
@@ -96,48 +93,43 @@
     "mdurl==0.1.2",
     "miservice-fork==2.4.3",
     "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
     "numexpr==2.10.0",
     "numpy==1.26.3",
-    "openai==1.17.1",
+    "openai==1.21.2",
     "orjson==3.10.0",
     "packaging==23.2",
     "prompt-toolkit==3.0.43",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
-    "py==1.11.0",
     "pyasn1==0.5.1",
     "pyasn1-modules==0.3.0",
-    "pycryptodome==3.9.9",
     "pydantic==2.5.3",
     "pydantic-core==2.14.6",
     "pygments==2.17.2",
     "pyjwt==2.8.0",
     "pyparsing==3.1.2 ; python_version > \"3.0\"",
-    "pytz==2020.5",
     "pyyaml==6.0.1",
     "regex==2023.12.25",
     "requests==2.31.0",
-    "retry==0.9.2",
     "rich==13.7.1",
     "rsa==4.9",
-    "six==1.16.0",
     "sniffio==1.3.0",
     "socksio==1.0.0",
     "soupsieve==2.5",
     "sqlalchemy==2.0.25",
     "tenacity==8.2.3",
+    "tetos==0.1.0",
     "tqdm==4.66.1",
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
-    "volcengine==1.0.136",
     "wcwidth==0.2.13",
     "websockets==12.0",
     "yarl==1.9.4",
     "zhipuai==2.0.1",
 ]
 
 [tool.pdm]
```

### Comparing `xiaogpt-2.50/xiaogpt/bot/__init__.py` & `xiaogpt-2.60/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/base_bot.py` & `xiaogpt-2.60/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.60/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.60/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.60/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.60/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.60/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.60/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/cli.py` & `xiaogpt-2.60/xiaogpt/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,35 +82,17 @@
         "--verbose",
         dest="verbose",
         action="store_true",
         default=None,
         help="show info",
     )
     parser.add_argument(
-        "--azure_tts_speech_key",
-        dest="azure_tts_speech_key",
-        help="if use azure tts",
-    )
-    parser.add_argument(
-        "--azure_tts_service_region",
-        dest="azure_tts_service_region",
-        help="if use azure tts",
-    )
-    tts_group = parser.add_mutually_exclusive_group()
-    tts_group.add_argument(
-        "--enable_edge_tts",
-        dest="tts",
-        action="store_const",
-        const="edge",
-        help="if use edge tts",
-    )
-    tts_group.add_argument(
         "--tts",
-        help="tts type",
-        choices=["mi", "edge", "openai", "azure"],
+        help="TTS provider",
+        choices=["mi", "edge", "openai", "azure", "google", "baidu", "volc"],
     )
     bot_group = parser.add_mutually_exclusive_group()
     bot_group.add_argument(
         "--use_chatgpt_api",
         dest="bot",
         action="store_const",
         const="chatgptapi",
@@ -186,14 +168,20 @@
         dest="deployment_id",
         help="specify deployment id, only used when api_base points to azure",
     )
 
     options = parser.parse_args()
     config = Config.from_options(options)
 
-    miboy = MiGPT(config)
+    async def main(config: Config) -> None:
+        miboy = MiGPT(config)
+        try:
+            await miboy.run_forever()
+        finally:
+            await miboy.close()
+
     loop = asyncio.get_event_loop()
-    loop.run_until_complete(miboy.run_forever())
+    loop.run_until_complete(main(config))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `xiaogpt-2.50/xiaogpt/config.py` & `xiaogpt-2.60/xiaogpt/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,14 @@
     "L07A": ("5-1", "5-5"),  # Redmi小爱音箱Play(l7a)
     "L15A": ("7-3", "7-4"),
     "X6A": ("7-3", "7-4"),  # 小米智能家庭屏6
     "X10A": ("7-3", "7-4"),  # 小米智能家庭屏10
     # add more here
 }
 
-EDGE_TTS_DICT = {
-    "用英语": "en-US-AriaNeural",
-    "用日语": "ja-JP-NanamiNeural",
-    "用法语": "fr-BE-CharlineNeural",
-    "用韩语": "ko-KR-SunHiNeural",
-    "用德语": "de-AT-JonasNeural",
-    # add more here
-}
-
 DEFAULT_COMMAND = ("5-1", "5-5")
 
 KEY_WORD = ("帮我", "请")
 CHANGE_PROMPT_KEY_WORD = ("更改提示词",)
 PROMPT = "以下请用100字以内回答，请只回答文字不要带链接"
 # simulate_xiaoai_question
 MI_ASK_SIMULATE_DATA = {
@@ -76,31 +67,19 @@
     api_base: str | None = None
     deployment_id: str | None = None
     use_command: bool = False
     verbose: bool = False
     start_conversation: str = "开始持续对话"
     end_conversation: str = "结束持续对话"
     stream: bool = False
-    tts: Literal["mi", "edge", "azure", "openai"] = "mi"
-    tts_voice: str | None = None
+    tts: Literal["mi", "edge", "azure", "openai", "baidu", "google", "volc"] = "mi"
+    tts_options: dict[str, Any] = field(default_factory=dict)
     gpt_options: dict[str, Any] = field(default_factory=dict)
     bing_cookie_path: str = ""
     bing_cookies: dict | None = None
-    azure_tts_speech_key: str | None = None
-    azure_tts_service_region: str = "eastasia"
-    volc_accesskey: str = os.getenv(
-        "VOLC_ACCESSKEY", ""
-    )  # https://console.volcengine.com/iam/keymanage/
-    volc_secretkey: str = os.getenv("VOLC_SECRETKEY", "")
-    volc_tts_app: str = os.getenv(
-        "VOLC_TTS_APP", ""
-    )  # https://console.volcengine.com/sami
-    volc_tts_speaker: str = os.getenv(
-        "VOLC_TTS_SPEAPER", "zh_female_qingxin"
-    )  # https://www.volcengine.com/docs/6489/93478
 
     def __post_init__(self) -> None:
         if self.proxy:
             validate_proxy(self.proxy)
         if self.bot == "newbing":
             if not (self.bing_cookie_path or self.bing_cookies):
                 raise Exception(
@@ -117,16 +96,14 @@
                 "https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions"
             )
         if self.bot in ["chatgptapi"]:
             if not self.openai_key:
                 raise Exception(
                     "Using GPT api needs openai API key, please google how to"
                 )
-        if self.tts == "azure" and not self.azure_tts_speech_key:
-            raise Exception("Using Azure TTS needs azure speech key")
 
     @property
     def tts_command(self) -> str:
         return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
 
     @property
     def wakeup_command(self) -> str:
```

### Comparing `xiaogpt-2.50/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.60/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/langchain/chain.py` & `xiaogpt-2.60/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/tts/base.py` & `xiaogpt-2.60/xiaogpt/tts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         is_playing = (
             json.loads(playing_info.get("data", {}).get("info", "{}")).get("status", -1)
             == 1
         )
         return is_playing
 
     @abc.abstractmethod
-    async def synthesize(self, query: str, text_stream: AsyncIterator[str]) -> None:
+    async def synthesize(self, lang: str, text_stream: AsyncIterator[str]) -> None:
         """Synthesize speech from a stream of text."""
         raise NotImplementedError
 
 
 class HTTPRequestHandler(SimpleHTTPRequestHandler):
     def log_message(self, format, *args):
         logger.debug(f"{self.address_string()} - {format}", *args)
@@ -83,28 +83,28 @@
         self, mina_service: MiNAService, device_id: str, config: Config
     ) -> None:
         super().__init__(mina_service, device_id, config)
         self.dirname = tempfile.TemporaryDirectory(prefix="xiaogpt-tts-")
         self._start_http_server()
 
     @abc.abstractmethod
-    async def make_audio_file(self, query: str, text: str) -> tuple[Path, float]:
+    async def make_audio_file(self, lang: str, text: str) -> tuple[Path, float]:
         """Synthesize speech from text and save it to a file.
         Return the file path and the duration of the audio in seconds.
         The file path must be relative to the self.dirname.
         """
         raise NotImplementedError
 
-    async def synthesize(self, query: str, text_stream: AsyncIterator[str]) -> None:
+    async def synthesize(self, lang: str, text_stream: AsyncIterator[str]) -> None:
         queue: asyncio.Queue[tuple[str, float]] = asyncio.Queue()
         finished = asyncio.Event()
 
         async def worker():
             async for text in text_stream:
-                path, duration = await self.make_audio_file(query, text)
+                path, duration = await self.make_audio_file(lang, text)
                 url = f"http://{self.hostname}:{self.port}/{path.name}"
                 await queue.put((url, duration))
             finished.set()
 
         task = asyncio.create_task(worker())
 
         while True:
```

### Comparing `xiaogpt-2.50/xiaogpt/tts/mi.py` & `xiaogpt-2.60/xiaogpt/tts/mi.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         else:
             await miio_command(
                 self.miio_service,
                 self.config.mi_did,
                 f"{self.config.tts_command} {text}",
             )
 
-    async def synthesize(self, query: str, text_stream: AsyncIterator[str]) -> None:
+    async def synthesize(self, lang: str, text_stream: AsyncIterator[str]) -> None:
         async for text in text_stream:
             await self.say(text)
             await self.wait_for_duration(calculate_tts_elapse(text))
```

### Comparing `xiaogpt-2.50/xiaogpt/utils.py` & `xiaogpt-2.60/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.50/xiaogpt/xiaogpt.py` & `xiaogpt-2.60/xiaogpt/xiaogpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from xiaogpt.config import (
     COOKIE_TEMPLATE,
     LATEST_ASK_API,
     MI_ASK_SIMULATE_DATA,
     WAKEUP_KEYWORD,
     Config,
 )
-from xiaogpt.tts import TTS, EdgeTTS, MiTTS, AzureTTS, VolcTTS
-from xiaogpt.tts.openai import OpenAITTS
+from xiaogpt.tts import TTS, MiTTS, TetosTTS
 from xiaogpt.utils import (
     parse_cookie_string,
 )
 
 EOF = object()
 
 
@@ -49,14 +48,17 @@
         # setup logger
         self.log = logging.getLogger("xiaogpt")
         self.log.setLevel(logging.DEBUG if config.verbose else logging.INFO)
         self.log.addHandler(RichHandler())
         self.log.debug(config)
         self.mi_session = ClientSession()
 
+    async def close(self):
+        await self.mi_session.close()
+
     async def poll_latest_ask(self):
         async with ClientSession() as session:
             session._cookie_jar = self.cookie_jar
             while True:
                 self.log.debug(
                     "Listening new message, timestamp: %s", self.last_timestamp
                 )
@@ -74,24 +76,24 @@
                     await self.stop_if_xiaoai_is_playing()
                 if (d := time.perf_counter() - start) < 1:
                     # sleep to avoid too many request
                     self.log.debug("Sleep %f, timestamp: %s", d, self.last_timestamp)
                     # if you want force mute xiaoai, comment this line below.
                     await asyncio.sleep(1 - d)
 
-    async def init_all_data(self, session):
-        await self.login_miboy(session)
+    async def init_all_data(self):
+        await self.login_miboy()
         await self._init_data_hardware()
         self.mi_session.cookie_jar.update_cookies(self.get_cookie())
         self.cookie_jar = self.mi_session.cookie_jar
         self.tts  # init tts
 
-    async def login_miboy(self, session):
+    async def login_miboy(self):
         account = MiAccount(
-            session,
+            self.mi_session,
             self.config.account,
             self.config.password,
             str(self.mi_token_home),
         )
         # Forced login to refresh to refresh token
         await account.login("micoapi")
         self.mina_service = MiNAService(account)
@@ -175,15 +177,15 @@
     def need_ask_gpt(self, record):
         if not record:
             return False
         query = record.get("query", "")
         return (
             self.in_conversation
             and not query.startswith(WAKEUP_KEYWORD)
-            or query.startswith(tuple(self.config.keyword))
+            or query.lower().startswith(tuple(w.lower() for w in self.config.keyword))
         )
 
     def need_change_prompt(self, record):
         query = record.get("query", "")
         return query.startswith(tuple(self.config.change_prompt_keyword))
 
     def _change_prompt(self, new_prompt):
@@ -221,15 +223,15 @@
                     print("Maybe outof date trying to re init it")
                     await self._retry()
             else:
                 return self._get_last_query(data)
         return None
 
     async def _retry(self):
-        await self.init_all_data(self.mi_session)
+        await self.init_all_data()
 
     def _get_last_query(self, data: dict) -> dict | None:
         if d := data.get("data"):
             records = json.loads(d).get("records")
             if not records:
                 return None
             last_record = records[0]
@@ -254,24 +256,18 @@
                 self.miio_service,
                 self.config.mi_did,
                 f"{self.config.tts_command} {value}",
             )
 
     @functools.cached_property
     def tts(self) -> TTS:
-        if self.config.tts == "edge":
-            return EdgeTTS(self.mina_service, self.device_id, self.config)
-        elif self.config.tts == "azure":
-            return AzureTTS(self.mina_service, self.device_id, self.config)
-        elif self.config.tts == "openai":
-            return OpenAITTS(self.mina_service, self.device_id, self.config)
-        elif self.config.tts == "volc":
-            return VolcTTS(self.mina_service, self.device_id, self.config)
-        else:
+        if self.config.tts == "mi":
             return MiTTS(self.mina_service, self.device_id, self.config)
+        else:
+            return TetosTTS(self.mina_service, self.device_id, self.config)
 
     async def wait_for_tts_finish(self):
         while True:
             if not await self.get_if_xiaoai_is_playing():
                 break
             await asyncio.sleep(1)
 
@@ -343,15 +339,15 @@
         return await miio_command(
             self.miio_service,
             self.config.mi_did,
             f"{self.config.wakeup_command} {WAKEUP_KEYWORD} 0",
         )
 
     async def run_forever(self):
-        await self.init_all_data(self.mi_session)
+        await self.init_all_data()
         task = asyncio.create_task(self.poll_latest_ask())
         assert task is not None  # to keep the reference to task, do not remove this
         print(
             f"Running xiaogpt now, 用[green]{'/'.join(self.config.keyword)}[/]开头来提问"
         )
         print(f"或用[green]{self.config.start_conversation}[/]开始持续对话")
         while True:
@@ -385,14 +381,15 @@
             # drop 帮我回答
             query = re.sub(rf"^({'|'.join(self.config.keyword)})", "", query)
 
             print("-" * 20)
             print("问题：" + query + "？")
             if not self.chatbot.has_history():
                 query = f"{query}，{self.config.prompt}"
+            query += "，并用本段话的language code作为开头，用|分隔，如：en-US|你好……"
             if self.config.mute_xiaoai:
                 await self.stop_if_xiaoai_is_playing()
             else:
                 # waiting for xiaoai speaker done
                 await asyncio.sleep(8)
             await self.do_tts(f"正在问{self.chatbot.name}请耐心等待")
             try:
@@ -400,15 +397,30 @@
                     "以下是小爱的回答: ",
                     new_record.get("answers", [])[0].get("tts", {}).get("text"),
                 )
             except IndexError:
                 print("小爱没回")
             print(f"以下是 {self.chatbot.name} 的回答: ", end="")
             try:
-                await self.tts.synthesize(query, self.ask_gpt(query))
+                await self.speak(self.ask_gpt(query))
             except Exception as e:
                 print(f"{self.chatbot.name} 回答出错 {str(e)}")
             else:
                 print("回答完毕")
             if self.in_conversation:
                 print(f"继续对话, 或用`{self.config.end_conversation}`结束对话")
                 await self.wakeup_xiaoai()
+
+    async def speak(self, text_stream: AsyncIterator[str]) -> None:
+        text = await anext(text_stream)
+        # See if the first part contains language code(e.g. en-US|Hello world)
+        lang, _, first_chunk = text.rpartition("|")
+        if len(lang) > 7:
+            # It is not a legal language code, discard it
+            lang, first_chunk = "", text
+
+        async def gen():  # reconstruct the generator
+            yield first_chunk
+            async for text in text_stream:
+                yield text
+
+        await self.tts.synthesize(lang or "zh-CN", gen())
```

### Comparing `xiaogpt-2.50/PKG-INFO` & `xiaogpt-2.60/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.50
+Version: 2.60
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
-Requires-Dist: edge-tts>=6.1.3
 Requires-Dist: EdgeGPT==0.1.26
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
-Requires-Dist: azure-cognitiveservices-speech>=1.37.0
-Requires-Dist: multidict>=6.0.5
-Requires-Dist: volcengine>=1.0.136
-Requires-Dist: aiohttp==3.9.4; extra == "locked"
+Requires-Dist: tetos>=0.1.0
+Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
-Requires-Dist: anyio==3.7.1; extra == "locked"
+Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
 Requires-Dist: beautifulsoup4==4.12.3; extra == "locked"
 Requires-Dist: bingimagecreator==0.5.0; extra == "locked"
 Requires-Dist: cachetools==5.3.2; extra == "locked"
 Requires-Dist: certifi==2024.2.2; extra == "locked"
 Requires-Dist: charset-normalizer==3.3.2; extra == "locked"
+Requires-Dist: click==8.1.7; extra == "locked"
 Requires-Dist: colorama==0.4.6; platform_system == "Windows" and extra == "locked"
-Requires-Dist: dashscope==1.10.0; extra == "locked"
+Requires-Dist: dashscope==1.17.0; extra == "locked"
 Requires-Dist: dataclasses-json==0.6.3; extra == "locked"
-Requires-Dist: decorator==5.1.1; extra == "locked"
 Requires-Dist: distro==1.9.0; extra == "locked"
 Requires-Dist: edge-tts==6.1.10; extra == "locked"
 Requires-Dist: edgegpt==0.1.26; extra == "locked"
 Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11" and extra == "locked"
 Requires-Dist: frozenlist==1.4.1; extra == "locked"
-Requires-Dist: google==3.0.0; extra == "locked"
-Requires-Dist: google-ai-generativelanguage==0.6.1; extra == "locked"
+Requires-Dist: google-ai-generativelanguage==0.6.2; extra == "locked"
 Requires-Dist: google-api-core==2.15.0; extra == "locked"
 Requires-Dist: google-api-core[grpc]==2.15.0; extra == "locked"
 Requires-Dist: google-api-python-client==2.125.0; extra == "locked"
 Requires-Dist: google-auth==2.26.1; extra == "locked"
 Requires-Dist: google-auth-httplib2==0.2.0; extra == "locked"
-Requires-Dist: google-generativeai==0.5.0; extra == "locked"
+Requires-Dist: google-cloud-texttospeech==2.16.3; extra == "locked"
+Requires-Dist: google-generativeai==0.5.1; extra == "locked"
 Requires-Dist: google-search-results==2.4.2; extra == "locked"
 Requires-Dist: googleapis-common-protos==1.62.0; extra == "locked"
 Requires-Dist: greenlet==3.0.3; (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64") and extra == "locked"
 Requires-Dist: grpcio==1.60.0; extra == "locked"
 Requires-Dist: grpcio-status==1.60.0; extra == "locked"
 Requires-Dist: h11==0.14.0; extra == "locked"
 Requires-Dist: httpcore==1.0.5; extra == "locked"
@@ -78,48 +75,43 @@
 Requires-Dist: mdurl==0.1.2; extra == "locked"
 Requires-Dist: miservice-fork==2.4.3; extra == "locked"
 Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
 Requires-Dist: numexpr==2.10.0; extra == "locked"
 Requires-Dist: numpy==1.26.3; extra == "locked"
-Requires-Dist: openai==1.17.1; extra == "locked"
+Requires-Dist: openai==1.21.2; extra == "locked"
 Requires-Dist: orjson==3.10.0; extra == "locked"
 Requires-Dist: packaging==23.2; extra == "locked"
 Requires-Dist: prompt-toolkit==3.0.43; extra == "locked"
 Requires-Dist: proto-plus==1.23.0; extra == "locked"
 Requires-Dist: protobuf==4.25.1; extra == "locked"
-Requires-Dist: py==1.11.0; extra == "locked"
 Requires-Dist: pyasn1==0.5.1; extra == "locked"
 Requires-Dist: pyasn1-modules==0.3.0; extra == "locked"
-Requires-Dist: pycryptodome==3.9.9; extra == "locked"
 Requires-Dist: pydantic==2.5.3; extra == "locked"
 Requires-Dist: pydantic-core==2.14.6; extra == "locked"
 Requires-Dist: pygments==2.17.2; extra == "locked"
 Requires-Dist: pyjwt==2.8.0; extra == "locked"
 Requires-Dist: pyparsing==3.1.2; python_version > "3.0" and extra == "locked"
-Requires-Dist: pytz==2020.5; extra == "locked"
 Requires-Dist: pyyaml==6.0.1; extra == "locked"
 Requires-Dist: regex==2023.12.25; extra == "locked"
 Requires-Dist: requests==2.31.0; extra == "locked"
-Requires-Dist: retry==0.9.2; extra == "locked"
 Requires-Dist: rich==13.7.1; extra == "locked"
 Requires-Dist: rsa==4.9; extra == "locked"
-Requires-Dist: six==1.16.0; extra == "locked"
 Requires-Dist: sniffio==1.3.0; extra == "locked"
 Requires-Dist: socksio==1.0.0; extra == "locked"
 Requires-Dist: soupsieve==2.5; extra == "locked"
 Requires-Dist: sqlalchemy==2.0.25; extra == "locked"
 Requires-Dist: tenacity==8.2.3; extra == "locked"
+Requires-Dist: tetos==0.1.0; extra == "locked"
 Requires-Dist: tqdm==4.66.1; extra == "locked"
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
-Requires-Dist: volcengine==1.0.136; extra == "locked"
 Requires-Dist: wcwidth==0.2.13; extra == "locked"
 Requires-Dist: websockets==12.0; extra == "locked"
 Requires-Dist: yarl==1.9.4; extra == "locked"
 Requires-Dist: zhipuai==2.0.1; extra == "locked"
 Provides-Extra: locked
 Description-Content-Type: text/markdown
 
@@ -140,20 +132,20 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-系统和Shell|Linux *sh|Windows CMD用户|Windows PowerShell用户
--|-|-|-
-1、安装包|`pip install miservice_fork`|`pip install miservice_fork`|`pip install miservice_fork`
-2、设置变量|`export MI_USER=xxx` <br> `export MI_PASS=xxx`|`set MI_USER=xxx`<br>`set MI_PASS=xxx`|`$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"`
-3、取得MI_DID|`micli list` |`micli list` |`micli list` 
-4、设置MI_DID|`export MI_DID=xxx`| `set MI_DID=xxx`| `$env:MI_DID="xxx"`
+| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
+| 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
+| 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
+| 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
+| 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
@@ -267,50 +259,44 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                     | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                                                                                     |
-| ------------------------ | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
-| hardware                 | 设备型号                                                                                    |                                                                                                           |                                                                                                                            |
-| account                  | 小爱账户                                                                                    |                                                                                                           |                                                                                                                            |
-| password                 | 小爱账户密码                                                                                |                                                                                                           |                                                                                                                            |
-| openai_key               | openai的apikey                                                                              |                                                                                                           |                                                                                                                            |
-| serpapi_api_key          | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                                                                            |
-| glm_key                  | chatglm 的 apikey                                                                           |                                                                                                           |                                                                                                                            |
-| gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
-| qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
-| cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
-| mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
-| use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
-| mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
-| verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
-| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                           | `chatgptapi`                                                                                              |                                                                                                                            |
-| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`                                                                                                 |
-| tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
-| prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
-| keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
-| change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
-| start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
-| end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
-| stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
-| proxy                    | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                                                                            |
-| gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
-| bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
-| bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
-| deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
-| api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
-| azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
-| azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
-| volc_accesskey | 火山引擎accesskey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 |  |
-| volc_secretkey | 火山引擎secretkey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 | |
-| volc_tts_app | 火山引擎  TTS app 服务   [参考]( https://console.volcengine.com/sami/)                          |                                  |  |
-| volc_tts_speaker | 火山引擎 TTS speaker   [参考]( https://www.volcengine.com/docs/6489/93478)                          |   `zh_female_qingxin`                               |  |
+| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                |
+| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
+| hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
+| account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
+| password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
+| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
+| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
+| mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
+| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
+| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
+| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                       |
+| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                       |
+| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                       |
+| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                       |
+| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                       |
+| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
+| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
+| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
+| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
+| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                       |
 
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
@@ -421,14 +407,15 @@
 
 - [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
+- [Tetos](https://github.com/frostming/tetos) TTS 云服务支持
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
 - @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
 - @[frostming](https://github.com/frostming) 重构了一些代码，支持了`持续会话功能`
 
 ## 赞赏
 
 谢谢就够了
```


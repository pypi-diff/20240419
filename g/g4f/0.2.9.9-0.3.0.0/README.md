# Comparing `tmp/g4f-0.2.9.9.tar.gz` & `tmp/g4f-0.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.9.9.tar", last modified: Mon Apr 15 20:20:40 2024, max compression
+gzip compressed data, was "g4f-0.3.0.0.tar", last modified: Thu Apr 18 19:48:07 2024, max compression
```

## Comparing `g4f-0.2.9.9.tar` & `g4f-0.3.0.0.tar`

### file list

```diff
@@ -1,240 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.024993 g4f-0.2.9.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-15 20:20:36.000000 g4f-0.2.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 20:20:36.000000 g4f-0.2.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-15 20:20:40.024993 g4f-0.2.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46685 2024-04-15 20:20:36.000000 g4f-0.2.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.988992 g4f-0.2.9.9/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.996992 g4f-0.2.9.9/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.996992 g4f-0.2.9.9/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31953 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.984992 g4f-0.2.9.9/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:20:40.024993 g4f-0.2.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-15 20:20:36.000000 g4f-0.2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.813260 g4f-0.3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-18 19:48:04.000000 g4f-0.3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 19:48:04.000000 g4f-0.3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-18 19:48:07.813260 g4f-0.3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    46685 2024-04-18 19:48:04.000000 g4f-0.3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.781260 g4f-0.3.0.0/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.785260 g4f-0.3.0.0/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.785260 g4f-0.3.0.0/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.793260 g4f-0.3.0.0/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.793260 g4f-0.3.0.0/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.793260 g4f-0.3.0.0/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.797260 g4f-0.3.0.0/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.797260 g4f-0.3.0.0/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.797260 g4f-0.3.0.0/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.797260 g4f-0.3.0.0/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.797260 g4f-0.3.0.0/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.777260 g4f-0.3.0.0/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.801260 g4f-0.3.0.0/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.805260 g4f-0.3.0.0/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.805260 g4f-0.3.0.0/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45681 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.805260 g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-18 19:48:04.000000 g4f-0.3.0.0/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:07.809260 g4f-0.3.0.0/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 19:48:07.000000 g4f-0.3.0.0/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:48:07.813260 g4f-0.3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-18 19:48:04.000000 g4f-0.3.0.0/setup.py
```

### Comparing `g4f-0.2.9.9/LICENSE` & `g4f-0.3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/PKG-INFO` & `g4f-0.3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.9
+Version: 0.3.0.0
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.9 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.0 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.2.9.9/README.md` & `g4f-0.3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Aichatos.py` & `g4f-0.3.0.0/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Aura.py` & `g4f-0.3.0.0/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Bing.py` & `g4f-0.3.0.0/g4f/Provider/Bing.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 def get_default_cookies():
     return {
         'SRCHD'         : 'AF=NOFORM',
         'PPLState'      : '1',
         'KievRPSSecAuth': '',
         'SUID'          : '',
-        'SRCHUSR'       : '',
+        'SRCHUSR'       : f'DOB={date.today().strftime("%Y%m%d")}&T={int(time.time())}',
         'SRCHHPGUSR'    : f'HV={int(time.time())}',
         'BCP'           : 'AD=1&AL=1&SM=1',
         '_Rwho'         : f'u=d&ts={date.today().isoformat()}',
     }
 
 def create_headers(cookies: Cookies = None, api_key: str = None) -> dict:
     if cookies is None:
```

### Comparing `g4f-0.2.9.9/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.0/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Blackbox.py` & `g4f-0.3.0.0/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.0/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.0/g4f/Provider/Chatgpt4Online.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import re
 import json
 from aiohttp import ClientSession
 
 from ..typing import Messages, AsyncResult
 from ..requests import get_args_from_browser
+from ..webdriver import WebDriver
 from .base_provider import AsyncGeneratorProvider
 from .helper import get_random_string
 
 class Chatgpt4Online(AsyncGeneratorProvider):
     url = "https://chatgpt4online.org"
     supports_message_history = True
     supports_gpt_35_turbo = True
@@ -19,17 +20,18 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
+        webdriver: WebDriver = None,
         **kwargs
     ) -> AsyncResult:
-        args = get_args_from_browser(f"{cls.url}/chat/", proxy=proxy)
+        args = get_args_from_browser(f"{cls.url}/chat/", webdriver, proxy=proxy)
         async with ClientSession(**args) as session:
             if not cls._wpnonce:
                 async with session.get(f"{cls.url}/chat/", proxy=proxy) as response:
                     response.raise_for_status()
                     response = await response.text()
                     result = re.search(r'restNonce&quot;:&quot;(.*?)&quot;', response)
                     if result:
```

### Comparing `g4f-0.2.9.9/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.0/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.0/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.0/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.0/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Cnote.py` & `g4f-0.3.0.0/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.0/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.0/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.0/g4f/Provider/not_working/Chatxyz.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 from __future__ import annotations
 
 import json
-import aiohttp
+from aiohttp import ClientSession
 
-from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from ..typing import AsyncResult, Messages
-from ..requests.raise_for_status import raise_for_status
+from ...typing import AsyncResult, Messages
+from ..base_provider import AsyncGeneratorProvider
 
-class DuckDuckGo(AsyncGeneratorProvider, ProviderModelMixin):
-    url = "https://duckduckgo.com/duckchat"
-    working = True
+class Chatxyz(AsyncGeneratorProvider):
+    url = "https://chat.3211000.xyz"
+    working = False
     supports_gpt_35_turbo = True
     supports_message_history = True
 
-    default_model = "gpt-3.5-turbo-0125"
-    models = ["gpt-3.5-turbo-0125", "claude-instant-1.2"]
-    model_aliases = {"gpt-3.5-turbo": "gpt-3.5-turbo-0125"}
-
-    status_url = "https://duckduckgo.com/duckchat/v1/status"
-    chat_url = "https://duckduckgo.com/duckchat/v1/chat"
-    user_agent = 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:123.0) Gecko/20100101 Firefox/123.0'
-    headers = {
-        'User-Agent': user_agent,
-        'Accept': 'text/event-stream',
-        'Accept-Language': 'de,en-US;q=0.7,en;q=0.3',
-        'Accept-Encoding': 'gzip, deflate, br',
-        'Referer': 'https://duckduckgo.com/',
-        'Content-Type': 'application/json',
-        'Origin': 'https://duckduckgo.com',
-        'Connection': 'keep-alive',
-        'Cookie': 'dcm=1',
-        'Sec-Fetch-Dest': 'empty',
-        'Sec-Fetch-Mode': 'cors',
-        'Sec-Fetch-Site': 'same-origin',
-        'Pragma': 'no-cache',
-        'TE': 'trailers'
-    }
-
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
+        proxy: str = None,
         **kwargs
     ) -> AsyncResult:
-        async with aiohttp.ClientSession(headers=cls.headers) as session:
-            async with session.get(cls.status_url, headers={"x-vqd-accept": "1"}) as response:
-                await raise_for_status(response)
-                vqd_4 = response.headers.get("x-vqd-4")
-            payload = {
-                'model': cls.get_model(model),
-                'messages': messages
-            }
-            async with session.post(cls.chat_url, json=payload, headers={"x-vqd-4": vqd_4}) as response:
-                await raise_for_status(response)
-                async for line in response.content:
-                    if line.startswith(b"data: "):
-                        chunk = line[6:]
-                        if chunk.startswith(b"[DONE]"):
+        headers = {
+            'Accept': 'text/event-stream',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Language': 'en-US,en;q=0.5',
+            'Alt-Used': 'chat.3211000.xyz',
+            'Content-Type': 'application/json',
+            'Host': 'chat.3211000.xyz',
+            'Origin': 'https://chat.3211000.xyz',
+            'Referer': 'https://chat.3211000.xyz/',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-origin',
+            'TE': 'trailers',
+            'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:121.0) Gecko/20100101 Firefox/121.0',
+            'x-requested-with': 'XMLHttpRequest'
+        }   
+        async with ClientSession(headers=headers) as session:
+            data = {
+                "messages": messages,
+                "stream": True,
+                "model": "gpt-3.5-turbo",
+                "temperature": 0.5,
+                "presence_penalty": 0,
+                "frequency_penalty": 0,
+                "top_p": 1,
+                **kwargs
+            }    
+            async with session.post(f'{cls.url}/api/openai/v1/chat/completions', json=data, proxy=proxy) as response:
+                response.raise_for_status()
+                async for chunk in response.content:
+                    line = chunk.decode() 
+                    if line.startswith("data: [DONE]"):
                             break
-                        data = json.loads(chunk)
-                        if "message" in data:
-                            yield data["message"]
+                    elif line.startswith("data: "):
+                            line = json.loads(line[6:])
+                            chunk = line["choices"][0]["delta"].get("content")
+                            if(chunk):
+                                yield chunk
```

### Comparing `g4f-0.2.9.9/g4f/Provider/Feedough.py` & `g4f-0.3.0.0/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.0/g4f/Provider/not_working/OnlineGpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,57 @@
 from __future__ import annotations
 
 import json
 from aiohttp import ClientSession
 
-from ..typing import AsyncResult, Messages
-from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from ..requests.raise_for_status import raise_for_status
+from ...typing import AsyncResult, Messages
+from ..base_provider import AsyncGeneratorProvider
+from ..helper import get_random_string
 
-class FlowGpt(AsyncGeneratorProvider, ProviderModelMixin):
-    url = "https://flowgpt.com/chat"
-    working = True
+class OnlineGpt(AsyncGeneratorProvider):
+    url = "https://onlinegpt.org"
+    working = False
     supports_gpt_35_turbo = True
-    supports_message_history = True
-    supports_system_message = True
-    default_model = "gpt-3.5-turbo"
-    models = [
-        "gpt-3.5-turbo",
-        "gpt-3.5-long",
-        "google-gemini",
-        "claude-v2",
-        "llama2-13b"
-    ]
-    model_aliases = {
-        "gemini": "google-gemini",
-        "gemini-pro": "google-gemini"
-    }
+    supports_message_history = False
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
-        temperature: float = 0.7,
         **kwargs
     ) -> AsyncResult:
-        model = cls.get_model(model)
         headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:122.0) Gecko/20100101 Firefox/122.0",
-            "Accept": "*/*",
-            "Accept-Language": "en-US;q=0.7,en;q=0.3",
+            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/119.0",
+            "Accept": "text/event-stream",
+            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
             "Accept-Encoding": "gzip, deflate, br",
-            "Referer": "https://flowgpt.com/",
+            "Referer": f"{cls.url}/chat/",
             "Content-Type": "application/json",
-            "Authorization": "Bearer null",
-            "Origin": "https://flowgpt.com",
+            "Origin": cls.url,
+            "Alt-Used": "onlinegpt.org",
             "Connection": "keep-alive",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-site",
+            "Sec-Fetch-Site": "same-origin",
             "TE": "trailers"
         }
         async with ClientSession(headers=headers) as session:
-            history = [message for message in messages[:-1] if message["role"] != "system"]
-            system_message = "\n".join([message["content"] for message in messages if message["role"] == "system"])
-            if not system_message:
-                system_message = "You are helpful assistant. Follow the user's instructions carefully."
             data = {
-                "model": model,
-                "nsfw": False,
-                "question": messages[-1]["content"],
-                "history": [{"role": "assistant", "content": "Hello, how can I help you today?"}, *history],
-                "system": system_message,
-                "temperature": temperature,
-                "promptId": f"model-{model}",
-                "documentIds": [],
-                "chatFileDocumentIds": [],
-                "generateImage": False,
-                "generateAudio": False
+                "botId": "default",
+                "customId": None,
+                "session": get_random_string(12),
+                "chatId": get_random_string(),
+                "contextId": 9,
+                "messages": messages,
+                "newMessage": messages[-1]["content"],
+                "newImageId": None,
+                "stream": True
             }
-            async with session.post("https://backend-k8s.flowgpt.com/v2/chat-anonymous", json=data, proxy=proxy) as response:
-                await raise_for_status(response)
+            async with session.post(f"{cls.url}/chatgpt/wp-json/mwai-ui/v1/chats/submit", json=data, proxy=proxy) as response:
+                response.raise_for_status()
                 async for chunk in response.content:
-                    if chunk.strip():
-                        message = json.loads(chunk)
-                        if "event" not in message:
-                            continue
-                        if message["event"] == "text":
-                            yield message["data"]
+                    if chunk.startswith(b"data: "):
+                        data = json.loads(chunk[6:])
+                        if data["type"] == "live":
+                            yield data["data"]
```

### Comparing `g4f-0.2.9.9/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.0/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.0/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.0/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.0/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/GigaChat.py` & `g4f-0.3.0.0/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.0/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.0/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.0/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Koala.py` & `g4f-0.3.0.0/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Liaobots.py` & `g4f-0.3.0.0/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Llama2.py` & `g4f-0.3.0.0/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Local.py` & `g4f-0.3.0.0/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.0/g4f/Provider/PerplexityLabs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import random
 import json
-from aiohttp import ClientSession, BaseConnector
 
 from ..typing import AsyncResult, Messages
+from ..requests import StreamSession, raise_for_status
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from .helper import get_connector
 
-API_URL = "https://labs-api.perplexity.ai/socket.io/"
-WS_URL = "wss://labs-api.perplexity.ai/socket.io/"
+API_URL = "https://www.perplexity.ai/socket.io/"
+WS_URL = "wss://www.perplexity.ai/socket.io/"
 
 class PerplexityLabs(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://labs.perplexity.ai"    
     working = True
     default_model = "mixtral-8x7b-instruct"
     models = [
         "sonar-small-online", "sonar-medium-online", "sonar-small-chat", "sonar-medium-chat", "mistral-7b-instruct", 
@@ -31,15 +30,14 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
-        connector: BaseConnector = None,
         **kwargs
     ) -> AsyncResult:
         headers = {
             "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:121.0) Gecko/20100101 Firefox/121.0",
             "Accept": "*/*",
             "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
             "Accept-Encoding": "gzip, deflate, br",
@@ -47,29 +45,30 @@
             "Connection": "keep-alive",
             "Referer": f"{cls.url}/",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-site",
             "TE": "trailers",
         }
-        async with ClientSession(headers=headers, connector=get_connector(connector, proxy)) as session:
+        async with StreamSession(headers=headers, proxies={"all": proxy}) as session:
             t = format(random.getrandbits(32), "08x")
             async with session.get(
                 f"{API_URL}?EIO=4&transport=polling&t={t}"
             ) as response:
+                await raise_for_status(response)
                 text = await response.text()
-
+            assert text.startswith("0")
             sid = json.loads(text[1:])["sid"]
             post_data = '40{"jwt":"anonymous-ask-user"}'
             async with session.post(
                 f"{API_URL}?EIO=4&transport=polling&t={t}&sid={sid}",
                 data=post_data
             ) as response:
-                assert await response.text() == "OK"
-                
+                await raise_for_status(response)
+                assert await response.text() == "OK"                
             async with session.ws_connect(f"{WS_URL}?EIO=4&transport=websocket&sid={sid}", autoping=False) as ws:
                 await ws.send_str("2probe")
                 assert(await ws.receive_str() == "3probe")
                 await ws.send_str("5")
                 assert(await ws.receive_str())
                 assert(await ws.receive_str() == "6")
                 message_data = {
```

### Comparing `g4f-0.2.9.9/g4f/Provider/Pi.py` & `g4f-0.3.0.0/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.0/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/Vercel.py` & `g4f-0.3.0.0/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.0/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/You.py` & `g4f-0.3.0.0/g4f/Provider/You.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,14 @@
             result = await response.json()
         result["user_filename"] = filename
         result["size"] = len(file)
         return result
 
     @classmethod
     async def get_cookies(cls, client: StreamSession) -> Cookies:
-
         if not cls._cookies or cls._cookies_used >= 5:
             cls._cookies = await cls.create_cookies(client)
             cls._cookies_used = 0
         cls._cookies_used += 1
         return cls._cookies        
 
     @classmethod
```

### Comparing `g4f-0.2.9.9/g4f/Provider/__init__.py` & `g4f-0.3.0.0/g4f/Provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 from .ChatForAi        import ChatForAi
 from .Chatgpt4Online   import Chatgpt4Online
 from .ChatgptAi        import ChatgptAi
 from .ChatgptFree      import ChatgptFree
 from .ChatgptNext      import ChatgptNext
 from .ChatgptX         import ChatgptX
 from .Cnote            import Cnote
+from .Cohere           import Cohere
 from .DeepInfra        import DeepInfra
 from .DeepInfraImage   import DeepInfraImage
 from .DuckDuckGo       import DuckDuckGo
+from .Ecosia           import Ecosia
 from .Feedough         import Feedough
 from .FlowGpt          import FlowGpt
 from .FreeChatgpt      import FreeChatgpt
 from .FreeGpt          import FreeGpt
 from .GigaChat         import GigaChat
 from .GeminiPro        import GeminiPro
 from .GeminiProChat    import GeminiProChat
```

### Comparing `g4f-0.2.9.9/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.0/g4f/Provider/bing/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     session (ClientSession): An instance of aiohttp's ClientSession.
     proxy (str, optional): Proxy URL. Defaults to None.
 
     Returns:
     Conversation: An instance representing the created conversation.
     """
     if tone == "Copilot":
-        url = "https://copilot.microsoft.com/turing/conversation/create?bundleVersion=1.1686.0"
+        url = "https://copilot.microsoft.com/turing/conversation/create?bundleVersion=1.1690.0"
     else:
-        url = "https://www.bing.com/turing/conversation/create?bundleVersion=1.1686.0"
+        url = "https://www.bing.com/turing/conversation/create?bundleVersion=1.1690.0"
     async with session.get(url, headers=headers) as response:
         if response.status == 404:
             raise RateLimitError("Response 404: Do less requests and reuse conversations")
         await raise_for_status(response, "Failed to create conversation")
         data = await response.json()
     conversationId = data.get('conversationId')
     clientId = data.get('clientId')
```

### Comparing `g4f-0.2.9.9/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.0/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.0/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.0/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,26 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
+        api_key: str = None,
         cookies: Cookies = None,
         connector: BaseConnector = None,
         image: ImageType = None,
         image_name: str = None,
         **kwargs
     ) -> AsyncResult:
         prompt = format_prompt(messages)
+        if api_key is not None:
+            if cookies is None:
+                cookies = {}
+            cookies["__Secure-1PSID"] = api_key
         cookies = cookies if cookies else get_cookies(".google.com", False, True)
         base_connector = get_connector(connector, proxy)
         async with ClientSession(
             headers=REQUEST_HEADERS,
             connector=base_connector
         ) as session:
             snlm0e  = await cls.fetch_snlm0e(session, cookies) if cookies else None
```

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .Openai import Openai
 from ...typing import AsyncResult, Messages
 
 class OpenRouter(Openai):
     label = "OpenRouter"
     url = "https://openrouter.ai"
     working = True
-    default_model = "openrouter/auto"
+    default_model = "mistralai/mistral-7b-instruct:free"
 
     @classmethod
     def get_models(cls):
         if not cls.models:
             url = 'https://openrouter.ai/api/v1/models'
             models = requests.get(url).json()["data"]
             cls.models = [model['id'] for model in models]
```

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,30 +52,30 @@
                 **extra_data
             )
             
             async with session.post(f"{api_base.rstrip('/')}/chat/completions", json=data) as response:
                 await raise_for_status(response)
                 if not stream:
                     data = await response.json()
+                    cls.raise_error(data)
                     choice = data["choices"][0]
                     if "content" in choice["message"]:
                         yield choice["message"]["content"].strip()
                     finish = cls.read_finish_reason(choice)
                     if finish is not None:
                         yield finish
                 else:
                     first = True
                     async for line in response.iter_lines():
                         if line.startswith(b"data: "):
                             chunk = line[6:]
                             if chunk == b"[DONE]":
                                 break
                             data = json.loads(chunk)
-                            if "error_message" in data:
-                                raise ResponseError(data["error_message"])
+                            cls.raise_error(data)
                             choice = data["choices"][0]
                             if "content" in choice["delta"] and choice["delta"]["content"]:
                                 delta = choice["delta"]["content"]
                                 if first:
                                     delta = delta.lstrip()
                                 if delta:
                                     first = False
@@ -85,14 +85,21 @@
                                 yield finish
 
     @staticmethod
     def read_finish_reason(choice: dict) -> Optional[FinishReason]:
         if "finish_reason" in choice and choice["finish_reason"] is not None:
             return FinishReason(choice["finish_reason"])
 
+    @staticmethod
+    def raise_error(data: dict):
+        if "error_message" in data:
+            raise ResponseError(data["error_message"])
+        elif "error" in data:
+            raise ResponseError(f'Error {data["error"]["code"]}: {data["error"]["message"]}')
+
     @classmethod
     def get_headers(cls, stream: bool, api_key: str = None, headers: dict = None) -> dict:
         return {
             "Accept": "text/event-stream" if stream else "application/json",
             "Content-Type": "application/json",
             **(
                 {"Authorization": f"Bearer {api_key}"}
```

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     from selenium.webdriver.support.ui import WebDriverWait
     from selenium.webdriver.support import expected_conditions as EC
 except ImportError:
     pass
 
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from ...webdriver import get_browser
-from ...typing import AsyncResult, Messages, Cookies, ImageType, Union, AsyncIterator
+from ...typing import AsyncResult, Messages, Cookies, ImageType, AsyncIterator
 from ...requests import get_args_from_browser, raise_for_status
 from ...requests.aiohttp import StreamSession
 from ...image import to_image, to_bytes, ImageResponse, ImageRequest
 from ...errors import MissingAuthError, ResponseError
 from ...providers.conversation import BaseConversation
 from ..openai.har_file import getArkoseAndAccessToken, NoValidHarFileError
 from ... import debug
 
 class OpenaiChat(AsyncGeneratorProvider, ProviderModelMixin):
     """A class for creating and managing conversations with OpenAI chat service"""
 
-    lebel = "OpenAI ChatGPT"
+    label = "OpenAI ChatGPT"
     url = "https://chat.openai.com"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     supports_message_history = True
     supports_system_message = True
     default_model = None
@@ -291,15 +291,15 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
-        timeout: int = 120,
+        timeout: int = 180,
         api_key: str = None,
         cookies: Cookies = None,
         auto_continue: bool = False,
         history_disabled: bool = True,
         action: str = "next",
         conversation_id: str = None,
         conversation: Conversation = None,
@@ -344,15 +344,15 @@
                 cls._headers = cls._api_key = None
             if cls._headers is None or cookies is not None:
                 cls._create_request_args(cookies)
             api_key = kwargs["access_token"] if "access_token" in kwargs else api_key
             if api_key is not None:
                 cls._set_api_key(api_key)
 
-            if cls.default_model is None and cls._api_key is not None:
+            if cls.default_model is None and (not cls.needs_auth or cls._api_key is not None):
                 try:
                     if not model:
                         cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
                     else:
                         cls.default_model = cls.get_model(model)
                 except Exception as e:
                     api_key = cls._api_key = None
@@ -364,20 +364,20 @@
 
             arkose_token = None
             if cls.default_model is None:
                 try:
                     arkose_token, api_key, cookies = await getArkoseAndAccessToken(proxy)
                     cls._create_request_args(cookies)
                     cls._set_api_key(api_key)
-                except NoValidHarFileError:
+                except NoValidHarFileError as e:
                     ...
                 if cls._api_key is None:
-                    if debug.logging:
-                        print("Getting access token with nodriver.")
                     await cls.nodriver_access_token()
+                if cls._api_key is None and cls.needs_auth:
+                    raise e
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             async with session.post(
                 f"{cls.url}/backend-anon/sentinel/chat-requirements" if not cls._api_key else
                 f"{cls.url}/backend-api/sentinel/chat-requirements",
                 json={"conversation_mode_kind": "primary_assistant"},
                 headers=cls._headers
@@ -585,18 +585,19 @@
         except ImportError:
             return
         try:
             from platformdirs import user_config_dir
             user_data_dir = user_config_dir("g4f-nodriver")
         except:
             user_data_dir = None
-        
+        if debug.logging:
+            print(f"Open nodriver with user_dir: {user_data_dir}")
         browser = await uc.start(user_data_dir=user_data_dir)
         page = await browser.get("https://chat.openai.com/")
-        while await page.query_selector("#prompt-textarea") is None:
+        while await page.find("[id^=headlessui-menu-button-]") is None:
             await asyncio.sleep(1)
         api_key = await page.evaluate(
             "(async () => {"
             "let session = await fetch('/api/auth/session');"
             "let data = await session.json();"
             "let accessToken = data['accessToken'];"
             "let expires = new Date(); expires.setTime(expires.getTime() + 60 * 60 * 4 * 1000);"
@@ -605,16 +606,17 @@
             "})();",
             await_promise=True
         )
         cookies = {}
         for c in await page.browser.cookies.get_all():
             if c.domain.endswith("chat.openai.com"):
                 cookies[c.name] = c.value
+        user_agent = await page.evaluate("window.navigator.userAgent")
         await page.close()
-        cls._create_request_args(cookies)
+        cls._create_request_args(cookies, user_agent)
         cls._set_api_key(api_key)
 
     @classmethod
     def browse_access_token(cls, proxy: str = None, timeout: int = 1200) -> None:
         """
         Browse to obtain an access token.
 
@@ -658,29 +660,31 @@
     @staticmethod
     def get_default_headers() -> dict:
         return {
             "accept-language": "en-US",
             "content-type": "application/json",
             "oai-device-id": str(uuid.uuid4()),
             "oai-language": "en-US",
-            "sec-ch-ua": "\"Chromium\";v=\"122\", \"Not(A:Brand\";v=\"24\", \"Google Chrome\";v=\"122\"",
+            "sec-ch-ua": "\"Google Chrome\";v=\"123\", \"Not:A-Brand\";v=\"8\", \"Chromium\";v=\"123\"",
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Linux\"",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin"
         }
 
     @staticmethod
     def _format_cookies(cookies: Cookies):
         return "; ".join(f"{k}={v}" for k, v in cookies.items() if k != "access_token")
 
     @classmethod
-    def _create_request_args(cls, cookies: Cookies = None):
+    def _create_request_args(cls, cookies: Cookies = None, user_agent: str = None):
         cls._headers = cls.get_default_headers()
+        if user_agent is not None:
+            cls._headers["user-agent"] = user_agent
         cls._cookies = {} if cookies is None else cookies
         cls._update_cookie_header()
 
     @classmethod
     def _update_request_args(cls, session: StreamSession):
         for c in session.cookie_jar if hasattr(session, "cookie_jar") else session.cookies.jar:
             cls._cookies[c.key if hasattr(c, "key") else c.name] = c.value
```

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.0/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.0/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.0/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.0/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.0/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.0/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.0/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.0/g4f/Provider/not_working/Gpt6.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,59 +2,53 @@
 
 import json
 from aiohttp import ClientSession
 
 from ...typing import AsyncResult, Messages
 from ..base_provider import AsyncGeneratorProvider
 
-class Chatxyz(AsyncGeneratorProvider):
-    url = "https://chat.3211000.xyz"
+class Gpt6(AsyncGeneratorProvider):
+    url = "https://gpt6.ai"
     working = False
     supports_gpt_35_turbo = True
-    supports_message_history = True
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         **kwargs
     ) -> AsyncResult:
         headers = {
-            'Accept': 'text/event-stream',
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Accept-Language': 'en-US,en;q=0.5',
-            'Alt-Used': 'chat.3211000.xyz',
-            'Content-Type': 'application/json',
-            'Host': 'chat.3211000.xyz',
-            'Origin': 'https://chat.3211000.xyz',
-            'Referer': 'https://chat.3211000.xyz/',
-            'Sec-Fetch-Dest': 'empty',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-origin',
-            'TE': 'trailers',
-            'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:121.0) Gecko/20100101 Firefox/121.0',
-            'x-requested-with': 'XMLHttpRequest'
-        }   
+            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/119.0",
+            "Accept": "*/*",
+            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Content-Type": "application/json",
+            "Origin": "https://gpt6.ai",
+            "Connection": "keep-alive",
+            "Referer": "https://gpt6.ai/",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "cross-site",
+            "TE": "trailers",
+        }
         async with ClientSession(headers=headers) as session:
             data = {
-                "messages": messages,
-                "stream": True,
-                "model": "gpt-3.5-turbo",
-                "temperature": 0.5,
-                "presence_penalty": 0,
-                "frequency_penalty": 0,
-                "top_p": 1,
-                **kwargs
-            }    
-            async with session.post(f'{cls.url}/api/openai/v1/chat/completions', json=data, proxy=proxy) as response:
+                "prompts":messages,
+                "geoInfo":{"ip":"100.90.100.222","hostname":"ip-100-090-100-222.um36.pools.vodafone-ip.de","city":"Muenchen","region":"North Rhine-Westphalia","country":"DE","loc":"44.0910,5.5827","org":"AS3209 Vodafone GmbH","postal":"41507","timezone":"Europe/Berlin"},
+                "paid":False,
+                "character":{"textContent":"","id":"52690ad6-22e4-4674-93d4-1784721e9944","name":"GPT6","htmlContent":""}
+            }
+            async with session.post(f"https://seahorse-app-d29hu.ondigitalocean.app/api/v1/query", json=data, proxy=proxy) as response:
                 response.raise_for_status()
-                async for chunk in response.content:
-                    line = chunk.decode() 
-                    if line.startswith("data: [DONE]"):
-                            break
-                    elif line.startswith("data: "):
-                            line = json.loads(line[6:])
-                            chunk = line["choices"][0]["delta"].get("content")
-                            if(chunk):
-                                yield chunk
+                async for line in response.content:
+                    print(line)
+                    if line.startswith(b"data: [DONE]"):
+                        break
+                    elif line.startswith(b"data: "):
+                        line = json.loads(line[6:-1])
+
+                        chunk = line["choices"][0]["delta"].get("content")
+                        if chunk:
+                            yield chunk
```

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.0/g4f/Provider/not_working/GptGo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 from __future__ import annotations
 
-import json
 from aiohttp import ClientSession
+import json
+import base64
+
+from ...typing       import AsyncResult, Messages
+from ..base_provider import AsyncGeneratorProvider, format_prompt
 
-from ...typing import AsyncResult, Messages
-from ..base_provider import AsyncGeneratorProvider
 
-class Gpt6(AsyncGeneratorProvider):
-    url = "https://gpt6.ai"
-    working = False
+class GptGo(AsyncGeneratorProvider):
+    url                   = "https://gptgo.ai"
+    working               = False
     supports_gpt_35_turbo = True
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         **kwargs
     ) -> AsyncResult:
         headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/119.0",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36",
             "Accept": "*/*",
-            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Content-Type": "application/json",
-            "Origin": "https://gpt6.ai",
-            "Connection": "keep-alive",
-            "Referer": "https://gpt6.ai/",
+            "Accept-language": "en-US",
+            "Origin": cls.url,
+            "Referer": f"{cls.url}/",
+            "sec-ch-ua": '"Google Chrome";v="116", "Chromium";v="116", "Not?A_Brand";v="24"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"Windows"',
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "cross-site",
-            "TE": "trailers",
+            "Sec-Fetch-Site": "same-origin",
         }
-        async with ClientSession(headers=headers) as session:
-            data = {
-                "prompts":messages,
-                "geoInfo":{"ip":"100.90.100.222","hostname":"ip-100-090-100-222.um36.pools.vodafone-ip.de","city":"Muenchen","region":"North Rhine-Westphalia","country":"DE","loc":"44.0910,5.5827","org":"AS3209 Vodafone GmbH","postal":"41507","timezone":"Europe/Berlin"},
-                "paid":False,
-                "character":{"textContent":"","id":"52690ad6-22e4-4674-93d4-1784721e9944","name":"GPT6","htmlContent":""}
-            }
-            async with session.post(f"https://seahorse-app-d29hu.ondigitalocean.app/api/v1/query", json=data, proxy=proxy) as response:
+        async with ClientSession(
+                headers=headers
+            ) as session:
+            async with session.post(
+                "https://gptgo.ai/get_token.php",
+                data={"ask": format_prompt(messages)},
+                proxy=proxy
+            ) as response:
+                response.raise_for_status()
+                token = await response.text();
+                if token == "error token":
+                    raise RuntimeError(f"Response: {token}")
+                token = base64.b64decode(token[10:-20]).decode()
+
+            async with session.get(
+                "https://api.gptgo.ai/web.php",
+                params={"array_chat": token},
+                proxy=proxy
+            ) as response:
                 response.raise_for_status()
                 async for line in response.content:
-                    print(line)
                     if line.startswith(b"data: [DONE]"):
                         break
-                    elif line.startswith(b"data: "):
-                        line = json.loads(line[6:-1])
-
-                        chunk = line["choices"][0]["delta"].get("content")
-                        if chunk:
-                            yield chunk
+                    if line.startswith(b"data: "):
+                        line = json.loads(line[6:])
+                        if "choices" not in line:
+                            raise RuntimeError(f"Response: {line}")
+                        content = line["choices"][0]["delta"].get("content")
+                        if content and content != "\n#GPTGO ":
+                            yield content
```

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.0/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.0/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.0/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 from __future__ import annotations
 
+import re
 from aiohttp import ClientSession
-import json
-import base64
 
-from ...typing       import AsyncResult, Messages
-from ..base_provider import AsyncGeneratorProvider, format_prompt
+from ...typing import AsyncResult, Messages
+from ..base_provider import AsyncGeneratorProvider
+from ..helper import format_prompt
 
 
-class GptGo(AsyncGeneratorProvider):
-    url                   = "https://gptgo.ai"
-    working               = False
+class ChatAiGpt(AsyncGeneratorProvider):
+    url                   = "https://chataigpt.org"
     supports_gpt_35_turbo = True
+    _nonce                = None
+    _post_id              = None
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         **kwargs
     ) -> AsyncResult:
         headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36",
+            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/118.0",
             "Accept": "*/*",
-            "Accept-language": "en-US",
+            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
+            "Accept-Encoding": "gzip, deflate, br",
             "Origin": cls.url,
-            "Referer": f"{cls.url}/",
-            "sec-ch-ua": '"Google Chrome";v="116", "Chromium";v="116", "Not?A_Brand";v="24"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
+            "Alt-Used": cls.url,
+            "Connection": "keep-alive",
+            "Referer": cls.url,
+            "Pragma": "no-cache",
+            "Cache-Control": "no-cache",
+            "TE": "trailers",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
         }
-        async with ClientSession(
-                headers=headers
-            ) as session:
-            async with session.post(
-                "https://gptgo.ai/get_token.php",
-                data={"ask": format_prompt(messages)},
-                proxy=proxy
-            ) as response:
+        async with ClientSession(headers=headers) as session:
+            if not cls._nonce:
+                async with session.get(f"{cls.url}/", proxy=proxy) as response:
+                    response.raise_for_status()
+                    response = await response.text()
+
+                    result = re.search(
+                        r'data-nonce=(.*?) data-post-id=([0-9]+)', response
+                    )
+
+                    if result:
+                        cls._nonce, cls._post_id = result.group(1), result.group(2)
+                    else:
+                        raise RuntimeError("No nonce found")
+            prompt = format_prompt(messages)
+            data = {
+                "_wpnonce": cls._nonce,
+                "post_id": cls._post_id,
+                "url": cls.url,
+                "action": "wpaicg_chat_shortcode_message",
+                "message": prompt,
+                "bot_id": 0
+            }
+            async with session.post(f"{cls.url}/wp-admin/admin-ajax.php", data=data, proxy=proxy) as response:
                 response.raise_for_status()
-                token = await response.text();
-                if token == "error token":
-                    raise RuntimeError(f"Response: {token}")
-                token = base64.b64decode(token[10:-20]).decode()
-
-            async with session.get(
-                "https://api.gptgo.ai/web.php",
-                params={"array_chat": token},
-                proxy=proxy
-            ) as response:
-                response.raise_for_status()
-                async for line in response.content:
-                    if line.startswith(b"data: [DONE]"):
-                        break
-                    if line.startswith(b"data: "):
-                        line = json.loads(line[6:])
-                        if "choices" not in line:
-                            raise RuntimeError(f"Response: {line}")
-                        content = line["choices"][0]["delta"].get("content")
-                        if content and content != "\n#GPTGO ":
-                            yield content
+                async for chunk in response.content:
+                    if chunk:
+                        yield chunk.decode()
```

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.0/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.0/g4f/Provider/unfinished/AiChatting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from __future__ import annotations
 
-import json
-from aiohttp import ClientSession
+from urllib.parse import unquote
 
 from ...typing import AsyncResult, Messages
-from ..base_provider import AsyncGeneratorProvider
-from ..helper import get_random_string
+from ..base_provider import AbstractProvider
+from ...webdriver import WebDriver
+from ...requests import Session, get_session_from_browser
 
-class OnlineGpt(AsyncGeneratorProvider):
-    url = "https://onlinegpt.org"
-    working = False
+class AiChatting(AbstractProvider):
+    url = "https://www.aichatting.net"
     supports_gpt_35_turbo = True
-    supports_message_history = False
+    _session: Session = None
 
     @classmethod
-    async def create_async_generator(
+    def create_completion(
         cls,
         model: str,
         messages: Messages,
+        stream: bool,
         proxy: str = None,
+        timeout: int = 120,
+        webdriver: WebDriver = None,
         **kwargs
     ) -> AsyncResult:
+        if not cls._session:
+            cls._session = get_session_from_browser(cls.url, webdriver, proxy, timeout)
+        visitorId = unquote(cls._session.cookies.get("aichatting.website.visitorId"))
+                        
         headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/119.0",
-            "Accept": "text/event-stream",
-            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Referer": f"{cls.url}/chat/",
-            "Content-Type": "application/json",
-            "Origin": cls.url,
-            "Alt-Used": "onlinegpt.org",
-            "Connection": "keep-alive",
-            "Sec-Fetch-Dest": "empty",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-origin",
-            "TE": "trailers"
+            "accept": "application/json, text/plain, */*",
+            "lang": "en",
+            "source": "web"
         }
-        async with ClientSession(headers=headers) as session:
-            data = {
-                "botId": "default",
-                "customId": None,
-                "session": get_random_string(12),
-                "chatId": get_random_string(),
-                "contextId": 9,
-                "messages": messages,
-                "newMessage": messages[-1]["content"],
-                "newImageId": None,
-                "stream": True
-            }
-            async with session.post(f"{cls.url}/chatgpt/wp-json/mwai-ui/v1/chats/submit", json=data, proxy=proxy) as response:
-                response.raise_for_status()
-                async for chunk in response.content:
-                    if chunk.startswith(b"data: "):
-                        data = json.loads(chunk[6:])
-                        if data["type"] == "live":
-                            yield data["data"]
+        data = {
+            "roleId": 0,
+        }
+        try:
+            response = cls._session.post("https://aga-api.aichatting.net/aigc/chat/record/conversation/create", json=data, headers=headers)
+            response.raise_for_status()
+            conversation_id = response.json()["data"]["conversationId"]
+        except Exception as e:
+            cls.reset()
+            raise e
+        headers = {
+            "authority": "aga-api.aichatting.net",
+            "accept": "text/event-stream,application/json, text/event-stream",
+            "lang": "en",
+            "source": "web",
+            "vtoken": visitorId,
+        }
+        data = {
+            "spaceHandle": True,
+            "roleId": 0,
+            "messages": messages,
+            "conversationId": conversation_id,
+        }
+        response = cls._session.post("https://aga-api.aichatting.net/aigc/chat/v2/stream", json=data, headers=headers, stream=True)
+        response.raise_for_status()
+        for chunk in response.iter_lines():
+            if chunk.startswith(b"data:"):
+                yield chunk[5:].decode().replace("-=- --", " ").replace("-=-n--", "\n").replace("--@DONE@--", "")
+
+    @classmethod
+    def reset(cls):
+        cls._session = None
```

### Comparing `g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.0/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.0/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.0/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.0/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.0/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.0/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.0/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.0/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.0/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.0/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.0/g4f/Provider/DuckDuckGo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 from __future__ import annotations
 
-import re
-from aiohttp import ClientSession
+import json
+import aiohttp
 
-from ...typing import AsyncResult, Messages
-from ..base_provider import AsyncGeneratorProvider
-from ..helper import format_prompt
-
-
-class ChatAiGpt(AsyncGeneratorProvider):
-    url                   = "https://chataigpt.org"
+from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
+from .helper import get_connector
+from ..typing import AsyncResult, Messages
+from ..requests.raise_for_status import raise_for_status
+from ..providers.conversation import BaseConversation
+
+class DuckDuckGo(AsyncGeneratorProvider, ProviderModelMixin):
+    url = "https://duckduckgo.com/duckchat"
+    working = True
     supports_gpt_35_turbo = True
-    _nonce                = None
-    _post_id              = None
+    supports_message_history = True
+
+    default_model = "gpt-3.5-turbo-0125"
+    models = ["gpt-3.5-turbo-0125", "claude-instant-1.2"]
+    model_aliases = {"gpt-3.5-turbo": "gpt-3.5-turbo-0125"}
+
+    status_url = "https://duckduckgo.com/duckchat/v1/status"
+    chat_url = "https://duckduckgo.com/duckchat/v1/chat"
+    user_agent = 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:123.0) Gecko/20100101 Firefox/123.0'
+    headers = {
+        'User-Agent': user_agent,
+        'Accept': 'text/event-stream',
+        'Accept-Language': 'de,en-US;q=0.7,en;q=0.3',
+        'Accept-Encoding': 'gzip, deflate, br',
+        'Referer': 'https://duckduckgo.com/',
+        'Content-Type': 'application/json',
+        'Origin': 'https://duckduckgo.com',
+        'Connection': 'keep-alive',
+        'Cookie': 'dcm=1',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Pragma': 'no-cache',
+        'TE': 'trailers'
+    }
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
+        connector: aiohttp.BaseConnector = None,
+        conversation: Conversation = None,
+        return_conversation: bool = False,
         **kwargs
     ) -> AsyncResult:
-        headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/118.0",
-            "Accept": "*/*",
-            "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Origin": cls.url,
-            "Alt-Used": cls.url,
-            "Connection": "keep-alive",
-            "Referer": cls.url,
-            "Pragma": "no-cache",
-            "Cache-Control": "no-cache",
-            "TE": "trailers",
-            "Sec-Fetch-Dest": "empty",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-origin",
-        }
-        async with ClientSession(headers=headers) as session:
-            if not cls._nonce:
-                async with session.get(f"{cls.url}/", proxy=proxy) as response:
-                    response.raise_for_status()
-                    response = await response.text()
-
-                    result = re.search(
-                        r'data-nonce=(.*?) data-post-id=([0-9]+)', response
-                    )
-
-                    if result:
-                        cls._nonce, cls._post_id = result.group(1), result.group(2)
-                    else:
-                        raise RuntimeError("No nonce found")
-            prompt = format_prompt(messages)
-            data = {
-                "_wpnonce": cls._nonce,
-                "post_id": cls._post_id,
-                "url": cls.url,
-                "action": "wpaicg_chat_shortcode_message",
-                "message": prompt,
-                "bot_id": 0
+        async with aiohttp.ClientSession(headers=cls.headers, connector=get_connector(connector, proxy)) as session:
+            if conversation is not None and len(messages) > 1:
+                vqd_4 = conversation.vqd_4
+                messages = [*conversation.messages, messages[-2], messages[-1]]
+            else:
+                async with session.get(cls.status_url, headers={"x-vqd-accept": "1"}) as response:
+                    await raise_for_status(response)
+                    vqd_4 = response.headers.get("x-vqd-4")
+                messages = [messages[-1]]
+            payload = {
+                'model': cls.get_model(model),
+                'messages': messages
             }
-            async with session.post(f"{cls.url}/wp-admin/admin-ajax.php", data=data, proxy=proxy) as response:
-                response.raise_for_status()
-                async for chunk in response.content:
-                    if chunk:
-                        yield chunk.decode()
+            async with session.post(cls.chat_url, json=payload, headers={"x-vqd-4": vqd_4}) as response:
+                await raise_for_status(response)
+                if return_conversation:
+                    yield Conversation(response.headers.get("x-vqd-4"), messages)
+                async for line in response.content:
+                    if line.startswith(b"data: "):
+                        chunk = line[6:]
+                        if chunk.startswith(b"[DONE]"):
+                            break
+                        data = json.loads(chunk)
+                        if "message" in data and data["message"]:
+                            yield data["message"]
+
+class Conversation(BaseConversation):
+    def __init__(self, vqd_4: str, messages: Messages) -> None:
+        self.vqd_4 = vqd_4
+        self.messages = messages
```

### Comparing `g4f-0.2.9.9/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.0/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.0/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/unfinished/Replicate.py` & `g4f-0.3.0.0/g4f/Provider/unfinished/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/Provider/you/har_file.py` & `g4f-0.3.0.0/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/__init__.py` & `g4f-0.3.0.0/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/api/__init__.py` & `g4f-0.3.0.0/g4f/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import logging
 import json
 import uvicorn
-import nest_asyncio
 
 from fastapi import FastAPI, Response, Request
 from fastapi.responses import StreamingResponse, RedirectResponse, HTMLResponse, JSONResponse
 from fastapi.exceptions import RequestValidationError
 from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
-from typing import List, Union
+from typing import List, Union, Optional
 
 import g4f
 import g4f.debug
-from g4f.client import Client
+from g4f.client import AsyncClient
 from g4f.typing import Messages
 
 class ChatCompletionsConfig(BaseModel):
     messages: Messages
     model: str
-    provider: Union[str, None] = None
+    provider: Optional[str] = None
     stream: bool = False
-    temperature: Union[float, None] = None
-    max_tokens: Union[int, None] = None
+    temperature: Optional[float] = None
+    max_tokens: Optional[int] = None
     stop: Union[list[str], str, None] = None
-    api_key: Union[str, None] = None
+    api_key: Optional[str] = None
+    web_search: Optional[bool] = None
 
 class Api:
     def __init__(self, engine: g4f, debug: bool = True, sentry: bool = False,
                  list_ignored_providers: List[str] = None) -> None:
         self.engine = engine
         self.debug = debug
         self.sentry = sentry
         self.list_ignored_providers = list_ignored_providers
 
         if debug:
             g4f.debug.logging = True
-        self.client = Client()
-
-        nest_asyncio.apply()
+        self.client = AsyncClient()
         self.app = FastAPI()
 
         self.routes()
         self.register_validation_exception_handler()
 
     def register_validation_exception_handler(self):
         @self.app.exception_handler(RequestValidationError)
@@ -86,15 +84,15 @@
                 'owned_by': model.base_provider
             } for model_id, model in model_list.items()]
             return JSONResponse(model_list)
 
         @self.app.get("/v1/models/{model_name}")
         async def model_info(model_name: str):
             try:
-                model_info = g4f.ModelUtils.convert[model_name]
+                model_info = g4f.models.ModelUtils.convert[model_name]
                 return JSONResponse({
                     'id': model_name,
                     'object': 'model',
                     'created': 0,
                     'owned_by': model_info.base_provider
                 })
             except:
@@ -115,25 +113,26 @@
                     ignored=self.list_ignored_providers
                 )
             except Exception as e:
                 logging.exception(e)
                 return Response(content=format_exception(e, config), status_code=500, media_type="application/json")
 
             if not config.stream:
-                return JSONResponse(response.to_json())
+                return JSONResponse((await response).to_json())
 
-            def streaming():
+            async def streaming():
                 try:
-                    for chunk in response:
+                    async for chunk in response:
                         yield f"data: {json.dumps(chunk.to_json())}\n\n"
                 except GeneratorExit:
                     pass
                 except Exception as e:
                     logging.exception(e)
-                    yield f'data: {format_exception(e, config)}'
+                    yield f'data: {format_exception(e, config)}\n\n'
+                yield "data: [DONE]\n\n"
 
             return StreamingResponse(streaming(), media_type="text/event-stream")
 
         @self.app.post("/v1/completions")
         async def completions():
             return Response(content=json.dumps({'info': 'Not working yet.'}, indent=4), media_type="application/json")
```

### Comparing `g4f-0.2.9.9/g4f/api/_logging.py` & `g4f-0.3.0.0/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/cli.py` & `g4f-0.3.0.0/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/async_client.py` & `g4f-0.3.0.0/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/client.py` & `g4f-0.3.0.0/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/helper.py` & `g4f-0.3.0.0/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/image_models.py` & `g4f-0.3.0.0/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/service.py` & `g4f-0.3.0.0/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/stubs.py` & `g4f-0.3.0.0/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/client/types.py` & `g4f-0.3.0.0/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/cookies.py` & `g4f-0.3.0.0/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/errors.py` & `g4f-0.3.0.0/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/__init__.py` & `g4f-0.3.0.0/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/index.html` & `g4f-0.3.0.0/g4f/gui/client/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
         import mistralTokenizer from "mistral-tokenizer-js"
     </script>
     <script type="module" src="https://belladoreai.github.io/llama-tokenizer-js/llama-tokenizer.js" async>
         import llamaTokenizer from "llama-tokenizer-js"
     </script>
     <script src="https://unpkg.com/gpt-tokenizer/dist/cl100k_base.js" async></script>
     <script src="/static/js/text_to_speech/index.js" async></script>
+    <!--
+            <script src="/static/js/whisper-web/index.js" async></script>
+    -->
     <script>
         const user_image = '<img src="/static/img/user.png" alt="your avatar">';
         const gpt_image = '<img src="/static/img/gpt.png" alt="your avatar">';
     </script>
     <script src="/static/js/highlight.min.js"></script>
     <script>window.conversation_id = "{{chat_id}}"</script>
     <title>g4f - gui</title>
@@ -85,14 +88,15 @@
             </div>
         </div>
         <div class="images hidden">
             
         </div>
         <div class="settings hidden">
             <div class="paper">
+            <h3>Settings</h3>
             <div class="field">
                 <span class="label">Web Access</span>
                 <input type="checkbox" id="switch" />
                 <label for="switch" class="toogle" title="Add the pages of the first 5 search results to the query."></label>
             </div>
             <div class="field">
                 <span class="label">Disable History</span>
@@ -123,35 +127,35 @@
             </div>
             <div class="field box">
                 <label for="DeepInfra-api_key" class="label" title="">DeepInfra:</label>
                 <textarea id="DeepInfra-api_key" name="DeepInfra[api_key]" class="DeepInfraImage-api_key" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="Gemini-api_key" class="label" title="">Gemini:</label>
-                <textarea id="Gemini-api_key" name="Gemini[api_key]" placeholder="Cookies"></textarea>
+                <textarea id="Gemini-api_key" name="Gemini[api_key]" placeholder="&quot;__Secure-1PSID&quot; cookie"></textarea>
             </div>
             <div class="field box">
-                <label for="GeminiPro-api_key" class="label" title="">GeminiPro:</label>
+                <label for="GeminiPro-api_key" class="label" title="">GeminiPro API:</label>
                 <textarea id="GeminiPro-api_key" name="GeminiPro[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="Groq-api_key" class="label" title="">Groq:</label>
                 <textarea id="Groq-api_key" name="Groq[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="HuggingFace-api_key" class="label" title="">HuggingFace:</label>
                 <textarea id="HuggingFace-api_key" name="HuggingFace[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
-                <label for="Openai-api_key" class="label" title="">Openai:</label>
+                <label for="Openai-api_key" class="label" title="">OpenAI API:</label>
                 <textarea id="Openai-api_key" name="Openai[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
-                <label for="OpenaiChat-api_key" class="label" title="">OpenaiChat:</label>
-                <textarea id="OpenaiChat-api_key" name="OpenaiChat[api_key]" placeholder="api_key"></textarea>
+                <label for="OpenaiAccount-api_key" class="label" title="">OpenAI ChatGPT:</label>
+                <textarea id="OpenaiAccount-api_key" name="OpenaiAccount[api_key]" placeholder="access_key"></textarea>
             </div>
             <div class="field box">
                 <label for="OpenRouter-api_key" class="label" title="">OpenRouter:</label>
                 <textarea id="OpenRouter-api_key" name="OpenRouter[api_key]" placeholder="api_key"></textarea>
             </div>
             </div>
             <div class="bottom_buttons">
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 New Conversation
 Open Settings
 discord ~ _d_i_s_c_o_r_d_._g_g_/_X_f_y_b_z_P_X_P_H_5
 github ~ _@_x_t_e_k_k_y_/_g_p_t_4_f_r_e_e
+******** SSeettttiinnggss ********
 Web Access??
 Disable History??
 Hide System prompt??
 Auto continue
 Input max. height[Unknown INPUT type]
 Speech recognition lang[                    ]
 Clear Conversations Export Conversations
```

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.0/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -598,15 +598,16 @@
 
 .settings .bottom_buttons button {
     display: inline-block;
     max-width: 210px;
     width: 100%;
 }
 
-.buttons input:checked+label:after {
+.buttons input:checked+label:after,
+.settings input:checked+label:after {
     left: calc(100% - 5px - 20px);
 }
 
 .buttons {
     display: flex;
     align-items: center;
     justify-content: left;
@@ -833,21 +834,30 @@
     transition: 0.33s;
 }
 
 .rotated {
     transform: rotate(360deg);
 }
 
+.settings h3 {
+    padding-left: 10px;
+    padding-top: 10px;
+}
+
 @media screen and (max-width: 990px) {
     .conversations {
         display: none;
         width: 100%;
         max-width: none;
     }
 
+    .settings h3 {
+        padding-left: 50px;
+    }
+
     .buttons {
         align-items: flex-start;
         flex-wrap: wrap;
         gap: 15px;
     }
 
     .mobile-sidebar {
@@ -1095,18 +1105,18 @@
     padding: var(--inner-gap) var(--inner-gap) var(--inner-gap) 0;
 }
 
 .settings, .images {
     width: 100%;
     display: flex;
     flex-direction: column;
+    overflow: auto;
 }
 
 .settings .paper {
-    overflow: auto;
     flex-direction: column;
     min-width: 400px;
 }
 
 .settings .field {
     margin: var(--inner-gap) 0;
 }
```

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.0/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/chat.v1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,15 @@
 const microLabel = document.querySelector(".micro-label");
 const inputCount = document.getElementById("input-count");
 const providerSelect = document.getElementById("provider");
 const modelSelect = document.getElementById("model");
 const modelProvider = document.getElementById("model2");
 const systemPrompt = document.getElementById("systemPrompt");
 const settings = document.querySelector(".settings");
+const chat = document.querySelector(".conversation");
 const album = document.querySelector(".images");
 
 let prompt_lock = false;
 
 let content, content_inner, content_count = null;
 
 const optionElements = document.querySelectorAll(".settings input, .settings textarea, #model, #model2, #provider")
@@ -129,15 +130,15 @@
                 let speechText = await get_message(window.conversation_id, message_el.dataset.index);
 
                 speechText = speechText.replaceAll(/([^0-9])\./gm, "$1.;");
                 speechText = speechText.replaceAll("?", "?;");
                 speechText = speechText.replaceAll(/\[(.+)\]\(.+\)/gm, "($1)");
                 speechText = speechText.replaceAll(/```[a-z]+/gm, "");
                 speechText = filter_message(speechText.replaceAll("`", "").replaceAll("#", ""))
-                const lines = speechText.trim().split(/\n|;/).filter(v => v.trim());
+                const lines = speechText.trim().split(/\n|;/).filter(v => count_words(v));
 
                 window.onSpeechResponse = (url) => {
                     if (!el.dataset.stopped) {
                         el.classList.remove("blink")
                     }
                     if (url) {
                         var sound = document.createElement('audio');
@@ -787,14 +788,15 @@
     return BigInt(`0b${unix}${random_bytes}`).toString();
 };
 
 async function hide_sidebar() {
     sidebar.classList.remove("shown");
     sidebar_button.classList.remove("rotated");
     settings.classList.add("hidden");
+    chat.classList.remove("hidden");
     if (window.location.pathname == "/menu/" || window.location.pathname == "/settings/") {
         history.back();
     }
 }
 
 window.addEventListener('popstate', hide_sidebar, false);
 
@@ -808,19 +810,21 @@
         history.pushState({}, null, "/menu/");
     }
     window.scrollTo(0, 0);
 });
 
 function open_settings() {
     if (settings.classList.contains("hidden")) {
+        chat.classList.add("hidden");
         sidebar.classList.remove("shown");
         settings.classList.remove("hidden");
         history.pushState({}, null, "/settings/");
     } else {
         settings.classList.add("hidden");
+        chat.classList.remove("hidden");
     }
 }
 
 function open_album() {
     if (album.classList.contains("hidden")) {
         sidebar.classList.remove("shown");
         settings.classList.add("hidden");
@@ -1278,28 +1282,22 @@
 
     const recognition = new SpeechRecognition();
     recognition.continuous = true;
     recognition.interimResults = true;
     recognition.maxAlternatives = 1;
 
     let startValue;
-    let shouldStop;
     let lastDebounceTranscript;
     recognition.onstart = function() {
         microLabel.classList.add("recognition");
         startValue = messageInput.value;
-        shouldStop = false;
         lastDebounceTranscript = "";
     };
     recognition.onend = function() {
-        if (shouldStop) {
-            messageInput.focus();
-        } else {
-            recognition.start();
-        }
+        messageInput.focus();
     };
     recognition.onresult = function(event) {
         if (!event.results) {
             return;
         }
         let result = event.results[event.resultIndex];
         let isFinal = result.isFinal && (result[0].confidence > 0);
@@ -1318,15 +1316,14 @@
             messageInput.style.height = messageInput.scrollHeight + "px";
             messageInput.scrollTop = messageInput.scrollHeight;
         }
     };
 
     microLabel.addEventListener("click", () => {
         if (microLabel.classList.contains("recognition")) {
-            shouldStop = true;
             recognition.stop();
             microLabel.classList.remove("recognition");
         } else {
             const lang = document.getElementById("recognition-language")?.value;
             recognition.lang = lang || navigator.language;
             recognition.start();
         }
```

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.0/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.0/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/api.py` & `g4f-0.3.0.0/g4f/gui/server/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         """
         return {
             provider.__name__: (provider.label
                 if hasattr(provider, "label")
                 else provider.__name__) +
                 (" (WebDriver)"
                 if "webdriver" in provider.get_parameters()
+                else "") + 
+                (" (Auth)"
+                if provider.needs_auth
                 else "")
             for provider in __providers__
             if provider.working
         }
 
     def get_version(self):
         """
```

### Comparing `g4f-0.2.9.9/g4f/gui/server/backend.py` & `g4f-0.3.0.0/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/config.py` & `g4f-0.3.0.0/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/internet.py` & `g4f-0.3.0.0/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/js_api.py` & `g4f-0.3.0.0/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/server/website.py` & `g4f-0.3.0.0/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/gui/webview.py` & `g4f-0.3.0.0/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/image.py` & `g4f-0.3.0.0/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/local/__init__.py` & `g4f-0.3.0.0/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/locals/models.py` & `g4f-0.3.0.0/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/locals/provider.py` & `g4f-0.3.0.0/g4f/locals/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,13 +62,16 @@
         prompt_template = "USER: {0}\nASSISTANT: "
         conversation    = "\n" . join(
             f"{message['role'].upper()}: {message['content']}"
             for message in messages
             if message["role"] != "system"
         ) + "\nASSISTANT: "
 
+        def should_not_stop(token_id: int, token: str):
+            return "USER" not in token
+
         with model.chat_session(system_message, prompt_template):
             if stream:
-                for token in model.generate(conversation, streaming=True):
+                for token in model.generate(conversation, streaming=True, callback=should_not_stop):
                     yield token
             else:
-                yield model.generate(conversation)
+                yield model.generate(conversation, callback=should_not_stop)
```

### Comparing `g4f-0.2.9.9/g4f/models.py` & `g4f-0.3.0.0/g4f/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     GigaChat,
     Liaobots,
     FreeGpt,
     Llama2,
     Vercel,
     Gemini,
     Koala,
+    Cohere,
     Bing,
     You,
     Pi,
 )
 
 @dataclass(unsafe_hash=True)
 class Model:
@@ -271,15 +272,15 @@
     base_provider = 'mistral',
     best_provider = RetryProvider([DeepInfra, PerplexityLabs])
 )
 
 command_r_plus = Model(
     name = 'CohereForAI/c4ai-command-r-plus',
     base_provider = 'mistral',
-    best_provider = HuggingChat
+    best_provider = RetryProvider([HuggingChat, Cohere])
 )
 
 class ModelUtils:
     """
     Utility class for mapping string identifiers to Model instances.
 
     Attributes:
```

### Comparing `g4f-0.2.9.9/g4f/providers/base_provider.py` & `g4f-0.3.0.0/g4f/providers/base_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,21 @@
 if sys.version_info < (3, 10):
     NoneType = type(None)
 else:
     from types import NoneType
 
 # Set Windows event loop policy for better compatibility with asyncio and curl_cffi
 if sys.platform == 'win32':
-    if isinstance(asyncio.get_event_loop_policy(), asyncio.WindowsProactorEventLoopPolicy):
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+    try:
+        from curl_cffi import aio
+        if not hasattr(aio, "_get_selector"):
+            if isinstance(asyncio.get_event_loop_policy(), asyncio.WindowsProactorEventLoopPolicy):
+                asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+    except ImportError:
+        pass
 
 def get_running_loop(check_nested: bool) -> Union[AbstractEventLoop, None]:
     try:
         loop = asyncio.get_running_loop()
         if check_nested and not hasattr(loop.__class__, "_nest_patched"):
             try:
                 import nest_asyncio
@@ -260,24 +265,26 @@
         Raises:
             NotImplementedError: If this method is not overridden in derived classes.
 
         Returns:
             AsyncResult: An asynchronous generator yielding results.
         """
         raise NotImplementedError()
-    
+
 class ProviderModelMixin:
     default_model: str
     models: list[str] = []
     model_aliases: dict[str, str] = {}
-    
+
     @classmethod
     def get_models(cls) -> list[str]:
+        if not cls.models:
+            return [cls.default_model]
         return cls.models
-    
+
     @classmethod
     def get_model(cls, model: str) -> str:
         if not model and cls.default_model is not None:
             model = cls.default_model
         elif model in cls.model_aliases:
             model = cls.model_aliases[model]
         elif model not in cls.get_models() and cls.models:
```

### Comparing `g4f-0.2.9.9/g4f/providers/create_images.py` & `g4f-0.3.0.0/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/providers/helper.py` & `g4f-0.3.0.0/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/providers/retry_provider.py` & `g4f-0.3.0.0/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/providers/types.py` & `g4f-0.3.0.0/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/requests/__init__.py` & `g4f-0.3.0.0/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/requests/aiohttp.py` & `g4f-0.3.0.0/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/requests/curl_cffi.py` & `g4f-0.3.0.0/g4f/requests/curl_cffi.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 from curl_cffi.requests import AsyncSession, Response
 try:
     from curl_cffi.requests import CurlMime
     has_curl_mime = True
 except ImportError:
     has_curl_mime = False
+try:
+    from curl_cffi.requests import CurlWsFlag
+    has_curl_ws = True
+except ImportError:
+    has_curl_ws = False
 from typing import AsyncGenerator, Any
 from functools import partialmethod
 import json
 
 class StreamResponse:
     """
     A wrapper class for handling asynchronous streaming responses.
@@ -69,14 +74,20 @@
         self, method: str, url: str, **kwargs
     ) -> StreamResponse:
         if isinstance(kwargs.get("data"), CurlMime):
             kwargs["multipart"] = kwargs.pop("data")
         """Create and return a StreamResponse object for the given HTTP request."""
         return StreamResponse(super().request(method, url, stream=True, **kwargs))
 
+    def ws_connect(self, url, *args, **kwargs):
+        return WebSocket(self, url)
+
+    def _ws_connect(self, url):
+        return super().ws_connect(url)
+
     # Defining HTTP methods as partial methods of the request method.
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
@@ -84,8 +95,29 @@
 if has_curl_mime:
     class FormData(CurlMime):
         def add_field(self, name, data=None, content_type: str = None, filename: str = None) -> None:
             self.addpart(name, content_type=content_type, filename=filename, data=data)
 else:
     class FormData():
         def __init__(self) -> None:
-            raise RuntimeError("CurlMimi in curl_cffi is missing | pip install -U g4f[curl_cffi]")
+            raise RuntimeError("CurlMimi in curl_cffi is missing | pip install -U g4f[curl_cffi]")
+
+class WebSocket():
+    def __init__(self, session, url) -> None:
+        if not has_curl_ws:
+            raise RuntimeError("CurlWsFlag in curl_cffi is missing | pip install -U g4f[curl_cffi]")
+        self.session: StreamSession = session
+        self.url: str = url
+
+    async def __aenter__(self):
+        self.inner = await self.session._ws_connect(self.url)
+        return self
+
+    async def __aexit__(self, *args):
+        self.inner.aclose()
+
+    async def receive_str(self) -> str:
+        bytes, _ = await self.inner.arecv()
+        return bytes.decode(errors="ignore")
+
+    async def send_str(self, data: str):
+        await self.inner.asend(data.encode(), CurlWsFlag.TEXT)
```

### Comparing `g4f-0.2.9.9/g4f/requests/defaults.py` & `g4f-0.3.0.0/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/requests/raise_for_status.py` & `g4f-0.3.0.0/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/stubs.py` & `g4f-0.3.0.0/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/typing.py` & `g4f-0.3.0.0/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/version.py` & `g4f-0.3.0.0/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f/webdriver.py` & `g4f-0.3.0.0/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.0/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.9
+Version: 0.3.0.0
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.9 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.0 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.2.9.9/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.0/g4f.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 g4f/Provider/ChatForAi.py
 g4f/Provider/Chatgpt4Online.py
 g4f/Provider/ChatgptAi.py
 g4f/Provider/ChatgptFree.py
 g4f/Provider/ChatgptNext.py
 g4f/Provider/ChatgptX.py
 g4f/Provider/Cnote.py
+g4f/Provider/Cohere.py
 g4f/Provider/DeepInfra.py
 g4f/Provider/DeepInfraImage.py
 g4f/Provider/DuckDuckGo.py
+g4f/Provider/Ecosia.py
 g4f/Provider/Feedough.py
 g4f/Provider/FlowGpt.py
 g4f/Provider/FreeChatgpt.py
 g4f/Provider/FreeGpt.py
 g4f/Provider/GeminiPro.py
 g4f/Provider/GeminiProChat.py
 g4f/Provider/GigaChat.py
@@ -101,14 +103,15 @@
 g4f/Provider/deprecated/Yqcloud.py
 g4f/Provider/deprecated/__init__.py
 g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
 g4f/Provider/needs_auth/Gemini.py
 g4f/Provider/needs_auth/Groq.py
 g4f/Provider/needs_auth/OpenRouter.py
 g4f/Provider/needs_auth/Openai.py
+g4f/Provider/needs_auth/OpenaiAccount.py
 g4f/Provider/needs_auth/OpenaiChat.py
 g4f/Provider/needs_auth/Poe.py
 g4f/Provider/needs_auth/Raycast.py
 g4f/Provider/needs_auth/Theb.py
 g4f/Provider/needs_auth/ThebApi.py
 g4f/Provider/needs_auth/__init__.py
 g4f/Provider/not_working/AItianhu.py
```

### Comparing `g4f-0.2.9.9/g4f.egg-info/requires.txt` & `g4f-0.3.0.0/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.9/setup.py` & `g4f-0.3.0.0/setup.py`

 * *Files identical despite different names*


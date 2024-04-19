# Comparing `tmp/llm-api-open-2.1.24.tar.gz` & `tmp/llm_api_open-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-api-open-2.1.24.tar", last modified: Tue Apr  9 22:01:48 2024, max compression
+gzip compressed data, was "llm_api_open-2.3.1.tar", last modified: Fri Apr 19 09:22:13 2024, max compression
```

## Comparing `llm-api-open-2.1.24.tar` & `llm_api_open-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.133995 llm-api-open-2.1.24/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/configs/chatgpt.json
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/configs/ms_copilot.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.133995 llm-api-open-2.1.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/llm_api_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/assistantGetLastMessage.js
--rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/conversationSearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/proxy_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/external_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/module_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/ms_copilot/
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/conversationManage.js
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/conversationParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    43383 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/ms_copilot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/proxy_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-19 09:22:09.000000 llm_api_open-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23207 2024-04-19 09:22:09.000000 llm_api_open-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.311290 llm_api_open-2.3.1/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.311290 llm_api_open-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 09:22:13.000000 llm_api_open-2.3.1/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11943 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:22:13.315290 llm_api_open-2.3.1/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43383 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 09:22:10.000000 llm_api_open-2.3.1/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm-api-open-2.1.24/LICENSE` & `llm_api_open-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/README.md` & `llm_api_open-2.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -147,34 +147,48 @@
 module.close(blocking=True)
 ```
 
 ----------
 
 ## 💻 CLI example
 
-```shell
+```text
 $ lmao --help        
-usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens-use TOKENS_USE [TOKENS_USE ...]]
+            [--tokens-manage TOKENS_MANAGE [TOKENS_MANAGE ...]] [--rate-limits-default RATE_LIMITS_DEFAULT [RATE_LIMITS_DEFAULT ...]] [--rate-limit-fast RATE_LIMIT_FAST]
+            [--no-logging-init]
 
 Unofficial open APIs for popular LLMs with self-hosted redirect capability
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -c CONFIGS, --configs CONFIGS
                         path to configs directory with each module config file (Default: configs)
   -t TEST, --test TEST  module name to test in cli instead of starting API server (eg. --test=chatgpt)
   -i IP, --ip IP        API server Host (IP) (Default: localhost)
   -p PORT, --port PORT  API server port (Default: 1312)
+  -s SSL [SSL ...], --ssl SSL [SSL ...]
+                        Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt" "path/to/private.key")
+  --tokens-use TOKENS_USE [TOKENS_USE ...]
+                        API tokens to enable authorization for /status, /ask, /stop and /delete (ex. --tokens-use "tokenForMyApp" "tokenForMyAnotherApp"
+                        "ultraPrivateTokeeeeeen")
+  --tokens-manage TOKENS_MANAGE [TOKENS_MANAGE ...]
+                        API tokens to enable authorization for /init and /close (ex. --tokens-manage "ultraPrivateTokeeeeeen")
+  --rate-limits-default RATE_LIMITS_DEFAULT [RATE_LIMITS_DEFAULT ...]
+                        Rate limits for all API requests except /status and /stop (Default: --rate-limits-default "10/minute", "1/second")
+  --rate-limit-fast RATE_LIMIT_FAST
+                        Rate limit /status and /stop API requests (Default: "2/second")
   --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
 examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
   lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens-use "tokenForMyApp" "tokenForMyAnotherApp" "ultraPrivateTokeeeeeen" --tokens-manage "ultraPrivateTokeeeeeen"
 ```
 
 ```shell
 $ lmao --test=chatgpt
 WARNING:root:Error adding cookie oai-did
 WARNING:root:Error adding cookie ajs_anonymous_id
 WARNING:root:Error adding cookie oai-allow-ne
@@ -184,14 +198,16 @@
 
 ----------
 
 ## 🌐 API example
 
 ### Start server
 
+> Please see `🔒 HTTPS server and token-based authorization` section for more info about HTTPS server and tokens
+
 ```shell
 $ lmao --configs "configs" --ip "0.0.0.0" --port "1312" 
 2024-03-30 23:14:50 INFO     Logging setup is complete
 2024-03-30 23:14:50 INFO     Loading config files from configs directory
 2024-03-30 23:14:50 INFO     Adding config of ms_copilot module
 2024-03-30 23:14:50 INFO     Adding config of chatgpt module
  * Serving Flask app 'lmao.external_api'
@@ -285,43 +301,73 @@
 
 > Please call `/api/status` to check if the module is initialized **BEFORE** calling `/api/init`.
 >
 > After calling `/api/init`, please call `/api/status` to **check if the module's initialization finished.**
 
 **Request (POST):**
 
-```json
-{
-    "module": "name of module from MODULES"
-}
-```
+> Maximum content length: `100 bytes`. Default rate limits: `10/minute`, `1/second`
+
+- Without authorization
+
+    ```json
+    {
+        "module": "name of module from MODULES"
+    }
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    ```json
+    {
+        "module": "name of module from MODULES",
+        "token": "YourStrongRandomToken from --tokens-manage argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If everything is ok: status code `200` and `{}` body
-- ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
+- ❌ In case of other error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
 $ curl --request POST --header "Content-Type: application/json" --data '{"module": "chatgpt"}' http://localhost:1312/api/init
 {}
 ```
 
 ----------
 
 ### 🌐 Status `/api/status`
 
 Retrieves the current status of all modules
 
-**Request (GET or POST):**
+**Request (POST):**
 
-```json
-{}
-```
+> Maximum content length: `100 bytes`. Default rate limits: `1/second`
+
+- Without authorization
+
+    ```json
+    {}
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    ```json
+    {
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If no errors during modules iteration: status code `200` and
 
 ```json
 [
@@ -330,20 +376,21 @@
         "status_code": "Module's status code as an integer",
         "status_name": "Module's status as a string",
         "error": "Empty or module's error message"
     },
 ]
 ```
 
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
 - ❌ In case of an modules iteration error: status code `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
-$ curl --request GET http://localhost:1312/api/status
+$ curl --request POST --header "Content-Type: application/json" --data '{}' http://localhost:1312/api/status
 [{"error":"","module":"chatgpt","status_code":2,"status_name":"Idle"}]
 ```
 
 ----------
 
 ### 🌐 Send request and get stream response `/api/ask`
 
@@ -351,39 +398,75 @@
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/ask`
 >
 > To stop the stream, please call `/api/stop`
 
 **Request (POST):**
 
-> For **ChatGPT**:
+> Maximum content length: `100 bytes`. Default rate limits: `10/minute`, `1/second`
 
-```text
-{
-    "chatgpt": {
-        "prompt": "Text request to send to the module",
-        "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
-        "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
+- Without authorization
+
+    > For **ChatGPT**:
+
+    ```text
+    {
+        "chatgpt": {
+            "prompt": "Text request to send to the module",
+            "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
+            "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
+        }
     }
-}
-```
+    ```
 
-> For **Microsoft Copilot**:
+    > For **Microsoft Copilot**:
 
-```text
-{
-    "ms_copilot": {
-        "prompt": "Text request",
-        "image": image as base64 to include into request,
-        "conversation_id": "empty string or existing conversation ID",
-        "style": "creative" / "balanced" / "precise",
-        "convert_to_markdown": True or False
+    ```text
+    {
+        "ms_copilot": {
+            "prompt": "Text request",
+            "image": image as base64 to include into request,
+            "conversation_id": "empty string or existing conversation ID",
+            "style": "creative" / "balanced" / "precise",
+            "convert_to_markdown": True or False
+        }
     }
-}
-```
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    > For **ChatGPT**:
+
+    ```text
+    {
+        "chatgpt": {
+            "prompt": "Text request to send to the module",
+            "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
+            "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
+        },
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
+
+    > For **Microsoft Copilot**:
+
+    ```text
+    {
+        "ms_copilot": {
+            "prompt": "Text request",
+            "image": image as base64 to include into request,
+            "conversation_id": "empty string or existing conversation ID",
+            "style": "creative" / "balanced" / "precise",
+            "convert_to_markdown": True or False
+        },
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
 
 **Yields:**
 
 - ✔️ A stream of JSON objects containing module responses
 
 > For **ChatGPT**, each JSON object has the following structure:
 
@@ -412,14 +495,15 @@
     ],
     "suggestions": ["array of suggestions of the requests"]
 }
 ```
 
 **Returns:**
 
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
 - ❌ In case of error: status code `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
 $ curl --request POST --header "Content-Type: application/json" --data '{"chatgpt": {"prompt": "Hi! Who are you?", "convert_to_markdown": true}}' http://localhost:1312/api/ask
 {"finished": false, "conversation_id": "1033be5b-d37d-46b3-b47c-9548da5b192c", "message_id": "00d9cc0d-c4d9-484d-a8e5-9c78eaf2a0e1", "response": "Hello! I'm ChatGPT, an AI developed by O"}
@@ -431,23 +515,39 @@
 
 ### 🌐 Stop stream response `/api/stop`
 
 Stops the specified module's streaming response (stops yielding from `/api/ask`)
 
 **Request (POST):**
 
-```json
-{
-    "module": "Name of the module from MODULES"
-}
-```
+> Maximum content length: `100 bytes`. Default rate limits: `1/second`
+
+- Without authorization
+
+    ```json
+    {
+        "module": "Name of the module from MODULES"
+    }
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    ```json
+    {
+        "module": "Name of the module from MODULES",
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If the stream stopped successfully: status code `200` and `{}` body
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
 $ curl --request POST --header "Content-Type: application/json" --data '{"module": "chatgpt"}' http://localhost:1312/api/stop
 {}
@@ -457,29 +557,70 @@
 
 ### 🌐 Delete conversation `/api/delete`
 
 Clears the module's conversation history
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/delete`
 
-**Request:**
+**Request (POST):**
 
-For ChatGPT:
+> Maximum content length: `500 bytes`. Default rate limits: `10/minute`, `1/second`
 
-```json
-{
-    "chatgpt": {
-        "conversation_id": "ID of conversation to delete or empty to delete the top one"
+- Without authorization
+
+    > For **ChatGPT**:
+
+    ```json
+    {
+        "chatgpt": {
+            "conversation_id": "ID of conversation to delete or empty to delete the top one"
+        }
     }
-}
-```
+    ```
+
+    > For **Microsoft Copilot**:
+
+    ```json
+    {
+        "ms_copilot": {
+            "conversation_id": "ID of conversation to delete or empty to delete the top one"
+        }
+    }
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    > For **ChatGPT**:
+
+    ```json
+    {
+        "chatgpt": {
+            "conversation_id": "ID of conversation to delete or empty to delete the top one"
+        },
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
+
+    > For **Microsoft Copilot**:
+
+    ```json
+    {
+        "ms_copilot": {
+            "conversation_id": "ID of conversation to delete or empty to delete the top one"
+        },
+        "token": "YourStrongRandomToken from --tokens-use argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If conversation deleted successfully: status code `200` and `{}` body
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
 $ curl --request POST --header "Content-Type: application/json" --data '{"chatgpt": {"conversation_id": "1033be5b-d37d-46b3-b47c-9548da5b192c"}}' http://localhost:1312/api/delete
 {}
@@ -491,19 +632,92 @@
 
 Requests the module's session to close (in a separate, non-blocking thread)
 
 > Please call `/api/status` to check if the module is initialized and its status is Idle or Failed **BEFORE** calling `/api/close`
 >
 > After calling `/api/close`, please call `/api/status` to **check if the module's closing finished**
 
-**Request:**
+**Request (POST):**
+
+> Maximum content length: `500 bytes`. Default rate limits: `10/minute`, `1/second`
 
-```json
-{
-    "module": "Name of the module from MODULES"
-}
-```
+- Without authorization
+
+    ```json
+    {
+        "module": "Name of the module from MODULES"
+    }
+    ```
+
+- With authorization
+
+    > Please see `🔒 HTTPS server and token-based authorization` section for more info
+
+    ```json
+    {
+        "module": "Name of the module from MODULES",
+        "token": "YourStrongRandomToken from --tokens-manage argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If requested successfully: status code `200` and `{}` body
+- ❌ Error codes `429`, `401` or `413` in case of rate limit, wrong token or too large request
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
+
+----------
+
+## 🔒 HTTPS server and token-based authorization
+
+> ⚠️ Better use proper SSL service and redirect to local port
+>
+> ⚠️ Don't use token-based authorization with bare HTTP (without any SSL). It's not safe!
+
+It's possible to start SSL (HTTPS) server instead of HTTP. For that, provide `--ssl` argument with path to certificate file and path to private key file.
+
+Example:
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key
+2024-04-19 02:09:10 INFO     Logging setup is complete
+2024-04-19 02:09:10 INFO     Loading config files from configs directory
+2024-04-19 02:09:10 INFO     Adding config of ms_copilot module
+2024-04-19 02:09:10 INFO     Adding config of chatgpt module
+2024-04-19 02:09:10 WARNING  No tokens provided. Everyone can use API
+2024-04-19 02:09:10 INFO     Rate limits for all API requests except /status and /stop: 10/minute, 1/second
+2024-04-19 02:09:10 INFO     Rate limits /status and /stop API requests: 1/second
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-19 02:09:10 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-19 02:09:10 INFO     Press CTRL+C to quit
+...
+```
+
+Also you can enable token-based authorization. For that, provide `--tokens-use` argument with a list of some strong random tokens. Requests that provided these tokens can access `/status`, `/ask`, `/stop` and `/delete`. For `/init` and `/stop`, provide `--tokens-manage` argument with a list of some REALLY strong random tokens
+
+⚠️ Make sure you provided at least one token to `--tokens-manage` if you're using `--tokens-use`. Otherwise **EVERYONE CAN ACCESS** `/init` and `/stop`
+
+Example (tokens for `/status`, `/ask`, `/stop` and `/delete`: `naixae3eeNao6suu`, `kahMeixoo9un9OhR`. Token for `/init` and `/stop`: `ofi2ohRi8maish4x`):
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key --tokens-use naixae3eeNao6suu kahMeixoo9un9OhR --tokens-manage ofi2ohRi8maish4x
+2024-04-19 02:07:02 INFO     Logging setup is complete
+2024-04-19 02:07:02 INFO     Loading config files from configs directory
+2024-04-19 02:07:02 INFO     Adding config of ms_copilot module
+2024-04-19 02:07:02 INFO     Adding config of chatgpt module
+2024-04-19 02:07:02 INFO     Token-based authorization enabled. Provided 2 tokens-use
+2024-04-19 02:07:02 INFO     Token-based authorization enabled. Provided 1 tokens-manage
+2024-04-19 02:07:02 INFO     Rate limits for all API requests except /status and /stop: 10/minute, 1/second
+2024-04-19 02:07:02 INFO     Rate limits /status and /stop API requests: 1/second
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-19 02:07:02 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on http://127.0.0.1:1312
+ * Running on http://192.168.0.3:1312
+2024-04-19 02:07:02 INFO     Press CTRL+C to quit
+...
+```
```

### Comparing `llm-api-open-2.1.24/configs/chatgpt.json` & `llm_api_open-2.3.1/configs/chatgpt.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/configs/ms_copilot.json` & `llm_api_open-2.3.1/configs/ms_copilot.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/setup.py` & `llm_api_open-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         "console_scripts": ["lmao = lmao.main:main"],
     },
     install_requires=[
         "selenium>=4.18.1",
         "undetected-chromedriver>=3.5.5",
         "beautifulsoup4>=4.12.3",
         "markdownify>=0.11.6",
-        "Flask>=3.0.2",
+        "Flask>=3,<4",
+        "Flask-Limiter>=3,<4",
     ],
     long_description=Path.open(Path("README.md"), encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["llm-api-open"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
```

### Comparing `llm-api-open-2.1.24/src/llm_api_open.egg-info/SOURCES.txt` & `llm_api_open-2.3.1/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/_version.py` & `llm_api_open-2.3.1/src/lmao/_version.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "2.1.24"
+__version__ = "2.3.1"
```

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm_api_open-2.3.1/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/chatgpt_api.py` & `llm_api_open-2.3.1/src/lmao/chatgpt/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/conversationSearch.js` & `llm_api_open-2.3.1/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/proxy_extension.py` & `llm_api_open-2.3.1/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/external_api.py` & `llm_api_open-2.3.1/src/lmao/external_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,56 +19,145 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import atexit
+from functools import wraps
 import json
 import logging
+import ssl
 import threading
-from typing import Dict, Literal
+from typing import Dict, List, Literal
 
-from flask import Flask, request, Response, jsonify
+from flask import Flask, abort, request, Response, jsonify
+from flask_limiter import Limiter
+from flask_limiter.util import get_remote_address
 
 from lmao.module_wrapper import (
     ModuleWrapper,
     STATUS_NOT_INITIALIZED,
     MODULES,
     STATUS_IDLE,
     STATUS_FAILED,
     STATUS_TO_STR,
 )
 
 
+def limit_content_length(max_length: int):
+    """Raises 413 (Request Entity Too Large) error if request.content_length exceeded max_length
+
+    Args:
+        max_length (int): maximum content length
+    """
+
+    def decorator(f):
+        @wraps(f)
+        def wrapper(*args, **kwargs):
+            content_length = request.content_length
+            if content_length is not None and content_length > max_length:
+                abort(413)
+            return f(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+def check_auth(tokens: List or None):
+    """Raises 401 (Unauthorized) error if request provided wrong token
+
+    Args:
+       tokens (List or None): list of tokens
+    """
+
+    def decorator(f):
+        @wraps(f)
+        def wrapper(*args, **kwargs):
+            if tokens:
+                request_json = request.get_json()
+                if "token" not in request_json or request_json["token"] not in tokens:
+                    abort(401)
+            return f(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
 class ExternalAPI:
-    def __init__(self, config: Dict):
+    def __init__(
+        self,
+        config: Dict,
+        rate_limits_default: List[str] or None = None,
+        rate_limit_fast: str = "2/second",
+        tokens_use: List or None = None,
+        tokens_manage: List or None = None,
+    ):
         self.config = config
+        self.rate_limit_fast = rate_limit_fast
+        self.tokens_use = tokens_use
+        self.tokens_manage = tokens_manage
+
+        if not self.tokens_use or len(self.tokens_use) == 0:
+            self.tokens_use = None
+        if not self.tokens_manage or len(self.tokens_manage) == 0:
+            self.tokens_manage = None
+
+        if self.tokens_use and not self.tokens_manage:
+            logging.warning("NO --tokens-manage PROVIDED! ANYONE CAN USE /init AND /close")
+
+        if self.tokens_use:
+            logging.info(f"Token-based authorization enabled. Provided {len(self.tokens_use)} tokens-use")
+        if self.tokens_manage:
+            logging.info(f"Token-based authorization enabled. Provided {len(self.tokens_manage)} tokens-manage")
+        if not self.tokens_use and not self.tokens_manage:
+            logging.warning("No tokens provided. Everyone can use API")
+
+        if rate_limits_default is None:
+            rate_limits_default = ["10/minute", "1/second"]
+
+        logging.info(f"Rate limits for all API requests except /status and /stop: {', '.join(rate_limits_default)}")
+        logging.info(f"Rate limits /status and /stop API requests: {rate_limit_fast}")
 
         self.app = Flask(__name__)
+        self.limiter = Limiter(
+            get_remote_address, app=self.app, default_limits=rate_limits_default, storage_uri="memory://"
+        )
         self.lock = threading.Lock()
 
         # name of module: class object
         self.modules = {}
 
         @self.app.route("/api/init", methods=["POST"])
+        @limit_content_length(100)
+        @check_auth(self.tokens_manage)
         def init() -> tuple[Response, Literal]:
             """Begins module initialization
             Please call /api/status to check if module is initialized BEFORE calling /api/init
             And AFTER calling /api/init please call /api/status to check if module's initialization finished
 
             Request:
                 {
-                    "module": "name of module from MODULES"
+                    "module": "name of module from MODULES",
+                    "token": "optional token if --tokens-manage argument provided"
                 }
+                Maximum content length: 100 bytes
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if everything is ok
                 or
                 {"error": "Error message"}, 400 or 500 in case of error
+                or
+                429 in case of rate limit
+                or
+                401 in case of wrong token
+                or
+                413 in case of too long request
             """
             try:
                 # Extract and check module name
                 module_name = request.get_json().get("module")
                 if module_name is None:
                     return (jsonify({"error": '"module" not specified'}), 400)
                 if module_name not in MODULES:
@@ -99,39 +188,54 @@
 
                 # Initialize in thread
                 module.initialize()
 
                 return jsonify({}), 200
             except Exception as e:
                 logging.error(f"/init error: {e}")
-                return jsonify({"error": e}), 500
+                return jsonify({"error": str(e)}), 500
 
-        @self.app.route("/", methods=["GET", "POST"])
-        @self.app.route("/index", methods=["GET", "POST"])
-        @self.app.route("/index.html", methods=["GET", "POST"])
-        @self.app.route("/index.php", methods=["GET", "POST"])
-        @self.app.route("/api/status", methods=["GET", "POST"])
+        @self.app.route("/", methods=["POST"])
+        @self.app.route("/index", methods=["POST"])
+        @self.app.route("/index.html", methods=["POST"])
+        @self.app.route("/index.php", methods=["POST"])
+        @self.app.route("/api", methods=["POST"])
+        @self.app.route("/api/status", methods=["POST"])
+        @self.limiter.limit(self.rate_limit_fast)
+        @limit_content_length(100)
+        @check_auth(self.tokens_use)
         def status() -> tuple[Response, Literal]:
             """Retrieves current status of all modules
 
-            Request: empty
+            Request:
+                {
+                    "token": "optional token if --tokens-use argument provided"
+                }
+                Maximum content length: 100 bytes
 
             Returns:
                 tuple[Response, Literal]: [
                     {
                         "module": "Name of the module from MODULES",
                         "status_code": "Module's status code as integer",
                         "status_name": "Module's status as string",
                         "error": "Empty or module's error message",
                     }
                 ], 200 if no errors while iterating modules
                 or
-                {"error": "Error message"}, 500 in case of error
+                {"error": "Error message"}, 400 or 500 in case of error
+                or
+                429 in case of rate limit
+                or
+                401 in case of wrong token
+                or
+                413 in case of too long request
             """
             try:
+                # Read and add statuses
                 statuses = []
                 for module_name, module in self.modules.items():
                     try:
                         statuses.append(
                             {
                                 "module": module_name,
                                 "status_code": module.status,
@@ -140,40 +244,46 @@
                             }
                         )
                     except Exception as e:
                         logging.warning(f"Can't read {module_name} status: {e}")
                 return jsonify(statuses), 200
             except Exception as e:
                 logging.error(f"/status error: {e}")
-                return jsonify({"error": e}), 500
+                return jsonify({"error": str(e)}), 500
 
         @self.app.route("/api/ask", methods=["POST"])
+        @limit_content_length(3 * 1024 * 1024)
+        @check_auth(self.tokens_use)
         def ask():
             """Initiates a request to the specified module and streams responses back
             Please call /api/status to check if module is initialized and not busy BEFORE calling /api/ask
 
             Request:
                 For ChatGPT:
                     {
                         "chatgpt": {
                             "prompt": "Text request to send to the module",
                             "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
                             "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
-                        }
+                        },
+                        "token": "optional token if --tokens-use argument provided"
                     }
                 For Microsoft Copilot:
                     {
                         "ms_copilot": {
                             "prompt": "Text request",
                             "image": image as base64 to include into request,
                             "conversation_id": "empty string or existing conversation ID",
                             "style": "creative" / "balanced" / "precise",
-                            "convert_to_markdown": True or False
-                        }
+                            "convert_to_markdown": True or False,
+                            "token": "optional token if --tokens-use argument provided"
+                        },
+                        "token": "optional token if --tokens-use argument provided"
                     }
+                Maximum content length: 3MB
 
             Yields: A stream of JSON objects containing module responses.
             For ChatGPT, each JSON object has the following structure:
                 {
                     "finished": "True if it's the last response, False if not",
                     "message_id": "ID of the current message (from assistant)",
                     "response": "Actual response as text"
@@ -190,24 +300,33 @@
                             "url": "URL of attribution"
                         },
                         ...
                     ],
                     "suggestions": ["array of suggestions of the requests"]
                 }
 
-            Returns: {"error": "Error message"}, 500 in case of error
+            Returns:
+                {"error": "Error message"}, 400 or 500 in case of error
+                or
+                429 in case of rate limit
+                or
+                401 in case of wrong token
+                or
+                413 in case of too long request
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
                 # Check request
-                prompt = request.get_json()
-                if prompt is None or len(prompt.items()) == 0:
+                if request_json is None or len(request_json.items()) == 0:
                     return (jsonify({"error": "Empty request"}), 400)
 
                 # Extract prompt data
-                module_name, prompt_request = list(prompt.items())[0]
+                module_name, prompt_request = list(request_json.items())[0]
 
                 # Check module
                 module = self.modules.get(module_name)
                 if module is None:
                     return jsonify({"error": f"No {module_name} module defined. Please initialize one first"}), 400
                 if module.status != STATUS_IDLE:
                     return jsonify({"error": f"{module_name} status is not {STATUS_TO_STR[STATUS_IDLE]}"}), 400
@@ -219,29 +338,34 @@
                             yield json.dumps(response) + "\n"
 
                 logging.info(f"/ask request for module {module_name}")
                 return Response(_stream_response(), content_type="application/json")
 
             except Exception as e:
                 logging.error(f"/ask error: {e}")
-                return jsonify({"error": e}), 500
+                return jsonify({"error": str(e)}), 500
 
-        @self.app.route("/api/stop", methods=["GET", "POST"])
+        @self.app.route("/api/stop", methods=["POST"])
+        @self.limiter.limit(self.rate_limit_fast)
+        @limit_content_length(100)
+        @check_auth(self.tokens_use)
         def response_stop() -> tuple[Response, Literal]:
             """Stops the specified module's streaming response (stops yielding in /ask)
 
             Request:
                 {
-                    "module": "Name of the module from MODULES"
+                    "module": "Name of the module from MODULES",
+                    "token": "optional token if --tokens-use argument provided"
                 }
+                Maximum content length: 100 bytes
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if the stream stopped successfully
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
                 # Extract module name
                 module_name = request.get_json().get("module")
                 if module_name is None:
                     return jsonify({"error": '"module" not specified'}), 400
 
@@ -257,39 +381,45 @@
                 return jsonify({}), 200
 
             except Exception as e:
                 logging.error(f"/stop error: {e}")
                 return jsonify({"error": str(e)}), 500
 
         @self.app.route("/api/delete", methods=["POST"])
+        @limit_content_length(500)
+        @check_auth(self.tokens_use)
         def delete_conversation() -> tuple[Response, Literal]:
             """Clears module's conversation history
             Please call /api/status to check if module is initialized and not busy BEFORE calling /api/delete
 
             Request:
                 {
                     // For ChatGPT
                     "module": {
                         "conversation_id": "ID of conversation to delete or empty to delete the top one"
-                    }
+                    },
+                    "token": "optional token if --tokens-use argument provided"
                 }
+                Maximum content length: 500 bytes
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if conversation deleted successfully
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
                 # Check request
-                prompt = request.get_json()
-                if prompt is None or len(prompt.items()) == 0:
+                if request_json is None or len(request_json.items()) == 0:
                     return (jsonify({"error": "Empty request"}), 400)
 
                 # Extract prompt data
-                module_name, conversation_data = list(prompt.items())[0]
+                module_name, conversation_data = list(request_json.items())[0]
 
                 # Check module
                 module = self.modules.get(module_name)
                 if module is None:
                     return jsonify({"error": f"No {module_name} module defined. Please initialize one first"}), 400
                 if module.status != STATUS_IDLE:
                     return jsonify({"error": f"{module_name} status is not {STATUS_TO_STR[STATUS_IDLE]}"}), 400
@@ -301,27 +431,31 @@
                 return jsonify({}), 200
 
             except Exception as e:
                 logging.error(f"/delete error: {e}")
                 return jsonify({"error": str(e)}), 500
 
         @self.app.route("/api/close", methods=["POST"])
+        @limit_content_length(100)
+        @check_auth(self.tokens_manage)
         def close():
             """Request module's session to close (in a separate thread)
             Please call /api/status to check if module is initialized and it's status is Idle or Failed
 
             Request:
                 {
-                    "module": "Name of the module from MODULES"
+                    "module": "Name of the module from MODULES",
+                    "token": "optional token if --tokens-manage argument provided"
                 }
+                Maximum content length: 100 bytes
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if requested successfully
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
                 # Extract module name
                 module_name = request.get_json().get("module")
                 if module_name is None:
                     return jsonify({"error": '"module" not specified'}), 400
 
@@ -355,16 +489,23 @@
         for module_name, module in self.modules.items():
             logging.info(f"Trying to close {module_name}")
             try:
                 module.close(blocking=True)
             except Exception as e:
                 logging.warning(f"Cannot close {module_name}: {e}")
 
-    def run(self, host: str, port: int):
+    def run(self, host: str, port: int, certfile: str or None = None, keyfile: str or None = None):
         """Starts API server
 
         Args:
             host (str): server host (ip)
             port (int): server port
+            certfile (str or None, optional): "path/to/certificate.crt" to enable SSL. Defaults to None
+            keyfile (str or None, optional): "path/to/private.key" to enable SSL. Defaults to None
         """
         atexit.register(self._close_modules)
-        self.app.run(host=host, port=port, debug=False)
+        if certfile and keyfile:
+            context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
+            context.load_cert_chain(certfile=certfile, keyfile=keyfile)
+            self.app.run(host=host, port=port, ssl_context=context, debug=False)
+        else:
+            self.app.run(host=host, port=port, debug=False)
```

### Comparing `llm-api-open-2.1.24/src/lmao/main.py` & `llm_api_open-2.3.1/src/lmao/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -58,37 +58,51 @@
 
     # Log test message
     logging.info("Logging setup is complete")
 
 
 def parse_args() -> argparse.Namespace:
     """Parses cli arguments
-    usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+    usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens-use TOKENS_USE [TOKENS_USE ...]]
+            [--tokens-manage TOKENS_MANAGE [TOKENS_MANAGE ...]] [--rate-limits-default RATE_LIMITS_DEFAULT [RATE_LIMITS_DEFAULT ...]] [--rate-limit-fast RATE_LIMIT_FAST]
+            [--no-logging-init]
 
     Unofficial open APIs for popular LLMs with self-hosted redirect capability
 
     options:
-    -h, --help            show this help message and exit
-    -v, --version         show program's version number and exit
-    -c CONFIGS, --configs CONFIGS
-                            path to configs directory with each module config file (Default: configs)
-    -t TEST, --test TEST  module name to test in cli instead of starting API server (eg. --test=chatgpt)
-    -i IP, --ip IP        API server Host (IP) (Default: localhost)
-    -p PORT, --port PORT  API server port (Default: 1312)
-    --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
+        -h, --help            show this help message and exit
+        -v, --version         show program's version number and exit
+        -c CONFIGS, --configs CONFIGS
+                                path to configs directory with each module config file (Default: configs)
+        -t TEST, --test TEST  module name to test in cli instead of starting API server (eg. --test=chatgpt)
+        -i IP, --ip IP        API server Host (IP) (Default: localhost)
+        -p PORT, --port PORT  API server port (Default: 1312)
+        -s SSL [SSL ...], --ssl SSL [SSL ...]
+                                Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt" "path/to/private.key")
+        --tokens-use TOKENS_USE [TOKENS_USE ...]
+                                API tokens to enable authorization for /status, /ask, /stop and /delete (ex. --tokens-use "tokenForMyApp" "tokenForMyAnotherApp"
+                                "ultraPrivateTokeeeeeen")
+        --tokens-manage TOKENS_MANAGE [TOKENS_MANAGE ...]
+                                API tokens to enable authorization for /init and /close (ex. --tokens-manage "ultraPrivateTokeeeeeen")
+        --rate-limits-default RATE_LIMITS_DEFAULT [RATE_LIMITS_DEFAULT ...]
+                                Rate limits for all API requests except /status and /stop (Default: --rate-limits-default "10/minute", "1/second")
+        --rate-limit-fast RATE_LIMIT_FAST
+                                Rate limit /status and /stop API requests (Default: "2/second")
+        --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
     Returns:
         argparse.Namespace: parsed arguments
     """
 
     # Example usage
     epilog = """examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
-  lmao --ip="0.0.0.0" --port=1312 --no-logging-init"""
+  lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens-use \"tokenForMyApp\" \"tokenForMyAnotherApp\" \"ultraPrivateTokeeeeeen\" --tokens-manage \"ultraPrivateTokeeeeeen\""""
 
     parser = argparse.ArgumentParser(
         prog="lmao",
         description="Unofficial open APIs for popular LLMs with self-hosted redirect capability",
         epilog=epilog,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
@@ -122,14 +136,50 @@
         "--port",
         type=int,
         default=int(os.getenv("PORT", str(_PORT_DEFAULT))),
         required=False,
         help=f"API server port (Default: {int(os.getenv('PORT', str(_PORT_DEFAULT)))})",
     )
     parser.add_argument(
+        "-s",
+        "--ssl",
+        nargs="+",
+        default=[],
+        required=False,
+        help='Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt" "path/to/private.key")',
+    )
+    parser.add_argument(
+        "--tokens-use",
+        nargs="+",
+        default=[],
+        required=False,
+        help='API tokens to enable authorization for /status, /ask, /stop and /delete (ex. --tokens-use "tokenForMyApp" "tokenForMyAnotherApp" "ultraPrivateTokeeeeeen")',
+    )
+    parser.add_argument(
+        "--tokens-manage",
+        nargs="+",
+        default=[],
+        required=False,
+        help='API tokens to enable authorization for /init and /close (ex. --tokens-manage "ultraPrivateTokeeeeeen")',
+    )
+    parser.add_argument(
+        "--rate-limits-default",
+        nargs="+",
+        default=["10/minute", "1/second"],
+        required=False,
+        help='Rate limits for all API requests except /status and /stop (Default: --rate-limits-default "10/minute", "1/second")',
+    )
+    parser.add_argument(
+        "--rate-limit-fast",
+        type=str,
+        default="2/second",
+        required=False,
+        help='Rate limit /status and /stop API requests (Default: "2/second")',
+    )
+    parser.add_argument(
         "--no-logging-init",
         action="store_true",
         required=False,
         help="specify to bypass logging initialization (will be set automatically when using --test)",
     )
 
     return parser.parse_args()
@@ -234,13 +284,26 @@
                 raise Exception(str(module.error))
         except Exception as e:
             logging.error(f"Error closing {args.test}", exc_info=e)
             return
 
     # Start API server if no --test mode specified
     else:
-        api = ExternalAPI(config)
-        api.run(args.ip, args.port)
+        if args.ssl and len(args.ssl) < 2:
+            logging.error("Please provide paths to both .crt and .key files")
+            return
+
+        api = ExternalAPI(
+            config,
+            rate_limits_default=args.rate_limits_default,
+            rate_limit_fast=args.rate_limit_fast,
+            tokens_use=args.tokens_use,
+            tokens_manage=args.tokens_manage,
+        )
+        if args.ssl and len(args.ssl) == 2:
+            api.run(args.ip, args.port, certfile=args.ssl[0], keyfile=args.ssl[1])
+        else:
+            api.run(args.ip, args.port)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm-api-open-2.1.24/src/lmao/module_wrapper.py` & `llm_api_open-2.3.1/src/lmao/module_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationManage.js` & `llm_api_open-2.3.1/src/lmao/ms_copilot/conversationManage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationParser.js` & `llm_api_open-2.3.1/src/lmao/ms_copilot/conversationParser.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/ms_copilot_api.py` & `llm_api_open-2.3.1/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/proxy_extension.py` & `llm_api_open-2.3.1/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*


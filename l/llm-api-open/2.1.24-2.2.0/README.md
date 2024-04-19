# Comparing `tmp/llm-api-open-2.1.24.tar.gz` & `tmp/llm_api_open-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-api-open-2.1.24.tar", last modified: Tue Apr  9 22:01:48 2024, max compression
+gzip compressed data, was "llm_api_open-2.2.0.tar", last modified: Fri Apr 19 01:00:37 2024, max compression
```

## Comparing `llm-api-open-2.1.24.tar` & `llm_api_open-2.2.0.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21650 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.009590 llm_api_open-2.2.0/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.009590 llm_api_open-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21650 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 01:00:37.000000 llm_api_open-2.2.0/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.009590 llm_api_open-2.2.0/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9730 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:37.013591 llm_api_open-2.2.0/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43383 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 01:00:33.000000 llm_api_open-2.2.0/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm-api-open-2.1.24/LICENSE` & `llm_api_open-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/PKG-INFO` & `llm_api_open-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.24
+Version: 2.2.0
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -184,34 +184,41 @@
 module.close(blocking=True)
 ```
 
 ----------
 
 ## 💻 CLI example
 
-```shell
+```text
 $ lmao --help        
-usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens TOKENS [TOKENS ...]]
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
+                        Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt"
+                        "path/to/private.key")
+  --tokens TOKENS [TOKENS ...]
+                        API tokens to enable authorization (ex. --tokens "abcdefg12345" "AAAAATESTtest")
   --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
 examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
   lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens myStrongRandomToken myStrongRandomToken2
 ```
 
 ```shell
 $ lmao --test=chatgpt
 WARNING:root:Error adding cookie oai-did
 WARNING:root:Error adding cookie ajs_anonymous_id
 WARNING:root:Error adding cookie oai-allow-ne
@@ -221,14 +228,16 @@
 
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
@@ -322,19 +331,32 @@
 
 > Please call `/api/status` to check if the module is initialized **BEFORE** calling `/api/init`.
 >
 > After calling `/api/init`, please call `/api/status` to **check if the module's initialization finished.**
 
 **Request (POST):**
 
-```json
-{
-    "module": "name of module from MODULES"
-}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If everything is ok: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -346,19 +368,31 @@
 
 ----------
 
 ### 🌐 Status `/api/status`
 
 Retrieves the current status of all modules
 
-**Request (GET or POST):**
+**Request (POST):**
 
-```json
-{}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If no errors during modules iteration: status code `200` and
 
 ```json
 [
@@ -372,15 +406,15 @@
 ```
 
 - ❌ In case of an modules iteration error: status code `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
-$ curl --request GET http://localhost:1312/api/status
+$ curl --request POST --header "Content-Type: application/json" --data '{}' http://localhost:1312/api/status
 [{"error":"","module":"chatgpt","status_code":2,"status_name":"Idle"}]
 ```
 
 ----------
 
 ### 🌐 Send request and get stream response `/api/ask`
 
@@ -388,39 +422,73 @@
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/ask`
 >
 > To stop the stream, please call `/api/stop`
 
 **Request (POST):**
 
-> For **ChatGPT**:
+- Without authorization
 
-```text
-{
-    "chatgpt": {
-        "prompt": "Text request to send to the module",
-        "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
-        "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Yields:**
 
 - ✔️ A stream of JSON objects containing module responses
 
 > For **ChatGPT**, each JSON object has the following structure:
 
@@ -468,19 +536,32 @@
 
 ### 🌐 Stop stream response `/api/stop`
 
 Stops the specified module's streaming response (stops yielding from `/api/ask`)
 
 **Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If the stream stopped successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -494,25 +575,63 @@
 
 ### 🌐 Delete conversation `/api/delete`
 
 Clears the module's conversation history
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/delete`
 
-**Request:**
+**Request (POST):**
 
-For ChatGPT:
+- Without authorization
 
-```json
-{
-    "chatgpt": {
-        "conversation_id": "ID of conversation to delete or empty to delete the top one"
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If conversation deleted successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -528,19 +647,76 @@
 
 Requests the module's session to close (in a separate, non-blocking thread)
 
 > Please call `/api/status` to check if the module is initialized and its status is Idle or Failed **BEFORE** calling `/api/close`
 >
 > After calling `/api/close`, please call `/api/status` to **check if the module's closing finished**
 
-**Request:**
+**Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If requested successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
+
+----------
+
+## 🔒 HTTPS server and token-based authorization
+
+It's possible to start SSL (HTTPS) server instead of HTTP. For that, provide `--ssl` argument with path to certificate file and path to private key file.
+
+Example:
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key
+2024-04-18 19:41:59 INFO     Logging setup is complete
+2024-04-18 19:41:59 INFO     Loading config files from configs directory
+2024-04-18 19:41:59 INFO     Adding config of ms_copilot module
+2024-04-18 19:41:59 INFO     Adding config of chatgpt module
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:41:59 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:41:59 INFO     Press CTRL+C to quit
+...
+```
+
+Also you can enable token-based authorization. For that, provide `--tokens` argument with a list of some strong random tokens.
+
+Example (tokens are `naixae3eeNao6suu`, `kahMeixoo9un9OhR` and `ofi2ohRi8maish4x`):
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key --tokens naixae3eeNao6suu kahMeixoo9un9OhR ofi2ohRi8maish4x
+2024-04-18 19:45:16 INFO     Logging setup is complete
+2024-04-18 19:45:16 INFO     Loading config files from configs directory
+2024-04-18 19:45:16 INFO     Adding config of ms_copilot module
+2024-04-18 19:45:16 INFO     Adding config of chatgpt module
+2024-04-18 19:45:16 INFO     Token-based authorization enabled
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:45:16 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:45:16 INFO     Press CTRL+C to quit
+```
```

### Comparing `llm-api-open-2.1.24/README.md` & `llm_api_open-2.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -147,34 +147,41 @@
 module.close(blocking=True)
 ```
 
 ----------
 
 ## 💻 CLI example
 
-```shell
+```text
 $ lmao --help        
-usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens TOKENS [TOKENS ...]]
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
+                        Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt"
+                        "path/to/private.key")
+  --tokens TOKENS [TOKENS ...]
+                        API tokens to enable authorization (ex. --tokens "abcdefg12345" "AAAAATESTtest")
   --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
 examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
   lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens myStrongRandomToken myStrongRandomToken2
 ```
 
 ```shell
 $ lmao --test=chatgpt
 WARNING:root:Error adding cookie oai-did
 WARNING:root:Error adding cookie ajs_anonymous_id
 WARNING:root:Error adding cookie oai-allow-ne
@@ -184,14 +191,16 @@
 
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
@@ -285,19 +294,32 @@
 
 > Please call `/api/status` to check if the module is initialized **BEFORE** calling `/api/init`.
 >
 > After calling `/api/init`, please call `/api/status` to **check if the module's initialization finished.**
 
 **Request (POST):**
 
-```json
-{
-    "module": "name of module from MODULES"
-}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If everything is ok: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -309,19 +331,31 @@
 
 ----------
 
 ### 🌐 Status `/api/status`
 
 Retrieves the current status of all modules
 
-**Request (GET or POST):**
+**Request (POST):**
 
-```json
-{}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If no errors during modules iteration: status code `200` and
 
 ```json
 [
@@ -335,15 +369,15 @@
 ```
 
 - ❌ In case of an modules iteration error: status code `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
-$ curl --request GET http://localhost:1312/api/status
+$ curl --request POST --header "Content-Type: application/json" --data '{}' http://localhost:1312/api/status
 [{"error":"","module":"chatgpt","status_code":2,"status_name":"Idle"}]
 ```
 
 ----------
 
 ### 🌐 Send request and get stream response `/api/ask`
 
@@ -351,39 +385,73 @@
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/ask`
 >
 > To stop the stream, please call `/api/stop`
 
 **Request (POST):**
 
-> For **ChatGPT**:
+- Without authorization
 
-```text
-{
-    "chatgpt": {
-        "prompt": "Text request to send to the module",
-        "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
-        "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Yields:**
 
 - ✔️ A stream of JSON objects containing module responses
 
 > For **ChatGPT**, each JSON object has the following structure:
 
@@ -431,19 +499,32 @@
 
 ### 🌐 Stop stream response `/api/stop`
 
 Stops the specified module's streaming response (stops yielding from `/api/ask`)
 
 **Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If the stream stopped successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -457,25 +538,63 @@
 
 ### 🌐 Delete conversation `/api/delete`
 
 Clears the module's conversation history
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/delete`
 
-**Request:**
+**Request (POST):**
 
-For ChatGPT:
+- Without authorization
 
-```json
-{
-    "chatgpt": {
-        "conversation_id": "ID of conversation to delete or empty to delete the top one"
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If conversation deleted successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -491,19 +610,76 @@
 
 Requests the module's session to close (in a separate, non-blocking thread)
 
 > Please call `/api/status` to check if the module is initialized and its status is Idle or Failed **BEFORE** calling `/api/close`
 >
 > After calling `/api/close`, please call `/api/status` to **check if the module's closing finished**
 
-**Request:**
+**Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If requested successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
+
+----------
+
+## 🔒 HTTPS server and token-based authorization
+
+It's possible to start SSL (HTTPS) server instead of HTTP. For that, provide `--ssl` argument with path to certificate file and path to private key file.
+
+Example:
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key
+2024-04-18 19:41:59 INFO     Logging setup is complete
+2024-04-18 19:41:59 INFO     Loading config files from configs directory
+2024-04-18 19:41:59 INFO     Adding config of ms_copilot module
+2024-04-18 19:41:59 INFO     Adding config of chatgpt module
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:41:59 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:41:59 INFO     Press CTRL+C to quit
+...
+```
+
+Also you can enable token-based authorization. For that, provide `--tokens` argument with a list of some strong random tokens.
+
+Example (tokens are `naixae3eeNao6suu`, `kahMeixoo9un9OhR` and `ofi2ohRi8maish4x`):
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key --tokens naixae3eeNao6suu kahMeixoo9un9OhR ofi2ohRi8maish4x
+2024-04-18 19:45:16 INFO     Logging setup is complete
+2024-04-18 19:45:16 INFO     Loading config files from configs directory
+2024-04-18 19:45:16 INFO     Adding config of ms_copilot module
+2024-04-18 19:45:16 INFO     Adding config of chatgpt module
+2024-04-18 19:45:16 INFO     Token-based authorization enabled
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:45:16 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:45:16 INFO     Press CTRL+C to quit
+```
```

### Comparing `llm-api-open-2.1.24/configs/chatgpt.json` & `llm_api_open-2.2.0/configs/chatgpt.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/configs/ms_copilot.json` & `llm_api_open-2.2.0/configs/ms_copilot.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/setup.py` & `llm_api_open-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/llm_api_open.egg-info/PKG-INFO` & `llm_api_open-2.2.0/src/llm_api_open.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.24
+Version: 2.2.0
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -184,34 +184,41 @@
 module.close(blocking=True)
 ```
 
 ----------
 
 ## 💻 CLI example
 
-```shell
+```text
 $ lmao --help        
-usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens TOKENS [TOKENS ...]]
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
+                        Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt"
+                        "path/to/private.key")
+  --tokens TOKENS [TOKENS ...]
+                        API tokens to enable authorization (ex. --tokens "abcdefg12345" "AAAAATESTtest")
   --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
 examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
   lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens myStrongRandomToken myStrongRandomToken2
 ```
 
 ```shell
 $ lmao --test=chatgpt
 WARNING:root:Error adding cookie oai-did
 WARNING:root:Error adding cookie ajs_anonymous_id
 WARNING:root:Error adding cookie oai-allow-ne
@@ -221,14 +228,16 @@
 
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
@@ -322,19 +331,32 @@
 
 > Please call `/api/status` to check if the module is initialized **BEFORE** calling `/api/init`.
 >
 > After calling `/api/init`, please call `/api/status` to **check if the module's initialization finished.**
 
 **Request (POST):**
 
-```json
-{
-    "module": "name of module from MODULES"
-}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If everything is ok: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -346,19 +368,31 @@
 
 ----------
 
 ### 🌐 Status `/api/status`
 
 Retrieves the current status of all modules
 
-**Request (GET or POST):**
+**Request (POST):**
 
-```json
-{}
-```
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If no errors during modules iteration: status code `200` and
 
 ```json
 [
@@ -372,15 +406,15 @@
 ```
 
 - ❌ In case of an modules iteration error: status code `500` and `{"error": "Error message"}` body
 
 **Example:**
 
 ```shell
-$ curl --request GET http://localhost:1312/api/status
+$ curl --request POST --header "Content-Type: application/json" --data '{}' http://localhost:1312/api/status
 [{"error":"","module":"chatgpt","status_code":2,"status_name":"Idle"}]
 ```
 
 ----------
 
 ### 🌐 Send request and get stream response `/api/ask`
 
@@ -388,39 +422,73 @@
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/ask`
 >
 > To stop the stream, please call `/api/stop`
 
 **Request (POST):**
 
-> For **ChatGPT**:
+- Without authorization
 
-```text
-{
-    "chatgpt": {
-        "prompt": "Text request to send to the module",
-        "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
-        "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Yields:**
 
 - ✔️ A stream of JSON objects containing module responses
 
 > For **ChatGPT**, each JSON object has the following structure:
 
@@ -468,19 +536,32 @@
 
 ### 🌐 Stop stream response `/api/stop`
 
 Stops the specified module's streaming response (stops yielding from `/api/ask`)
 
 **Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If the stream stopped successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -494,25 +575,63 @@
 
 ### 🌐 Delete conversation `/api/delete`
 
 Clears the module's conversation history
 
 > Please call `/api/status` to check if the module is initialized and not busy **BEFORE** calling `/api/delete`
 
-**Request:**
+**Request (POST):**
 
-For ChatGPT:
+- Without authorization
 
-```json
-{
-    "chatgpt": {
-        "conversation_id": "ID of conversation to delete or empty to delete the top one"
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
+        "token": "YourStrongRandomToken from --tokens argument"
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If conversation deleted successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
 
 **Example:**
@@ -528,19 +647,76 @@
 
 Requests the module's session to close (in a separate, non-blocking thread)
 
 > Please call `/api/status` to check if the module is initialized and its status is Idle or Failed **BEFORE** calling `/api/close`
 >
 > After calling `/api/close`, please call `/api/status` to **check if the module's closing finished**
 
-**Request:**
+**Request (POST):**
 
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
+        "token": "YourStrongRandomToken from --tokens argument"
+    }
+    ```
 
 **Returns:**
 
 - ✔️ If requested successfully: status code `200` and `{}` body
 - ❌ In case of an error: status code `400` or `500` and `{"error": "Error message"}` body
+
+----------
+
+## 🔒 HTTPS server and token-based authorization
+
+It's possible to start SSL (HTTPS) server instead of HTTP. For that, provide `--ssl` argument with path to certificate file and path to private key file.
+
+Example:
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key
+2024-04-18 19:41:59 INFO     Logging setup is complete
+2024-04-18 19:41:59 INFO     Loading config files from configs directory
+2024-04-18 19:41:59 INFO     Adding config of ms_copilot module
+2024-04-18 19:41:59 INFO     Adding config of chatgpt module
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:41:59 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:41:59 INFO     Press CTRL+C to quit
+...
+```
+
+Also you can enable token-based authorization. For that, provide `--tokens` argument with a list of some strong random tokens.
+
+Example (tokens are `naixae3eeNao6suu`, `kahMeixoo9un9OhR` and `ofi2ohRi8maish4x`):
+
+```shell
+$ lmao --configs "configs" --ip "0.0.0.0" --port "1312" --ssl certificate.crt private.key --tokens naixae3eeNao6suu kahMeixoo9un9OhR ofi2ohRi8maish4x
+2024-04-18 19:45:16 INFO     Logging setup is complete
+2024-04-18 19:45:16 INFO     Loading config files from configs directory
+2024-04-18 19:45:16 INFO     Adding config of ms_copilot module
+2024-04-18 19:45:16 INFO     Adding config of chatgpt module
+2024-04-18 19:45:16 INFO     Token-based authorization enabled
+ * Serving Flask app 'lmao.external_api'
+ * Debug mode: off
+2024-04-18 19:45:16 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
+ * Running on all addresses (0.0.0.0)
+ * Running on https://127.0.0.1:1312
+ * Running on https://192.168.0.3:1312
+2024-04-18 19:45:16 INFO     Press CTRL+C to quit
+```
```

### Comparing `llm-api-open-2.1.24/src/llm_api_open.egg-info/SOURCES.txt` & `llm_api_open-2.2.0/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/_version.py` & `llm_api_open-2.2.0/src/lmao/_version.py`

 * *Files 1% similar despite different names*

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
+__version__ = "2.2.0"
```

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm_api_open-2.2.0/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/chatgpt_api.py` & `llm_api_open-2.2.0/src/lmao/chatgpt/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/conversationSearch.js` & `llm_api_open-2.2.0/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/chatgpt/proxy_extension.py` & `llm_api_open-2.2.0/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/external_api.py` & `llm_api_open-2.2.0/src/lmao/external_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,31 +22,40 @@
 SOFTWARE.
 """
 
 import atexit
 import json
 import logging
 import threading
-from typing import Dict, Literal
+from typing import Dict, List, Literal, Tuple
 
 from flask import Flask, request, Response, jsonify
 
 from lmao.module_wrapper import (
     ModuleWrapper,
     STATUS_NOT_INITIALIZED,
     MODULES,
     STATUS_IDLE,
     STATUS_FAILED,
     STATUS_TO_STR,
 )
 
+# 401 error
+NOT_AUTHORIZED_ERROR_TEXT = "Not authorized"
+
 
 class ExternalAPI:
-    def __init__(self, config: Dict):
+    def __init__(self, config: Dict, tokens: List or None = None):
         self.config = config
+        self.tokens = tokens
+
+        if not self.tokens or len(self.tokens) == 0:
+            self.tokens = None
+        if self.tokens:
+            logging.info("Token-based authorization enabled")
 
         self.app = Flask(__name__)
         self.lock = threading.Lock()
 
         # name of module: class object
         self.modules = {}
 
@@ -54,25 +63,34 @@
         def init() -> tuple[Response, Literal]:
             """Begins module initialization
             Please call /api/status to check if module is initialized BEFORE calling /api/init
             And AFTER calling /api/init please call /api/status to check if module's initialization finished
 
             Request:
                 {
-                    "module": "name of module from MODULES"
+                    "module": "name of module from MODULES",
+                    "token": "optional token if --tokens argument provided"
                 }
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if everything is ok
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
+                # Check token
+                if self.tokens:
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
+
                 # Extract and check module name
-                module_name = request.get_json().get("module")
+                module_name = request_json.get("module")
                 if module_name is None:
                     return (jsonify({"error": '"module" not specified'}), 400)
                 if module_name not in MODULES:
                     return (jsonify({"error": f"No module named {module_name}"}), 400)
 
                 logging.info(f"/init request for module {module_name}")
 
@@ -101,37 +119,47 @@
                 module.initialize()
 
                 return jsonify({}), 200
             except Exception as e:
                 logging.error(f"/init error: {e}")
                 return jsonify({"error": e}), 500
 
-        @self.app.route("/", methods=["GET", "POST"])
-        @self.app.route("/index", methods=["GET", "POST"])
-        @self.app.route("/index.html", methods=["GET", "POST"])
-        @self.app.route("/index.php", methods=["GET", "POST"])
-        @self.app.route("/api/status", methods=["GET", "POST"])
+        @self.app.route("/", methods=["POST"])
+        @self.app.route("/index", methods=["POST"])
+        @self.app.route("/index.html", methods=["POST"])
+        @self.app.route("/index.php", methods=["POST"])
+        @self.app.route("/api/status", methods=["POST"])
         def status() -> tuple[Response, Literal]:
             """Retrieves current status of all modules
 
-            Request: empty
+            Request:
+                {
+                    "token": "optional token if --tokens argument provided"
+                }
 
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
+                {"error": "Error message"}, 401 or 500 in case of error
             """
             try:
+                # Check token
+                if self.tokens:
+                    request_json = request.get_json()
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
+
+                # Read and add statuses
                 statuses = []
                 for module_name, module in self.modules.items():
                     try:
                         statuses.append(
                             {
                                 "module": module_name,
                                 "status_code": module.status,
@@ -154,25 +182,28 @@
             Request:
                 For ChatGPT:
                     {
                         "chatgpt": {
                             "prompt": "Text request to send to the module",
                             "conversation_id": "Optional conversation ID (to continue existing chat) or empty for a new conversation",
                             "convert_to_markdown": true or false //(Optional flag for converting response to Markdown)
-                        }
+                        },
+                        "token": "optional token if --tokens argument provided"
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
+                            "token": "optional token if --tokens argument provided"
+                        },
+                        "token": "optional token if --tokens argument provided"
                     }
 
             Yields: A stream of JSON objects containing module responses.
             For ChatGPT, each JSON object has the following structure:
                 {
                     "finished": "True if it's the last response, False if not",
                     "message_id": "ID of the current message (from assistant)",
@@ -190,24 +221,31 @@
                             "url": "URL of attribution"
                         },
                         ...
                     ],
                     "suggestions": ["array of suggestions of the requests"]
                 }
 
-            Returns: {"error": "Error message"}, 500 in case of error
+            Returns: {"error": "Error message"}, 401 or 500 in case of error
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
+                # Check token
+                if self.tokens:
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
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
@@ -221,31 +259,40 @@
                 logging.info(f"/ask request for module {module_name}")
                 return Response(_stream_response(), content_type="application/json")
 
             except Exception as e:
                 logging.error(f"/ask error: {e}")
                 return jsonify({"error": e}), 500
 
-        @self.app.route("/api/stop", methods=["GET", "POST"])
+        @self.app.route("/api/stop", methods=["POST"])
         def response_stop() -> tuple[Response, Literal]:
             """Stops the specified module's streaming response (stops yielding in /ask)
 
             Request:
                 {
-                    "module": "Name of the module from MODULES"
+                    "module": "Name of the module from MODULES",
+                    "token": "optional token if --tokens argument provided"
                 }
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if the stream stopped successfully
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
+                # Check token
+                if self.tokens:
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
+
                 # Extract module name
-                module_name = request.get_json().get("module")
+                module_name = request_json.get("module")
                 if module_name is None:
                     return jsonify({"error": '"module" not specified'}), 400
 
                 # Check if module exists
                 module = self.modules.get(module_name)
                 if module is None:
                     return jsonify({"error": f"No {module_name} module defined. Please initialize one first"}), 400
@@ -266,30 +313,38 @@
             Please call /api/status to check if module is initialized and not busy BEFORE calling /api/delete
 
             Request:
                 {
                     // For ChatGPT
                     "module": {
                         "conversation_id": "ID of conversation to delete or empty to delete the top one"
-                    }
+                    },
+                    "token": "optional token if --tokens argument provided"
                 }
 
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
+                # Check token
+                if self.tokens:
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
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
@@ -307,25 +362,34 @@
         @self.app.route("/api/close", methods=["POST"])
         def close():
             """Request module's session to close (in a separate thread)
             Please call /api/status to check if module is initialized and it's status is Idle or Failed
 
             Request:
                 {
-                    "module": "Name of the module from MODULES"
+                    "module": "Name of the module from MODULES",
+                    "token": "optional token if --tokens argument provided"
                 }
 
             Returns:
                 tuple[Response, Literal]: {}, 200 if requested successfully
                 or
-                {"error": "Error message"}, 400 or 500 in case of error
+                {"error": "Error message"}, 400 / 401 or 500 in case of error
             """
             try:
+                # Parse request as JSON
+                request_json = request.get_json()
+
+                # Check token
+                if self.tokens:
+                    if "token" not in request_json or request_json["token"] not in self.tokens:
+                        return (jsonify({"error": NOT_AUTHORIZED_ERROR_TEXT}), 401)
+
                 # Extract module name
-                module_name = request.get_json().get("module")
+                module_name = request_json.get("module")
                 if module_name is None:
                     return jsonify({"error": '"module" not specified'}), 400
 
                 # Check if module exists
                 module = self.modules.get(module_name)
                 if module is None:
                     return jsonify({"error": f"No {module_name} module defined. Please initialize one first"}), 400
@@ -355,16 +419,23 @@
         for module_name, module in self.modules.items():
             logging.info(f"Trying to close {module_name}")
             try:
                 module.close(blocking=True)
             except Exception as e:
                 logging.warning(f"Cannot close {module_name}: {e}")
 
-    def run(self, host: str, port: int):
+    def run(self, host: str, port: int, ssl_context: Tuple[str, str] or None = None):
         """Starts API server
 
         Args:
             host (str): server host (ip)
             port (int): server port
+            ssl_context (Tuple[str, str] or None, optional): ("path/to/certificate.crt", "path/to/private.key")
+            Specify ssl_context to enable HTTPS server instead of HTTP
         """
         atexit.register(self._close_modules)
-        self.app.run(host=host, port=port, debug=False)
+        if ssl_context and len(ssl_context) == 0:
+            ssl_context = None
+        if ssl_context:
+            self.app.run(host=host, port=port, ssl_context=ssl_context, debug=False)
+        else:
+            self.app.run(host=host, port=port, debug=False)
```

### Comparing `llm-api-open-2.1.24/src/lmao/main.py` & `llm_api_open-2.2.0/src/lmao/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,37 +58,44 @@
 
     # Log test message
     logging.info("Logging setup is complete")
 
 
 def parse_args() -> argparse.Namespace:
     """Parses cli arguments
-    usage: lmao [-h] [-v] [-c CONFIG] [-t TEST] [-i IP] [-p PORT] [--no-logging-init]
+    usage: lmao [-h] [-v] [-c CONFIGS] [-t TEST] [-i IP] [-p PORT] [-s SSL [SSL ...]] [--tokens TOKENS [TOKENS ...]]
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
+    -s SSL [SSL ...], --ssl SSL [SSL ...]
+                            Paths to SSL certificate and private key (ex. --ssl "path/to/certificate.crt"
+                            "path/to/private.key")
+    --tokens TOKENS [TOKENS ...]
+                            API tokens to enable authorization (ex. --tokens "abcdefg12345" "AAAAATESTtest")
     --no-logging-init     specify to bypass logging initialization (will be set automatically when using --test)
 
     Returns:
         argparse.Namespace: parsed arguments
     """
 
     # Example usage
     epilog = """examples:
   lmao --test=chatgpt
   lmao --ip="0.0.0.0" --port=1312
-  lmao --ip="0.0.0.0" --port=1312 --no-logging-init"""
+  lmao --ip="0.0.0.0" --port=1312 --no-logging-init
+  lmao --ip "0.0.0.0" --port=1312 --ssl certificate.crt private.key --tokens myStrongRandomToken myStrongRandomToken2"""
 
     parser = argparse.ArgumentParser(
         prog="lmao",
         description="Unofficial open APIs for popular LLMs with self-hosted redirect capability",
         epilog=epilog,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
@@ -122,14 +129,29 @@
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
+        "--tokens",
+        nargs="+",
+        default=[],
+        required=False,
+        help='API tokens to enable authorization (ex. --tokens "abcdefg12345" "AAAAATESTtest")',
+    )
+    parser.add_argument(
         "--no-logging-init",
         action="store_true",
         required=False,
         help="specify to bypass logging initialization (will be set automatically when using --test)",
     )
 
     return parser.parse_args()
@@ -234,13 +256,13 @@
                 raise Exception(str(module.error))
         except Exception as e:
             logging.error(f"Error closing {args.test}", exc_info=e)
             return
 
     # Start API server if no --test mode specified
     else:
-        api = ExternalAPI(config)
-        api.run(args.ip, args.port)
+        api = ExternalAPI(config, tokens=args.tokens)
+        api.run(args.ip, args.port, ssl_context=tuple(args.ssl))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm-api-open-2.1.24/src/lmao/module_wrapper.py` & `llm_api_open-2.2.0/src/lmao/module_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationManage.js` & `llm_api_open-2.2.0/src/lmao/ms_copilot/conversationManage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationParser.js` & `llm_api_open-2.2.0/src/lmao/ms_copilot/conversationParser.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/ms_copilot_api.py` & `llm_api_open-2.2.0/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.24/src/lmao/ms_copilot/proxy_extension.py` & `llm_api_open-2.2.0/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*


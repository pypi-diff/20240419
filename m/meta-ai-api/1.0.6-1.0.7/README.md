# Comparing `tmp/meta_ai_api-1.0.6.tar.gz` & `tmp/meta_ai_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.6.tar", last modified: Thu Apr 18 22:58:04 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.7.tar", last modified: Fri Apr 19 00:09:23 2024, max compression
```

## Comparing `meta_ai_api-1.0.6.tar` & `meta_ai_api-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.775576 meta_ai_api-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.775576 meta_ai_api-1.0.6/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.525811 meta_ai_api-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.525811 meta_ai_api-1.0.7/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.6/PKG-INFO` & `meta_ai_api-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
```

### Comparing `meta_ai_api-1.0.6/README.md` & `meta_ai_api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.6/setup.py` & `meta_ai_api-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.6/src/meta_ai_api/main.py` & `meta_ai_api-1.0.7/src/meta_ai_api/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import json
+import random
+import time
 import urllib
+import uuid
 
 import requests
 from requests_html import HTMLSession
 
 
 class MetaAI:
     """
     A class to interact with the Meta AI API to obtain and use access tokens for sending
     and receiving messages from the Meta AI Chat API.
     """
 
     def __init__(self):
         self.session = requests.Session()
         self.access_token = None
+        self.cookies = None
 
     def get_access_token(self) -> str:
         """
         Retrieves an access token using Meta's authentication API.
 
         Returns:
             str: A valid access token.
         """
-        cookies = self.get_cookies()
+        self.cookies = self.get_cookies()
         url = "https://www.meta.ai/api/graphql/"
 
         payload = {
             "av": "0",
             "__user": "0",
             "__a": "1",
             "__req": "4",
@@ -42,15 +46,15 @@
             },
             "server_timestamps": "true",
             "doc_id": "7604648749596940",
         }
         payload = urllib.parse.urlencode(payload)
         headers = {
             "content-type": "application/x-www-form-urlencoded",
-            "cookie": f'_js_datr={cookies["_js_datr"]}; abra_csrf={cookies["abra_csrf"]};',
+            "cookie": f'_js_datr={self.cookies["_js_datr"]}; abra_csrf={self.cookies["abra_csrf"]};',
             "dpr": "2",
             "sec-fetch-site": "same-origin",
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             "x-fb-friendly-name": "useAbraAcceptTOSForTempUserMutation",
             "x-fb-lsd": "AVrWIDJrQQI",
         }
 
@@ -76,34 +80,22 @@
             Exception: If unable to obtain a valid response after several attempts.
         """
         if not self.access_token:
             self.access_token = self.get_access_token()
 
         url = "https://graph.meta.ai/graphql?locale=user"
         payload = {
-            "av": "0",
             "access_token": self.access_token,
-            "__user": "0",
-            "__a": "1",
-            "__req": "p",
-            "__hs": "19831.HYP:abra_pkg.2.1..0.0",
-            "dpr": "1",
-            "__ccg": "UNKNOWN",
-            "__s": ":0ryskm:ewvpqb",
-            "__comet_req": "46",
-            "lsd": "AVrLt4uZ-4k",
-            "__spin_b": "trunk",
-            "__jssesw": "1",
             "fb_api_caller_class": "RelayModern",
             "fb_api_req_friendly_name": "useAbraSendMessageMutation",
             "variables": json.dumps(
                 {
                     "message": {"sensitive_string_value": message},
-                    "externalConversationId": "dae20bda-6450-4ce7-880c-1db1b3ae7da3",
-                    "offlineThreadingId": "7186784311738402039",
+                    "externalConversationId": str(uuid.uuid4()),
+                    "offlineThreadingId": self.generate_offline_threading_id(),
                     "suggestedPromptIndex": None,
                     "flashVideoRecapInput": {"images": []},
                     "flashPreviewInput": None,
                     "promptPrefix": None,
                     "entrypoint": "ABRA__CHAT__TEXT",
                     "icebreaker_type": "TEXT",
                     "__relay_internal__pv__AbraDebugDevOnlyrelayprovider": False,
@@ -119,21 +111,26 @@
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             "x-fb-friendly-name": "useAbraSendMessageMutation",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         raw_response = response.text
         last_streamed_response = None
-        text = ""
         for line in raw_response.split("\n"):
             try:
                 json_line = json.loads(line)
             except json.JSONDecodeError:
                 continue
-            if "errors" not in json_line.keys():
+            bot_response_message = (
+                json_line.get("data", {})
+                .get("node", {})
+                .get("bot_response_message", {})
+            )
+            streaming_state = bot_response_message.get("streaming_state")
+            if streaming_state == "OVERALL_DONE":
                 last_streamed_response = json_line
 
         if last_streamed_response is None:
             if attempts > 3:
                 raise Exception(
                     "MetaAI is having issues and was not able to respond (Server Error)"
                 )
@@ -184,11 +181,42 @@
         text = ""
         for content in response["data"]["node"]["bot_response_message"][
             "composed_text"
         ]["content"]:
             text += content["text"] + "\n"
         return text
 
+    def generate_offline_threading_id(self) -> str:
+        """
+        Generates an offline threading ID.
+
+        Returns:
+            str: The generated offline threading ID.
+        """
+        # Maximum value for a 64-bit integer in Python
+        max_int = (1 << 64) - 1
+        mask22_bits = (1 << 22) - 1
+
+        # Function to get the current timestamp in milliseconds
+        def get_current_timestamp():
+            return int(time.time() * 1000)
+
+        # Function to generate a random 64-bit integer
+        def get_random_64bit_int():
+            return random.getrandbits(64)
+
+        # Combine timestamp and random value
+        def combine_and_mask(timestamp, random_value):
+            shifted_timestamp = timestamp << 22
+            masked_random = random_value & mask22_bits
+            return (shifted_timestamp | masked_random) & max_int
+
+        timestamp = get_current_timestamp()
+        random_value = get_random_64bit_int()
+        threading_id = combine_and_mask(timestamp, random_value)
+
+        return str(threading_id)
+
 
 if __name__ == "__main__":
     meta = MetaAI()
     print(meta.prompt("Whats the weather in San Francisco today?"))
```

### Comparing `meta_ai_api-1.0.6/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.7/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
```


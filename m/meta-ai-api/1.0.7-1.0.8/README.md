# Comparing `tmp/meta_ai_api-1.0.7.tar.gz` & `tmp/meta_ai_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.7.tar", last modified: Fri Apr 19 00:09:23 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.8.tar", last modified: Fri Apr 19 01:08:57 2024, max compression
```

## Comparing `meta_ai_api-1.0.7.tar` & `meta_ai_api-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.525811 meta_ai_api-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.525811 meta_ai_api-1.0.7/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-19 00:09:18.000000 meta_ai_api-1.0.7/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:09:23.529811 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 00:09:23.000000 meta_ai_api-1.0.7/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:08:57.318445 meta_ai_api-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.7/setup.py` & `meta_ai_api-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.7/src/meta_ai_api/main.py` & `meta_ai_api-1.0.8/src/meta_ai_api/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import random
 import time
 import urllib
 import uuid
+from typing import Dict, List
 
 import requests
 from requests_html import HTMLSession
 
 
 class MetaAI:
     """
@@ -46,30 +47,30 @@
             },
             "server_timestamps": "true",
             "doc_id": "7604648749596940",
         }
         payload = urllib.parse.urlencode(payload)
         headers = {
             "content-type": "application/x-www-form-urlencoded",
-            "cookie": f'_js_datr={self.cookies["_js_datr"]}; abra_csrf={self.cookies["abra_csrf"]};',
+            "cookie": f'_js_datr={self.cookies["_js_datr"]}; abra_csrf={self.cookies["abra_csrf"]}; datr={self.cookies["datr"]};',
             "dpr": "2",
             "sec-fetch-site": "same-origin",
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             "x-fb-friendly-name": "useAbraAcceptTOSForTempUserMutation",
             "x-fb-lsd": "AVrWIDJrQQI",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         auth_json = response.json()
         access_token = auth_json["data"]["xab_abra_accept_terms_of_service"][
             "new_temp_user_auth"
         ]["access_token"]
         return access_token
 
-    def prompt(self, message: str, attempts: int = 0) -> str:
+    def prompt(self, message: str, attempts: int = 0) -> Dict:
         """
         Sends a message to the Meta AI and returns the response.
 
         Args:
             message (str): The message to send.
             attempts (int): The number of attempts made (used for recursion).
 
@@ -122,39 +123,42 @@
                 continue
             bot_response_message = (
                 json_line.get("data", {})
                 .get("node", {})
                 .get("bot_response_message", {})
             )
             streaming_state = bot_response_message.get("streaming_state")
+            fetch_id = bot_response_message.get("fetch_id")
             if streaming_state == "OVERALL_DONE":
                 last_streamed_response = json_line
 
         if last_streamed_response is None:
             if attempts > 3:
                 raise Exception(
                     "MetaAI is having issues and was not able to respond (Server Error)"
                 )
             self.access_token = self.get_access_token()
             return self.prompt(message=message, attempts=attempts + 1)
         response = self.format_response(response=last_streamed_response)
-        return response
+        sources = self.fetch_sources(fetch_id)
+        return {"message": response, "sources": sources}
 
     def get_cookies(self) -> dict:
         """
         Extracts necessary cookies from the Meta AI main page.
 
         Returns:
             dict: A dictionary containing essential cookies.
         """
         session = HTMLSession()
         response = session.get("https://www.meta.ai/")
         return {
             "_js_datr": self._extract_value(response.text, "_js_datr"),
             "abra_csrf": self._extract_value(response.text, "abra_csrf"),
+            "datr": self._extract_value(response.text, "datr"),
         }
 
     def _extract_value(self, text: str, key: str) -> str:
         """
         Helper function to extract a specific value from the given text using a key.
 
         Args:
@@ -212,11 +216,52 @@
 
         timestamp = get_current_timestamp()
         random_value = get_random_64bit_int()
         threading_id = combine_and_mask(timestamp, random_value)
 
         return str(threading_id)
 
+    def fetch_sources(self, fetch_id: str) -> List[Dict]:
+        """
+        Fetches sources from the Meta AI API based on the given query.
+
+        Args:
+            fetch_id (str): The fetch ID to use for the query.
+
+        Returns:
+            list: A list of dictionaries containing the fetched sources.
+        """
+
+        url = "https://graph.meta.ai/graphql?locale=user"
+        payload = {
+            "access_token": self.access_token,
+            "fb_api_caller_class": "RelayModern",
+            "fb_api_req_friendly_name": "AbraSearchPluginDialogQuery",
+            "variables": json.dumps({"abraMessageFetchID": fetch_id}),
+            "server_timestamps": "true",
+            "doc_id": "6946734308765963",
+        }
+
+        payload = urllib.parse.urlencode(payload)
+
+        headers = {
+            "authority": "graph.meta.ai",
+            "accept-language": "en-US,en;q=0.9,fr-FR;q=0.8,fr;q=0.7",
+            "content-type": "application/x-www-form-urlencoded",
+            "cookie": f'dpr=2; abra_csrf={self.cookies["abra_csrf"]}; datr={self.cookies["datr"]}; ps_n=1; ps_l=1',
+            "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
+            "x-fb-friendly-name": "AbraSearchPluginDialogQuery",
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+        response_json = response.json()
+        search_results = response_json["data"]["message"]["searchResults"]
+        if search_results is None:
+            return []
+
+        references = search_results["references"]
+        return references
+
 
 if __name__ == "__main__":
     meta = MetaAI()
-    print(meta.prompt("Whats the weather in San Francisco today?"))
+    print(meta.prompt("What was the Warriors score last game?"))
```


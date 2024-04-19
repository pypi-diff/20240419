# Comparing `tmp/meta_ai_api-1.1.0.tar.gz` & `tmp/meta_ai_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.1.0.tar", last modified: Fri Apr 19 01:31:22 2024, max compression
+gzip compressed data, was "meta_ai_api-1.1.1.tar", last modified: Fri Apr 19 17:45:57 2024, max compression
```

## Comparing `meta_ai_api-1.1.0.tar` & `meta_ai_api-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:45:57.474937 meta_ai_api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-19 17:45:57.474937 meta_ai_api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 17:45:57.474937 meta_ai_api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:45:57.470937 meta_ai_api-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:45:57.474937 meta_ai_api-1.1.1/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/src/meta_ai_api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 17:45:52.000000 meta_ai_api-1.1.1/src/meta_ai_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:45:57.474937 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-19 17:45:57.000000 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 17:45:57.000000 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:45:57.000000 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 17:45:57.000000 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 17:45:57.000000 meta_ai_api-1.1.1/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.1.0/PKG-INFO` & `meta_ai_api-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -59,31 +59,39 @@
 response = ai.prompt(message="Whats the weather in San Francisco today? And what is the date?")
 print(response)
  
 ```
 result:
 ```json
 {
-   "message":"The weather in San Francisco, California, today includes ¹:\nNo precipitation with skies ranging from clear to cloudy\nWind speeds range from 0 to 21 miles per hour\nTemperatures range from 52 to 69 degrees Fahrenheit\nPlease note that the weather forecast is continually changing ² ³ ⁴.\n",
+   "message":"The weather in San Francisco today is mostly clear to overcast, with no precipitation, a wind speed between 0 and 8 miles per hour and temperatures ranging from 51 to 55 degrees Fahrenheit ¹. The date is Friday, April 19, 2024 ². Please note that the weather forecast is continually changing ³ ⁴ ⁵ ⁶.\n",
    "sources":[
       {
-         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today",
+         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today+and+date",
          "title":"WolframAlpha"
       },
       {
+         "link":"https://www.timeanddate.com/weather/usa/san-francisco",
+         "title":"Weather for San Francisco, California, USA - timeanddate.com"
+      },
+      {
+         "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-today/347629",
+         "title":"Weather Today for San Francisco, CA | AccuWeather"
+      },
+      {
          "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-forecast/347629",
-         "title":"San Francisco, CA Weather Forecast - AccuWeather"
+         "title":"San Francisco, CA Weather Forecast | AccuWeather"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/San+Francisco+CA+USCA0987:1:US",
-         "title":"10-Day Weather Forecast for San Francisco, CA"
+         "link":"https://forecast.weather.gov/zipcity.php?inputstring=San%20francisco%2CCA",
+         "title":"National Weather Service"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/Inverness+CA?canonicalCityId=61b2ebcaa5e78eebca92d21eaff7a0439eb081e8e60287fca37af4186f8242b7",
-         "title":"10-Day Weather Forecast for Inverness, CA"
+         "link":"https://www.wunderground.com/weather/us/ca/san-francisco",
+         "title":"San Francisco, CA Weather Conditions | Weather Underground"
       }
    ]
 }
 ```
 
 ```python
 from meta_ai_api import MetaAI
```

### Comparing `meta_ai_api-1.1.0/README.md` & `meta_ai_api-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,39 @@
 response = ai.prompt(message="Whats the weather in San Francisco today? And what is the date?")
 print(response)
  
 ```
 result:
 ```json
 {
-   "message":"The weather in San Francisco, California, today includes ¹:\nNo precipitation with skies ranging from clear to cloudy\nWind speeds range from 0 to 21 miles per hour\nTemperatures range from 52 to 69 degrees Fahrenheit\nPlease note that the weather forecast is continually changing ² ³ ⁴.\n",
+   "message":"The weather in San Francisco today is mostly clear to overcast, with no precipitation, a wind speed between 0 and 8 miles per hour and temperatures ranging from 51 to 55 degrees Fahrenheit ¹. The date is Friday, April 19, 2024 ². Please note that the weather forecast is continually changing ³ ⁴ ⁵ ⁶.\n",
    "sources":[
       {
-         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today",
+         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today+and+date",
          "title":"WolframAlpha"
       },
       {
+         "link":"https://www.timeanddate.com/weather/usa/san-francisco",
+         "title":"Weather for San Francisco, California, USA - timeanddate.com"
+      },
+      {
+         "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-today/347629",
+         "title":"Weather Today for San Francisco, CA | AccuWeather"
+      },
+      {
          "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-forecast/347629",
-         "title":"San Francisco, CA Weather Forecast - AccuWeather"
+         "title":"San Francisco, CA Weather Forecast | AccuWeather"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/San+Francisco+CA+USCA0987:1:US",
-         "title":"10-Day Weather Forecast for San Francisco, CA"
+         "link":"https://forecast.weather.gov/zipcity.php?inputstring=San%20francisco%2CCA",
+         "title":"National Weather Service"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/Inverness+CA?canonicalCityId=61b2ebcaa5e78eebca92d21eaff7a0439eb081e8e60287fca37af4186f8242b7",
-         "title":"10-Day Weather Forecast for Inverness, CA"
+         "link":"https://www.wunderground.com/weather/us/ca/san-francisco",
+         "title":"San Francisco, CA Weather Conditions | Weather Underground"
       }
    ]
 }
 ```
 
 ```python
 from meta_ai_api import MetaAI
```

### Comparing `meta_ai_api-1.1.0/setup.py` & `meta_ai_api-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.1.0/src/meta_ai_api/main.py` & `meta_ai_api-1.1.1/src/meta_ai_api/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         Returns:
             str: A valid access token.
         """
         self.cookies = self.get_cookies()
         url = "https://www.meta.ai/api/graphql/"
 
         payload = {
-            "lsd": "AVrWIDJrQQI",
+            "lsd": self.cookies["lsd"],
             "fb_api_caller_class": "RelayModern",
             "fb_api_req_friendly_name": "useAbraAcceptTOSForTempUserMutation",
             "variables": {
                 "dob": "1999-01-01",
                 "icebreaker_type": "TEXT",
                 "__relay_internal__pv__WebPixelRatiorelayprovider": 1,
             },
@@ -52,15 +52,14 @@
         }
         payload = urllib.parse.urlencode(payload)
         headers = {
             "content-type": "application/x-www-form-urlencoded",
             "cookie": f'_js_datr={self.cookies["_js_datr"]}; abra_csrf={self.cookies["abra_csrf"]}; datr={self.cookies["datr"]};',
             "sec-fetch-site": "same-origin",
             "x-fb-friendly-name": "useAbraAcceptTOSForTempUserMutation",
-            "x-fb-lsd": "AVrWIDJrQQI",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         auth_json = response.json()
         access_token = auth_json["data"]["xab_abra_accept_terms_of_service"][
             "new_temp_user_auth"
         ]["access_token"]
@@ -147,17 +146,26 @@
 
         Returns:
             dict: A dictionary containing essential cookies.
         """
         session = HTMLSession()
         response = session.get("https://www.meta.ai/")
         return {
-            "_js_datr": extract_value(response.text, "_js_datr"),
-            "abra_csrf": extract_value(response.text, "abra_csrf"),
-            "datr": extract_value(response.text, "datr"),
+            "_js_datr": extract_value(
+                response.text, start_str='_js_datr":{"value":"', end_str='",'
+            ),
+            "abra_csrf": extract_value(
+                response.text, start_str='abra_csrf":{"value":"', end_str='",'
+            ),
+            "datr": extract_value(
+                response.text, start_str='datr":{"value":"', end_str='",'
+            ),
+            "lsd": extract_value(
+                response.text, start_str='"LSD",[],{"token":"', end_str='"}'
+            ),
         }
 
     def fetch_sources(self, fetch_id: str) -> List[Dict]:
         """
         Fetches sources from the Meta AI API based on the given query.
 
         Args:
```

### Comparing `meta_ai_api-1.1.0/src/meta_ai_api/utils.py` & `meta_ai_api-1.1.1/src/meta_ai_api/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,28 @@
     timestamp = get_current_timestamp()
     random_value = get_random_64bit_int()
     threading_id = combine_and_mask(timestamp, random_value)
 
     return str(threading_id)
 
 
-def extract_value(text: str, key: str) -> str:
+def extract_value(text: str, start_str: str, end_str: str) -> str:
     """
     Helper function to extract a specific value from the given text using a key.
 
     Args:
         text (str): The text from which to extract the value.
-        key (str): The key associated with the value.
+        start_str (str): The starting key.
+        end_str (str): The ending key.
 
     Returns:
         str: The extracted value.
     """
-    start = text.find(f'{key}":{{"value":"') + len(f'{key}":{{"value":"')
-    end = text.find('",', start)
+    start = text.find(start_str) + len(start_str)
+    end = text.find(end_str, start)
     return text[start:end]
 
 
 def format_response(response: dict) -> str:
     """
     Formats the response from Meta AI to remove unnecessary characters.
```

### Comparing `meta_ai_api-1.1.0/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.1.1/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -59,31 +59,39 @@
 response = ai.prompt(message="Whats the weather in San Francisco today? And what is the date?")
 print(response)
  
 ```
 result:
 ```json
 {
-   "message":"The weather in San Francisco, California, today includes ¹:\nNo precipitation with skies ranging from clear to cloudy\nWind speeds range from 0 to 21 miles per hour\nTemperatures range from 52 to 69 degrees Fahrenheit\nPlease note that the weather forecast is continually changing ² ³ ⁴.\n",
+   "message":"The weather in San Francisco today is mostly clear to overcast, with no precipitation, a wind speed between 0 and 8 miles per hour and temperatures ranging from 51 to 55 degrees Fahrenheit ¹. The date is Friday, April 19, 2024 ². Please note that the weather forecast is continually changing ³ ⁴ ⁵ ⁶.\n",
    "sources":[
       {
-         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today",
+         "link":"https://www.wolframalpha.com/input?i=San+Francisco+weather+today+and+date",
          "title":"WolframAlpha"
       },
       {
+         "link":"https://www.timeanddate.com/weather/usa/san-francisco",
+         "title":"Weather for San Francisco, California, USA - timeanddate.com"
+      },
+      {
+         "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-today/347629",
+         "title":"Weather Today for San Francisco, CA | AccuWeather"
+      },
+      {
          "link":"https://www.accuweather.com/en/us/san-francisco/94103/weather-forecast/347629",
-         "title":"San Francisco, CA Weather Forecast - AccuWeather"
+         "title":"San Francisco, CA Weather Forecast | AccuWeather"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/San+Francisco+CA+USCA0987:1:US",
-         "title":"10-Day Weather Forecast for San Francisco, CA"
+         "link":"https://forecast.weather.gov/zipcity.php?inputstring=San%20francisco%2CCA",
+         "title":"National Weather Service"
       },
       {
-         "link":"https://weather.com/weather/tenday/l/Inverness+CA?canonicalCityId=61b2ebcaa5e78eebca92d21eaff7a0439eb081e8e60287fca37af4186f8242b7",
-         "title":"10-Day Weather Forecast for Inverness, CA"
+         "link":"https://www.wunderground.com/weather/us/ca/san-francisco",
+         "title":"San Francisco, CA Weather Conditions | Weather Underground"
       }
    ]
 }
 ```
 
 ```python
 from meta_ai_api import MetaAI
```


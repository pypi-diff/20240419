# Comparing `tmp/meta_ai_api-1.0.4.tar.gz` & `tmp/meta_ai_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.4.tar", last modified: Thu Apr 18 21:48:00 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.5.tar", last modified: Thu Apr 18 22:04:17 2024, max compression
```

## Comparing `meta_ai_api-1.0.4.tar` & `meta_ai_api-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-18 21:47:55.000000 meta_ai_api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:47:55.000000 meta_ai_api-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:47:55.000000 meta_ai_api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:47:55.000000 meta_ai_api-1.0.4/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-18 21:47:55.000000 meta_ai_api-1.0.4/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:48:00.499813 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-18 21:48:00.000000 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:48:00.000000 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:48:00.000000 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:48:00.000000 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:48:00.000000 meta_ai_api-1.0.4/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.831620 meta_ai_api-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.831620 meta_ai_api-1.0.5/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.4/PKG-INFO` & `meta_ai_api-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -25,15 +25,15 @@
 Requires-Dist: requests
 Requires-Dist: requests-html
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI API Wrapper
 
-MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
+MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
```

### Comparing `meta_ai_api-1.0.4/README.md` & `meta_ai_api-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MetaAI API Wrapper
 
-MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
+MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
```

### Comparing `meta_ai_api-1.0.4/setup.py` & `meta_ai_api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.4/src/meta_ai_api/main.py` & `meta_ai_api-1.0.5/src/meta_ai_api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             json_line = json.loads(line)
             if "errors" not in json_line.keys():
                 last_streamed_response = json_line
 
         if last_streamed_response is None:
             if attempts > 3:
                 raise Exception(
-                    "Was not able to query Meta AI. Either patched or MetaAI is having issues."
+                    "MetaAI is having issues and was not able to respond (Server Error)"
                 )
             self.access_token = self.get_access_token()
             return self.prompt(message=message, attempts=attempts + 1)
         for content in last_streamed_response["data"]["node"]["bot_response_message"][
             "composed_text"
         ]["content"]:
             text += content["text"] + "\n"
```

### Comparing `meta_ai_api-1.0.4/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.5/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -25,15 +25,15 @@
 Requires-Dist: requests
 Requires-Dist: requests-html
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI API Wrapper
 
-MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
+MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
```


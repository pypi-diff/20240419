# Comparing `tmp/webscout-1.3.1.tar.gz` & `tmp/webscout-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.1.tar", last modified: Fri Apr 19 06:35:35 2024, max compression
+gzip compressed data, was "webscout-1.3.2.tar", last modified: Fri Apr 19 10:46:01 2024, max compression
```

## Comparing `webscout-1.3.1.tar` & `webscout-1.3.2.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.205617 webscout-1.3.1/
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.749132 webscout-1.3.1/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.771130 webscout-1.3.1/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.804826 webscout-1.3.1/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.820831 webscout-1.3.1/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.1/LICENSE.md
--rw-rw-rw-   0        0        0    31533 2024-04-19 06:35:35.200620 webscout-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    29342 2024-04-19 06:32:44.000000 webscout-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 06:35:35.205617 webscout-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2725 2024-04-19 06:30:17.000000 webscout-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.088616 webscout-1.3.1/webscout/
--rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-19 06:26:09.000000 webscout-1.3.1/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.1/webscout/LLM.py
--rw-rw-rw-   0        0        0      572 2024-04-19 06:18:21.000000 webscout-1.3.1/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.1/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-19 06:30:29.000000 webscout-1.3.1/webscout/version.py
--rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.1/webscout/voice.py
--rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.188618 webscout-1.3.1/webscout.egg-info/
--rw-rw-rw-   0        0        0    31533 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2024-04-19 06:35:34.000000 webscout-1.3.1/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.674465 webscout-1.3.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.008720 webscout-1.3.2/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.024723 webscout-1.3.2/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.053714 webscout-1.3.2/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.073717 webscout-1.3.2/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0    30426 2024-04-19 10:46:01.669462 webscout-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    28235 2024-04-19 10:44:32.000000 webscout-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:46:01.675459 webscout-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2725 2024-04-19 08:30:45.000000 webscout-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.634425 webscout-1.3.2/webscout/
+-rw-rw-rw-   0        0        0    93054 2024-04-19 10:20:12.000000 webscout-1.3.2/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24126 2024-04-19 10:31:02.000000 webscout-1.3.2/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.2/webscout/LLM.py
+-rw-rw-rw-   0        0        0      977 2024-04-19 10:22:02.000000 webscout-1.3.2/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    16358 2024-04-19 06:46:37.000000 webscout-1.3.2/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.2/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-19 08:30:29.000000 webscout-1.3.2/webscout/version.py
+-rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.2/webscout/voice.py
+-rw-rw-rw-   0        0        0    74262 2024-04-19 10:21:11.000000 webscout-1.3.2/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.664465 webscout-1.3.2/webscout.egg-info/
+-rw-rw-rw-   0        0        0    30426 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.1/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.2/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.2/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.2/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.2/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/networks/network_configs.py` & `webscout-1.3.2/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.2/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/utilsdw/enver.py` & `webscout-1.3.2/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.2/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/LICENSE.md` & `webscout-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/PKG-INFO` & `webscout-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.1
+Version: 1.3.2
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -60,15 +60,14 @@
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
@@ -93,14 +92,15 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
+    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
@@ -121,27 +121,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI version of webscout.AI
-| Command | Description |
-|-----------------------------------------------|--------------------------------------------------------------------------------------------------------|
-| `python -m webscout.AI phindsearch --prompt "your search query"` | CLI function to perform a search query using Webscout.AI's Phindsearch feature. |
-| `python -m webscout.AI yepchat --message "your_message_here"` | CLI function to send a message using Webscout.AI's Yepchat feature. |
-| `python -m webscout.AI youchat --prompt "your_prompt_here"` | CLI function to generate a response based on a prompt using Webscout.AI's Youchat feature. |
-| `python -m webscout.AI gemini --message "tell me about gemma 7b"` | CLI function to get information about a specific topic using Webscout.AI's Gemini feature. |
-| `python -m webscout.AI prodia --prompt "car"` | CLI function to generate content related to a prompt using Webscout.AI's Prodia feature. |
-| `python -m webscout.AI blackboxai --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's Blackbox search feature. |
-| `python -m webscout.AI perplexity --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's PERPLEXITY feature. |
-| `python -m webscout.AI opengpt --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's OPENGPT feature. |
-
-
 ## CLI to use LLM 
 ```python
 python -m webscout.LLM model_name 
 ```
 [Go To TOP](#TOP)
 
 ## Regions
@@ -694,14 +681,24 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
+### 10. `Sean` - chat With Sean
+```python
+from webscout.AI import Sean
+
+a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
+# This example sends a simple greeting and prints the response
+prompt = "tell me about india"
+response_str = a.chat(prompt)
+print(response_str)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.1 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.2 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos and have TTS support Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -27,22 +27,21 @@
 Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
 Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
-      [Install](#install) - [CLI version](#cli-version) - [CLI version of
-webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
-Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
-  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
- before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:]
-   (#text-to-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL
-   voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
+ [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
+   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
+Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
+(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
+ remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
+ Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
+[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
 classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
   - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
   search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
 DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
   yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
   images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
   search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
@@ -58,51 +57,34 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
-   internet) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
+opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
+ chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
+webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
    k Text | CLI function to perform a suggestions search using Webscout. | |
  python -m webscout text -k Text | CLI function to perform a text search using
  Webscout. | | python -m webscout translate -k Text | CLI function to perform
    translate using Webscout. | | python -m webscout version | A command-line
    interface command that prints and returns the version of the program. | |
   python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
- specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
- prodia --prompt "car"` | CLI function to generate content related to a prompt
- using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
-      prompt "Your prompt here"` | CLI function to perform a search using
-Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
-      prompt "Your prompt here"` | CLI function to perform a search using
- Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
-  "Your prompt here"` | CLI function to perform a search using Webscout.AI's
-     OPENGPT feature. | ## CLI to use LLM ```python python -m webscout.LLM
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
  model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
 Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
  Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
  for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
  China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
 Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
  gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
@@ -318,50 +300,54 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
- (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-`LLM` ```python from webscout.LLM import LLM # Read the system message from the
-   file with open('system.txt', 'r') as file: system_message = file.read() #
-   Initialize the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
- __future__ import annotations from typing import List, Optional from webscout
-  import LLM from webscout import WEBS import warnings system_message: str =
- ( "As AI, you possess internet access and are capable of executing real-time
-  web searches based on user inputs. " "You shall utilize this capability to
- enrich conversations, offer informed insights, and augment your ability to "
-  "respond accurately and thoroughly. However, refrain from stating 'You have
-  provided a list of strings,' ensuring " "seamless interactions with users.
-Embrace a responsive demeanor, harnessing available online resources to address
- " "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-                  ", response) else: print("No response") ```
+(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
+Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
+sends a simple greeting and prints the response prompt = "tell me about india"
+response_str = a.chat(prompt) print(response_str) ``` ## usage of special .LLM
+file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+                        else: print("No response") ```
```

### Comparing `webscout-1.3.1/README.md` & `webscout-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
@@ -41,14 +40,15 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
+    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
@@ -69,27 +69,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI version of webscout.AI
-| Command | Description |
-|-----------------------------------------------|--------------------------------------------------------------------------------------------------------|
-| `python -m webscout.AI phindsearch --prompt "your search query"` | CLI function to perform a search query using Webscout.AI's Phindsearch feature. |
-| `python -m webscout.AI yepchat --message "your_message_here"` | CLI function to send a message using Webscout.AI's Yepchat feature. |
-| `python -m webscout.AI youchat --prompt "your_prompt_here"` | CLI function to generate a response based on a prompt using Webscout.AI's Youchat feature. |
-| `python -m webscout.AI gemini --message "tell me about gemma 7b"` | CLI function to get information about a specific topic using Webscout.AI's Gemini feature. |
-| `python -m webscout.AI prodia --prompt "car"` | CLI function to generate content related to a prompt using Webscout.AI's Prodia feature. |
-| `python -m webscout.AI blackboxai --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's Blackbox search feature. |
-| `python -m webscout.AI perplexity --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's PERPLEXITY feature. |
-| `python -m webscout.AI opengpt --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's OPENGPT feature. |
-
-
 ## CLI to use LLM 
 ```python
 python -m webscout.LLM model_name 
 ```
 [Go To TOP](#TOP)
 
 ## Regions
@@ -642,14 +629,24 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
+### 10. `Sean` - chat With Sean
+```python
+from webscout.AI import Sean
+
+a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
+# This example sends a simple greeting and prints the response
+prompt = "tell me about india"
+response_str = a.chat(prompt)
+print(response_str)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
-      [Install](#install) - [CLI version](#cli-version) - [CLI version of
-webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
-Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
-  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
- before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:]
-   (#text-to-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL
-   voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
+ [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
+   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
+Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
+(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
+ remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
+ Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
+[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
 classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
   - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
   search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
 DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
   yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
   images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
   search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
@@ -30,51 +29,34 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
-   internet) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
+opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
+ chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
+webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
    k Text | CLI function to perform a suggestions search using Webscout. | |
  python -m webscout text -k Text | CLI function to perform a text search using
  Webscout. | | python -m webscout translate -k Text | CLI function to perform
    translate using Webscout. | | python -m webscout version | A command-line
    interface command that prints and returns the version of the program. | |
   python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
- specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
- prodia --prompt "car"` | CLI function to generate content related to a prompt
- using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
-      prompt "Your prompt here"` | CLI function to perform a search using
-Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
-      prompt "Your prompt here"` | CLI function to perform a search using
- Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
-  "Your prompt here"` | CLI function to perform a search using Webscout.AI's
-     OPENGPT feature. | ## CLI to use LLM ```python python -m webscout.LLM
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
  model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
 Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
  Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
  for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
  China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
 Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
  gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
@@ -290,50 +272,54 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
- (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-`LLM` ```python from webscout.LLM import LLM # Read the system message from the
-   file with open('system.txt', 'r') as file: system_message = file.read() #
-   Initialize the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
- __future__ import annotations from typing import List, Optional from webscout
-  import LLM from webscout import WEBS import warnings system_message: str =
- ( "As AI, you possess internet access and are capable of executing real-time
-  web searches based on user inputs. " "You shall utilize this capability to
- enrich conversations, offer informed insights, and augment your ability to "
-  "respond accurately and thoroughly. However, refrain from stating 'You have
-  provided a list of strings,' ensuring " "seamless interactions with users.
-Embrace a responsive demeanor, harnessing available online resources to address
- " "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-                  ", response) else: print("No response") ```
+(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
+Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
+sends a simple greeting and prints the response prompt = "tell me about india"
+response_str = a.chat(prompt) print(response_str) ``` ## usage of special .LLM
+file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+                        else: print("No response") ```
```

### Comparing `webscout-1.3.1/setup.py` & `webscout-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.1", 
+    version="1.3.2", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.3.1/webscout/AI.py` & `webscout-1.3.2/webscout/AI.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,716 @@
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts
 from webscout.AIbase import Provider
 from Helpingai_T2 import Perplexity
 from typing import Any
 import logging
+#----------------------------------------------------------Sean-----------------------------------------------------------
+class Sean:
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENGPT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = (
+            "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.assistant_id = "281bc620-b9f3-47c6-bf74-3f0e5b6e7dac"
+        self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
+
+        self.headers = {
+            "authority": self.authority,
+            "accept": "text/event-stream",
+            "accept-language": "en-US,en;q=0.7",
+            "cache-control": "no-cache",
+            "content-type": "application/json",
+            "origin": "https://opengpts-example-vz4y4ooboq-uc.a.run.app",
+            "pragma": "no-cache",
+            "referer": "https://opengpts-example-vz4y4ooboq-uc.a.run.app/",
+            "sec-fetch-site": "same-origin",
+            "sec-gpc": "1",
+            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "messages": [
+                {
+                    "content": "Hello there",
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": false
+                },
+                {
+                    "content": "Hello! How can I assist you today?",
+                    "additional_kwargs": {
+                    "agent": {
+                        "return_values": {
+                            "output": "Hello! How can I assist you today?"
+                            },
+                        "log": "Hello! How can I assist you today?",
+                        "type": "AgentFinish"
+                    }
+                },
+                "type": "ai",
+                "example": false
+                }]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        self.session.headers.update(
+            dict(
+                cookie=f"opengpts_user_id={uuid4().__str__()}",
+            )
+        )
+        payload = {
+            "input": [
+                {
+                    "content": conversation_prompt,
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": False,
+                },
+            ],
+            "assistant_id": self.assistant_id,
+            "thread_id": "",
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/event-stream; charset=utf-8"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    modified_value = re.sub("data:", "", value)
+                    resp = json.loads(modified_value)
+                    if len(resp) == 1:
+                        continue
+                    self.last_response.update(resp[1])
+                    yield value if raw else resp[1]
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["content"]
+#----------------------------------------------------------OpenAI-----------------------------------------------------------
+class OPENAI(Provider):
+    model = "gpt-3.5-turbo"
+    def __init__(
+        self,
+        api_key: str,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 1,
+        model: str = model,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENAI
+
+        Args:
+            api_key (key): OpenAI's API key.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_key = api_key
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.openai.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
+            "object": "chat.completion",
+            "created": 1704623244,
+            "model": "gpt-3.5-turbo",
+            "usage": {
+                "prompt_tokens": 0,
+                "completion_tokens": 0,
+                "total_tokens": 0
+                },
+            "choices": [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": "Hello! How can I assist you today?"
+                },
+                "finish_reason": "stop",
+                "index": 0
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.session.headers.update(self.headers)
+        payload = {
+            "frequency_penalty": self.frequency_penalty,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+            "presence_penalty": self.presence_penalty,
+            "stream": stream,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "data:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    incomplete_message = self.get_message(resp)
+                    if incomplete_message:
+                        message_load += incomplete_message
+                        resp["choices"][0]["delta"]["content"] = message_load
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    elif raw:
+                        yield value
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type", "") == "application/json"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            resp = response.json()
+            self.last_response.update(resp)
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            return resp
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
+            return ""
+#--------------------------------------LEO-----------------------------------------
+class LEO(Provider):
+    
+    model = "llama-2-13b-chat"
+
+    key = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u"
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.2,
+        top_k: int = -1,
+        top_p: float = 0.999,
+        model: str = model,
+        brave_key: str = key,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
+            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeput (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.stop_sequences = ["</response>", "</s>"]
+        self.temperature = temperature
+        self.top_k = top_k
+        self.top_p = top_p
+        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "accept": "text/event-stream",
+            "x-brave-key": brave_key,
+            "accept-language": "en-US,en;q=0.9",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
+        }
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.ession.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+        self.system_prompt = (
+            "\n\nYour name is Leo, a helpful"
+            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
+            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
+            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
+            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
+            "If you don't know the answer to a question, please don't share false information.\n"
+        )
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "completion": "\nNext: domestic cat breeds with short hair >>",
+            "stop_reason": null,
+            "truncated": false,
+            "stop": null,
+            "model": "llama-2-13b-chat",
+            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
+            "exception": null
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "max_tokens_to_sample": self.max_tokens_to_sample,
+            "model": self.model,
+            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
+            "self.stop_sequence": self.stop_sequences,
+            "stream": stream,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/event-stream; charset=utf-8"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "data:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type", "") == "application/json"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            resp = response.json()
+            self.last_response.update(resp)
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            return resp
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("completion")
 #------------------------------------------------------KOBOLDAI-----------------------------------------------------------
 class KOBOLDAI(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         temperature: float = 1,
@@ -855,14 +1557,15 @@
         """Sends a request to the BLACKBOXAI API and processes the response."""
         blackbox_ai = BLACKBOXAI()  # Initialize a BLACKBOXAI instance
         response = blackbox_ai.ask(prompt)  # Perform a chat with the given prompt
         processed_response = blackbox_ai.get_message(response)  # Process the response
         print(processed_response)
 #------------------------------------------------------phind-------------------------------------------------------------
 class PhindSearch:
+    # default_model = "Phind Model"
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 8000,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
@@ -1219,41 +1922,203 @@
     @staticmethod
     def chat_cli(prompt):
         """Generate completion based on the provided prompt"""
         you_chat = youChat()
         completion = you_chat.create(prompt)
         print(completion)
 #-------------------------------------------------------Gemini--------------------------------------------------------        
-class Gemini:
-    def __init__(self):
-        self.messages = []
-
-    def chat(self, *args):
-        assert args != ()
-
-        message = " ".join(args)
-        self.messages.append({"role": "user", "content": message})
-
-        response = g4f.ChatCompletion.create(
-            model=g4f.models.default,
-            provider=g4f.Provider.Gemini,
-            messages=self.messages,
-            stream=True,
-        )
-        ms = ""
-        for message in response:
-            ms += message
-        self.messages.append({"role": "assistant", "content": ms.strip()}) # Strip whitespace from the message content
-        return ms.strip() # Return the message without trailing whitespace
+from Bard import Chatbot
+import logging
+from os import path
+from json import load
+from json import dumps
+import warnings
 
-    @staticmethod
-    def chat_cli(message):
-        """Generate completion based on the provided message"""
-        gemini = Gemini()
-        return gemini.chat(message)
+logging.getLogger("httpx").setLevel(logging.ERROR)
+
+warnings.simplefilter("ignore", category=UserWarning)
+class GEMINI(Provider):
+    def __init__(
+        self,
+        cookie_file: str,
+        proxy: dict = {},
+        timeout: int = 30,
+    ):
+        """Initializes GEMINI
+
+        Args:
+            cookie_file (str): Path to `bard.google.com.cookies.json` file
+            proxy (dict, optional): Http request proxy. Defaults to {}.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+        """
+        self.conversation = Conversation(False)
+        self.session_auth1 = None
+        self.session_auth2 = None
+        assert isinstance(
+            cookie_file, str
+        ), f"cookie_file should be of {str} only not '{type(cookie_file)}'"
+        if path.isfile(cookie_file):
+            # let's assume auth is a path to exported .json cookie-file
+            with open(cookie_file) as fh:
+                entries = load(fh)
+            for entry in entries:
+                if entry["name"] == "__Secure-1PSID":
+                    self.session_auth1 = entry["value"]
+                elif entry["name"] == "__Secure-1PSIDTS":
+                    self.session_auth2 = entry["value"]
+
+            assert all(
+                [self.session_auth1, self.session_auth2]
+            ), f"Failed to extract the required cookie value from file '{cookie_file}'"
+        else:
+            raise Exception(f"{cookie_file} is not a valid file path")
+
+        self.session = Chatbot(self.session_auth1, self.session_auth2, proxy, timeout)
+        self.last_response = {}
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+            Args:
+                prompt (str): Prompt to be send.
+                stream (bool, optional): Flag for streaming response. Defaults to False.
+                raw (bool, optional): Stream back raw response as received. Defaults to False.
+                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
+                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+            Returns:
+               dict : {}
+            ```json
+            {
+                "content": "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]",
+                "conversation_id": "c_f13f6217f9a997aa",
+                "response_id": "r_d3665f95975c368f",
+                "factualityQueries": null,
+                "textQuery": [
+                    "hello there",
+                    1
+                    ],
+                "choices": [
+                    {
+                        "id": "rc_ea075c9671bfd8cb",
+                        "content": [
+                            "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]"
+                        ]
+                    },
+                    {
+                        "id": "rc_de6dd3fb793a5402",
+                        "content": [
+                            "General Kenobi! (or just a friendly hello, whichever you prefer!). \n\nI see you're a person of culture as well. *Star Wars* references are always appreciated.  \n\nHow can I help you today?\n"
+                            ]
+                    },
+                {
+                    "id": "rc_a672ac089caf32db",
+                    "content": [
+                        "General Kenobi! (or just a friendly hello if you're not a Star Wars fan!). \n\nHow can I help you today? Feel free to ask me anything, or tell me what you'd like to chat about. I'm here to assist in any way I can.\n[Image of Obi-Wan Kenobi saying hello there]"
+                    ]
+                }
+            ],
+
+            "images": [
+                "https://i.pinimg.com/originals/40/74/60/407460925c9e419d82b93313f0b42f71.jpg"
+            ]
+        }
+
+            ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        def for_stream():
+            response = self.session.ask(prompt)
+            self.last_response.update(response)
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            yield dumps(response) if raw else response
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["content"]
+
+    def reset(self):
+        """Reset the current conversation"""
+        self.session.async_chatbot.conversation_id = ""
+        self.session.async_chatbot.response_id = ""
+        self.session.async_chatbot.choice_id = ""
 #-------------------------------------------------------Prodia-------------------------------------------------------------------------
 class Prodia:
     """
     This class provides methods for generating images based on prompts.
     """
 
     def create(self, prompt):
@@ -1375,18 +2240,14 @@
     YepChat.chat_cli(message)
 
 @cli.command()
 @click.option('--prompt', prompt='Enter your prompt', help='The prompt to generate a completion from.')
 def youchat(prompt):
     youChat.chat_cli(prompt)
 
-@cli.command()
-@click.option('--message', prompt='Enter your message', help='The message to send.')
-def gemini(message):
-    Gemini.chat_cli(message)
 
 @cli.command()
 @click.option('--prompt', prompt='Enter your prompt', help='The prompt for generating the image.')
 def prodia(prompt):
     """Generate an image based on the provided prompt."""
     Prodia.prodia_cli(prompt)
```

### Comparing `webscout-1.3.1/webscout/AIbase.py` & `webscout-1.3.2/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/AIutel.py` & `webscout-1.3.2/webscout/AIutel.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             with open(self.file, "a") as fh:
                 fh.write(new_history)
         self.chat_history += new_history
 
 
 class AwesomePrompts:
     awesome_prompt_url = (
-        "https://github.com/Simatwa/gpt-cli/blob/main/assets/all-acts.json?raw=true"
+        "https://raw.githubusercontent.com/OE-LUCIFER/prompts/main/prompt.json"
     )
     awesome_prompt_path = os.path.join(default_path, "all-acts.json")
 
     __is_prompt_updated = False
 
     def __init__(self):
         self.acts = self.all_acts
@@ -359,17 +359,17 @@
                 json.dump(current_prompts, fh, indent=4)
             logging.info(f"Prompt deleted successfully - `{name}`")
         else:
             return False
 
 
 class Updates:
-    """Pytgpt latest release info"""
+    """Webscout latest release info"""
 
-    url = "https://api.github.com/repos/Simatwa/python-tgpt/releases/latest"
+    url = "https://api.github.com/repos/OE-LUCIFER/Webscout/releases/latest"
 
     @property
     def latest_version(self):
         return self.latest(version=True)
 
     def executable(self, system: str = platform.system()) -> str:
         """Url pointing to executable for particular system
@@ -381,15 +381,15 @@
             str: url
         """
         for entry in self.latest()["assets"]:
             if entry.get("target") == system:
                 return entry.get("url")
 
     def latest(self, whole: bool = False, version: bool = False) -> dict:
-        """Check pytgpt latest version info
+        """Check Webscout latest version info
 
         Args:
             whole (bool, optional): Return whole json response. Defaults to False.
             version (bool, optional): return version only. Defaults to False.
 
         Returns:
             bool|dict: version str or whole dict info
@@ -504,15 +504,15 @@
         self.python_version = (
             f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
             if self.internal_exec
             else run_system_command(
                 f"{self.interpreter} --version",
                 exit_on_error=True,
                 stdout_error=True,
-                help="If you're using pytgpt-cli, use the flag '--internal-exec'",
+                help="If you're using Webscout-cli, use the flag '--internal-exec'",
             )[1].stdout.split(" ")[1]
         )
 
     @property
     def intro_prompt(self):
         return f"""
 You are a command-line coding assistant called Rawdog that generates and auto-executes Python scripts.
@@ -584,15 +584,15 @@
         Args:
             message (str): Log message
             category (str, optional): Log level. Defaults to 'info'.
         """
         if self.quiet:
             return
 
-        message = "[PYTGPT] - " + message
+        message = "[Webscout] - " + message
         if category == "error":
             logging.error(message)
         else:
             logging.info(message)
 
     def main(self, response: str) -> None:
         """Exec code in response accordingly
```

### Comparing `webscout-1.3.1/webscout/DWEBS.py` & `webscout-1.3.2/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/HelpingAI.py` & `webscout-1.3.2/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/LLM.py` & `webscout-1.3.2/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/cli.py` & `webscout-1.3.2/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/models.py` & `webscout-1.3.2/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/transcriber.py` & `webscout-1.3.2/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/utils.py` & `webscout-1.3.2/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/voice.py` & `webscout-1.3.2/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/webscout_search.py` & `webscout-1.3.2/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout/webscout_search_async.py` & `webscout-1.3.2/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.1/webscout.egg-info/PKG-INFO` & `webscout-1.3.2/webscout.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.1
+Version: 1.3.2
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -60,15 +60,14 @@
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
@@ -93,14 +92,15 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
+    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
@@ -121,27 +121,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI version of webscout.AI
-| Command | Description |
-|-----------------------------------------------|--------------------------------------------------------------------------------------------------------|
-| `python -m webscout.AI phindsearch --prompt "your search query"` | CLI function to perform a search query using Webscout.AI's Phindsearch feature. |
-| `python -m webscout.AI yepchat --message "your_message_here"` | CLI function to send a message using Webscout.AI's Yepchat feature. |
-| `python -m webscout.AI youchat --prompt "your_prompt_here"` | CLI function to generate a response based on a prompt using Webscout.AI's Youchat feature. |
-| `python -m webscout.AI gemini --message "tell me about gemma 7b"` | CLI function to get information about a specific topic using Webscout.AI's Gemini feature. |
-| `python -m webscout.AI prodia --prompt "car"` | CLI function to generate content related to a prompt using Webscout.AI's Prodia feature. |
-| `python -m webscout.AI blackboxai --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's Blackbox search feature. |
-| `python -m webscout.AI perplexity --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's PERPLEXITY feature. |
-| `python -m webscout.AI opengpt --prompt "Your prompt here"` | CLI function to perform a search using Webscout.AI's OPENGPT feature. |
-
-
 ## CLI to use LLM 
 ```python
 python -m webscout.LLM model_name 
 ```
 [Go To TOP](#TOP)
 
 ## Regions
@@ -694,14 +681,24 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
+### 10. `Sean` - chat With Sean
+```python
+from webscout.AI import Sean
+
+a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
+# This example sends a simple greeting and prints the response
+prompt = "tell me about india"
+response_str = a.chat(prompt)
+print(response_str)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.1 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.2 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos and have TTS support Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -27,22 +27,21 @@
 Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
 Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
-      [Install](#install) - [CLI version](#cli-version) - [CLI version of
-webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
-Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
-  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
- before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:]
-   (#text-to-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL
-   voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
+ [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
+   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
+Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
+(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
+ remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
+ Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
+[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
 classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
   - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
   search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
 DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
   yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
   images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
   search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
@@ -58,51 +57,34 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
-   internet) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
+opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
+ chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
+webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
    k Text | CLI function to perform a suggestions search using Webscout. | |
  python -m webscout text -k Text | CLI function to perform a text search using
  Webscout. | | python -m webscout translate -k Text | CLI function to perform
    translate using Webscout. | | python -m webscout version | A command-line
    interface command that prints and returns the version of the program. | |
   python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
- specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
- prodia --prompt "car"` | CLI function to generate content related to a prompt
- using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
-      prompt "Your prompt here"` | CLI function to perform a search using
-Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
-      prompt "Your prompt here"` | CLI function to perform a search using
- Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
-  "Your prompt here"` | CLI function to perform a search using Webscout.AI's
-     OPENGPT feature. | ## CLI to use LLM ```python python -m webscout.LLM
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
  model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
 Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
  Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
  for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
  China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
 Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
  gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
@@ -318,50 +300,54 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
- (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-`LLM` ```python from webscout.LLM import LLM # Read the system message from the
-   file with open('system.txt', 'r') as file: system_message = file.read() #
-   Initialize the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
- __future__ import annotations from typing import List, Optional from webscout
-  import LLM from webscout import WEBS import warnings system_message: str =
- ( "As AI, you possess internet access and are capable of executing real-time
-  web searches based on user inputs. " "You shall utilize this capability to
- enrich conversations, offer informed insights, and augment your ability to "
-  "respond accurately and thoroughly. However, refrain from stating 'You have
-  provided a list of strings,' ensuring " "seamless interactions with users.
-Embrace a responsive demeanor, harnessing available online resources to address
- " "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-                  ", response) else: print("No response") ```
+(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
+Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
+sends a simple greeting and prints the response prompt = "tell me about india"
+response_str = a.chat(prompt) print(response_str) ``` ## usage of special .LLM
+file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+                        else: print("No response") ```
```

### Comparing `webscout-1.3.1/webscout.egg-info/SOURCES.txt` & `webscout-1.3.2/webscout.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 webscout/DWEBS.py
 webscout/HelpingAI.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
 webscout/cli.py
 webscout/exceptions.py
+webscout/g4f.py
 webscout/models.py
 webscout/transcriber.py
 webscout/utils.py
 webscout/version.py
 webscout/voice.py
+webscout/webai.py
 webscout/webscout_search.py
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
 webscout.egg-info/entry_points.txt
 webscout.egg-info/requires.txt
```


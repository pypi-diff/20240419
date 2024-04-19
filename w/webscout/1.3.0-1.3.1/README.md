# Comparing `tmp/webscout-1.3.0.tar.gz` & `tmp/webscout-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.0.tar", last modified: Tue Apr 16 06:20:30 2024, max compression
+gzip compressed data, was "webscout-1.3.1.tar", last modified: Fri Apr 19 06:35:35 2024, max compression
```

## Comparing `webscout-1.3.0.tar` & `webscout-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:30.401520 webscout-1.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.274165 webscout-1.3.0/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.316481 webscout-1.3.0/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.398477 webscout-1.3.0/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:28.487584 webscout-1.3.0/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.0/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.0/LICENSE.md
--rw-rw-rw-   0        0        0    28244 2024-04-16 06:20:30.394520 webscout-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    26069 2024-04-16 06:09:35.000000 webscout-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 06:20:30.402520 webscout-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2817 2024-04-16 06:11:02.000000 webscout-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:29.891443 webscout-1.3.0/webscout/
--rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/LLM.py
--rw-rw-rw-   0        0        0      550 2024-04-16 06:01:50.000000 webscout-1.3.0/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.0/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-16 06:11:14.000000 webscout-1.3.0/webscout/version.py
--rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.0/webscout/voice.py
--rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.0/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:20:30.369522 webscout-1.3.0/webscout.egg-info/
--rw-rw-rw-   0        0        0    28244 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2024-04-16 06:20:27.000000 webscout-1.3.0/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 06:20:26.000000 webscout-1.3.0/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.205617 webscout-1.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.749132 webscout-1.3.1/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.771130 webscout-1.3.1/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.804826 webscout-1.3.1/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:34.820831 webscout-1.3.1/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.1/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0    31533 2024-04-19 06:35:35.200620 webscout-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29342 2024-04-19 06:32:44.000000 webscout-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 06:35:35.205617 webscout-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2725 2024-04-19 06:30:17.000000 webscout-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.088616 webscout-1.3.1/webscout/
+-rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-19 06:26:09.000000 webscout-1.3.1/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.1/webscout/LLM.py
+-rw-rw-rw-   0        0        0      572 2024-04-19 06:18:21.000000 webscout-1.3.1/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.1/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-19 06:30:29.000000 webscout-1.3.1/webscout/version.py
+-rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.1/webscout/voice.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.1/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:35:35.188618 webscout-1.3.1/webscout.egg-info/
+-rw-rw-rw-   0        0        0    31533 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2024-04-19 06:35:34.000000 webscout-1.3.1/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 06:35:33.000000 webscout-1.3.1/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.0/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.1/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.1/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.1/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.1/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/networks/network_configs.py` & `webscout-1.3.1/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.1/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/utilsdw/enver.py` & `webscout-1.3.1/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.1/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/LICENSE.md` & `webscout-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/PKG-INFO` & `webscout-1.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,7 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.3.0
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Requires-Dist: orjson
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
-
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
@@ -95,14 +43,15 @@
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
+    - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -700,15 +649,106 @@
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
-def chat(model_name, system_message="You are Jarvis"):# system prompt
-    AI = LLM(model_name, system_message)
-    AI.chat()
+# Read the system message from the file
+with open('system.txt', 'r') as file:
+    system_message = file.read()
 
-if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
-    chat(model_name)
+# Initialize the LLM class with the model name and system message
+llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+
+while True:
+    # Get the user input
+    user_input = input("User: ")
+
+    # Define the messages to be sent
+    messages = [
+        {"role": "user", "content": user_input}
+    ]
+
+    # Use the mistral_chat method to get the response
+    response = llm.chat(messages)
+
+    # Print the response
+    print("AI: ", response)
 ```
+### `LLM` with internet
+```python
+from __future__ import annotations
+from typing import List, Optional
+
+from webscout import LLM
+from webscout import WEBS
+import warnings
+
+system_message: str = (
+    "As AI, you possess internet access and are capable of executing real-time web searches based on user inputs. "
+    "You shall utilize this capability to enrich conversations, offer informed insights, and augment your ability to "
+    "respond accurately and thoroughly. However, refrain from stating 'You have provided a list of strings,' ensuring "
+    "seamless interactions with users. Embrace a responsive demeanor, harnessing available online resources to address "
+    "queries, share pertinent content, and facilitate meaningful exchanges. By doing so, you create value through "
+    "connection and engagement, ultimately enhancing overall user satisfaction and experience. Additionally, "
+    "continue upholding the principles of respect, impartiality, and intellectual integrity throughout all interactions."
+)
+
+# Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+
+
+def chat(
+    user_input: str, webs: WEBS, max_results: int = 10
+) -> Optional[str]:
+    """
+    Chat function to perform a web search based on the user input and generate a response using the LLM model.
+
+    Parameters
+    ----------
+    user_input : str
+        The user input to be used for the web search
+    webs : WEBS
+        The web search instance to be used to perform the search
+    max_results : int, optional
+        The maximum number of search results to include in the response, by default 10
+
+    Returns
+    -------
+    Optional[str]
+        The response generated by the LLM model, or None if there is no response
+    """
+    # Perform a web search based on the user input
+    search_results: List[str] = []
+    for r in webs.text(
+        user_input, region="wt-wt", safesearch="off", timelimit="y", max_results=max_results
+    ):
+        search_results.append(str(r))  # Convert each result to a string
+
+    # Define the messages to be sent, including the user input, search results, and system message
+    messages = [
+        {"role": "user", "content": user_input + "\n" + "websearch results are:" + "\n".join(search_results)},
+    ]
+
+    # Use the chat method to get the response
+    response = LLM.chat(messages)
+
+    return response
+
+
+if __name__ == "__main__":
+    while True:
+        # Get the user input
+        user_input = input("User: ")
+
+        # Perform a web search based on the user input
+        with WEBS() as webs:
+            response = chat(user_input, webs)
+
+        # Print the response
+        if response:
+            print("AI:", response)
+        else:
+            print("No response")
+```
```

#### html2text {}

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.0 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
-now can transcribe yt videos Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
-lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
-Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
       [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
@@ -60,40 +32,40 @@
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
   opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
   special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+ from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
+   internet) ## Install ```python pip install -U webscout ``` ## CLI version
+```python3 python -m webscout --help ``` | Command | Description | |-----------
+--------------------------------|----------------------------------------------
+---------------------------------------------------------| | python -m webscout
+answers -k Text | CLI function to perform an answers search using Webscout. | |
+ python -m webscout images -k Text | CLI function to perform an images search
+using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
+maps search using Webscout. | | python -m webscout news -k Text | CLI function
+ to perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -319,12 +291,49 @@
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
-     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
- system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
-         text generation models on deepinfra.com. chat(model_name) ```
+`LLM` ```python from webscout.LLM import LLM # Read the system message from the
+   file with open('system.txt', 'r') as file: system_message = file.read() #
+   Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+                  ", response) else: print("No response") ```
```

### Comparing `webscout-1.3.0/README.md` & `webscout-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,59 @@
+Metadata-Version: 2.1
+Name: webscout
+Version: 1.3.1
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7
+Requires-Dist: curl_cffi>=0.6.0b7
+Requires-Dist: lxml>=5.1.0
+Requires-Dist: nest-asyncio>=1.6.0
+Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: Helpingai-T2
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: orjson
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
@@ -43,14 +95,15 @@
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
+    - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -648,15 +701,106 @@
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
-def chat(model_name, system_message="You are Jarvis"):# system prompt
-    AI = LLM(model_name, system_message)
-    AI.chat()
+# Read the system message from the file
+with open('system.txt', 'r') as file:
+    system_message = file.read()
+
+# Initialize the LLM class with the model name and system message
+llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+
+while True:
+    # Get the user input
+    user_input = input("User: ")
+
+    # Define the messages to be sent
+    messages = [
+        {"role": "user", "content": user_input}
+    ]
+
+    # Use the mistral_chat method to get the response
+    response = llm.chat(messages)
+
+    # Print the response
+    print("AI: ", response)
+```
+### `LLM` with internet
+```python
+from __future__ import annotations
+from typing import List, Optional
+
+from webscout import LLM
+from webscout import WEBS
+import warnings
+
+system_message: str = (
+    "As AI, you possess internet access and are capable of executing real-time web searches based on user inputs. "
+    "You shall utilize this capability to enrich conversations, offer informed insights, and augment your ability to "
+    "respond accurately and thoroughly. However, refrain from stating 'You have provided a list of strings,' ensuring "
+    "seamless interactions with users. Embrace a responsive demeanor, harnessing available online resources to address "
+    "queries, share pertinent content, and facilitate meaningful exchanges. By doing so, you create value through "
+    "connection and engagement, ultimately enhancing overall user satisfaction and experience. Additionally, "
+    "continue upholding the principles of respect, impartiality, and intellectual integrity throughout all interactions."
+)
+
+# Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+
+
+def chat(
+    user_input: str, webs: WEBS, max_results: int = 10
+) -> Optional[str]:
+    """
+    Chat function to perform a web search based on the user input and generate a response using the LLM model.
+
+    Parameters
+    ----------
+    user_input : str
+        The user input to be used for the web search
+    webs : WEBS
+        The web search instance to be used to perform the search
+    max_results : int, optional
+        The maximum number of search results to include in the response, by default 10
+
+    Returns
+    -------
+    Optional[str]
+        The response generated by the LLM model, or None if there is no response
+    """
+    # Perform a web search based on the user input
+    search_results: List[str] = []
+    for r in webs.text(
+        user_input, region="wt-wt", safesearch="off", timelimit="y", max_results=max_results
+    ):
+        search_results.append(str(r))  # Convert each result to a string
+
+    # Define the messages to be sent, including the user input, search results, and system message
+    messages = [
+        {"role": "user", "content": user_input + "\n" + "websearch results are:" + "\n".join(search_results)},
+    ]
+
+    # Use the chat method to get the response
+    response = LLM.chat(messages)
+
+    return response
+
 
 if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
-    chat(model_name)
+    while True:
+        # Get the user input
+        user_input = input("User: ")
+
+        # Perform a web search based on the user input
+        with WEBS() as webs:
+            response = chat(user_input, webs)
+
+        # Print the response
+        if response:
+            print("AI:", response)
+        else:
+            print("No response")
 ```
```

#### html2text {}

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1 Name: webscout Version: 1.3.1 Summary: Search for words,
+documents, images, videos, news, maps and text translation using the Google,
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
+transcribe yt videos and have TTS support Author: OEvortex Author-email:
+helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
+URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
+Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
+github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
+youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Description-Content-Type: text/
+markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
+lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
+Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
+Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
+Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
+Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
+Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models and now can transcribe yt videos ## Table
 of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
       [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
@@ -32,40 +60,40 @@
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
   opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
   special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+ from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
+   internet) ## Install ```python pip install -U webscout ``` ## CLI version
+```python3 python -m webscout --help ``` | Command | Description | |-----------
+--------------------------------|----------------------------------------------
+---------------------------------------------------------| | python -m webscout
+answers -k Text | CLI function to perform an answers search using Webscout. | |
+ python -m webscout images -k Text | CLI function to perform an images search
+using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
+maps search using Webscout. | | python -m webscout news -k Text | CLI function
+ to perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -291,12 +319,49 @@
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
-     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
- system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
-         text generation models on deepinfra.com. chat(model_name) ```
+`LLM` ```python from webscout.LLM import LLM # Read the system message from the
+   file with open('system.txt', 'r') as file: system_message = file.read() #
+   Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+                  ", response) else: print("No response") ```
```

### Comparing `webscout-1.3.0/setup.py` & `webscout-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from setuptools import setup, find_packages
 
-# version = None
-# with open("webscout/version.py") as version_file:
-#     exec(version_file.read())
-
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.0", 
-    description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos",
+    version="1.3.1", 
+    description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `webscout-1.3.0/webscout/AI.py` & `webscout-1.3.1/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/AIbase.py` & `webscout-1.3.1/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/AIutel.py` & `webscout-1.3.1/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/DWEBS.py` & `webscout-1.3.1/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/HelpingAI.py` & `webscout-1.3.1/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/__init__.py` & `webscout-1.3.1/webscout/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 import logging
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
+from .LLM import LLM
 
 
 __all__ = ["WEBS", "AsyncWEBS", "__version__", "cli"]
 
 logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-1.3.0/webscout/cli.py` & `webscout-1.3.1/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/models.py` & `webscout-1.3.1/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/transcriber.py` & `webscout-1.3.1/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/utils.py` & `webscout-1.3.1/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/voice.py` & `webscout-1.3.1/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/webscout_search.py` & `webscout-1.3.1/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout/webscout_search_async.py` & `webscout-1.3.1/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.0/webscout.egg-info/PKG-INFO` & `webscout-1.3.1/webscout.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.0
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
+Version: 1.3.1
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -95,14 +95,15 @@
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
+    - [`LLM` with internet](#llm-with-internet)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -700,15 +701,106 @@
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
-def chat(model_name, system_message="You are Jarvis"):# system prompt
-    AI = LLM(model_name, system_message)
-    AI.chat()
+# Read the system message from the file
+with open('system.txt', 'r') as file:
+    system_message = file.read()
+
+# Initialize the LLM class with the model name and system message
+llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+
+while True:
+    # Get the user input
+    user_input = input("User: ")
+
+    # Define the messages to be sent
+    messages = [
+        {"role": "user", "content": user_input}
+    ]
+
+    # Use the mistral_chat method to get the response
+    response = llm.chat(messages)
+
+    # Print the response
+    print("AI: ", response)
+```
+### `LLM` with internet
+```python
+from __future__ import annotations
+from typing import List, Optional
+
+from webscout import LLM
+from webscout import WEBS
+import warnings
+
+system_message: str = (
+    "As AI, you possess internet access and are capable of executing real-time web searches based on user inputs. "
+    "You shall utilize this capability to enrich conversations, offer informed insights, and augment your ability to "
+    "respond accurately and thoroughly. However, refrain from stating 'You have provided a list of strings,' ensuring "
+    "seamless interactions with users. Embrace a responsive demeanor, harnessing available online resources to address "
+    "queries, share pertinent content, and facilitate meaningful exchanges. By doing so, you create value through "
+    "connection and engagement, ultimately enhancing overall user satisfaction and experience. Additionally, "
+    "continue upholding the principles of respect, impartiality, and intellectual integrity throughout all interactions."
+)
+
+# Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+
+
+def chat(
+    user_input: str, webs: WEBS, max_results: int = 10
+) -> Optional[str]:
+    """
+    Chat function to perform a web search based on the user input and generate a response using the LLM model.
+
+    Parameters
+    ----------
+    user_input : str
+        The user input to be used for the web search
+    webs : WEBS
+        The web search instance to be used to perform the search
+    max_results : int, optional
+        The maximum number of search results to include in the response, by default 10
+
+    Returns
+    -------
+    Optional[str]
+        The response generated by the LLM model, or None if there is no response
+    """
+    # Perform a web search based on the user input
+    search_results: List[str] = []
+    for r in webs.text(
+        user_input, region="wt-wt", safesearch="off", timelimit="y", max_results=max_results
+    ):
+        search_results.append(str(r))  # Convert each result to a string
+
+    # Define the messages to be sent, including the user input, search results, and system message
+    messages = [
+        {"role": "user", "content": user_input + "\n" + "websearch results are:" + "\n".join(search_results)},
+    ]
+
+    # Use the chat method to get the response
+    response = LLM.chat(messages)
+
+    return response
+
 
 if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
-    chat(model_name)
+    while True:
+        # Get the user input
+        user_input = input("User: ")
+
+        # Perform a web search based on the user input
+        with WEBS() as webs:
+            response = chat(user_input, webs)
+
+        # Print the response
+        if response:
+            print("AI:", response)
+        else:
+            print("No response")
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.0 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.1 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
-now can transcribe yt videos Author: OEvortex Author-email:
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
+transcribe yt videos and have TTS support Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
 youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
@@ -60,40 +60,40 @@
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
   opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
   special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+ from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
+   internet) ## Install ```python pip install -U webscout ``` ## CLI version
+```python3 python -m webscout --help ``` | Command | Description | |-----------
+--------------------------------|----------------------------------------------
+---------------------------------------------------------| | python -m webscout
+answers -k Text | CLI function to perform an answers search using Webscout. | |
+ python -m webscout images -k Text | CLI function to perform an images search
+using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
+maps search using Webscout. | | python -m webscout news -k Text | CLI function
+ to perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -319,12 +319,49 @@
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
-       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
-     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
- system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
-         text generation models on deepinfra.com. chat(model_name) ```
+`LLM` ```python from webscout.LLM import LLM # Read the system message from the
+   file with open('system.txt', 'r') as file: system_message = file.read() #
+   Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+                  ", response) else: print("No response") ```
```

### Comparing `webscout-1.3.0/webscout.egg-info/SOURCES.txt` & `webscout-1.3.1/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*


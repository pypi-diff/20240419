# Comparing `tmp/conva_ai-0.0.3.tar.gz` & `tmp/conva_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.3.tar", last modified: Thu Apr 18 11:52:47 2024, max compression
+gzip compressed data, was "conva_ai-0.0.4.tar", last modified: Fri Apr 19 13:16:30 2024, max compression
```

## Comparing `conva_ai-0.0.3.tar` & `conva_ai-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 11:52:47.332940 conva_ai-0.0.3/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2786 2024-04-18 11:52:47.332639 conva_ai-0.0.3/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2196 2024-04-18 11:51:23.000000 conva_ai-0.0.3/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 11:52:47.330904 conva_ai-0.0.3/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-16 19:28:53.000000 conva_ai-0.0.3/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      760 2024-04-18 11:48:00.000000 conva_ai-0.0.3/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-18 06:03:49.000000 conva_ai-0.0.3/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-18 06:03:49.000000 conva_ai-0.0.3/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 11:52:47.332319 conva_ai-0.0.3/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2786 2024-04-18 11:52:47.000000 conva_ai-0.0.3/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-18 11:52:47.000000 conva_ai-0.0.3/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-18 11:52:47.000000 conva_ai-0.0.3/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-18 11:52:47.000000 conva_ai-0.0.3/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-18 11:52:47.000000 conva_ai-0.0.3/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      607 2024-04-18 11:49:55.000000 conva_ai-0.0.3/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-16 16:45:03.000000 conva_ai-0.0.3/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-18 11:52:47.332999 conva_ai-0.0.3/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.506140 conva_ai-0.0.4/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3269 2024-04-19 13:16:30.505880 conva_ai-0.0.4/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2614 2024-04-19 13:16:17.000000 conva_ai-0.0.4/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.504352 conva_ai-0.0.4/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.4/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:16:17.000000 conva_ai-0.0.4/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.4/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.4/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.505606 conva_ai-0.0.4/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3269 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:16:17.000000 conva_ai-0.0.4/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.4/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:16:30.506205 conva_ai-0.0.4/setup.cfg
```

### Comparing `conva_ai-0.0.3/PKG-INFO` & `conva_ai-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,32 @@
-Metadata-Version: 2.1
-Name: conva_ai
-Version: 0.0.3
-Summary: Python SDK for using Conva AI co-pilots
-Author-email: Slang Labs <support@slanglabs.in>
-Project-URL: Homepage, http://www.slanglabs.in
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: annotated-types==0.6.0
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: pydantic-core==2.18.1
-Requires-Dist: sseclient-py==1.8.0
-Requires-Dist: typing-extensions==4.11.0
-
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
-```
-import asyncio
-from conva_ai.client import AsyncConvaAI
+```import asyncio
+from conva_ai import AsyncConvaAI
 
-async def generate(query: str, stream: bool):
-    client = AsyncConvaAI(
-        copilot_id="<YOUR_COPILOT_ID>", 
-        copilot_version="<YOUR_COPILOT_VERSION>", 
-        api_key="<YOUR_API_KEY>"
+client = AsyncConvaAI(
+        copilot_id="68a17a87a0284d918e8986ab9ad6e4d9", 
+        copilot_version="1.0.2", 
+        api_key="b77ab18ad8324f01baf9a7b11a4c28db",
+        host="http://localhost:8080"
     )
+
+async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
-    out = "" 
+    out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
-        print(out)
     return out
 
-final_response = asyncio.run(generate("how are you", True))
+final_response = asyncio.run(generate(client, "how are you", True))
 print(final_response)
 ```
 
 ### 2. How to clear history
 
 Conva AI client, by default keeps track of your conversation history and uses it as the context for responding intelligently
 
@@ -58,38 +41,54 @@
 )
 client.clear_history()
 ```
 
 In case you are buliding an application where you don't want to track conversation history, you can disable history tracking
 
 ```
-from conva_ai.client import AsyncConvaAI
-client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
-    api_key="<YOUR_API_KEY>"
-)
-client.disable_history(False)
+client.use_history(False)
+```
+
+You can enable history by
+
+```
+client.enable_history(True)
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
 import asyncio
 from conva_ai.client import AsyncConvaAI
 
-async def generate(query: str, stream: bool):
-    client = AsyncConvaAI(
+client = AsyncConvaAI(
         copilot_id="<YOUR_COPILOT_ID>", 
         copilot_version="<YOUR_COPILOT_VERSION>", 
         api_key="<YOUR_API_KEY>"
     )
+
+async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
+    out=""
     async for res in response:
-        out = res.model_dump_json(indent=4)
+        out = res
     return out
 
 final_response = asyncio.run(generate("how are you", True))
 print(final_response.reason)
 ```
+
+### How to use capability groups
+
+Capability Groups are used to control the list of Capabilities that Co pilot will have access. 
+You can make use of the capability group while using the `invoke_capability` method
+
+```
+async def generate(client: AsyncConvaAI, query: str, stream: bool):
+    response = client.client.invoke_capability(query, stream=stream, capability_group="<CAPABILITY_GROUP_NAME>")
+    out=""
+    async for res in response:
+        out = res
+    return out
+```
```

### Comparing `conva_ai-0.0.3/conva_ai/base.py` & `conva_ai-0.0.4/conva_ai/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,12 +15,10 @@
 
     def clear_history(self):
         """
         Clears the history tracked by the client
         """
         self.history: str = ""
 
-    def disable_history(self, use_history: bool):
-        """
-        Disables conversation history tracking by the client
-        """
-        self.keep_conversation_history = use_history
+    def use_history(self, use_history):
+        self.history = use_history
+
```

### Comparing `conva_ai-0.0.3/conva_ai/client.py` & `conva_ai-0.0.4/conva_ai/client.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.3/conva_ai/response.py` & `conva_ai-0.0.4/conva_ai/response.py`

 * *Files identical despite different names*


# Comparing `tmp/conva_ai-0.0.5.tar.gz` & `tmp/conva_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.5.tar", last modified: Fri Apr 19 13:20:55 2024, max compression
+gzip compressed data, was "conva_ai-0.0.6.tar", last modified: Fri Apr 19 13:24:23 2024, max compression
```

## Comparing `conva_ai-0.0.5.tar` & `conva_ai-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.034510 conva_ai-0.0.5/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3266 2024-04-19 13:20:55.034254 conva_ai-0.0.5/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2611 2024-04-19 13:20:27.000000 conva_ai-0.0.5/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.032501 conva_ai-0.0.5/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.5/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.5/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.5/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.5/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.033943 conva_ai-0.0.5/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3266 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:20:27.000000 conva_ai-0.0.5/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.5/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:20:55.034565 conva_ai-0.0.5/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.300703 conva_ai-0.0.6/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3194 2024-04-19 13:24:23.300420 conva_ai-0.0.6/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2539 2024-04-19 13:24:01.000000 conva_ai-0.0.6/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.298929 conva_ai-0.0.6/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.6/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.6/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.6/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.6/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.300104 conva_ai-0.0.6/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3194 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:24:14.000000 conva_ai-0.0.6/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.6/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:24:23.300764 conva_ai-0.0.6/setup.cfg
```

### Comparing `conva_ai-0.0.5/PKG-INFO` & `conva_ai-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,22 +21,19 @@
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```import asyncio
 from conva_ai import AsyncConvaAI
-
 client = AsyncConvaAI(
-        copilot_id="68a17a87a0284d918e8986ab9ad6e4d9", 
-        copilot_version="1.0.2", 
-        api_key="b77ab18ad8324f01baf9a7b11a4c28db",
-        host="http://localhost:8080"
-    )
-
+    copilot_id="<YOUR_COPILOT_ID>", 
+    copilot_version="<YOUR_COPILOT_VERSION>", 
+    api_key="<YOUR_API_KEY>"
+)
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
```

### Comparing `conva_ai-0.0.5/README.md` & `conva_ai-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```import asyncio
 from conva_ai import AsyncConvaAI
-
 client = AsyncConvaAI(
-        copilot_id="68a17a87a0284d918e8986ab9ad6e4d9", 
-        copilot_version="1.0.2", 
-        api_key="b77ab18ad8324f01baf9a7b11a4c28db",
-        host="http://localhost:8080"
-    )
-
+    copilot_id="<YOUR_COPILOT_ID>", 
+    copilot_version="<YOUR_COPILOT_VERSION>", 
+    api_key="<YOUR_API_KEY>"
+)
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
```

### Comparing `conva_ai-0.0.5/conva_ai/base.py` & `conva_ai-0.0.6/conva_ai/base.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.5/conva_ai/client.py` & `conva_ai-0.0.6/conva_ai/client.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.5/conva_ai/response.py` & `conva_ai-0.0.6/conva_ai/response.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.5/conva_ai.egg-info/PKG-INFO` & `conva_ai-0.0.6/conva_ai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,22 +21,19 @@
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```import asyncio
 from conva_ai import AsyncConvaAI
-
 client = AsyncConvaAI(
-        copilot_id="68a17a87a0284d918e8986ab9ad6e4d9", 
-        copilot_version="1.0.2", 
-        api_key="b77ab18ad8324f01baf9a7b11a4c28db",
-        host="http://localhost:8080"
-    )
-
+    copilot_id="<YOUR_COPILOT_ID>", 
+    copilot_version="<YOUR_COPILOT_VERSION>", 
+    api_key="<YOUR_API_KEY>"
+)
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
```

### Comparing `conva_ai-0.0.5/pyproject.toml` & `conva_ai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```


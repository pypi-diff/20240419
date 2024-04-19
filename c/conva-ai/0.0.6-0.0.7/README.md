# Comparing `tmp/conva_ai-0.0.6.tar.gz` & `tmp/conva_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.6.tar", last modified: Fri Apr 19 13:24:23 2024, max compression
+gzip compressed data, was "conva_ai-0.0.7.tar", last modified: Fri Apr 19 13:31:02 2024, max compression
```

## Comparing `conva_ai-0.0.6.tar` & `conva_ai-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.300703 conva_ai-0.0.6/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3194 2024-04-19 13:24:23.300420 conva_ai-0.0.6/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2539 2024-04-19 13:24:01.000000 conva_ai-0.0.6/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.298929 conva_ai-0.0.6/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.6/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.6/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.6/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.6/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:24:23.300104 conva_ai-0.0.6/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3194 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:24:23.000000 conva_ai-0.0.6/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:24:14.000000 conva_ai-0.0.6/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.6/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:24:23.300764 conva_ai-0.0.6/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:31:02.119455 conva_ai-0.0.7/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3195 2024-04-19 13:31:02.119181 conva_ai-0.0.7/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2540 2024-04-19 13:29:41.000000 conva_ai-0.0.7/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:31:02.117782 conva_ai-0.0.7/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.7/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.7/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.7/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.7/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:31:02.118897 conva_ai-0.0.7/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3195 2024-04-19 13:31:02.000000 conva_ai-0.0.7/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:31:02.000000 conva_ai-0.0.7/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:31:02.000000 conva_ai-0.0.7/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:31:02.000000 conva_ai-0.0.7/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:31:02.000000 conva_ai-0.0.7/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:30:55.000000 conva_ai-0.0.7/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.7/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:31:02.119525 conva_ai-0.0.7/setup.cfg
```

### Comparing `conva_ai-0.0.6/PKG-INFO` & `conva_ai-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,16 @@
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
-```import asyncio
+```
+import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
     copilot_id="<YOUR_COPILOT_ID>", 
     copilot_version="<YOUR_COPILOT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
```

### Comparing `conva_ai-0.0.6/README.md` & `conva_ai-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
-```import asyncio
+```
+import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
     copilot_id="<YOUR_COPILOT_ID>", 
     copilot_version="<YOUR_COPILOT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
```

### Comparing `conva_ai-0.0.6/conva_ai/base.py` & `conva_ai-0.0.7/conva_ai/base.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.6/conva_ai/client.py` & `conva_ai-0.0.7/conva_ai/client.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.6/conva_ai/response.py` & `conva_ai-0.0.7/conva_ai/response.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.6/conva_ai.egg-info/PKG-INFO` & `conva_ai-0.0.7/conva_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,16 @@
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
-```import asyncio
+```
+import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
     copilot_id="<YOUR_COPILOT_ID>", 
     copilot_version="<YOUR_COPILOT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
```

### Comparing `conva_ai-0.0.6/pyproject.toml` & `conva_ai-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```


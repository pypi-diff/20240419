# Comparing `tmp/conva_ai-0.0.4.tar.gz` & `tmp/conva_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.4.tar", last modified: Fri Apr 19 13:16:30 2024, max compression
+gzip compressed data, was "conva_ai-0.0.5.tar", last modified: Fri Apr 19 13:20:55 2024, max compression
```

## Comparing `conva_ai-0.0.4.tar` & `conva_ai-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.506140 conva_ai-0.0.4/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3269 2024-04-19 13:16:30.505880 conva_ai-0.0.4/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2614 2024-04-19 13:16:17.000000 conva_ai-0.0.4/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.504352 conva_ai-0.0.4/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.4/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:16:17.000000 conva_ai-0.0.4/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.4/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.4/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:16:30.505606 conva_ai-0.0.4/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3269 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:16:30.000000 conva_ai-0.0.4/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:16:17.000000 conva_ai-0.0.4/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.4/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:16:30.506205 conva_ai-0.0.4/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.034510 conva_ai-0.0.5/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3266 2024-04-19 13:20:55.034254 conva_ai-0.0.5/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2611 2024-04-19 13:20:27.000000 conva_ai-0.0.5/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.032501 conva_ai-0.0.5/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.5/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.5/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.5/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.5/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 13:20:55.033943 conva_ai-0.0.5/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3266 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 13:20:55.000000 conva_ai-0.0.5/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      662 2024-04-19 13:20:27.000000 conva_ai-0.0.5/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.5/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 13:20:55.034565 conva_ai-0.0.5/setup.cfg
```

### Comparing `conva_ai-0.0.4/PKG-INFO` & `conva_ai-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 ```
 client.use_history(False)
 ```
 
 You can enable history by
 
 ```
-client.enable_history(True)
+client.use_history(True)
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
```

### Comparing `conva_ai-0.0.4/README.md` & `conva_ai-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ```
 client.use_history(False)
 ```
 
 You can enable history by
 
 ```
-client.enable_history(True)
+client.use_history(True)
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
```

### Comparing `conva_ai-0.0.4/conva_ai/base.py` & `conva_ai-0.0.5/conva_ai/base.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.4/conva_ai/client.py` & `conva_ai-0.0.5/conva_ai/client.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.4/conva_ai/response.py` & `conva_ai-0.0.5/conva_ai/response.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.0.4/conva_ai.egg-info/PKG-INFO` & `conva_ai-0.0.5/conva_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/conva-omni
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 ```
 client.use_history(False)
 ```
 
 You can enable history by
 
 ```
-client.enable_history(True)
+client.use_history(True)
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
```

### Comparing `conva_ai-0.0.4/pyproject.toml` & `conva_ai-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```


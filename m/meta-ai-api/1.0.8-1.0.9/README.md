# Comparing `tmp/meta_ai_api-1.0.8.tar.gz` & `tmp/meta_ai_api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.8.tar", last modified: Fri Apr 19 01:08:57 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.9.tar", last modified: Fri Apr 19 01:17:52 2024, max compression
```

## Comparing `meta_ai_api-1.0.8.tar` & `meta_ai_api-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:08:57.318445 meta_ai_api-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-04-19 01:08:48.000000 meta_ai_api-1.0.8/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:08:57.314445 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:08:57.000000 meta_ai_api-1.0.8/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.501037 meta_ai_api-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.8/PKG-INFO` & `meta_ai_api-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -33,14 +33,19 @@
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
 
+## Features
+- **Prompt AI**: Send a message to the AI and get a response from Llama 3.
+- **Get Up To Date Information**: Get the latest information from the AI thanks to its connection to the internet.
+- **Get Sources**: Get the sources of the information provided by the AI.
+
 ## Usage
 **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```

### Comparing `meta_ai_api-1.0.8/README.md` & `meta_ai_api-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
 
+## Features
+- **Prompt AI**: Send a message to the AI and get a response from Llama 3.
+- **Get Up To Date Information**: Get the latest information from the AI thanks to its connection to the internet.
+- **Get Sources**: Get the sources of the information provided by the AI.
+
 ## Usage
 **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```

### Comparing `meta_ai_api-1.0.8/setup.py` & `meta_ai_api-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.8/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.9/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -33,14 +33,19 @@
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
 
+## Features
+- **Prompt AI**: Send a message to the AI and get a response from Llama 3.
+- **Get Up To Date Information**: Get the latest information from the AI thanks to its connection to the internet.
+- **Get Sources**: Get the sources of the information provided by the AI.
+
 ## Usage
 **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```


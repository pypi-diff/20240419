# Comparing `tmp/meta_ai_api-1.0.9.tar.gz` & `tmp/meta_ai_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.9.tar", last modified: Fri Apr 19 01:17:52 2024, max compression
+gzip compressed data, was "meta_ai_api-1.1.0.tar", last modified: Fri Apr 19 01:31:22 2024, max compression
```

## Comparing `meta_ai_api-1.0.9.tar` & `meta_ai_api-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.501037 meta_ai_api-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-19 01:17:48.000000 meta_ai_api-1.0.9/src/meta_ai_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:17:52.505037 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:17:52.000000 meta_ai_api-1.0.9/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-19 01:31:15.000000 meta_ai_api-1.1.0/src/meta_ai_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:31:22.629679 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 01:31:22.000000 meta_ai_api-1.1.0/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.9/PKG-INFO` & `meta_ai_api-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.9
+Version: 1.1.0
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
+Requires-Dist: lxml_html_clean
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
```

### Comparing `meta_ai_api-1.0.9/README.md` & `meta_ai_api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.9/setup.py` & `meta_ai_api-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,9 +32,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     extras_require={
         "dev": ["check-manifest"],
     },
-    install_requires=["requests", "requests-html"],
+    install_requires=["requests", "requests-html", "lxml_html_clean"],
 )
```

### Comparing `meta_ai_api-1.0.9/src/meta_ai_api/main.py` & `meta_ai_api-1.1.0/src/meta_ai_api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import urllib
 import uuid
 from typing import Dict, List
 
 import requests
 from requests_html import HTMLSession
 
-from src.meta_ai_api.utils import (
+from meta_ai_api.utils import (
     generate_offline_threading_id,
     extract_value,
     format_response,
 )
 
 
 class MetaAI:
```

### Comparing `meta_ai_api-1.0.9/src/meta_ai_api/utils.py` & `meta_ai_api-1.1.0/src/meta_ai_api/utils.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.9/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.1.0/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.9
+Version: 1.1.0
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
+Requires-Dist: lxml_html_clean
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
```


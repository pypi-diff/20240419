# Comparing `tmp/browserbase_haystack-0.0.1.tar.gz` & `tmp/browserbase_haystack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase_haystack-0.0.1.tar", last modified: Thu Apr 18 18:40:09 2024, max compression
+gzip compressed data, was "browserbase_haystack-0.0.2.tar", last modified: Fri Apr 19 11:20:26 2024, max compression
```

## Comparing `browserbase_haystack-0.0.1.tar` & `browserbase_haystack-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-18 18:40:09.069164 browserbase_haystack-0.0.1/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2165 2024-04-18 18:40:09.069164 browserbase_haystack-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1574 2024-04-18 18:39:19.000000 browserbase_haystack-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-18 18:40:09.065164 browserbase_haystack-0.0.1/browserbase_haystack/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      816 2024-04-18 18:39:19.000000 browserbase_haystack-0.0.1/browserbase_haystack/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-18 18:40:09.069164 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2165 2024-04-18 18:40:09.000000 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      276 2024-04-18 18:40:09.000000 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-18 18:40:09.000000 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2024-04-18 18:40:09.000000 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2024-04-18 18:40:09.000000 browserbase_haystack-0.0.1/browserbase_haystack.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      672 2024-04-18 18:39:19.000000 browserbase_haystack-0.0.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-18 18:40:09.069164 browserbase_haystack-0.0.1/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.443551 browserbase_haystack-0.0.2/
+-rw-r--r--   0 mish       (501) staff       (20)     1063 2024-04-18 21:20:37.000000 browserbase_haystack-0.0.2/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     2191 2024-04-19 11:20:26.443290 browserbase_haystack-0.0.2/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)     1578 2024-04-19 11:13:39.000000 browserbase_haystack-0.0.2/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.442211 browserbase_haystack-0.0.2/browserbase_haystack/
+-rw-r--r--   0 mish       (501) staff       (20)      825 2024-04-19 11:20:09.000000 browserbase_haystack-0.0.2/browserbase_haystack/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.443057 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     2191 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      284 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       24 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       21 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      672 2024-04-19 11:18:27.000000 browserbase_haystack-0.0.2/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-19 11:20:26.443595 browserbase_haystack-0.0.2/setup.cfg
```

### Comparing `browserbase_haystack-0.0.1/PKG-INFO` & `browserbase_haystack-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: browserbase-haystack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Browserbase Haystack Fetcher
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Issues, https://github.com/browserbase/haystack/issues
 Project-URL: Source, https://github.com/browserbase/haystack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: haystack-ai
 Requires-Dist: browserbase
 
 # Browserbase Haystack Fetcher
 
 [Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
 
 ## Installation and setup
 
-- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_KEY`).
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
 pip install browserbase-haystack
 ```
 
 ## Usage
```

### Comparing `browserbase_haystack-0.0.1/README.md` & `browserbase_haystack-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Browserbase Haystack Fetcher
 
 [Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
 
 ## Installation and setup
 
-- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_KEY`).
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
 pip install browserbase-haystack
 ```
 
 ## Usage
```

### Comparing `browserbase_haystack-0.0.1/browserbase_haystack/__init__.py` & `browserbase_haystack-0.0.2/browserbase_haystack/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from haystack import component
 from haystack.dataclasses import Document
 from browserbase import Browserbase
-from typing import List
+from typing import Optional, List, Sequence
 
 
 @component
 class BrowserbaseFetcher:
-    def __init__(self, api_key: str = os.environ["BROWSERBASE_KEY"]) -> None:
+    def __init__(self, api_key: Optional[str] = None) -> None:
         self.browserbase = Browserbase(api_key=api_key)
 
     @component.output_types(documents=List[Document])
-    def run(self, urls: List[str], text_content: bool = False):
+    def run(self, urls: Sequence[str], text_content: bool = False):
         pages = self.browserbase.load_urls(urls, text_content)
 
         documents = []
         for i, page in enumerate(pages):
             documents.append(
                 Document(
                     content=page,
```

### Comparing `browserbase_haystack-0.0.1/browserbase_haystack.egg-info/PKG-INFO` & `browserbase_haystack-0.0.2/browserbase_haystack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: browserbase-haystack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Browserbase Haystack Fetcher
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Issues, https://github.com/browserbase/haystack/issues
 Project-URL: Source, https://github.com/browserbase/haystack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: haystack-ai
 Requires-Dist: browserbase
 
 # Browserbase Haystack Fetcher
 
 [Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
 
 ## Installation and setup
 
-- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_KEY`).
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
 pip install browserbase-haystack
 ```
 
 ## Usage
```

### Comparing `browserbase_haystack-0.0.1/pyproject.toml` & `browserbase_haystack-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase-haystack"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Haystack Fetcher"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```


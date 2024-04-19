# Comparing `tmp/browserbase-0.0.8.tar.gz` & `tmp/browserbase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.0.8.tar", last modified: Tue Apr 16 18:32:11 2024, max compression
+gzip compressed data, was "browserbase-0.0.9.tar", last modified: Fri Apr 19 10:54:26 2024, max compression
```

## Comparing `browserbase-0.0.8.tar` & `browserbase-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.311587 browserbase-0.0.8/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.0.8/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-16 18:32:11.311361 browserbase-0.0.8/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      544 2024-04-15 14:52:48.000000 browserbase-0.0.8/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.309580 browserbase-0.0.8/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)     3217 2024-04-16 18:31:30.000000 browserbase-0.0.8/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.310579 browserbase-0.0.8/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.0.8/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.0.8/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.311081 browserbase-0.0.8/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       19 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      618 2024-04-16 18:31:37.000000 browserbase-0.0.8/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-16 18:32:11.311638 browserbase-0.0.8/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.814656 browserbase-0.0.9/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.0.9/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1524 2024-04-19 10:54:26.814443 browserbase-0.0.9/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      942 2024-04-19 10:53:32.000000 browserbase-0.0.9/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.812392 browserbase-0.0.9/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)     3186 2024-04-18 21:05:58.000000 browserbase-0.0.9/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.813836 browserbase-0.0.9/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.0.9/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.0.9/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.814180 browserbase-0.0.9/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1524 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       19 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      653 2024-04-19 10:54:21.000000 browserbase-0.0.9/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-19 10:54:26.816197 browserbase-0.0.9/setup.cfg
```

### Comparing `browserbase-0.0.8/LICENSE` & `browserbase-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.0.8/PKG-INFO` & `browserbase-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.8
+Version: 0.0.9
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
-Project-URL: Homepage, https://github.com/browserbase/python-sdk
+Project-URL: Homepage, https://browserbase.com
+Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright>=1.43.0
 
 # Browserbase Python SDK
 
-Example usage:
+[Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
+
+## Installation and setup
+
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
+- Install the required dependencies:
 
 ```
-pip install browserbase
+pip install browserbase-haystack
 ```
 
+## Usage
+
 ```py
 from browserbase import Browserbase
 
 # Init the SDK
-browserbase = Browserbase(os.environ["BROWSERBASE_KEY"])
+browserbase = Browserbase(os.environ["BROWSERBASE_API_KEY"])
 
 # Load a webpage
 result = browserbase.load("https://example.com")
 
 # Load multiple webpages (returns iterator)
 result = browserbase.load(["https://example.com"])
```

### Comparing `browserbase-0.0.8/README.md` & `browserbase-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # Browserbase Python SDK
 
-Example usage:
+[Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
+
+## Installation and setup
+
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
+- Install the required dependencies:
 
 ```
-pip install browserbase
+pip install browserbase-haystack
 ```
 
+## Usage
+
 ```py
 from browserbase import Browserbase
 
 # Init the SDK
-browserbase = Browserbase(os.environ["BROWSERBASE_KEY"])
+browserbase = Browserbase(os.environ["BROWSERBASE_API_KEY"])
 
 # Load a webpage
 result = browserbase.load("https://example.com")
 
 # Load multiple webpages (returns iterator)
 result = browserbase.load(["https://example.com"])
```

### Comparing `browserbase-0.0.8/browserbase/__init__.py` & `browserbase-0.0.9/browserbase/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import os
-from typing import List, Union
+from typing import Optional, Sequence, Union
 from playwright.sync_api import sync_playwright
 
 
 class Browserbase:
-    def __init__(self, api_key: str = os.environ["BROWSERBASE_KEY"]):
-        """Create new Browserbase instance"""
-        if not api_key:
-            raise ValueError("Browserbase API key was not provided")
+    def __init__(self, api_key: Optional[str] = None):
+        """Create new Browserbase SDK client instance"""
+        self.api_key = api_key or os.environ["BROWSERBASE_API_KEY"]
 
-        self.api_key = api_key
-
-    def load(self, url: Union[str, List[str]], **args):
+    def load(self, url: Union[str, Sequence[str]], **args):
         if isinstance(url, str):
             return self.load_url(url, **args)
-        elif isinstance(url, list):
+        elif isinstance(url, Sequence):
             return self.load_urls(url, **args)
         else:
-            raise TypeError("Input must be a URL string or a list of URLs")
+            raise TypeError("Input must be a URL string or a Sequence of URLs")
 
     def load_url(self, url: str, text_content: bool = False):
         """Load a page in a headless browser and return the contents"""
         if not url:
             raise ValueError("Page URL was not provided")
 
         with sync_playwright() as p:
@@ -39,15 +36,15 @@
                 }""")
 
                 html = f"{readable['title']}\n{readable['textContent']}"
             browser.close()
 
             return html
 
-    def load_urls(self, urls: List[str], text_content: bool = False):
+    def load_urls(self, urls: Sequence[str], text_content: bool = False):
         """Load multiple pages in a headless browser and return the contents"""
         if not urls:
             raise ValueError("Page URL was not provided")
 
         with sync_playwright() as p:
             browser = p.chromium.connect_over_cdp(
                 "wss://api.browserbase.com?apiKey=" + self.api_key
```

### Comparing `browserbase-0.0.8/browserbase.egg-info/PKG-INFO` & `browserbase-0.0.9/browserbase.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.8
+Version: 0.0.9
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
-Project-URL: Homepage, https://github.com/browserbase/python-sdk
+Project-URL: Homepage, https://browserbase.com
+Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright>=1.43.0
 
 # Browserbase Python SDK
 
-Example usage:
+[Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
+
+## Installation and setup
+
+- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
+- Install the required dependencies:
 
 ```
-pip install browserbase
+pip install browserbase-haystack
 ```
 
+## Usage
+
 ```py
 from browserbase import Browserbase
 
 # Init the SDK
-browserbase = Browserbase(os.environ["BROWSERBASE_KEY"])
+browserbase = Browserbase(os.environ["BROWSERBASE_API_KEY"])
 
 # Load a webpage
 result = browserbase.load("https://example.com")
 
 # Load multiple webpages (returns iterator)
 result = browserbase.load(["https://example.com"])
```

### Comparing `browserbase-0.0.8/pyproject.toml` & `browserbase-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,13 +14,14 @@
 ]
 
 dependencies = [
   "playwright >= 1.43.0"
 ]
 
 [project.urls]
-Homepage = "https://github.com/browserbase/python-sdk"
+Homepage = "https://browserbase.com"
+Source = "https://github.com/browserbase/python-sdk"
 Issues = "https://github.com/browserbase/python-sdk/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```


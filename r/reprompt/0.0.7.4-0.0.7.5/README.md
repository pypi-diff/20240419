# Comparing `tmp/reprompt-0.0.7.4.tar.gz` & `tmp/reprompt-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.4.tar` & `reprompt-0.0.7.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      334 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.pypirc
--rw-r--r--   0        0        0      459 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/LICENSE
--rw-r--r--   0        0        0     7855 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/README.md
--rw-r--r--   0        0        0      634 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/pyproject.toml
--rw-r--r--   0        0        0     1241 2024-04-18 00:06:01.921841 reprompt-0.0.7.4/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      167 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/config.py
--rw-r--r--   0        0        0     3371 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/test_openai_tracing.py
--rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 reprompt-0.0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/LICENSE
+-rw-r--r--   0        0        0     7737 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/README.md
+-rw-r--r--   0        0        0      634 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1241 2024-04-18 23:41:29.063994 reprompt-0.0.7.5/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      167 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/config.py
+-rw-r--r--   0        0        0     3371 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0     9640 1970-01-01 00:00:00.000000 reprompt-0.0.7.5/PKG-INFO
```

### Comparing `reprompt-0.0.7.4/.devcontainer/devcontainer.json` & `reprompt-0.0.7.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.5/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/.gitignore` & `reprompt-0.0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/.pre-commit-config.yaml` & `reprompt-0.0.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/.vscode/settings.json` & `reprompt-0.0.7.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/LICENSE` & `reprompt-0.0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/README.md` & `reprompt-0.0.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 pip install -r requirements.txt
 ```
 
 ## Initialize with API key
 
 To use reprompt, you need to initialize it with an API key. Obtain your API key from the [Reprompt dashboard](https://app.repromptai.com/). Once you have your API key, initialize the reprompt package as follows:
 
-<img width="1286" alt="Screenshot 2024-04-17 at 5 01 07 PM" src="https://github.com/reprompt/reprompt/assets/1288339/afa3dc4f-0cc8-4b46-8a83-a3f19babfa8c">
+![Screenshot 2024-04-17 at 5 01 07 PM](https://github.com/reprompt/reprompt/assets/1288339/afa3dc4f-0cc8-4b46-8a83-a3f19babfa8c)
 
 
 ```
 import reprompt
 reprompt.init(api_key="your_api_key_here")
 ```
 
@@ -42,15 +42,15 @@
 overrides = await get_edits(message)
 ```
 
 ## Add edits
 
 Head over to [Reprompt Dashboard](https://app.repromptai.com/tune) and create a couple edits.
 
-<img width="1423" alt="Screenshot 2024-04-17 at 5 02 26 PM" src="https://github.com/reprompt/reprompt/assets/1288339/85ff3dcc-1f97-4c7d-845f-00d3b49814a8">
+![](https://github.com/reprompt/reprompt/assets/1288339/85ff3dcc-1f97-4c7d-845f-00d3b49814a8)
 
 
 ### Full Integration Example
 
 Here's how you might integrate Reprompt into a specific part of your FastAPI application, focusing on generating responses with OpenAI and using Reprompt for tracing and edits:
 
 
@@ -179,15 +179,15 @@
 
 trace = FunctionTrace("your_function_name", {"arg1": "value1"})
 your_function_to_trace()
 trace.end_trace({"result": "your_function_result"})
 ```
 
 This will automatically collect the traces and upload them.
-<img width="1286" alt="Screenshot 2024-04-17 at 5 01 54 PM" src="https://github.com/reprompt/reprompt/assets/1288339/2eb0f04e-741f-49af-9ef9-b3c130e79248">
+![Screenshot 2024-04-17 at 5 01 54 PM](https://github.com/reprompt/reprompt/assets/1288339/2eb0f04e-741f-49af-9ef9-b3c130e79248)
 
 ### Tracing Example
 
 Here is an example if you are building an AI chain if you're using FastAPI + Weaviate + OpenAI.
 
 ```python
 from fastapi import FastAPI, HTTPException, Request, JSONResponse
```

### Comparing `reprompt-0.0.7.4/docs/Makefile` & `reprompt-0.0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/docs/conf.py` & `reprompt-0.0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/docs/make.bat` & `reprompt-0.0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/docs/pylint.md` & `reprompt-0.0.7.5/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/pyproject.toml` & `reprompt-0.0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/src/reprompt/__init__.py` & `reprompt-0.0.7.5/src/reprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import config
 from .tracing import FunctionTrace, get_edits, write_traces
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.4"
+__version__ = "0.0.7.5"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces", "get_edits"]
 
 
 def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
     if debug:
         logger.setLevel(logging.DEBUG)
```

### Comparing `reprompt-0.0.7.4/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.5/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/src/reprompt/tracing.py` & `reprompt-0.0.7.5/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/tests/conftest.py` & `reprompt-0.0.7.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/tests/test_openai_tracing.py` & `reprompt-0.0.7.5/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.4/PKG-INFO` & `reprompt-0.0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -58,15 +58,15 @@
 pip install -r requirements.txt
 ```
 
 ## Initialize with API key
 
 To use reprompt, you need to initialize it with an API key. Obtain your API key from the [Reprompt dashboard](https://app.repromptai.com/). Once you have your API key, initialize the reprompt package as follows:
 
-<img width="1286" alt="Screenshot 2024-04-17 at 5 01 07 PM" src="https://github.com/reprompt/reprompt/assets/1288339/afa3dc4f-0cc8-4b46-8a83-a3f19babfa8c">
+![Screenshot 2024-04-17 at 5 01 07 PM](https://github.com/reprompt/reprompt/assets/1288339/afa3dc4f-0cc8-4b46-8a83-a3f19babfa8c)
 
 
 ```
 import reprompt
 reprompt.init(api_key="your_api_key_here")
 ```
 
@@ -85,15 +85,15 @@
 overrides = await get_edits(message)
 ```
 
 ## Add edits
 
 Head over to [Reprompt Dashboard](https://app.repromptai.com/tune) and create a couple edits.
 
-<img width="1423" alt="Screenshot 2024-04-17 at 5 02 26 PM" src="https://github.com/reprompt/reprompt/assets/1288339/85ff3dcc-1f97-4c7d-845f-00d3b49814a8">
+![](https://github.com/reprompt/reprompt/assets/1288339/85ff3dcc-1f97-4c7d-845f-00d3b49814a8)
 
 
 ### Full Integration Example
 
 Here's how you might integrate Reprompt into a specific part of your FastAPI application, focusing on generating responses with OpenAI and using Reprompt for tracing and edits:
 
 
@@ -222,15 +222,15 @@
 
 trace = FunctionTrace("your_function_name", {"arg1": "value1"})
 your_function_to_trace()
 trace.end_trace({"result": "your_function_result"})
 ```
 
 This will automatically collect the traces and upload them.
-<img width="1286" alt="Screenshot 2024-04-17 at 5 01 54 PM" src="https://github.com/reprompt/reprompt/assets/1288339/2eb0f04e-741f-49af-9ef9-b3c130e79248">
+![Screenshot 2024-04-17 at 5 01 54 PM](https://github.com/reprompt/reprompt/assets/1288339/2eb0f04e-741f-49af-9ef9-b3c130e79248)
 
 ### Tracing Example
 
 Here is an example if you are building an AI chain if you're using FastAPI + Weaviate + OpenAI.
 
 ```python
 from fastapi import FastAPI, HTTPException, Request, JSONResponse
```


# Comparing `tmp/sysaidmin-0.2.0.tar.gz` & `tmp/sysaidmin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysaidmin-0.2.0.tar", max compression
+gzip compressed data, was "sysaidmin-0.2.1.tar", max compression
```

## Comparing `sysaidmin-0.2.0.tar` & `sysaidmin-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2023-11-26 16:21:34.494437 sysaidmin-0.2.0/LICENSE
--rw-r--r--   0        0        0     2990 2023-12-03 01:35:43.074737 sysaidmin-0.2.0/README.md
--rw-r--r--   0        0        0      598 2023-12-05 00:19:39.728659 sysaidmin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-26 20:32:40.186359 sysaidmin-0.2.0/sysaidmin/__init__.py
--rwxr-xr-x   0        0        0     7407 2023-12-02 17:36:16.137794 sysaidmin-0.2.0/sysaidmin/cli.py
--rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 sysaidmin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-26 16:21:34.494437 sysaidmin-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2990 2023-12-03 01:35:43.074737 sysaidmin-0.2.1/README.md
+-rw-r--r--   0        0        0      621 2024-04-19 16:17:18.981670 sysaidmin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-26 20:32:40.186359 sysaidmin-0.2.1/sysaidmin/__init__.py
+-rwxr-xr-x   0        0        0     7533 2023-12-08 03:11:51.797479 sysaidmin-0.2.1/sysaidmin/cli.py
+-rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 sysaidmin-0.2.1/PKG-INFO
```

### Comparing `sysaidmin-0.2.0/LICENSE` & `sysaidmin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysaidmin-0.2.0/README.md` & `sysaidmin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sysaidmin-0.2.0/pyproject.toml` & `sysaidmin-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "sysaidmin"
-version = "0.2.0"
+version = "0.2.1"
 description = "A GPT-powered sysadmin."
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 repository = "https://github.com/skorokithakis/sysaidmin/"
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 sysaidmin = "sysaidmin.cli:cli"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1"
+python = ">=3.8.1"
 openai = "^1.3.5"
+setuptools = "^69.5.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sysaidmin-0.2.0/sysaidmin/cli.py` & `sysaidmin-0.2.1/sysaidmin/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     VERSION = "0.0.0"
 
 
 class Assistant:
     def __init__(self, model: str) -> None:
         self._client = openai.OpenAI()
         self._assistant = self._client.beta.assistants.create(
+            name="Sysaidmin",
             instructions=(
                 "You are a helpful system administrator. You are helping to debug Unix "
                 "issues the user is facing by using their terminal. You run commands "
                 "on your own, rather than asking the user to run them."
             ),
             model=model,
             tools=[
@@ -107,15 +108,16 @@
         # Let's see what we got.
         response = command = None
         if self._last_run.status == "requires_action":  # type: ignore[attr-defined]
             function = self._last_run.required_action.submit_tool_outputs.tool_calls[  # type: ignore[attr-defined]
                 0
             ].function
             if function.name == "end_session":
-                # The AI wants to end the session.
+                # The AI wants to end the session, clean up the assistant.
+                self._client.beta.assistants.delete(self._assistant.id)
                 return None
             else:
                 command = json.loads(function.arguments)["command"]
         elif self._last_run.status == "completed":  # type: ignore[attr-defined]
             thread_messages = self._client.beta.threads.messages.list(
                 self._thread.id, limit=4
             )
```

### Comparing `sysaidmin-0.2.0/PKG-INFO` & `sysaidmin-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sysaidmin
-Version: 0.2.0
+Version: 0.2.1
 Summary: A GPT-powered sysadmin.
 Home-page: https://github.com/skorokithakis/sysaidmin/
 License: AGPL-3.0-or-later
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.3.5,<2.0.0)
+Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Project-URL: Repository, https://github.com/skorokithakis/sysaidmin/
 Description-Content-Type: text/markdown
 
 # Sysaidmin
 
 Sysaidmin is a GPT-powered sysadmin for your machine. You can ask it to solve a problem,
 and it will run commands on your system (with your permission) to debug what's going on.
```


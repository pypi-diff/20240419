# Comparing `tmp/agentrun-0.2.2.tar.gz` & `tmp/agentrun-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentrun-0.2.2.tar", last modified: Wed Apr 17 02:59:39 2024, max compression
+gzip compressed data, was "agentrun-0.2.3.tar", last modified: Fri Apr 19 20:36:12 2024, max compression
```

## Comparing `agentrun-0.2.2.tar` & `agentrun-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:39.792084 agentrun-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-17 02:59:33.000000 agentrun-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15679 2024-04-17 02:59:39.792084 agentrun-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-17 02:59:33.000000 agentrun-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:39.792084 agentrun-0.2.2/agentrun/
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-17 02:59:33.000000 agentrun-0.2.2/agentrun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:39.792084 agentrun-0.2.2/agentrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15679 2024-04-17 02:59:39.000000 agentrun-0.2.2/agentrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 02:59:39.000000 agentrun-0.2.2/agentrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:59:39.000000 agentrun-0.2.2/agentrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 02:59:39.000000 agentrun-0.2.2/agentrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 02:59:39.000000 agentrun-0.2.2/agentrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-17 02:59:33.000000 agentrun-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:59:39.792084 agentrun-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:39.792084 agentrun-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-17 02:59:33.000000 agentrun-0.2.2/tests/test_agentrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:36:12.180093 agentrun-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-19 20:36:03.000000 agentrun-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-04-19 20:36:12.180093 agentrun-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-19 20:36:03.000000 agentrun-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:36:12.176093 agentrun-0.2.3/agentrun/
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-19 20:36:03.000000 agentrun-0.2.3/agentrun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:36:12.180093 agentrun-0.2.3/agentrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-04-19 20:36:12.000000 agentrun-0.2.3/agentrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 20:36:12.000000 agentrun-0.2.3/agentrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:36:12.000000 agentrun-0.2.3/agentrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 20:36:12.000000 agentrun-0.2.3/agentrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 20:36:12.000000 agentrun-0.2.3/agentrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 20:36:03.000000 agentrun-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:36:12.180093 agentrun-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:36:12.180093 agentrun-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-19 20:36:03.000000 agentrun-0.2.3/tests/test_agentrun.py
```

### Comparing `agentrun-0.2.2/LICENSE` & `agentrun-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentrun-0.2.2/PKG-INFO` & `agentrun-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentrun
-Version: 0.2.2
+Version: 0.2.3
 Summary: The easiest way to run AI or user generated python code safely in a docker container
 Author-email: Jonathan Adly <gadly0123@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jonathan-adly/agentrun
 Project-URL: Changelog, https://github.com/jonathan-adly/agentrun/releases
 Project-URL: Issues, https://github.com/jonathan-adly/agentrun/issues
 Project-URL: CI, https://github.com/jonathan-adly/agentrun/actions
@@ -28,22 +28,22 @@
 
 [![PyPI](https://img.shields.io/pypi/v/agentrun.svg)](https://pypi.org/project/agentrun/)
 [![Tests](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/jonathan-adly/agentrun?include_prereleases&label=changelog)](https://github.com/jonathan-adly/agentrun/releases)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/agentrun)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FJonathan-Adly%2FAgentRun%2Fdevelop%2Fpyproject.toml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/jonathan-adly/agentrun/blob/main/LICENSE)
-[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/agentrun-docs/)
+[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/AgentRun/)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Jonathan_Adly_?style=social)](https://twitter.com/Jonathan_Adly_)
 
 AgentRun is a Python library that makes it easy to run Python code safely from large language models (LLMs) with a single line of code. Built on top of the Docker Python SDK and RestrictedPython, it provides a simple, transparent, and user-friendly API to manage isolated code execution.
 
 AgentRun automatically installs and uninstalls dependencies with optional caching, limits resource consumption, checks code safety, and sets execution timeouts. It has 97% test coverage with full static typing and only two dependencies.
 
-- [Documentation](https://jonathan-adly.github.io/agentrun-docs/)
+- [Documentation](https://jonathan-adly.github.io/AgentRun/)
 
 - [Get started in minutes](#getting-started)
 
 ## Why?
 
 Giving code execution ability to LLMs is a massive upgrade. Consider the following user query: `what is 12345 * 54321?` or even something more ambitious like `what is the average daily move of Apple stock during the last week?`? With code execution it is possible for LLMs to answer both accurately by executing code.
```

### Comparing `agentrun-0.2.2/README.md` & `agentrun-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 [![PyPI](https://img.shields.io/pypi/v/agentrun.svg)](https://pypi.org/project/agentrun/)
 [![Tests](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/jonathan-adly/agentrun?include_prereleases&label=changelog)](https://github.com/jonathan-adly/agentrun/releases)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/agentrun)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FJonathan-Adly%2FAgentRun%2Fdevelop%2Fpyproject.toml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/jonathan-adly/agentrun/blob/main/LICENSE)
-[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/agentrun-docs/)
+[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/AgentRun/)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Jonathan_Adly_?style=social)](https://twitter.com/Jonathan_Adly_)
 
 AgentRun is a Python library that makes it easy to run Python code safely from large language models (LLMs) with a single line of code. Built on top of the Docker Python SDK and RestrictedPython, it provides a simple, transparent, and user-friendly API to manage isolated code execution.
 
 AgentRun automatically installs and uninstalls dependencies with optional caching, limits resource consumption, checks code safety, and sets execution timeouts. It has 97% test coverage with full static typing and only two dependencies.
 
-- [Documentation](https://jonathan-adly.github.io/agentrun-docs/)
+- [Documentation](https://jonathan-adly.github.io/AgentRun/)
 
 - [Get started in minutes](#getting-started)
 
 ## Why?
 
 Giving code execution ability to LLMs is a massive upgrade. Consider the following user query: `what is 12345 * 54321?` or even something more ambitious like `what is the average daily move of Apple stock during the last week?`? With code execution it is possible for LLMs to answer both accurately by executing code.
```

### Comparing `agentrun-0.2.2/agentrun/__init__.py` & `agentrun-0.2.3/agentrun/__init__.py`

 * *Files identical despite different names*

### Comparing `agentrun-0.2.2/agentrun.egg-info/PKG-INFO` & `agentrun-0.2.3/agentrun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentrun
-Version: 0.2.2
+Version: 0.2.3
 Summary: The easiest way to run AI or user generated python code safely in a docker container
 Author-email: Jonathan Adly <gadly0123@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jonathan-adly/agentrun
 Project-URL: Changelog, https://github.com/jonathan-adly/agentrun/releases
 Project-URL: Issues, https://github.com/jonathan-adly/agentrun/issues
 Project-URL: CI, https://github.com/jonathan-adly/agentrun/actions
@@ -28,22 +28,22 @@
 
 [![PyPI](https://img.shields.io/pypi/v/agentrun.svg)](https://pypi.org/project/agentrun/)
 [![Tests](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-adly/agentrun/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/jonathan-adly/agentrun?include_prereleases&label=changelog)](https://github.com/jonathan-adly/agentrun/releases)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/agentrun)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FJonathan-Adly%2FAgentRun%2Fdevelop%2Fpyproject.toml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/jonathan-adly/agentrun/blob/main/LICENSE)
-[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/agentrun-docs/)
+[![MkDocs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=fff)](https://jonathan-adly.github.io/AgentRun/)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Jonathan_Adly_?style=social)](https://twitter.com/Jonathan_Adly_)
 
 AgentRun is a Python library that makes it easy to run Python code safely from large language models (LLMs) with a single line of code. Built on top of the Docker Python SDK and RestrictedPython, it provides a simple, transparent, and user-friendly API to manage isolated code execution.
 
 AgentRun automatically installs and uninstalls dependencies with optional caching, limits resource consumption, checks code safety, and sets execution timeouts. It has 97% test coverage with full static typing and only two dependencies.
 
-- [Documentation](https://jonathan-adly.github.io/agentrun-docs/)
+- [Documentation](https://jonathan-adly.github.io/AgentRun/)
 
 - [Get started in minutes](#getting-started)
 
 ## Why?
 
 Giving code execution ability to LLMs is a massive upgrade. Consider the following user query: `what is 12345 * 54321?` or even something more ambitious like `what is the average daily move of Apple stock during the last week?`? With code execution it is possible for LLMs to answer both accurately by executing code.
```

### Comparing `agentrun-0.2.2/pyproject.toml` & `agentrun-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "agentrun"
-version = "0.2.2"
+version = "0.2.3"
 description = "The easiest way to run AI or user generated python code safely in a docker container"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Jonathan Adly", email = "gadly0123@gmail.com"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `agentrun-0.2.2/tests/test_agentrun.py` & `agentrun-0.2.3/tests/test_agentrun.py`

 * *Files identical despite different names*


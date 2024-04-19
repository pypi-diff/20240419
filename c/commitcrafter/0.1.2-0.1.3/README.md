# Comparing `tmp/commitcrafter-0.1.2.tar.gz` & `tmp/commitcrafter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcrafter-0.1.2.tar", max compression
+gzip compressed data, was "commitcrafter-0.1.3.tar", max compression
```

## Comparing `commitcrafter-0.1.2.tar` & `commitcrafter-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.2/commitcrafter/__init__.py
--rw-r--r--   0        0        0      611 2024-04-19 14:07:25.263294 commitcrafter-0.1.2/commitcrafter/cli.py
--rw-r--r--   0        0        0      544 2024-04-19 14:04:56.564239 commitcrafter-0.1.2/commitcrafter/git_tools.py
--rw-r--r--   0        0        0     1104 2024-04-19 14:04:56.564241 commitcrafter-0.1.2/commitcrafter/gpt_integration.py
--rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.2/commitcrafter/prompt.txt
--rw-r--r--   0        0        0      427 2024-04-19 14:07:48.804228 commitcrafter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 commitcrafter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.3/commitcrafter/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-19 15:11:09.409768 commitcrafter-0.1.3/commitcrafter/cli.py
+-rw-r--r--   0        0        0     1747 2024-04-19 15:10:31.464108 commitcrafter-0.1.3/commitcrafter/commitcrafter.py
+-rw-r--r--   0        0        0       42 2024-04-19 14:52:43.909465 commitcrafter-0.1.3/commitcrafter/exceptions.py
+-rw-r--r--   0        0        0      544 2024-04-19 14:23:56.857977 commitcrafter-0.1.3/commitcrafter/git_tools.py
+-rw-r--r--   0        0        0     1010 2024-04-19 14:55:53.329167 commitcrafter-0.1.3/commitcrafter/gpt_integration.py
+-rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.3/commitcrafter/prompt.txt
+-rw-r--r--   0        0        0      444 2024-04-19 15:12:14.838943 commitcrafter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 commitcrafter-0.1.3/PKG-INFO
```

### Comparing `commitcrafter-0.1.2/commitcrafter/git_tools.py` & `commitcrafter-0.1.3/commitcrafter/git_tools.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.2/commitcrafter/gpt_integration.py` & `commitcrafter-0.1.3/commitcrafter/gpt_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 from openai import OpenAI
 
 
 def get_openai_client() -> OpenAI:
     """Get an OpenAI client with the API key from the environment variables."""
     api_key = os.getenv("COMMITCRAFT_OPENAI_API_KEY")
     if not api_key:
-        raise ValueError(
-            "OpenAI API key not set.-> export COMMITCRAFT_OPENAI_API_KEY=<your_api_key>"
-            " or add it to you shell profile."
-        )
+        raise ValueError("OpenAI API key not found in environment variables")
     return OpenAI(api_key=api_key)
 
 
 def generate_commit_names_using_chat(diff):
     """Generate commit names using the chat endpoint of the OpenAI API."""
     prompts_path = os.path.join(os.path.dirname(__file__), "prompt.txt")
```

### Comparing `commitcrafter-0.1.2/commitcrafter/prompt.txt` & `commitcrafter-0.1.3/commitcrafter/prompt.txt`

 * *Files identical despite different names*


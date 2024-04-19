# Comparing `tmp/good-gpt-0.1.0.tar.gz` & `tmp/good-gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "good-gpt-0.1.0.tar", last modified: Thu Mar  7 11:29:10 2024, max compression
+gzip compressed data, was "good-gpt-0.1.1.tar", last modified: Fri Apr 19 19:36:37 2024, max compression
```

## Comparing `good-gpt-0.1.0.tar` & `good-gpt-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 11:29:10.022779 good-gpt-0.1.0/
--rw-rw-rw-   0        0        0     4533 2024-03-07 11:29:10.020774 good-gpt-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-07 11:29:09.935565 good-gpt-0.1.0/good_gpt/
--rw-rw-rw-   0        0        0        0 2024-03-05 11:12:07.000000 good-gpt-0.1.0/good_gpt/__init__.py
--rw-rw-rw-   0        0        0     6145 2024-03-07 10:31:16.000000 good-gpt-0.1.0/good_gpt/good_gpt.py
--rw-rw-rw-   0        0        0     2002 2024-03-07 10:27:48.000000 good-gpt-0.1.0/good_gpt/post_install.py
-drwxrwxrwx   0        0        0        0 2024-03-07 11:29:10.013391 good-gpt-0.1.0/good_gpt.egg-info/
--rw-rw-rw-   0        0        0     4533 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-07 11:29:09.000000 good-gpt-0.1.0/good_gpt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-07 11:29:10.017778 good-gpt-0.1.0/scripts/
--rw-rw-rw-   0        0        0       45 2024-03-05 11:17:42.000000 good-gpt-0.1.0/scripts/gg
--rw-rw-rw-   0        0        0       42 2024-03-07 11:29:10.023780 good-gpt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1558 2024-03-07 11:28:16.000000 good-gpt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:36:37.055326 good-gpt-0.1.1/
+-rw-rw-rw-   0        0        0     4550 2024-04-19 19:36:37.052319 good-gpt-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 19:36:37.006324 good-gpt-0.1.1/good_gpt/
+-rw-rw-rw-   0        0        0        0 2024-03-05 11:12:07.000000 good-gpt-0.1.1/good_gpt/__init__.py
+-rw-rw-rw-   0        0        0     6761 2024-04-19 19:32:58.000000 good-gpt-0.1.1/good_gpt/good_gpt.py
+-rw-rw-rw-   0        0        0     2002 2024-03-07 10:27:48.000000 good-gpt-0.1.1/good_gpt/post_install.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:36:37.042337 good-gpt-0.1.1/good_gpt.egg-info/
+-rw-rw-rw-   0        0        0     4550 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 19:36:36.000000 good-gpt-0.1.1/good_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 19:36:37.049320 good-gpt-0.1.1/scripts/
+-rw-rw-rw-   0        0        0       45 2024-03-05 11:17:42.000000 good-gpt-0.1.1/scripts/gg
+-rw-rw-rw-   0        0        0       42 2024-04-19 19:36:37.055326 good-gpt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1896 2024-04-19 19:34:36.000000 good-gpt-0.1.1/setup.py
```

### Comparing `good-gpt-0.1.0/PKG-INFO` & `good-gpt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: good-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI command line assistant. Describe a command and get the output.
 Home-page: https://github.com/emilamaj/good-gpt
 Author: Emile Amajar
 License: MIT
 Keywords: ai assistant openai gpt command-line terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,17 @@
 pip install good-gpt
 ```
 or if you have multiple python installations:
 ```bash
 pip3 install good-gpt
 ```
 
-This will install the package, but you may not yet have the `gg` command available in your terminal. For that, you need to add the installation location to your PATH environment variable.
+This will install the package, but you may not yet have the `gg` command available in your terminal at this point.
+
+For that, you need to add the installation location to your PATH environment variable.
 The installation location by default is `%APPDATA%\Python\Python3XX\Scripts\Lib\site-packages\good_gpt` on Windows and `$HOME/.local/lib/python3.XX/site-packages/good_gpt/` on linux.
 
 If PATH is not correctly set, you need to run the `post_install.py` script to add the installation location to your PATH.
 
 For that, find the location of the `post_install.py` script using the following command:
 ```bash
 pip show good-gpt
```

### Comparing `good-gpt-0.1.0/good_gpt/good_gpt.py` & `good-gpt-0.1.1/good_gpt/good_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 import sys
 import os
 import requests
 import json
 import pathlib
+import re
 
 def get_response(
     user_access_token,
     message_thread,
     maxTokens=256,
     temperature=1.0,
     frequencyPenalty=0,
@@ -85,14 +86,29 @@
             thread.append({"role": "assistant", "content": message_content})
         elif thread[-1]["role"] == "assistant":
             thread.append({"role": "user", "content": message_content})
         else:
             raise ValueError("Invalid role in message thread")
     return thread
 
+def filter_output(output_str):
+    """
+    Filters the output string. For example, code is often enclosed in triple quotes:
+    ```programming_language
+    some command to execute
+    ```
+    """
+    # Regex to grab the command from the code block
+    # Make sure to discard the language part of the code block
+    output_str = output_str.strip()
+    if "```" in output_str:
+        output_str = re.sub(r"```.*\n", "", output_str)
+        output_str = output_str.replace("```", "")
+    return output_str
+
 def main():
     """
     Main function to run the shell command assistant.
     """
     # Read OpenAI API key from file. First line of file should contain the raw API key.
     package_directory = pathlib.Path(__file__).parent.absolute()
     env_path = package_directory / "openai_api_key.env"
@@ -136,14 +152,17 @@
     # Send the command to the assistant
     system_message = "You are a shell command assistant. A desired command is specified using natural language. You provide directly a corresponding single-line command, raw, without any additional explanation."
     system_message += "# USER_SYSTEM_PLATFORM: " + sys.platform
     thread = thread_add_message(system_message)
     thread = thread_add_message(user_command, thread)
     suggested_command = get_response(user_access_token, thread)
 
+    # Filter the output
+    suggested_command = filter_output(suggested_command)
+
     print(f"Do you want to execute this suggested command for {sys.platform}? [y/n]")
     print(f"--> {suggested_command}")
 
     try:
         choice = input().lower()
     except (EOFError, KeyboardInterrupt):
         choice = "n"
```

### Comparing `good-gpt-0.1.0/good_gpt/post_install.py` & `good-gpt-0.1.1/good_gpt/post_install.py`

 * *Files identical despite different names*

### Comparing `good-gpt-0.1.0/good_gpt.egg-info/PKG-INFO` & `good-gpt-0.1.1/good_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: good-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI command line assistant. Describe a command and get the output.
 Home-page: https://github.com/emilamaj/good-gpt
 Author: Emile Amajar
 License: MIT
 Keywords: ai assistant openai gpt command-line terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,17 @@
 pip install good-gpt
 ```
 or if you have multiple python installations:
 ```bash
 pip3 install good-gpt
 ```
 
-This will install the package, but you may not yet have the `gg` command available in your terminal. For that, you need to add the installation location to your PATH environment variable.
+This will install the package, but you may not yet have the `gg` command available in your terminal at this point.
+
+For that, you need to add the installation location to your PATH environment variable.
 The installation location by default is `%APPDATA%\Python\Python3XX\Scripts\Lib\site-packages\good_gpt` on Windows and `$HOME/.local/lib/python3.XX/site-packages/good_gpt/` on linux.
 
 If PATH is not correctly set, you need to run the `post_install.py` script to add the installation location to your PATH.
 
 For that, find the location of the `post_install.py` script using the following command:
 ```bash
 pip show good-gpt
```


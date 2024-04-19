# Comparing `tmp/cli-FSD-0.75.tar.gz` & `tmp/cli-FSD-0.9.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-FSD-0.75.tar", last modified: Sat Mar  2 16:57:04 2024, max compression
+gzip compressed data, was "cli-FSD-0.9.43.tar", last modified: Fri Apr 19 17:23:07 2024, max compression
```

## Comparing `cli-FSD-0.75.tar` & `cli-FSD-0.9.43.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0 icarus    (1000) icarus    (1000)        0 2024-03-02 16:57:04.431192 cli-FSD-0.75/
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)    35149 2024-03-02 16:43:07.000000 cli-FSD-0.75/LICENSE
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)     4417 2024-03-02 16:57:04.429192 cli-FSD-0.75/PKG-INFO
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)     3980 2024-03-02 16:43:07.000000 cli-FSD-0.75/README.md
-drwxrwxrwx   0 icarus    (1000) icarus    (1000)        0 2024-03-02 16:57:04.307191 cli-FSD-0.75/cli_FSD/
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)      694 2024-03-02 16:44:41.000000 cli-FSD-0.75/cli_FSD/__init__.py
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)     5806 2024-03-02 16:43:07.000000 cli-FSD-0.75/cli_FSD/engine.py
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)    41629 2024-03-02 16:52:42.000000 cli-FSD-0.75/cli_FSD/main.py
-drwxrwxrwx   0 icarus    (1000) icarus    (1000)        0 2024-03-02 16:57:04.414195 cli-FSD-0.75/cli_FSD/resources/
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)        0 2024-03-02 16:44:24.000000 cli-FSD-0.75/cli_FSD/resources/__init__.py
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)     5674 2024-03-02 16:53:39.000000 cli-FSD-0.75/cli_FSD/resources/assembler.py
-drwxrwxrwx   0 icarus    (1000) icarus    (1000)        0 2024-03-02 16:57:04.383192 cli-FSD-0.75/cli_FSD.egg-info/
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)     4417 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/PKG-INFO
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)      329 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/SOURCES.txt
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)        1 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/dependency_links.txt
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)       40 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/entry_points.txt
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)       45 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/requires.txt
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)        8 2024-03-02 16:57:04.000000 cli-FSD-0.75/cli_FSD.egg-info/top_level.txt
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)       38 2024-03-02 16:57:04.432193 cli-FSD-0.75/setup.cfg
--rwxrwxrwx   0 icarus    (1000) icarus    (1000)      827 2024-03-02 16:48:08.000000 cli-FSD-0.75/setup.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.327409 cli-FSD-0.9.43/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-0.9.43/LICENSE
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5148 2024-04-19 17:23:07.324409 cli-FSD-0.9.43/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-0.9.43/README.md
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:06.971381 cli-FSD-0.9.43/cli_FSD/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/engine.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-0.9.43/cli_FSD/main.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.202726 cli-FSD-0.9.43/cli_FSD/resources/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/resources/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/resources/assembler.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-0.9.43/cli_FSD/resources/test-ollama.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.119704 cli-FSD-0.9.43/cli_FSD.egg-info/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5148 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      362 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/SOURCES.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/dependency_links.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/entry_points.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       47 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/requires.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/top_level.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-19 17:23:07.328410 cli-FSD-0.9.43/setup.cfg
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      831 2024-04-19 17:20:07.000000 cli-FSD-0.9.43/setup.py
```

### Comparing `cli-FSD-0.75/LICENSE` & `cli-FSD-0.9.43/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.75/PKG-INFO` & `cli-FSD-0.9.43/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-Metadata-Version: 2.1
-Name: cli-FSD
-Version: 0.75
-Summary: LLM-enabled companion utility for your terminal.
-Home-page: https://github.com/wazacraft/cli-FSD
-Author: JG
-Author-email: wazacraftRFID@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cli-FSD
 Natural language interface for your command line. 
 
-A lightweight and portable autopilot utility for CLI tasks. Takes natural language as input and uses the OpenAI API to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or make script modules and microservices on the fly. 
+A lightweight and portable autopilot utility for CLI tasks that takes natural language as input and uses the LLM of your choice to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or script modules and microservices on the fly. 
 
 **Warning**: Giving LLMs shell-level access to your computer is dangerous and should only be done in sandbox or otherwise expendable environments.
 
 ##### I made cli-FSD for experimenting and problem solving in low stakes development environments. If you don't have access to a machine like that you can try it below: 
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.10 or later (may work with earlier versions)
 - pip 24.0 or later 
-- An OpenAI API key
+- An OpenAI API key **or** Anthropic API key **or** Ollama running in the same environment as cli-FSD
 
 ### Installation
 
 0. **Pre-requisites:**
    
 - Upgrade pip
 
@@ -104,21 +90,31 @@
 If you don't want to run it locally:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 
 ## Project Progress
-### To Do
+v0.94
+- [x] - Added support for [Ollama]([url](https://github.com/ollama/ollama)) (use -o to run cli-FSD using any supported local LLM model)
+- [x] - support for script custom gpt-4-turbo assistant OpenAI's Assistants API to revie
+v0.87
+- [x] - finish OpenAI Assistants integration (done but but needs to be made accessible in main.py)
+- [x] - integrate other LLM providers with http request APIs similar to /v1/completions (pass -c with your query to use Anthropic API's Claude 3 Opus)
+- [x] - improved error handling 
+
+v0.75
+- [x] - overhauled and refactored error resolution function to address a bug that sometimes prevented the resolution from executing
+- [x] - fixed niche text handling errors and submodule implementation for upcoming OpenAI AssistantsAPI integration
+v0.52
 - [x] - implement LLM error handling and resolution flows 
 - [x] - refactor flags for SafeMode, Autopilot
-- [ ] - implement restricted commands parser
-- [ ] - refactor and expand CMD module. 
-- [ ] - finish OpenAI Assistants integration
-- [ ] - integrate other LLM providers with http request APIs similar to /v1/completions
+
+### To Do
+- [ ] - refactor and expand CMD module 
 - [ ] - build advanced menu and config options
 
 ## Considering
 - [ ] - passive error detection and resolution for CLI interactions
 - [ ] - voice control
    - [ ] - voice notation
 - [ ] - automation schedules and background states
```

### Comparing `cli-FSD-0.75/README.md` & `cli-FSD-0.9.43/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+Metadata-Version: 2.1
+Name: cli-FSD
+Version: 0.9.43
+Summary: LLM-enabled companion utility for your terminal.
+Home-page: https://github.com/wazacraft/cli-FSD
+Author: JG
+Author-email: wazacraftRFID@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cli-FSD
 Natural language interface for your command line. 
 
-A lightweight and portable autopilot utility for CLI tasks. Takes natural language as input and uses the OpenAI API to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or make script modules and microservices on the fly. 
+A lightweight and portable autopilot utility for CLI tasks that takes natural language as input and uses the LLM of your choice to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or script modules and microservices on the fly. 
 
 **Warning**: Giving LLMs shell-level access to your computer is dangerous and should only be done in sandbox or otherwise expendable environments.
 
 ##### I made cli-FSD for experimenting and problem solving in low stakes development environments. If you don't have access to a machine like that you can try it below: 
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.10 or later (may work with earlier versions)
 - pip 24.0 or later 
-- An OpenAI API key
+- An OpenAI API key **or** Anthropic API key **or** Ollama running in the same environment as cli-FSD
 
 ### Installation
 
 0. **Pre-requisites:**
    
 - Upgrade pip
 
@@ -90,21 +106,31 @@
 If you don't want to run it locally:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 
 ## Project Progress
-### To Do
+v0.94
+- [x] - Added support for [Ollama]([url](https://github.com/ollama/ollama)) (use -o to run cli-FSD using any supported local LLM model)
+- [x] - support for script custom gpt-4-turbo assistant OpenAI's Assistants API to revie
+v0.87
+- [x] - finish OpenAI Assistants integration (done but but needs to be made accessible in main.py)
+- [x] - integrate other LLM providers with http request APIs similar to /v1/completions (pass -c with your query to use Anthropic API's Claude 3 Opus)
+- [x] - improved error handling 
+
+v0.75
+- [x] - overhauled and refactored error resolution function to address a bug that sometimes prevented the resolution from executing
+- [x] - fixed niche text handling errors and submodule implementation for upcoming OpenAI AssistantsAPI integration
+v0.52
 - [x] - implement LLM error handling and resolution flows 
 - [x] - refactor flags for SafeMode, Autopilot
-- [ ] - implement restricted commands parser
-- [ ] - refactor and expand CMD module. 
-- [ ] - finish OpenAI Assistants integration
-- [ ] - integrate other LLM providers with http request APIs similar to /v1/completions
+
+### To Do
+- [ ] - refactor and expand CMD module 
 - [ ] - build advanced menu and config options
 
 ## Considering
 - [ ] - passive error detection and resolution for CLI interactions
 - [ ] - voice control
    - [ ] - voice notation
 - [ ] - automation schedules and background states
@@ -124,7 +150,9 @@
 
 This project is licensed under the GNU GPL - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Acknowledgments
 
 - OpenAI for providing the API used for generating chat responses.
 - Flask and Flask-CORS for the web server functionality.
+
+
```

### Comparing `cli-FSD-0.75/cli_FSD/__init__.py` & `cli-FSD-0.9.43/cli_FSD/__init__.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.75/cli_FSD/engine.py` & `cli-FSD-0.9.43/cli_FSD/engine.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.75/cli_FSD/main.py` & `cli-FSD-0.9.43/cli_FSD/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+#0.9.4d
+# adding Ollama support
 
-#0.75 - Refactored resolution process 
-#to-do: clean up old resolution flow, fix CMD mode, fixed assembly assist import
+# Added claude-3-opus mode and flag (-c)
+# added foundation for OpenAI assistants api routing but it's not working yet 
+   
+#to-do: resolve response threadID error, fix flag for assistants api (ci) reimplement replicate flow, robust CMD mode and help log           
 
 import os
 import requests
 import json
 import time
 import subprocess
 import re
@@ -19,14 +23,19 @@
 import asyncio
 import time
 import argparse
 import sys
 import threading
 import shlex
 import queue
+import ollama
+from ollama import Client
+import httpx
+import urllib.parse
+
 
 global llm_suggestions 
 global replicate_suggestions  # This will store suggestions from Replicate
 replicate_suggestions = ""
 
 suggestions_queue = queue.Queue()
 
@@ -155,15 +164,15 @@
         # Execute the suggestion if it's a valid command
         if suggestion.strip().startswith("chmod"):
             subprocess.run(suggestion, shell=True, text=True)
             print(f"{GREEN}Suggestion executed: {suggestion}{RESET}")
         suggestions_queue.task_done()
 
 
-def execute_shell_command(command, api_key, stream_output=True, safe_mode=False):
+def execute_shell_command(command, api_key, stream_output=True, safe_mode=False, scriptreviewer_on=False):
     global llm_suggestions
     
     if command.startswith('./'):
         os.chmod(command[2:], 0o755)  # Ensure the script is executable
 
     if safe_mode:
         user_confirmation = input(f"Do you want to execute the following command: {command}? (yes/no): ").strip()
@@ -183,15 +192,18 @@
         
         process.stdout.close()
         return_code = process.wait()
 
         if return_code != 0:
             error_context = "\n".join(output_lines)  # Combine all output lines to form the error context
             print(f"{RED}Error encountered executing command: {error_context}{RESET}")
-            resolution = consult_llm_for_error_resolution(error_context, api_key)
+            if scriptreviewer_on:
+                resolution = consult_openai_for_error_resolution(error_context, get_system_info())
+            else:
+                resolution = consult_llm_for_error_resolution(error_context, api_key)
             scripts = extract_script_from_response(resolution)
             for script in scripts:
                 execute_resolution_script(script)
                 llm_suggestions = None
         else:
             print(f"{GREEN}Command executed successfully.{RESET}")
     except subprocess.CalledProcessError as e:
@@ -209,44 +221,107 @@
         start = resolution.find("'''") + len("run the command")
         command = resolution[start:].strip()
         # Safely split the command into a list for subprocess
         return shlex.split(command)
     # Add more parsing rules as needed based on the format of resolutions
     return None
 
-def chat_with_model(message, autopilot=False):
-    headers = {
-        "Content-Type": "application/json",
-        "Authorization": f"Bearer {api_key}"
-    }
-    data = {
-        "model": models[current_model],
-        "messages": [
-            {"role": "system", "content": "Generate bash commands for tasks. Comment minimally, you are expected to produce code that is runnable. You are part of a chain."},
-            {"role": "user", "content": message}
-        ]
-    }
+def chat_with_model(message, autopilot=False, use_claude=False, use_ollama=False, ollama_client=None, scriptreviewer_on=False):
+    dotenv_path = Path('.env')
+    load_dotenv(dotenv_path=dotenv_path)
+    scriptreviewer_on=scriptreviewer_on
+    if use_ollama:
+        if not ollama_client:
+            print("Ollama client not initialized.")
+            return "Ollama client missing."
+        
+        system_prompt = ("Generate bash commands for tasks. "
+                         "Comment minimally, you are expected to produce code that is runnable. "
+                         "You are part of a chain.")
+
+        try:
+            # Use the Ollama client to chat, including the system prompt for context
+            response = ollama_client.chat(
+                model='llama3',
+                messages=[
+                    {"role": "system", "content": system_prompt},
+                    {"role": "user", "content": message},
+                ]
+            )
+
+            # Check for the 'content' in the 'message' part of the response
+            if 'message' in response and 'content' in response['message']:
+                assistant_message = response['message']['content']
+                print(f"Ollama responded: {assistant_message}")
+                return assistant_message
+            else:
+                print(f"Unexpected response format: {response}")
+                return "Unexpected response format."
+
+        except Exception as e:
+            print(f"Error while chatting with Ollama: {e}")
+            return f"Error: {e}"
+        
+    if use_claude:
+        anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
+        if not anthropic_api_key:
+            print("Anthropic API key not found. Ensure it's set in your .env file.")
+            return "Anthropic API key missing."
+        # Claude-specific setup
+        headers = {
+            "x-api-key": f"{anthropic_api_key}",
+            "Content-Type": "application/json",
+            "Anthropic-Version": "2023-06-01"
+        }
+        data = {
+            "model": "claude-3-opus-20240229",
+            "system": "Generate bash commands for tasks. Comment minimally, you are expected to produce code that is runnable. You are part of a chain.",  # System prompt at the top level
+            "messages": [
+                {"role": "user", "content": message},
+            ],
+            "max_tokens": 4096,
+            "temperature": 0.7
+        }
+        endpoint = "https://api.anthropic.com/v1/messages"
+    else:
+        # Existing setup for OpenAI
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {api_key}"
+        }
+        data = {
+            "model": models[current_model],
+            "messages": [
+                {"role": "system", "content": "Generate bash commands for tasks. Comment minimally, you are expected to produce code that is runnable. You are part of a chain."},
+                {"role": "user", "content": message}
+            ]
+        }
+        endpoint = "https://api.openai.com/v1/chat/completions"
 
     try:
-        response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, data=json.dumps(data))
-        response.raise_for_status()  # This will raise an exception for HTTP errors
-        model_response = response.json().get('choices', [{}])[0].get('message', {}).get('content', 'No response')
+        response = requests.post(endpoint, headers=headers, data=json.dumps(data))
+        response.raise_for_status()
+        if use_claude:
+            content_blocks = response.json().get('content', [])
+            model_response = ' '.join(block['text'] for block in content_blocks if block['type'] == 'text')
+        else:
+            model_response = response.json().get('choices', [{}])[0].get('message', {}).get('content', 'No response')
     except requests.exceptions.HTTPError as http_err:
-        model_response = f"HTTP error occurred: {http_err}"  # Provide a more graceful error message
+        model_response = f"HTTP error occurred: {http_err}"
     except Exception as err:
-        model_response = f"Other error occurred: {err}"  # Handle other possible errors
+        model_response = f"Other error occurred: {err}"
 
     if autopilot:  
         print(f"{CYAN}Generated command:{RESET} {model_response}")
     else:
-        # Append to conversation history here if needed
-        pass
+        pass  # Append to conversation history here if needed
 
     return model_response
 
+
 def extract_script_from_response(response):
     if not isinstance(response, str):
         print("Error: 'response' expected to be a string, received:", type(response))
         return []
     # Proceed with extracting scripts from the string 'response'
     matches = re.findall(r"```(?:bash|python)?\n(.*?)```", response, re.DOTALL)
     scripts = [(match, "sh", "bash") for match in matches]  # Adjusted to return a tuple (script, ext, lang)
@@ -350,26 +425,26 @@
         else:
             print("No advice was returned by the model.")
             return None
     except requests.exceptions.RequestException as e:
         print(f"API request error: {e}")
         return None
 
-def consult_openai_for_error_resolution(error_message, system_info="", api_key=api_key):
+def consult_openai_for_error_resolution(error_message, system_info=""):
     instructions = "You are a code debugging assistant. Provide debugging advice."
-    scriptReviewer = AssemblyAssist(api_key, instructions)  # Instance of AssemblyAssist
+    scriptReviewer = AssemblyAssist(instructions) 
     system_info = get_system_info()
 
 
     """
     Consults the OpenAI API through the Script Reviewer for advice on resolving an encountered error,
     including system information and previous LLM suggestions.
     """
     # Ensure api_key is defined globally or passed as an argument
-    llm_suggestion = consult_llm_for_error_resolution(error_message, api_key)
+    llm_suggestion = llm_suggestions if llm_suggestions else "No previous LLM suggestion."
     if not llm_suggestion:
         print("Failed to get LLM suggestion.")
         return
 
     # Constructing the full message with system info and LLM suggestions
     full_message = f"Error encountered: {error_message}.\nSystem Info: {system_info}\nLLM Suggestion: {llm_suggestion}. How can I resolve it?"
 
@@ -631,20 +706,20 @@
     except Exception as e:
         return {"status": "error", "message": str(e)}
 
 def clear_line():
     sys.stdout.write("\033[K")  # ANSI escape code to clear the line
     sys.stdout.flush()
     
-def process_input_in_autopilot_mode(query, autopilot_mode):
+def process_input_in_autopilot_mode(query, autopilot_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client):
     stop_event = threading.Event()
     loading_thread = threading.Thread(target=animated_loading, args=(stop_event,))
     loading_thread.start()
     print(f"{CYAN}Sending command to LLM...{RESET}")
-    llm_response = chat_with_model(query, autopilot=autopilot_mode)
+    llm_response = chat_with_model(query, autopilot=autopilot_mode, use_claude=use_claude, scriptreviewer_on=scriptreviewer_on, use_ollama=use_ollama, ollama_client=ollama_client)
     scripts = extract_script_from_response(llm_response)
     if scripts:
         final_script = assemble_final_script(scripts, api_key)
         auto_handle_script_execution(final_script, autopilot=autopilot_mode, stream_output=True)
         stop_event.clear()  # Reset the stop_event for reuse
         stop_event.set()
 
@@ -690,16 +765,16 @@
         print(f"{weather}")
         print(f"{system_info}")
         print("What would you like to do today?")
 
         # Flush the output to ensure it's displayed before waiting for input
         sys.stdout.flush()
 
-def process_input_in_safe_mode(query, safe_mode):
-    llm_response = chat_with_model(query, autopilot=False)
+def process_input_in_safe_mode(query, safe_mode, use_claude,scriptreviewer_on):
+    llm_response = chat_with_model(query, autopilot=False, use_claude=use_claude)
     print_streamed_message(llm_response, CYAN)  # Ensure the LLM's response is printed
 
     scripts = extract_script_from_response(llm_response)
     if scripts:
         for script, file_extension, _ in scripts:
             full_filename = save_script(script, file_extension)  # This function saves the script and returns the filename
             print(f"Script extracted and saved as {full_filename}.")
@@ -711,55 +786,85 @@
                 else:
                     print("Script execution aborted by the user.")
             else:
                 execute_shell_command(f"bash {full_filename}", api_key, safe_mode=safe_mode)
     else:
         print("No executable script found in the LLM response.")
 
-def process_input_based_on_mode(query, safe_mode, autopilot_mode):
+def process_input_based_on_mode(query, safe_mode, autopilot_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client):
     if safe_mode:
-        process_input_in_safe_mode(query, safe_mode)
+        process_input_in_safe_mode(query, safe_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client)
     elif autopilot_mode:
-        process_input_in_autopilot_mode(query, autopilot_mode)
+        process_input_in_autopilot_mode(query, autopilot_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client)
     else:
-        process_input(query)
-                      
+        process_input(query, use_claude, scriptreviewer_on, use_ollama, ollama_client)
+
+
+def initialize_ollama_client():
+    host = 'http://localhost:11434'
+    try:
+        # Attempt to create a client to verify connectivity
+        client = ollama.Client(host=host)
+        # Attempt to fetch the list of available models as a connection test
+        response = client.list()
+        if response:
+            print(f"Connected to Ollama at {host}.")
+        else:
+            print(f"Connected to Ollama at {host}, but no models found.")
+        return client
+    except Exception as e:
+        print(f"Failed to connect to Ollama at {host}: {str(e)}")
+    return None
+
+
 def main():
     global llm_suggestions
-
+    global scriptreviewer_on
     last_response = ""
     command_mode = False
     cleanup_previous_assembled_scripts()
     print_instructions_once_per_day()
     display_greeting()
     stop_event = threading.Event()
 
     # Setup argument parser
     parser = argparse.ArgumentParser(description="Terminal Companion with Full Self Drive Mode")
     parser.add_argument("-s", "--safe", action="store_true", help="Run in safe mode")
     parser.add_argument("-a", "--autopilot", choices=['on', 'off'], default='off',
                         help="Turn autopilot mode on or off at startup")
+    parser.add_argument("-c", "--claude", action="store_true", help="Use Claude for processing requests")
+    parser.add_argument("-ci", "--assistantsAPI", action="store_true", help="Use OpenAI for error resolution")
+    parser.add_argument("-o", "--ollama", action="store_true", help="Use Ollama for processing requests")
+
     args, unknown = parser.parse_known_args()
-    
+
     # If additional arguments are provided, join them into a single string
     query = ' '.join(unknown)
-
-    # Set autopilot mode based on the -a or --autopilot argument
+    # Initialize the Ollama client if the -o flag is provided
+    ollama_client = None
+    if args.ollama:
+        ollama_client = initialize_ollama_client()
+        if ollama_client:
+            print("Ollama mode activated.")
+        else:
+            print("Ollama client could not be initialized.")
     autopilot_mode = args.autopilot
     safe_mode = args.safe 
-
-
+    use_claude = args.claude
+    scriptreviewer_on = args.assistantsAPI
+    use_ollama=args.ollama 
 
     # Start the animated loading in a separate thread only if a query is present
     if query:
-        process_input_based_on_mode(query, safe_mode, autopilot_mode)            # Process the input in safe mode
+        process_input_based_on_mode(query, safe_mode, autopilot_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client)            # Process the input in safe mode
 
     while True:
         user_input = input(f"{YELLOW}@:{RESET} ").strip()
         scripts = [] 
+    
 
         if command_mode:
             command = input("\033[92mCMD>\033[0m ").strip().lower()
             if command == 'quit':
                 break
             elif command == 'reset':
                 reset_conversation()
@@ -816,58 +921,58 @@
             elif user_input.lower() == 'normal':
                 safe_mode = False
                 autopilot_mode = False
                 print("Switched to normal mode.")
 
             # If no special commands, process input based on current mode
             if not command_mode:
-                process_input_based_on_mode(user_input, safe_mode, autopilot_mode)            
+                process_input_based_on_mode(user_input, safe_mode, autopilot_mode, use_claude, scriptreviewer_on, use_ollama, ollama_client)            
                 
             elif autopilot_mode:
-                llm_response = chat_with_model(user_input, autopilot=True)
+                llm_response = chat_with_model(user_input, autopilot=True, use_claude=use_claude, scriptreviewer_on=scriptreviewer_on, use_ollama=use_ollama, ollama_client=ollama_client)
                 scripts = extract_script_from_response(llm_response)
             if scripts:
                 for script, file_extension, _ in scripts:
                     filename = input("Enter a filename for the script (without extension): ")   
                     full_filename = f"{filename}.{file_extension}"
                     with open(full_filename, "w") as file:
                         file.write(script)
             
                     if file_extension == "py":
                         final_script = assemble_final_script([(script, file_extension, "python")], api_key)
                         # Execute only Python scripts with error handling and consultation
                         execute_script_with_repl_and_consultation(final_script, api_key)
                     elif file_extension == "sh":
                         # Add the `safe_mode` parameter when executing the script
-                        execute_shell_command(f"bash {full_filename}", api_key, safe_mode=safe_mode)
+                        execute_shell_command(f"bash {full_filename}", api_key, safe_mode=safe_mode,  scriptreviewer_on=scriptreviewer_on)
                     else:
                         print(f"Bypassing repl test and executing in local environment: {script[:30]}...")
                         process_input_in_autopilot_mode(user_input, autopilot_mode)
                         stop_event.set()
 
                         print("Enter another task or press ctrl+z to quit.")
                         
             else:
                     print("No executable script found in the LLM response.")
         if not autopilot_mode or safe_mode:
             user_input = input(f"{YELLOW}@:{RESET} ").strip()
             # Non-autopilot mode processing
-            process_input_in_safe_mode(query, safe_mode)  # This function should handle the safe mode logic
+            process_input_in_safe_mode(query, safe_mode, use_claude, scriptreviewer_on)  # This function should handle the safe mode logic
             print_streamed_message(last_response, CYAN)
 
         elif safe_mode == True:
             user_input = input(f"{YELLOW}@:{RESET} ").strip()
             # Non-autopilot mode processing
-            process_input_in_safe_mode(query, safe_mode)  # This function should handle the safe mode logic
+            process_input_in_safe_mode(query, safe_mode, use_claude, scriptreviewer_on)  # This function should handle the safe mode logic
             print_streamed_message(last_response, CYAN)
 
         elif autopilot_mode == True:
             user_input = input(f"{YELLOW}@:{RESET} ").strip()
             # Non-autopilot mode processing
-            process_input_in_autopilot_mode(query, safe_mode)  # This function should handle the safe mode logic
+            process_input_in_autopilot_mode(query, safe_mode, use_claude, scriptreviewer_on)  # This function should handle the safe mode logic
             print_streamed_message(last_response, CYAN)
                                                                 
 
 
     print("Operation completed.")
     stop_event.set()
```

### Comparing `cli-FSD-0.75/cli_FSD/resources/assembler.py` & `cli-FSD-0.9.43/cli_FSD/resources/assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import requests
+import os
 import time
 
 class AssemblyAssist:
-    def __init__(self, api_key, instructions="You are a helpful assistant.", name="Helpful Assistant"):
-        self.api_key = api_key
+    def __init__(self, instructions="You are a helpful assistant.", name="Helpful Assistant"):
+        self.api_key = os.getenv("OPENAI_API_KEY")
+        if not self.api_key:
+            raise ValueError("OPENAI_API_KEY environment variable not set.")
         self.instructions = instructions
         self.name = name
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
             "OpenAI-Beta": "assistants=v1"
         }
@@ -115,28 +118,28 @@
                 print("Failed to delete the assistant.")
         else:
             print("No assistant to delete.")    
     
     def start_conversation(self):
         self.assistant_id = self.create_assistant()
         if not self.assistant_id:
-            print("Failed to create assistant.")
+            print("Failed to create assistant.") 
             return False
         self.thread_id = self.create_thread()
         if not self.thread_id:
             print("Failed to create thread.")
             return False
         print("Assistant created and thread initiated.")
         return True
     
 # Testing block
 if __name__ == "__main__":
-    # api_key = YOUR OPENAI-API-KEY# Replace with your actual OpenAI API key
+#    api_key = *YOUR OPENAI_API_KEY*
     instructions = "You are a code debugging assistant. Provide debugging advice."  # Example instructions
-    chatbot = AssemblyAssist(api_key, instructions)
+    chatbot = AssemblyAssist(instructions)
 
     try:
         chatbot.start_conversation()
         while True:
             user_input = input("You: ")
             if user_input.lower() == "exit":
                 break
```

### Comparing `cli-FSD-0.75/cli_FSD.egg-info/PKG-INFO` & `cli-FSD-0.9.43/cli_FSD.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 0.75
+Version: 0.9.43
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cli-FSD
 Natural language interface for your command line. 
 
-A lightweight and portable autopilot utility for CLI tasks. Takes natural language as input and uses the OpenAI API to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or make script modules and microservices on the fly. 
+A lightweight and portable autopilot utility for CLI tasks that takes natural language as input and uses the LLM of your choice to take the appropriate actions by generating and parsing shell scripts. Find answers to questions and let AI execute commands with your permission in Safe Mode or enable Autopilot to automate tasks or script modules and microservices on the fly. 
 
 **Warning**: Giving LLMs shell-level access to your computer is dangerous and should only be done in sandbox or otherwise expendable environments.
 
 ##### I made cli-FSD for experimenting and problem solving in low stakes development environments. If you don't have access to a machine like that you can try it below: 
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.10 or later (may work with earlier versions)
 - pip 24.0 or later 
-- An OpenAI API key
+- An OpenAI API key **or** Anthropic API key **or** Ollama running in the same environment as cli-FSD
 
 ### Installation
 
 0. **Pre-requisites:**
    
 - Upgrade pip
 
@@ -104,21 +106,31 @@
 If you don't want to run it locally:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?repo=wazacraft/cli-FSD&ref=main)
 
 [![Run on Replit](https://replit.com/badge/github/wazacraft/cli-FSD)](https://replit.com/@wazacraft/cli-FSD)
 
 ## Project Progress
-### To Do
+v0.94
+- [x] - Added support for [Ollama]([url](https://github.com/ollama/ollama)) (use -o to run cli-FSD using any supported local LLM model)
+- [x] - support for script custom gpt-4-turbo assistant OpenAI's Assistants API to revie
+v0.87
+- [x] - finish OpenAI Assistants integration (done but but needs to be made accessible in main.py)
+- [x] - integrate other LLM providers with http request APIs similar to /v1/completions (pass -c with your query to use Anthropic API's Claude 3 Opus)
+- [x] - improved error handling 
+
+v0.75
+- [x] - overhauled and refactored error resolution function to address a bug that sometimes prevented the resolution from executing
+- [x] - fixed niche text handling errors and submodule implementation for upcoming OpenAI AssistantsAPI integration
+v0.52
 - [x] - implement LLM error handling and resolution flows 
 - [x] - refactor flags for SafeMode, Autopilot
-- [ ] - implement restricted commands parser
-- [ ] - refactor and expand CMD module. 
-- [ ] - finish OpenAI Assistants integration
-- [ ] - integrate other LLM providers with http request APIs similar to /v1/completions
+
+### To Do
+- [ ] - refactor and expand CMD module 
 - [ ] - build advanced menu and config options
 
 ## Considering
 - [ ] - passive error detection and resolution for CLI interactions
 - [ ] - voice control
    - [ ] - voice notation
 - [ ] - automation schedules and background states
@@ -138,7 +150,9 @@
 
 This project is licensed under the GNU GPL - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Acknowledgments
 
 - OpenAI for providing the API used for generating chat responses.
 - Flask and Flask-CORS for the web server functionality.
+
+
```

### Comparing `cli-FSD-0.75/setup.py` & `cli-FSD-0.9.43/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-FSD',
-    version='0.75',
+    version='0.9.43',
     author='JG',
     author_email='wazacraftRFID@gmail.com',
     description='LLM-enabled companion utility for your terminal.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wazacraft/cli-FSD',
     packages=find_packages(),
@@ -16,16 +16,16 @@
         ],
     },
     install_requires=[
         'Flask',
         'flask-cors',
         'python-dotenv',
         'requests',
-        'json',
+        'ollama'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-)
+)
```


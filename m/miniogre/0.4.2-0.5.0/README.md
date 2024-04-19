# Comparing `tmp/miniogre-0.4.2.tar.gz` & `tmp/miniogre-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniogre-0.4.2.tar", max compression
+gzip compressed data, was "miniogre-0.5.0.tar", max compression
```

## Comparing `miniogre-0.4.2.tar` & `miniogre-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6171 2024-03-11 05:03:52.946267 miniogre-0.4.2/.env
--rw-r--r--   0        0        0    11357 2024-03-11 05:03:52.946267 miniogre-0.4.2/LICENSE
--rw-r--r--   0        0        0     4134 2024-03-11 05:03:52.946267 miniogre-0.4.2/README.md
--rw-r--r--   0        0        0      125 2024-03-11 05:03:52.946267 miniogre-0.4.2/miniogre/__init__.py
--rw-r--r--   0        0        0    16780 2024-03-11 05:03:52.946267 miniogre-0.4.2/miniogre/actions.py
--rw-r--r--   0        0        0     4548 2024-03-11 05:03:52.946267 miniogre-0.4.2/miniogre/config.py
--rw-r--r--   0        0        0     3190 2024-03-11 05:03:52.946267 miniogre-0.4.2/miniogre/constants.py
--rw-r--r--   0        0        0     2968 2024-03-11 05:03:52.946267 miniogre-0.4.2/miniogre/main.py
--rw-r--r--   0        0        0      767 2024-03-11 05:03:52.946267 miniogre-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5190 1970-01-01 00:00:00.000000 miniogre-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     7173 2024-04-19 06:43:53.709826 miniogre-0.5.0/.env
+-rw-r--r--   0        0        0    11357 2024-04-19 06:43:53.709826 miniogre-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4134 2024-04-19 06:43:53.709826 miniogre-0.5.0/README.md
+-rw-r--r--   0        0        0      125 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/__init__.py
+-rw-r--r--   0        0        0    19542 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/actions.py
+-rw-r--r--   0        0        0     4564 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/config.py
+-rw-r--r--   0        0        0    10297 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/constants.py
+-rw-r--r--   0        0        0     2630 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/main.py
+-rw-r--r--   0        0        0      793 2024-04-19 06:43:53.713826 miniogre-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 miniogre-0.5.0/PKG-INFO
```

### Comparing `miniogre-0.4.2/.env` & `miniogre-0.5.0/.env`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,90 @@
-OGRE_DIR = 'ogre_dir'
-OGRE_BASEIMAGE = 'ogrerun/base:ubuntu22.04-{}'
-OPENAI_MODEL = 'gpt-4-turbo-preview'
-OPENAI_SECRET_PROMPT = "You are a Python requirements generator.
-You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
-The raw text sent by the user consists of a combination of the README file contents and the source code contents.
-You generate only the file contents as answer.
-If the text sent by the user is invalid or is empty, just generate an empty content.
-You should ignore the Python version 2 or 3.
-The python package should not be included in the requirements file.
-Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldn't be added to the requirements.txt file.
-Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
-Your output should be a raw ASCII text file."
-OCTOAI_MODEL = 'mistral-7b-instruct-fp16'
-OCTOAI_SECRET_PROMPT = "You are a Python requirements generator.
-You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
-The raw text sent by the user consists of a combination of the README file contents and the source code contents.
-If the text sent by the user is invalid or is empty, just generate an empty content.
-You should ignore the Python version 2 or 3.
-The python package should not be included in the requirements file.
-Some packages do not exist in the PyPi repository, they are only local, and thus shouldn't be added to the requirements.txt file.
-Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
-Your output should be a raw ASCII text file.
-Do not return parts of the text sent by the user. We just want the requirements list.
-Only return the list of requirements. No other text like the filename at the top of the response or symbols are allowed."
-REWRITE_README_PROMPT="You are a specialist in understanding and explaining source code. 
-You are also a specialist in writing clear documentation (e.g README files) that helps people to understand the source code.
-Your task is to take a text input containing the current README and the code and use it to write an updated version of the README file.
-The README file should highlight the actual requirements that need to be installed.
-"
-#GROQ_MODEL = 'llama2-70b-4096'
-GROQ_MODEL = 'mixtral-8x7b-32768'
-GROQ_SECRET_PROMPT="You are a Python requirements generator.
-You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
-The raw text sent by the user consists of a combination of the README file contents and the source code contents.
-If the text sent by the user is invalid or is empty, just generate an empty content.
-You should ignore the Python version 2 or 3.
-The python package should not be included in the requirements file.
-Some packages do not exist in the PyPi repository, they are only local, and thus shouldn't be added to the requirements.txt file.
-Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
-Your output should be a raw ASCII text file containg only the list of requirements. Do not return sentences. 
-Do not return parts of the text sent by the user. We just want the requirements list."
-#MISTRAL_MODEL = 'open-mixtral-8x7b'
-MISTRAL_MODEL = 'mistral-large-latest'
-MISTRAL_SECRET_PROMPT="You are a Python requirements generator.
-You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
-The raw text sent by the user consists of a combination of the README file contents and the source code contents.
-You generate only the file contents as answer.
-If the text sent by the user is invalid or is empty, just generate an empty content.
-You should ignore the Python version 2 or 3.
-The python package should not be included in the requirements file.
-Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldn't be added to the requirements.txt file.
-Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
-Your output should be a raw ASCII text file."
-CLEAN_REQUIREMENTS_SECRET_PROMPT = "Here is the content of a requirements.txt file. 
-It is a list of Python libraries to be installed in the a Python environment. 
-Not all entries in the list are actual Python libraries available on the PyPi repository. 
-Identify those that aren't available on PyPi and remove them from the list.
-Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
-If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
-For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
-Do not explain how the new list is generated. Do not provide any context related to how you proceeded.
-Your response must contain only the list of packages to be installed.
-Remove any blank lines."
-GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT = "Here is the content of a requirements.txt file. 
-It is a list of Python libraries to be installed in the a Python environment. 
-Not all entries in the list are actual Python libraries available on the PyPi repository. 
-Identify those that aren't available on PyPi and remove them from the list.
-Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
-If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
-For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
-No explanation notes on your reasoning are allowed. Nobody wants to know which packages were removed. Your response must contain only the list of packages to be installed.
-Remove any blank lines."
+# OGRE_DIR='ogre_dir'
+# OGRE_BASEIMAGE='ogrerun/base:ubuntu22.04-{}'
+
+# OLLAMA_MODEL='mistral:7b'
+# OLLAMA_API_SERVER='http://localhost:11434/v1'
+# OLLAMA_SECRET_PROMPT='You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# You generate only the file contents as answer.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file.'
+
+# OPENAI_MODEL='gpt-4-turbo-preview'
+# OPENAI_SECRET_PROMPT='You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# You generate only the file contents as answer.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file.'
+
+# OCTOAI_MODEL='mistral-7b-instruct-fp16'
+# OCTOAI_SECRET_PROMPT='You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file.
+# Do not return parts of the text sent by the user. We just want the requirements list.
+# Only return the list of requirements. No other text like the filename at the top of the response or symbols are allowed.'
+
+# REWRITE_README_PROMPT='You are a specialist in understanding and explaining source code. 
+# You are also a specialist in writing clear documentation (e.g README files) that helps people to understand the source code.
+# Your task is to take a text input containing the current README and the code and use it to write an updated version of the README file.
+# The README file should highlight the actual requirements that need to be installed.'
+
+# GROQ_MODEL='mixtral-8x7b-32768'
+# GROQ_SECRET_PROMPT='You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file containg only the list of requirements. Do not return sentences. 
+# Do not return parts of the text sent by the user. We just want the requirements list.'
+
+# MISTRAL_MODEL='mistral-large-latest'
+# MISTRAL_SECRET_PROMPT='You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# You generate only the file contents as answer.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file.'
+
+# CLEAN_REQUIREMENTS_SECRET_PROMPT='Here is the content of a requirements.txt file. 
+# It is a list of Python libraries to be installed in the a Python environment. 
+# Not all entries in the list are actual Python libraries available on the PyPi repository. 
+# Identify those that arent available on PyPi and remove them from the list.
+# Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
+# If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
+# For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
+# Do not explain how the new list is generated. Do not provide any context related to how you proceeded.
+# Your response must contain only the list of packages to be installed.
+# Remove any blank lines.'
+
+# GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT='Here is the content of a requirements.txt file. 
+# It is a list of Python libraries to be installed in the a Python environment. 
+# Not all entries in the list are actual Python libraries available on the PyPi repository. 
+# Identify those that arent available on PyPi and remove them from the list.
+# Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
+# If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
+# For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
+# No explanation notes on your reasoning are allowed. Nobody wants to know which packages were removed. Your response must contain only the list of packages to be installed.
+# Remove any blank lines.'
```

### Comparing `miniogre-0.4.2/LICENSE` & `miniogre-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniogre-0.4.2/README.md` & `miniogre-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `miniogre-0.4.2/miniogre/actions.py` & `miniogre-0.5.0/miniogre/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 def requirements_emoji():
     print(emoji.emojize(':thinking_face: Generating requirements...'))
 
 def cleaning_requirements_emoji():
     print(emoji.emojize(':cooking: Refining...'))
 
+def generate_context_emoji():
+    print(emoji.emojize(':magnifying_glass_tilted_left: Generating context...'))
+
 def readme_emoji():
     print(emoji.emojize(':notebook: Generating new README.md...'))
 
 def list_files(project_path):
     # List all files in current directory and subdirectories
     files = []
     for root, dirs, filenames in os.walk(project_path):
@@ -141,15 +144,15 @@
                             i += 1
                 
         external_imports = [imp.split('.')[0] for sublist in external_imports for imp in sublist]
         external_imports = list(set(external_imports))
 
         requirements = '\n'.join(external_imports)
     else:
-        with open('{}/requirements.txt'.format(os.getenv('OGRE_DIR')), 'r') as f:
+        with open('{}/requirements.txt'.format(os.getenv('OGRE_DIR', OGRE_DIR)), 'r') as f:
             requirements = f.read()
     return requirements
 
 
 
 def append_files_with_ext(project_path, ext, limit, output_file):
     files = list_files(project_path)
@@ -191,31 +194,31 @@
     elif provider == 'octoai':
         res = extract_requirements_octoai(contents)
     elif provider == 'groq':
         res = extract_requirements_groq(contents)
     return res
 
 def extract_requirements_openai(contents):
-    model = os.getenv('OPENAI_MODEL')
-    prompt = os.getenv('OPENAI_SECRET_PROMPT')
+    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
+    prompt = os.getenv('OPENAI_SECRET_PROMPT', OPENAI_SECRET_PROMPT)
     client = OpenAI()
     completion = client.chat.completions.create(
                   model=model,
                   messages=[
                       {"role": "system", "content": prompt},
                       {"role": "user", "content": contents}
                   ]
               )
     requirements = completion.choices[0].message.content
     
     return requirements
 
 def extract_requirements_octoai(contents):
-    model = os.getenv('OCTOAI_MODEL')
-    prompt = os.getenv('OCTOAI_SECRET_PROMPT')
+    model = os.getenv('OCTOAI_MODEL', OCTOAI_MODEL)
+    prompt = os.getenv('OCTOAI_SECRET_PROMPT', OCTOAI_SECRET_PROMPT)
     client = OctoAiClient()
 
     completion = client.chat.completions.create(
     messages=[
             {
                 "role": "system",
                 "content": prompt
@@ -232,55 +235,75 @@
     top_p=0.9)
 
     requirements = completion.choices[0].message.content
 
     return requirements
 
 def extract_requirements_groq(contents):
-    prompt = os.getenv('GROQ_SECRET_PROMPT')
+    prompt = os.getenv('GROQ_SECRET_PROMPT', GROQ_SECRET_PROMPT)
     with Completion() as completion:
         full_prompt = prompt + " " + contents
         response, id, stats = completion.send_prompt("llama2-70b-4096", user_prompt=full_prompt)
         if response != "":
             print(f"\nPrompt: {prompt}\n")
             print(f"Request ID: {id}")
             print(f"Output:\n {response}\n")
             print(f"Stats:\n {stats}\n")
     return response
 
 def clean_requirements(provider, requirements):
     cleaning_requirements_emoji()
     if provider == 'openai':
         res = clean_requirements_openai(requirements)
+    elif provider == 'ollama':
+        res = clean_requirements_ollama(requirements)
     elif provider == 'octoai':
         res = clean_requirements_octoai(requirements)
     elif provider == 'groq':
         res = clean_requirements_groq(requirements)
     elif provider == 'mistral':
         res = clean_requirements_mistral(requirements)
     return res
 
+def clean_requirements_ollama(requirements):
+    model = os.getenv('OLLAMA_MODEL', OLLAMA_MODEL)
+    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
+    api_server = os.getenv('OLLAMA_API_SERVER', OLLAMA_API_SERVER)
+    # print(f"{api_server=} {model=} {prompt=}")
+    client = OpenAI(base_url=api_server, api_key='ollama')
+    completion = client.chat.completions.create(
+                  model=model,
+                  messages=[
+                      {"role": "system", "content": prompt},
+                      {"role": "user", "content": requirements}
+                  ]
+              )
+    requirements = completion.choices[0].message.content
+
+    return requirements
+
 def clean_requirements_openai(requirements):
-    model = os.getenv('OPENAI_MODEL')
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT')
+    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
+    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
+    # print(f"{model=} {prompt=}")
     client = OpenAI()
     completion = client.chat.completions.create(
                   model=model,
                   messages=[
                       {"role": "system", "content": prompt},
                       {"role": "user", "content": requirements}
                   ]
               )
     requirements = completion.choices[0].message.content
 
     return requirements
 
 def clean_requirements_mistral(requirements):
-    model = os.getenv('MISTRAL_MODEL')
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT')
+    model = os.getenv('MISTRAL_MODEL', MISTRAL_MODEL)
+    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
     api_key = os.environ["MISTRAL_API_KEY"]
     client = MistralClient(api_key=api_key)
     content = prompt + '\n' + requirements
     messages = [ChatMessage(role="user", content=content)]
 
     # No streaming
     chat_response = client.chat(
@@ -288,25 +311,25 @@
         messages=messages,
     )
     requirements = chat_response.choices[0].message.content
 
     return requirements
 
 def clean_requirements_groq(requirements):
-    model = os.getenv('GROQ_MODEL')
-    prompt = os.getenv('GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT')
+    model = os.getenv('GROQ_MODEL', GROQ_MODEL)
+    prompt = os.getenv('GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT', GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT)
     with Completion() as completion:
         full_prompt = prompt + " " + requirements
         response, id, stats = completion.send_prompt(model, user_prompt=full_prompt)
         
     return response
 
 def clean_requirements_octoai(requirements):
-    model = os.getenv('OCTOAI_MODEL')
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT')
+    model = os.getenv('OCTOAI_MODEL', OCTOAI_MODEL)
+    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
     client = OctoAiClient()
 
     completion = client.chat.completions.create(
         messages=[
                 {
                     "role": "system",
                     "content": prompt
@@ -330,67 +353,88 @@
     requirements_fullpath = os.path.join(ogre_dir_path, 'requirements.txt')
     with open(requirements_fullpath, 'w') as f:
         f.write(requirements)
     return requirements_fullpath 
 
 def rewrite_readme(provider, readme):
     readme_emoji()
+    
     if provider == 'openai':
         res = rewrite_readme_openai(readme)
+    elif provider == 'ollama':
+        res = rewrite_readme_ollama(readme)
     elif provider == 'octoai':
         res = rewrite_readme_octoai(readme)
     elif provider == 'groq':
         res = rewrite_readme_groq(readme)
     elif provider == 'mistral':
         res = rewrite_readme_mistral(readme)
     return res
 
 def rewrite_readme_openai(readme):
-    model = os.getenv('OPENAI_MODEL')
-    prompt = os.getenv('REWRITE_README_PROMPT')
+    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
+    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
     client = OpenAI()
     if 'OPENAI_API_KEY' not in os.environ:
         raise EnvironmentError("OPENAI_API_KEY environment variable not defined")
     
     try:
         completion = client.chat.completions.create(
                         model=model,
                         messages=[
                             {"role": "system", "content": prompt},
                             {"role": "user", "content": readme}
                         ]
                     )
+        # print(completion)
         new_readme = completion.choices[0].message.content
     except Exception as e:
         print(e)
 
     return new_readme
 
+def rewrite_readme_ollama(readme):
+    model = os.getenv('OLLAMA_MODEL', OLLAMA_MODEL)
+    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
+    api_server = os.getenv('OLLAMA_API_SERVER', OLLAMA_API_SERVER)
+    # print(f"{api_server=} {model=} {prompt=}")
+    client = OpenAI(base_url=api_server, api_key='ollama')
+    completion = client.chat.completions.create(
+                  model=model,
+                  messages=[
+                      {"role": "system", "content": prompt},
+                      {"role": "user", "content": readme}
+                  ]
+              )
+    new_readme = completion.choices[0].message.content
+
+    return new_readme
+
 def rewrite_readme_octoai(readme):
     raise NotImplementedError("rewrite_readme_octoai is not implemented.")
 
 def rewrite_readme_groq(readme):
     raise NotImplementedError("rewrite_readme_groq is not implemented.")
 
 def rewrite_readme_mistral(readme):
-    model = os.getenv('MISTRAL_MODEL')
-    prompt = os.getenv('REWRITE_README_PROMPT')
+    model = os.getenv('MISTRAL_MODEL', MISTRAL_MODEL)
+    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
     api_key = os.environ["MISTRAL_API_KEY"]
     client = MistralClient(api_key=api_key)
     content = prompt + '\n' + readme
     messages = [ChatMessage(role="user", content=content)]
     
     # No streaming
     chat_response = client.chat(
         model=model,
         messages=messages,
     )
-    requirements = chat_response.choices[0].message.content
+    new_readme = chat_response.choices[0].message.content
 
-    return requirements
+    return new_readme
 
 def save_readme(readme, ogre_dir_path):
     readme_fullpath = os.path.join(ogre_dir_path, 'README.md')
     with open(readme_fullpath, 'w') as f:
         f.write(readme)
     return readme_fullpath 
 
@@ -485,38 +529,58 @@
     f = Figlet(font="slant")
     # Get version
     # ogre_version = pkg_resources.get_distribution('miniogre').version
     rprint("[cyan] {} [/cyan]".format(f.renderText("miniogre")))
     rprint("[blue bold]miniogre - {}[/blue bold]".format("https://ogre.run"))
     print("\n")
 
-def create_virtualenv(requirements, python_version):
+# def create_virtualenv(requirements, python_version):
   
-    env_name = 'miniogre-env'
+#     env_name = 'miniogre-env'
 
-    venv_cmd = "python -m venv {}".format(env_name)
-    # venv_activate_cmd = 'source {}/bin/activate'.format(env_name) 
+#     venv_cmd = "python -m venv {}".format(env_name)
+#     # venv_activate_cmd = 'source {}/bin/activate'.format(env_name) 
 
-    #os.popen(venv_cmd)
-    #os.popen(venv_activate_cmd)
-    p = subprocess.Popen(venv_cmd, stdout=subprocess.PIPE, shell=True)
-    (out, err) = p.communicate()
-    p_status = p.wait()
+#     #os.popen(venv_cmd)
+#     #os.popen(venv_activate_cmd)
+#     p = subprocess.Popen(venv_cmd, stdout=subprocess.PIPE, shell=True)
+#     (out, err) = p.communicate()
+#     p_status = p.wait()
+
+#     venv_activate_cmd = 'source {}/bin/activate'.format(env_name)
+#     p = subprocess.Popen(venv_activate_cmd, stdout=subprocess.PIPE, shell=True)
+#     (out, err) = p.communicate()
+#     p_status = p.wait()
+
+#     pip_cmd = '{}/bin/pip'.format(env_name)
+#     with open(requirements) as f:
+#         requirements_list = []
+#         for line in f:
+#             requirements_list.append(line.strip('\n'))
+
+#         pip_cmd = 'pip' 
+#         for req in requirements_list:
+#             print(req)
+#             input()
+#             subprocess.call([pip_cmd, 'install', req.strip()])
+
+def run_gptify(repo_path):
+
+    generate_context_emoji()
+    
+    if not os.path.exists("ogre_dir"):
+        os.mkdir("ogre_dir")
 
-    venv_activate_cmd = 'source {}/bin/activate'.format(env_name)
-    p = subprocess.Popen(venv_activate_cmd, stdout=subprocess.PIPE, shell=True)
+    gptrepo_cmd = 'gptify {} --output "ogre_dir/gptify_output.txt"'.format(repo_path)
+    p = subprocess.Popen(gptrepo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     (out, err) = p.communicate()
     p_status = p.wait()
 
-    pip_cmd = '{}/bin/pip'.format(env_name)
-    with open(requirements) as f:
-        requirements_list = []
-        for line in f:
-            requirements_list.append(line.strip('\n'))
-
-        pip_cmd = 'pip' 
-        for req in requirements_list:
-            print(req)
-            input()
-            subprocess.call([pip_cmd, 'install', req.strip()])
-
+    with open('ogre_dir/gptify_output.txt', 'r') as f:
+        return f.read()
 
+def cleanup():
+    """
+    Delete unnecessary files
+    """
+    if os.path.exists('ogre_dir/gptify_output.txt'):
+        os.remove('ogre_dir/gptify_output.txt')
```

### Comparing `miniogre-0.4.2/miniogre/config.py` & `miniogre-0.5.0/miniogre/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     return os.path.isfile("{}/Dockerfile".format(ogre_dir))
 
 
 def config_baseimage():
 
     platform_machine = "{}".format(platform.machine())
-    baseimage = (os.getenv("OGRE_BASEIMAGE")).format(platform_machine)
+    baseimage = (os.getenv("OGRE_BASEIMAGE", OGRE_BASEIMAGE)).format(platform_machine)
 
     return baseimage
     
 def config_requirements(project_dir, ogre_dir, force=False):
 
     # Check if requirements.txt is in the root folder
     if os.path.isfile("{}/requirements.txt".format(project_dir)):
```

### Comparing `miniogre-0.4.2/miniogre/main.py` & `miniogre-0.5.0/miniogre/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,91 @@
+import importlib.metadata
 import os
+
 import typer
-from openai import OpenAI
 from dotenv import load_dotenv
+from openai import OpenAI
+
 from .actions import *
 from .config import *
 
-
 app = typer.Typer()
 load_dotenv()
 
 project_path = os.getcwd()
-prompt = os.getenv('OPENAI_SECRET_PROMPT')
-prompt_rewrite_readme = os.getenv('PROMPT_REWRITE_README')
 
 @app.command()
-def readme(provider: str = 'openai',
-           limit_source_files: int = 1):
+def version():
+    """
+    Display version
+    """
+    version_string = importlib.metadata.version('miniogre')
+    print("{}".format(version_string))
+
+    return 0
+
+@app.command()
+def readme(provider: str = "openai"):
     """
     Rewrite readme
     """
 
     display_figlet()
     starting_emoji()
 
-    files = list_files(project_path)
-    extensions = get_extensions(files)
-    counts = count_extensions(extensions)
-    most_ext = determine_most_ext(counts)
-    readme_path = find_readme(project_path)
-    readme_contents = read_file_contents(readme_path)
-    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv('OGRE_DIR')))
-    source_contents = append_files_with_ext(project_path, most_ext, limit_source_files, 
-                                            "{}/source_contents.txt".format(ogre_dir_path))
-    context_contents = generate_context_file(readme_contents, source_contents, 
-                                             "{}/context_file.txt".format(ogre_dir_path))
+    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR)))
+    context_contents = run_gptify(os.getcwd())
     new_readme = rewrite_readme(provider, context_contents)
     readme_path = save_readme(new_readme, ogre_dir_path)
-    end_emoji() 
+    end_emoji()
 
     return 0
 
 @app.command()
-def run(provider: str = 'openai',
-        baseimage: str = 'auto',
-        port: str = '8001',
-        dry: bool = False,
-        force_requirements_generation: bool = True,
-        sbom_format: str = 'pip-licenses',
-        no_container: bool = False,
-        verbose: bool = False):
+def run(
+    provider: str = "openai",
+    baseimage: str = "auto",
+    port: str = "8001",
+    dry: bool = False,
+    force_requirements_generation: bool = True,
+    sbom_format: str = "pip-licenses",
+    no_container: bool = False,
+    verbose: bool = False,
+    with_readme: bool = False
+):
     """
-    Run miniogre
+    Run full miniogre pipeline
     """
 
     display_figlet()
     starting_emoji()
 
-    if baseimage == 'auto':
+    if baseimage == "auto":
         baseimage = config_baseimage()
 
     project_name = os.path.basename(project_path)
 
     files = list_files(project_path)
     extensions = get_extensions(files)
     counts = count_extensions(extensions)
     most_ext = determine_most_ext(counts)
-    readme_path = find_readme(project_path)
-    readme_contents = read_file_contents(readme_path)
-    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv('OGRE_DIR')))
+    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR)))
+    if with_readme:
+        context_contents = run_gptify(os.getcwd())
+        new_readme = rewrite_readme(provider, context_contents)
+        readme_path = save_readme(new_readme, ogre_dir_path)
     generate_requirements = config_requirements(project_path, ogre_dir_path, force_requirements_generation)
     local_requirements = extract_requirements_from_code(project_path, most_ext, generate_requirements)
     final_requirements = clean_requirements(provider, local_requirements)
     requirements_fullpath = save_requirements(final_requirements, ogre_dir_path)
     config_bashrc(project_path, ogre_dir_path, None, None, None)
     config_dockerfile(project_path, project_name, ogre_dir_path, baseimage, dry)
     create_sbom(project_name, project_path, sbom_format, verbose)
     if no_container == False:
-        build_docker_image(os.path.join(ogre_dir_path, "Dockerfile"), project_name, verbose)
+        build_docker_image(
+            os.path.join(ogre_dir_path, "Dockerfile"), project_name, verbose
+        )
         spin_up_container(project_name, project_path, port)
     end_emoji()
-    
-if __name__ == '__main__':
-    app()
+
+if __name__ == "__main__":
+    app()
```

### Comparing `miniogre-0.4.2/pyproject.toml` & `miniogre-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "miniogre"
-version = "0.4.2"
-description = "miniogre: automate the installation of Python dependencies with AI, to ensure your code runs on any computer"
+version = "0.5.0"
+description = "miniogre: from source code to reproducible environment, in seconds."
 readme = "README.md"
 authors = ["Wilder Lopes <wilder@ogre.run>"]
 include = [".env"]
+homepage = "https://github.com/ogre-run/miniogre"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 typer = "0.9.0"
 docker = "^5.0.0"
 python-dotenv = "^0.19.0"
-openai = "1.12.0"
+openai = "1.21.2"
 emoji = "^2.10.1"
 pyfiglet = "^1.0.2"
 rich = "^13.7.0"
 groq = "^0.3.0"
 yaspin = "^3.0.1"
 octoai-sdk = "^0.9.0"
 mistralai = "^0.1.3"
 autopep8 = "^2.0.4"
 cyclonedx-py = "^1.0.1"
 pip-licenses = "^4.3.4"
+gptify = "0.3.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `miniogre-0.4.2/PKG-INFO` & `miniogre-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: miniogre
-Version: 0.4.2
-Summary: miniogre: automate the installation of Python dependencies with AI, to ensure your code runs on any computer
+Version: 0.5.0
+Summary: miniogre: from source code to reproducible environment, in seconds.
+Home-page: https://github.com/ogre-run/miniogre
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autopep8 (>=2.0.4,<3.0.0)
 Requires-Dist: cyclonedx-py (>=1.0.1,<2.0.0)
 Requires-Dist: docker (>=5.0.0,<6.0.0)
 Requires-Dist: emoji (>=2.10.1,<3.0.0)
+Requires-Dist: gptify (==0.3.2)
 Requires-Dist: groq (>=0.3.0,<0.4.0)
 Requires-Dist: mistralai (>=0.1.3,<0.2.0)
 Requires-Dist: octoai-sdk (>=0.9.0,<0.10.0)
-Requires-Dist: openai (==1.12.0)
+Requires-Dist: openai (==1.21.2)
 Requires-Dist: pip-licenses (>=4.3.4,<5.0.0)
 Requires-Dist: pyfiglet (>=1.0.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: typer (==0.9.0)
 Requires-Dist: yaspin (>=3.0.1,<4.0.0)
 Description-Content-Type: text/markdown
```


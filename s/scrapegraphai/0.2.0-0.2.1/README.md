# Comparing `tmp/scrapegraphai-0.2.0.tar.gz` & `tmp/scrapegraphai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.2.0.tar", max compression
+gzip compressed data, was "scrapegraphai-0.2.1.tar", max compression
```

## Comparing `scrapegraphai-0.2.0.tar` & `scrapegraphai-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.0/LICENSE
--rw-r--r--   0        0        0     7791 2024-04-16 18:31:56.226271 scrapegraphai-0.2.0/README.md
--rw-r--r--   0        0        0     1644 2024-04-17 17:49:15.944949 scrapegraphai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.0/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.0/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.0/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-17 12:02:40.635791 scrapegraphai-0.2.0/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3635 2024-04-14 10:41:13.044574 scrapegraphai-0.2.0/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4644 2024-04-14 10:41:13.045393 scrapegraphai-0.2.0/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2386 2024-04-17 12:02:40.635921 scrapegraphai-0.2.0/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.0/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-14 10:41:13.045562 scrapegraphai-0.2.0/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-14 10:41:13.045723 scrapegraphai-0.2.0/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.2.0/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.2.0/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.0/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.0/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.0/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.0/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.0/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.0/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.0/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.0/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.0/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.0/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      503 2024-04-17 12:02:40.636158 scrapegraphai-0.2.0/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.0/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-14 10:41:13.045957 scrapegraphai-0.2.0/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3355 2024-04-17 12:02:40.636764 scrapegraphai-0.2.0/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6893 2024-04-17 16:00:30.423051 scrapegraphai-0.2.0/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6695 2024-04-17 12:02:40.637516 scrapegraphai-0.2.0/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-16 09:55:22.963496 scrapegraphai-0.2.0/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-14 10:41:13.047465 scrapegraphai-0.2.0/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-14 10:41:13.047679 scrapegraphai-0.2.0/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4939 2024-04-14 10:41:13.048326 scrapegraphai-0.2.0/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4545 2024-04-16 09:55:22.963797 scrapegraphai-0.2.0/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-14 10:41:13.048881 scrapegraphai-0.2.0/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.0/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.2.0/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.2.0/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.0/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.0/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1454 2024-04-17 12:02:40.637920 scrapegraphai-0.2.0/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.0/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.0/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.0/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9416 1970-01-01 00:00:00.000000 scrapegraphai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7782 2024-04-19 08:24:29.305029 scrapegraphai-0.2.1/README.md
+-rw-r--r--   0        0        0     1644 2024-04-19 08:25:59.485392 scrapegraphai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-17 12:02:40.635791 scrapegraphai-0.2.1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-19 08:24:33.530797 scrapegraphai-0.2.1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4644 2024-04-14 10:41:13.045393 scrapegraphai-0.2.1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2386 2024-04-19 08:24:33.531116 scrapegraphai-0.2.1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-14 10:41:13.045562 scrapegraphai-0.2.1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-14 10:41:13.045723 scrapegraphai-0.2.1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.2.1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.2.1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      503 2024-04-17 12:02:40.636158 scrapegraphai-0.2.1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-14 10:41:13.045957 scrapegraphai-0.2.1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3355 2024-04-19 08:24:33.531603 scrapegraphai-0.2.1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6893 2024-04-17 16:00:30.423051 scrapegraphai-0.2.1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6695 2024-04-19 08:24:33.532283 scrapegraphai-0.2.1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-16 09:55:22.963496 scrapegraphai-0.2.1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-14 10:41:13.047465 scrapegraphai-0.2.1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-14 10:41:13.047679 scrapegraphai-0.2.1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4939 2024-04-14 10:41:13.048326 scrapegraphai-0.2.1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4545 2024-04-16 09:55:22.963797 scrapegraphai-0.2.1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-14 10:41:13.048881 scrapegraphai-0.2.1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.2.1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.2.1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     1454 2024-04-19 08:24:33.532803 scrapegraphai-0.2.1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 scrapegraphai-0.2.1/PKG-INFO
```

### Comparing `scrapegraphai-0.2.0/LICENSE` & `scrapegraphai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/README.md` & `scrapegraphai-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
-ScrapeGraphAI is a *web scraping* python library which uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
+ScrapeGraphAI is a *web scraping* python library that uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 
 ## 🚀 Quick install
 
-The reference page for Scrapegraph-ai is avaible on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
+The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
 ## 🔍 Demo
 Official streamlit demo:
 
@@ -39,30 +39,30 @@
 
 Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
 
 ## 💻 Usage
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
-### Case 1: Extracting informations using Ollama
+### Case 1: Extracting information using Ollama
 Remember to download the model on Ollama separately!
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
         "model": "ollama/mistral",
         "temperature": 0,
         "format": "json",  # Ollama needs the format to be specified explicitly
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
     },
     "embeddings": {
         "model": "ollama/nomic-embed-text",
         "temperature": 0,
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
     }
 }
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the articles",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects",
@@ -70,17 +70,17 @@
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 ```
 
-### Case 2: Extracting informations using Docker
+### Case 2: Extracting information using Docker
 
-Note: before using the local model remeber to create the docker container!
+Note: before using the local model remember to create the docker container!
 ```text
     docker-compose up -d
     docker exec -it ollama ollama run stablelm-zephyr
 ```
 You can use which models avaiable on Ollama or your own model instead of stablelm-zephyr
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
@@ -102,15 +102,15 @@
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
 
-### Case 3: Extracting informations using Openai model
+### Case 3: Extracting information using Openai model
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
 graph_config = {
     "llm": {
         "api_key": OPENAI_API_KEY,
@@ -125,15 +125,15 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 4: Extracting informations using Gemini 
+### Case 4: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
@@ -149,32 +149,32 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-The output for alle 3 the cases will be a dictionary with the extracted information, for example:
+The output for all 3 the cases will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
         'Rotary Pendulum RL'
         ],
     'descriptions': [
         'Open Source project aimed at controlling a real life rotary pendulum using RL algorithms'
         ]
 }
 ```
 
 ## 🤝 Contributing
 
-Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
+Feel free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
-For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
+Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraph)
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
@@ -183,15 +183,15 @@
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
     author = {Marco Perini, Lorenzo Padoan, Marco Vinciguerra},
     title = {Scrapegraph-ai},
     year = {2024},
     url = {https://github.com/VinciGit00/Scrapegraph-ai},
-    note = {A Python library for scraping data from graphs}
+    note = {A Python library for scraping leveraging large language models}
   }
 ```
 
 ## Authors
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/logo_authors.png" alt="Authors Logos">
```

### Comparing `scrapegraphai-0.2.0/pyproject.toml` & `scrapegraphai-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.2.0"
+version = "0.2.1"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
@@ -22,15 +22,15 @@
 
 [tool.poetry.dependencies]
 python = ">3.9,<4.0"
 langchain = "0.1.14"
 langchain-openai = "0.1.1"
 langchain-google-genai = "1.0.1"
 html2text = "2020.1.16"
-faiss-cpu = "1.7.4"
+faiss-cpu = "1.8.0"
 beautifulsoup4 = "4.12.3"
 pandas = "2.0.3"
 python-dotenv = "1.0.1"
 tiktoken = {version = ">=0.5.2,<0.6.0"}
 tqdm = "4.66.1"
 graphviz = "0.20.1"
 google = "3.0.0"
```

### Comparing `scrapegraphai-0.2.0/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.2.1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.2.1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.2.1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.2.1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.2.1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.2.1/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/gemini.py` & `scrapegraphai-0.2.1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.2.1/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/ollama.py` & `scrapegraphai-0.2.1/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/openai.py` & `scrapegraphai-0.2.1/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.2.1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.2.1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.2.1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/remover.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.2.1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.0/PKG-INFO` & `scrapegraphai-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.2.0
+Version: 0.2.1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (==4.12.3)
-Requires-Dist: faiss-cpu (==1.7.4)
+Requires-Dist: faiss-cpu (==1.8.0)
 Requires-Dist: google (==3.0.0)
 Requires-Dist: graphviz (==0.20.1)
 Requires-Dist: html2text (==2020.1.16)
 Requires-Dist: langchain (==0.1.14)
 Requires-Dist: langchain-google-genai (==1.0.1)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: minify-html (==0.15.0)
@@ -38,25 +38,25 @@
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
-ScrapeGraphAI is a *web scraping* python library which uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
+ScrapeGraphAI is a *web scraping* python library that uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 
 ## 🚀 Quick install
 
-The reference page for Scrapegraph-ai is avaible on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
+The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
 ## 🔍 Demo
 Official streamlit demo:
 
@@ -74,30 +74,30 @@
 
 Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
 
 ## 💻 Usage
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
-### Case 1: Extracting informations using Ollama
+### Case 1: Extracting information using Ollama
 Remember to download the model on Ollama separately!
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 
 graph_config = {
     "llm": {
         "model": "ollama/mistral",
         "temperature": 0,
         "format": "json",  # Ollama needs the format to be specified explicitly
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
     },
     "embeddings": {
         "model": "ollama/nomic-embed-text",
         "temperature": 0,
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+        "base_url": "http://localhost:11434",  # set Ollama URL arbitrarily
     }
 }
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the articles",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects",
@@ -105,17 +105,17 @@
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 ```
 
-### Case 2: Extracting informations using Docker
+### Case 2: Extracting information using Docker
 
-Note: before using the local model remeber to create the docker container!
+Note: before using the local model remember to create the docker container!
 ```text
     docker-compose up -d
     docker exec -it ollama ollama run stablelm-zephyr
 ```
 You can use which models avaiable on Ollama or your own model instead of stablelm-zephyr
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
@@ -137,15 +137,15 @@
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
 
-### Case 3: Extracting informations using Openai model
+### Case 3: Extracting information using Openai model
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
 graph_config = {
     "llm": {
         "api_key": OPENAI_API_KEY,
@@ -160,15 +160,15 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 4: Extracting informations using Gemini 
+### Case 4: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
@@ -184,32 +184,32 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-The output for alle 3 the cases will be a dictionary with the extracted information, for example:
+The output for all 3 the cases will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
         'Rotary Pendulum RL'
         ],
     'descriptions': [
         'Open Source project aimed at controlling a real life rotary pendulum using RL algorithms'
         ]
 }
 ```
 
 ## 🤝 Contributing
 
-Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
+Feel free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
-For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
+Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraph)
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
@@ -218,15 +218,15 @@
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
     author = {Marco Perini, Lorenzo Padoan, Marco Vinciguerra},
     title = {Scrapegraph-ai},
     year = {2024},
     url = {https://github.com/VinciGit00/Scrapegraph-ai},
-    note = {A Python library for scraping data from graphs}
+    note = {A Python library for scraping leveraging large language models}
   }
 ```
 
 ## Authors
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/logo_authors.png" alt="Authors Logos">
```


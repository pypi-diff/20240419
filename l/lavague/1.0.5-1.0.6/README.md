# Comparing `tmp/lavague-1.0.5.tar.gz` & `tmp/lavague-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague-1.0.5.tar", last modified: Thu Apr  4 18:08:05 2024, max compression
+gzip compressed data, was "lavague-1.0.6.tar", last modified: Fri Apr 19 15:35:22 2024, max compression
```

## Comparing `lavague-1.0.5.tar` & `lavague-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/
--rw-rw-r--   0 vscode    (1003) vscode    (1003)    11357 2024-03-13 17:11:17.000000 lavague-1.0.5/LICENSE
--rw-r--r--   0 vscode    (1003) vscode    (1003)    20848 2024-04-04 18:08:05.650190 lavague-1.0.5/PKG-INFO
--rw-r--r--   0 vscode    (1003) vscode    (1003)     5425 2024-04-04 14:09:01.000000 lavague-1.0.5/README.md
--rw-r--r--   0 vscode    (1003) vscode    (1003)     2383 2024-04-04 18:07:13.000000 lavague-1.0.5/pyproject.toml
--rw-r--r--   0 vscode    (1003) vscode    (1003)       38 2024-04-04 18:08:05.650190 lavague-1.0.5/setup.cfg
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/lavague/
--rw-r--r--   0 vscode    (1003) vscode    (1003)     4272 2024-04-04 17:28:18.000000 lavague-1.0.5/src/lavague/__init__.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     5555 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/action_engine.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     7157 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/command_center.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     1565 2024-04-04 17:50:35.000000 lavague-1.0.5/src/lavague/defaults.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)      964 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/driver.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)    11308 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/prompts.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)      494 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/telemetry.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     1547 2024-04-04 15:30:32.000000 lavague-1.0.5/src/lavague/utils.py
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/lavague.egg-info/
--rw-r--r--   0 vscode    (1003) vscode    (1003)    20848 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/PKG-INFO
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      442 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/SOURCES.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        1 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1003) vscode    (1003)       80 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/entry_points.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      893 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/requires.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        8 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.776496 lavague-1.0.6/
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)    11357 2024-03-13 17:11:17.000000 lavague-1.0.6/LICENSE
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    20739 2024-04-19 15:35:22.776496 lavague-1.0.6/PKG-INFO
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     5213 2024-04-19 15:31:38.000000 lavague-1.0.6/README.md
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     2400 2024-04-19 15:31:49.000000 lavague-1.0.6/pyproject.toml
+-rw-r--r--   0 vscode    (1003) vscode    (1003)       38 2024-04-19 15:35:22.776496 lavague-1.0.6/setup.cfg
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague/
+-rw-r--r--   0 vscode    (1003) vscode    (1003)        0 2024-04-17 21:11:17.000000 lavague-1.0.6/src/lavague/__init__.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     5625 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/action_engine.py
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague/cli/
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     3906 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/cli/commands.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     2383 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/cli/config.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     1877 2024-04-18 12:59:17.000000 lavague-1.0.6/src/lavague/cli/main.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     7160 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/command_center.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     3729 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/defaults.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     3329 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/driver.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     2101 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/format_utils.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    16696 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/prompts.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     2007 2024-04-18 13:03:11.000000 lavague-1.0.6/src/lavague/telemetry.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)      632 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/vscode_extension.py
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague.egg-info/
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    20739 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/PKG-INFO
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)      559 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/SOURCES.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)        1 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1003) vscode    (1003)       49 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/entry_points.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)      934 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/requires.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)        8 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.5/LICENSE` & `lavague-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague-1.0.5/PKG-INFO` & `lavague-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.5
+Version: 1.0.6
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -243,23 +243,26 @@
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: gradio==4.21.0
+Requires-Dist: ipython
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: cuda
 Requires-Dist: accelerate==0.28.0; extra == "cuda"
 Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
 Provides-Extra: huggingface
 Requires-Dist: llama-index-embeddings-huggingface==0.1.4; extra == "huggingface"
 Requires-Dist: llama-index-llms-huggingface==0.1.4; extra == "huggingface"
+Provides-Extra: playwright
+Requires-Dist: playwright==1.42.0; extra == "playwright"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
   <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
@@ -278,19 +281,21 @@
 </h4>
   <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+LaVague is an **open-source** project designed to automate automation for devs! 
+
+We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
 
 ### LaVague in Action
 
-Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
+Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -305,20 +310,31 @@
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
 sudo bash setup.sh
 ```
 
 2. Run your LaVague command!
+
+You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+```
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+```
+
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
 ```
-lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
 ```
 
 For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
+## 🎭 Playwright integration
+
+If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
+
 ## 🙋 Contributing
 
 We would love your help in making La Vague a reality. 
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
@@ -328,23 +344,14 @@
 5) ⬆️ You should submit your work as a PR
 6) ✅ We will review & merge your code or request changes/give feedback
 
 Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
 If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-
-## ✨ Features
-
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
-
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
 This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.5/README.md` & `lavague-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 </h4>
   <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+LaVague is an **open-source** project designed to automate automation for devs! 
+
+We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
 
 ### LaVague in Action
 
-Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
+Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -46,20 +48,31 @@
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
 sudo bash setup.sh
 ```
 
 2. Run your LaVague command!
+
+You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+```
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+```
+
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
 ```
-lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
 ```
 
 For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
+## 🎭 Playwright integration
+
+If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
+
 ## 🙋 Contributing
 
 We would love your help in making La Vague a reality. 
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
@@ -69,23 +82,14 @@
 5) ⬆️ You should submit your work as a PR
 6) ✅ We will review & merge your code or request changes/give feedback
 
 Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
 If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-
-## ✨ Features
-
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
-
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
 This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

#### html2text {}

```diff
@@ -1,54 +1,52 @@
            _[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]_[_F_o_r_k_s_]_[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_A_p_a_c_h_e_ _L_i_c_e_n_s_e_]
                                 [LaVague Logo]
                        ************ WWeellccoommee ttoo LLaaVVaagguuee ************
                    ****** _[[_JJ_oo_ii_nn_ _oo_uu_rr_ _DD_ii_ss_cc_oo_rr_dd_ _ss_ee_rr_vv_ee_rr_!!_]]_[[_DD_oo_cc_ss_]] ******
                     Copilot for devs to automate automation
-## ðââï¸ What is LaVague? LaVague is an open-source project designed to
-automate automation for devs! By turning natural language queries into Python
-code leveraging Selenium, LaVague is designed to make it easy for users to
-automate express web workflows and execute them on a browser. ### LaVague in
-Action Here's an examples to show how LaVague can execute natural lanaguge
-instructions on a browser to automate interactions with a website:
+## ðââï¸ What is LaVague? LaVague is an **open-source** project
+designed to automate automation for devs! We use **advanced AI techniques**
+(RAG, Few-shot learning, Chain of Thought) to turn **natural language
+instructions** into Python code leveraging **Selenium**. LaVague is designed to
+make it easy for users to **automate web workflows** and execute them on a
+browser. ### LaVague in Action Here's an example to show how LaVague can
+execute natural language instructions on a browser to automate interactions
+with a website:
 [LaVague Interaction Example]LLaaVVaagguuee iinntteerraaccttiinngg wwiitthh HHuuggggiinngg FFaaccee''ss wweebbssiittee..
 
 ## ð Getting Started ### Running LaVague in your local env You can get
 started with `LaVague` in 2 steps: 1. Install LaVague & dependencies ``` wget
 https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh && sudo bash
-setup.sh ``` 2. Run your LaVague command! ``` lavague-build --file_path tests/
-hf.txt --config_file examples/api/openai.py ``` For a step-by-step guide or to
-run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/
-latest/docs/get-started/quick-tour/) which will walk you through how to get
-set-up and launch LaVague with our CLI tool. ## ð Contributing We would love
-your help in making La Vague a reality. To avoid having multiple people working
-on the same things & being unable to merge your work, we have outlined the
-following contribution process: 1) ð¢ We outline tasks on our [`backlog`]
+setup.sh ``` 2. Run your LaVague command! You can either `launch` an
+interactive demo, where LaVague will execute and show you the results of the
+automation code it generates for your instruction. ``` lavague --instructions
+examples/instructions/huggingface.yaml --config examples/configurations/api/
+openai_api.py launch ``` Or you can use the `build` command to directly get the
+Python code leveraging Selenium in a file, which you can then inspect & execute
+locally. ``` lavague --instructions examples/instructions/huggingface.yaml --
+config examples/configurations/api/openai_api.py build ``` For a step-by-step
+guide or to run LaVague in a Google Colab, see our [quick-tour](https://
+docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you
+through how to get set-up and launch LaVague with our CLI tool. ## ð­
+Playwright integration If you want to get started with LaVague build using
+Playwright as your underlying automation tool, see our [Playwright integration
+guide](./docs/docs/get-started/playwright.md) ## ð Contributing We would
+love your help in making La Vague a reality. To avoid having multiple people
+working on the same things & being unable to merge your work, we have outlined
+the following contribution process: 1) ð¢ We outline tasks on our [`backlog`]
 (https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check
 out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/
 labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-
 ai/LaVague/labels/good%20first%20issue) labels 2) ðââï¸ If you are
 interested in working on one of these tasks, comment on the issue! 3) ð¤ We
 will discuss with you and assign you the task with a [`community assigned`]
 (https://github.com/lavague-ai/LaVague/labels/community-assigned) label 4) ð¬
 We will then be available to discuss this task with you 5) â¬ï¸ You should
 submit your work as a PR 6) â We will review & merge your code or request
 changes/give feedback Please check out our [`contributing guide`](./
 contributing.md) for a more detailed guide. If you want to ask questions,
 contribute, or have proposals, please come on our [`Discord`](https://
-discord.gg/SDxn9KpqX9) to chat! ## â¨ Features - **Natural Language
-Processing**: Understands instructions in natural language to perform browser
-interactions. - **Selenium Integration**: Seamlessly integrates with Selenium
-for automating web browsers. - **Open-Source**: Built on open-source projects
-such as transformers and llama-index, and compatible with open-source models,
-either locally or remote, to ensure the transparency of the agent and ensures
-that it is aligned with users' interests. - **Local models for privacy and
-control**: Supports local models like ``Gemma-7b`` so that users can fully
-control their AI assistant and have privacy guarantees. - **Advanced AI
-techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform
-RAG to extract the most relevant HTML pieces to feed the LLM answering the
-query. Then leverages Few-shot learning and Chain of Thought to elicit the most
-relevant Selenium code to perform the action without having to finetune the LLM
-for code generation. ## ðºï¸ Roadmap TO keep up to date with our project
-backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2). ### ð¨
-Disclaimer This project executes LLM-generated code using `exec`. This is not
-considered a safe practice. We therefore recommend taking extra care when using
-LaVague (such as running LaVague in a sandboxed environment)!
+discord.gg/SDxn9KpqX9) to chat! ## ðºï¸ Roadmap TO keep up to date with our
+project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
+### ð¨ Disclaimer This project executes LLM-generated code using `exec`. This
+is not considered a safe practice. We therefore recommend taking extra care
+when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.5/pyproject.toml` & `lavague-1.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["pip>=24", "setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lavague"
-version = "1.0.5"
+version = "1.0.6"
 description = "Selenium code generation from text instructions"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["IA", "AI", "selenium", "generation"]
 authors = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
@@ -51,22 +51,23 @@
   "tree-sitter==0.21.0",
   "tree-sitter-languages==1.10.2",
   "nest_asyncio==1.6.0",
   "selenium==4.18.1",
   "google-search-results==2.4.2",
   "python-dotenv==1.0.1",
   "gradio==4.21.0",
+  "ipython",
 ]
 
 [project.optional-dependencies]
 dev = ["ruff", "ipykernel"]
 cuda = ["accelerate==0.28.0", "bitsandbytes==0.42.0"]
 huggingface = ["llama-index-embeddings-huggingface==0.1.4", "llama-index-llms-huggingface==0.1.4"]
+playwright = ["playwright==1.42.0"]
 
 [project.urls]
 "Homepage" = "https://mithrilsecurity.io"
 "Bug Reports" = "https://github.com/lavague-ai/LaVague/issues"
 "Source" = "https://github.com/lavague-ai/LaVague/"
 
 [project.scripts]
-lavague-build = "lavague:build"
-lavague-launch = "lavague:launch"
+lavague = "lavague.cli.main:cli"
```

### Comparing `lavague-1.0.5/src/lavague/__init__.py` & `lavague-1.0.6/src/lavague/cli/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,121 @@
-from .telemetry import send_telemetry
-from .utils import load_action_engine, load_instructions
-from .command_center import GradioDemo
-
-import os
-import argparse
-import importlib.util
-from pathlib import Path
-from tqdm import tqdm
-import inspect
-
-import warnings
-
-warnings.filterwarnings("ignore")
-
-
-def import_from_path(path):
-    # Convert the path to a Python module path
-    module_name = Path(path).stem
-    spec = importlib.util.spec_from_file_location(module_name, path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-    return module
-
-
-def build():
-    parser = argparse.ArgumentParser(description="Process a file.")
-
-    # Add the arguments
-    parser.add_argument(
-        "--file_path", type=str, required=True, help="the path to the file"
-    )
-
-    parser.add_argument(
-        "--config_path",
-        type=str,
-        required=True,
-        help="the path to the Python config file",
-    )
-    # Execute the parse_args() method
-    args = parser.parse_args()
-
-    file_path = args.file_path
-    config_path = args.config_path
-
-    # Load the action engine and driver from config file
-    action_engine, get_driver = load_action_engine(config_path)
-
-    abstractDriver = get_driver()
-
-    # Gets the original source code of the get_driver method
-    source_code = inspect.getsource(get_driver)
-
-    # Split the source code into lines and remove the first line (method definition)
-    source_code_lines = source_code.splitlines()[1:]
-    source_code_lines = [line.strip() for line in source_code_lines[:-1]]
-
-    # Execute the import lines
-    import_lines = [
-        line
-        for line in source_code_lines
-        if line.startswith("from") or line.startswith("import")
-    ]
-    exec("\n".join(import_lines))
-
-    output = "\n".join(source_code_lines)
-
-    base_url, instructions = load_instructions(file_path)
-
-    abstractDriver.goTo(base_url)
-    output += f"\ndriver.get('{base_url.strip()}')\n"
-
-    template_code = """\n########################################\n# Query: {instruction}\n# Code:\n{code}"""
-
-    file_path = os.path.basename(file_path)
-    file_path, _ = os.path.splitext(file_path)
+from typing import Optional
+import click
+from ..format_utils import extract_code_from_funct, extract_imports_from_lines
+
+
+@click.group()
+def cli():
+    pass
+
+
+@cli.command()
+@click.pass_context
+def launch(ctx):
+    """Start a local gradio demo of lavague"""
+    from .config import Config, Instructions
+    from ..command_center import GradioDemo
+
+    config = Config.from_path(ctx.obj["config"])
+    instructions = Instructions.from_yaml(ctx.obj["instructions"])
+    action_engine = config.make_action_engine()
+    driver = config.get_driver()
+    command_center = GradioDemo(action_engine, driver)
+    command_center.run(instructions.url, instructions.instructions)
 
-    config_path = os.path.basename(config_path)
-    config_path, _ = os.path.splitext(config_path)
 
-    output_fn = file_path + "_" + config_path + "_gen.py"
+@cli.command()
+@click.option(
+    "--output-file",
+    "-o",
+    type=click.Path(exists=True),
+    required=False,
+    help="The path of the output file",
+)
+@click.pass_context
+def build(ctx, output_file: Optional[str], test: bool = False):
+    """Generate a python script that can run the successive actions in one go."""
+    from tqdm import tqdm
+    import os
+    from .config import Config, Instructions
+    from ..telemetry import send_telemetry
+    from ..action_engine import TestActionEngine
+
+    def build_name(config_path: str, instructions_path: str) -> str:
+        instructions_path = os.path.basename(instructions_path)
+        instructions_path, _ = os.path.splitext(instructions_path)
+
+        config_path = os.path.basename(config_path)
+        config_path, _ = os.path.splitext(config_path)
+
+        output_path = instructions_path + "_" + config_path + "_gen"
+        base_path = str(output_path)
+        output_path += ".py"
+        i = 1
+        while os.path.exists(output_path):
+            output_path = base_path + str(i) + ".py"
+            i += 1
+        return output_path
+
+    config: Config = Config.from_path(ctx.obj["config"])
+    instructions: Instructions = Instructions.from_yaml(ctx.obj["instructions"])
+    abstractDriver = config.get_driver()
+    if test:
+        action_engine = TestActionEngine(abstractDriver.getDummyCode())
+    else:
+        action_engine = config.make_action_engine()
+    abstractDriver.goTo(instructions.url)
+
+    source_code_lines = extract_code_from_funct(config.get_driver)
+    exec(extract_imports_from_lines(source_code_lines))
+
+    # Prepare the file
+    if output_file is None:
+        output_file = build_name(ctx.obj["config"], ctx.obj["instructions"])
+    output = "\n".join(source_code_lines)
+    output += f"\n{abstractDriver.goToUrlCode(instructions.url.strip())}\n"
+    driver_name, driver = abstractDriver.getDriver()
+    exec(f"{driver_name} = driver")  # define driver
 
-    for instruction in tqdm(instructions):
+    for instruction in tqdm(instructions.instructions):
         print(f"Processing instruction: {instruction}")
         html = abstractDriver.getHtml()
         code = action_engine.get_action(instruction, html)
         try:
-            driver = abstractDriver.getDriver()  # define driver for exec
             exec(code)
             success = True
         except Exception as e:
             print(f"Error in code execution: {code}")
             print("Error:", e)
-            print(f"Saving output to {output_fn}")
+            print(f"Saving output to {output_file}")
             success = False
-            with open(output_fn, "w") as file:
+            with open(output_file, "w") as file:
                 file.write(output)
                 break
         output += (
-            "\n" + template_code.format(instruction=instruction, code=code).strip()
+            "\n\n"
+            + "#" * 80
+            + "\n"
+            + f"# Query: {instruction}\n# Code:\n{code}".strip()
         )
         send_telemetry(
-            action_engine.llm.metadata.model_name,
+            config.llm.metadata.model_name,
             code,
-            b"",
+            "",
             html,
             instruction,
-            base_url,
+            instructions.url,
             "Lavague-build",
             success,
+            test,
         )
-
-    print(f"Saving output to {output_fn}")
-    with open(output_fn, "w") as file:
+    abstractDriver.destroy()
+    print(f"Saving output to {output_file}")
+    with open(output_file, "w") as file:
         file.write(output)
 
 
-def launch():
-    parser = argparse.ArgumentParser(description="Process a file.")
-
-    # Add the arguments
-    parser.add_argument(
-        "--file_path", type=str, required=True, help="the path to the file"
-    )
-
-    parser.add_argument(
-        "--config_path",
-        type=str,
-        required=True,
-        help="the path to the Python config file",
-    )
-    # Execute the parse_args() method
-    args = parser.parse_args()
-
-    file_path = args.file_path
-    config_path = args.config_path
-
-    # Load the action engine and driver setup function from config file
-    action_engine, get_driver = load_action_engine(config_path)
-
-    # Initialize the driver
-    driver = get_driver()
-
-    command_center = GradioDemo(action_engine, driver)
-
-    base_url, instructions = load_instructions(file_path)
-    command_center.run(base_url, instructions)
+@cli.command()
+@click.pass_context
+def test(ctx):
+    """Does a test run of LaVague build without actually querying model"""
+    ctx.invoke(build, test=True)
```

### Comparing `lavague-1.0.5/src/lavague/action_engine.py` & `lavague-1.0.6/src/lavague/action_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Callable, Optional, Generator, Tuple
+from typing import Callable, Optional, Generator
 from abc import ABC, abstractmethod
 from llama_index.core import Document
 from llama_index.core.node_parser import CodeSplitter
 from llama_index.retrievers.bm25 import BM25Retriever
 from llama_index.core import VectorStoreIndex
 from llama_index.core.query_engine import RetrieverQueryEngine
 from llama_index.core import get_response_synthesizer
 from llama_index.core import PromptTemplate
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.base.embeddings.base import BaseEmbedding
-from .prompts import DEFAULT_PROMPT
-import requests
-import re
+from .prompts import SELENIUM_PROMPT
+from .defaults import default_python_code_extractor
 
 
 class BaseActionEngine(ABC):
     """
     Abstract class for ActionEngine
     """
 
@@ -44,28 +43,14 @@
 
         Return:
             `str`: The generated code
         """
         pass
 
 
-def extract_first_python_code(markdown_text: str):
-    # Pattern to match the first ```python ``` code block
-    pattern = r"```python(.*?)```"
-
-    # Using re.DOTALL to make '.' match also newlines
-    match = re.search(pattern, markdown_text, re.DOTALL)
-    if match:
-        # Return the first matched group, which is the code inside the ```python ```
-        return match.group(1).strip()
-    else:
-        # Return None if no match is found
-        return None
-
-
 class ActionEngine(BaseActionEngine):
     """
     ActionEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         llm (`LLMPredictorType`):
             The llm that will be used the generate the python code
@@ -81,16 +66,18 @@
             A chunk can't be larger than max_chars_pc
     """
 
     def __init__(
         self,
         llm: BaseLLM,
         embedder: BaseEmbedding,
-        prompt_template: str = DEFAULT_PROMPT,
-        cleaning_function: Callable[[str], Optional[str]] = extract_first_python_code,
+        prompt_template: str = SELENIUM_PROMPT,
+        cleaning_function: Callable[
+            [str], Optional[str]
+        ] = default_python_code_extractor,
         top_k: int = 3,
         max_chars_pc: int = 1500,
     ):
         self.llm = llm
         self.embedder = embedder
         self.prompt_template = prompt_template
         self.cleaning_function = cleaning_function
@@ -160,7 +147,25 @@
         return code
 
     def get_action_streaming(self, query: str, html: str) -> Generator[str, None, None]:
         query_engine = self.get_query_engine(html, streaming=True)
         streaming_response = query_engine.query(query)
         for text in streaming_response.response_gen:
             yield text
+
+
+class TestActionEngine(BaseActionEngine):
+    """
+    TestActionEngine removes any querying and returns a default code - is used to quickly test software
+
+    Args:
+        dummy_code: (`str`)
+    """
+
+    def __init__(self, dummy_code: str):
+        self.dummy_code = dummy_code
+
+    def get_action(self, query: str, html: str) -> str:
+        return self.dummy_code
+
+    def get_action_streaming(self, query: str, html: str) -> Generator[str, None, None]:
+        return self.dummy_code
```

### Comparing `lavague-1.0.5/src/lavague/command_center.py` & `lavague-1.0.6/src/lavague/command_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         return telemetry
 
     def __exec_code(self):
         def exec_code(code, full_code):
             code = self.actionEngine.cleaning_function(code)
             html = self.driver.getHtml()
-            driver = self.driver.getDriver()  # define driver for exec
+            _, driver = self.driver.getDriver()  # define driver for exec
             try:
                 exec(code)
                 output = "Successful code execution"
                 status = """<p style="color: green; font-size: 20px; font-weight: bold;">Success!</p>"""
                 self.success = True
                 full_code += code
             except Exception as e:
```

### Comparing `lavague-1.0.5/src/lavague/prompts.py` & `lavague-1.0.6/src/lavague/prompts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFAULT_PROMPT = '''
+SELENIUM_PROMPT = '''
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
 Don't assume attribute values are unique, try use the combination of text content and class or ID if available to more precisely target the element.
 Even if there is mutliple elements doing the same action, choose the most relevant and target it precisely.
@@ -206,15 +206,15 @@
 HTML:
 {context_str}
 Query: {query_str}
 Completion:
 '''
 
 
-GEMMA_PROMPT = '''
+SELENIUM_GEMMA_PROMPT = '''
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
 You can assume the following code has been executed:
 ```python
@@ -410,12 +410,222 @@
 ```
 
 ---
 
 HTML:
 {context_str}
 Query: {query_str}
+Completion:
+```python
+# Let's proceed step by step.
+
+'''
+
+PLAYWRIGHT_PROMPT = '''
+Your goal is to write Playwright Python code to answer queries.
+
+Your answer must be a Python markdown only.
+You can have access to external websites and libraries.
+
+You can assume the following code has been executed:
+```python
+from playwright.sync_api import sync_playwright
+p = playwright().__enter__()
+browser = p.chromium.launch()
+page = browser.new_page()
+```
+
+---
+
+HTML:
+<!DOCTYPE html>
+<html>
+<head>
+    <title>Mock Search Page</title>
+</head>
+<body>
+    <h1>Search Page Example</h1>
+    <input id="searchBar" type="text" placeholder="Type here to search...">
+    <button id="searchButton">Search</button>
+    <script>
+        document.getElementById('searchButton').onclick = function() {{
+            var searchText = document.getElementById('searchBar').value;
+            alert("Searching for: " + searchText);
+        }};
+    </script>
+</body>
+</html>
+
+Query: Click on the search bar 'Type here to search...', type 'playwright', and press the 'Enter' key
+
+Completion:
+```python
+# Let's proceed step by step.
+# First we need to identify the component first, then we can click on it.
+
+# Based on the HTML, the link can be uniquely identified using the ID "searchBar"
+# Click on the search bar
+search_bar = page.locator('#searchBar')
+search_bar.click()
+
+# Type 'playwright' into the search bar
+page.type('#searchBar', 'playwright')
+
+# Press the 'Enter' key
+page.keyboard.press('Enter')
+
+```
+
+---
+
+HTML:
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <title>Mock Page for Playwright</title>
+</head>
+<body>
+    <h1>Welcome to the Mock Page</h1>
+    <div id="links">
+        <a href="#link1" id="link1">Link 1</a>
+        <br>
+        <a href="#link2" class="link">Link 2</a>
+        <br>
+    </div>
+</body>
+</html>
+
+Query: Click on the title Link 1 and then click on the title Link 2
+
+Completion:
+```python
+# Let's proceed step by step.
+# First we need to identify the first component, then we can click on it. Then we can identify the second component and click on it.
+
+# Based on the HTML, the first link the link can be uniquely identified using the ID "link1"
+# Let's use this ID with playwright to identify the link
+link1 = page.locator('#link1')
+
+# Then we click on the link
+link1.click()
+
+# The other link can be uniquely identified using the class "link"
+# Let's use this class to identify the link
+link2 = page.locator('.link')
+
+# Click on the element found
+link2.click()
+```
+
+---
+
+HTML:
+<!DOCTYPE html>
+<html>
+<head>
+    <title>Mock Page</title>
+</head>
+<body>
+    <p id="para1">This is the first paragraph.</p>
+    <p id="para2">This is the second paragraph.</p>
+    <p id="para3">This is the third paragraph, which we will select and copy.</p>
+    <p id="para4">This is the fourth paragraph.</p>
+</body>
+</html>
+
+Query: Select the text inside the third paragraph
+
+Completion:
+```python
+# Let's proceed step by step.
+
+# To select a paragraph, we can execute a JS script to select the text using the DOM
+# In the provided HTML, the third paragraph can be identified using the ID "para3"
+# We need to use getElementById to select the paragraph precisely
+js_script = """
+    // This part depends on the specific HTML, here is the identified ID "para3"
+    var para = document.getElementById('para3');
+    // The rest is standard
+    if (document.body.createTextRange) {{
+        var range = document.body.createTextRange();
+        range.moveToElementText(para);
+        range.select();
+    }} else if (window.getSelection) {{
+        var selection = window.getSelection();
+        var range = document.createRange();
+        range.selectNodeContents(para);
+        selection.removeAllRanges();
+        selection.addRange(range);
+    }}
+"""
+
+# Then we execute JavaScript
+page.evaluate(js_script)
+```
+
+---
+
+HTML:
+
+Query: Scroll up a bit
+
+Completion:
+```python
+# Let's proceed step by step.
+# We don't need to use the HTML data as this is a stateless operation.
+# 200 pixels should be sufficient. Let's execute the JavaScript to scroll up.
+
+page.evaluate("window.scrollBy(0, 200)")
+```
+
+---
+
+---
+
+HTML:
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <title>Enhanced Mock Page for Playwright Testing</title>
+</head>
+<body>
+    <h1>Enhanced Test Page for Playwright</h1>
+    <div class="container">
+        <button id="firstButton" onclick="alert('First button clicked!');">First Button</button>
+        <!-- This is the button we're targeting with the class name "action-btn" -->
+        <button class="action-btn" onclick="alert('Action button clicked!');">Action Button</button>
+        <div class="nested-container">
+            <button id="testButton" onclick="alert('Test Button clicked!');">Test Button</button>
+        </div>
+        <button class="hidden" onclick="alert('Hidden button clicked!');">Hidden Button</button>
+    </div>
+</body>
+</html>
+
+
+Query: Click on the Button 'Action Button'
+
+Completion:
+```python
+# Let's proceed step by step.
+# First we need to identify the button first, then we can click on it.
+
+# Based on the HTML provided, we need to devise the best strategy to select the button.
+# The action button can be identified using the class name "action-btn"
+action_button = page.locator('.action-btn')
+
+# Then we can click on it
+await action_button.click()
+```
+
+---
+
+HTML:
+{context_str}
+Query: {query_str}
 Completion:
 ```python
 # Let's proceed step by step.
 
 '''
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-DEFAULT_PROMPT = ''' Your goal is to write Selenium code to answer queries.
+SELENIUM_PROMPT = ''' Your goal is to write Selenium code to answer queries.
 Your answer must be a Python markdown only. You can have access to external
 websites and libraries. Don't assume attribute values are unique, try use the
 combination of text content and class or ID if available to more precisely
 target the element. Even if there is mutliple elements doing the same action,
 choose the most relevant and target it precisely. Donât forget to use
 contains@class if multi-class. You can assume the following code has been
 executed: ```python from selenium import webdriver from
@@ -57,19 +57,19 @@
 Hidden Button
 Query: Click on the Button 'First Button' Completion: ```python # Let's proceed
 step by step. # First we need to identify the button first, then we can click
 on it. # Based on the HTML provided, we need to devise the best strategy to
 select the button. # The action button can be identified using the class name
 "action-btn" action_button = driver.find_element(By.XPATH, "//*[@class='action-
 btn']") # Then we can click on it action_button.click() ``` --- HTML:
-{context_str} Query: {query_str} Completion: ''' GEMMA_PROMPT = ''' Your goal
-is to write Selenium code to answer queries. Your answer must be a Python
-markdown only. You can have access to external websites and libraries. You can
-assume the following code has been executed: ```python from selenium import
-webdriver from selenium.webdriver.common.by import By driver =
+{context_str} Query: {query_str} Completion: ''' SELENIUM_GEMMA_PROMPT = '''
+Your goal is to write Selenium code to answer queries. Your answer must be a
+Python markdown only. You can have access to external websites and libraries.
+You can assume the following code has been executed: ```python from selenium
+import webdriver from selenium.webdriver.common.by import By driver =
 webdriver.Firefox() ``` --- HTML:
 ************ SSeeaarrcchh PPaaggee EExxaammppllee ************
 [                    ]Search
 Query: Click on the search bar 'Type here to search...', type 'selenium', and
 press the 'Enter' key Completion: ```python # Let's proceed step by step. #
 First we need to identify the component first, then we can click on it. # Based
 on the HTML, the link can be uniquely identified using the ID "searchBar" #
@@ -117,8 +117,66 @@
 Query: Click on the Button 'First Button' Completion: ```python # Let's proceed
 step by step. # First we need to identify the button first, then we can click
 on it. # Based on the HTML provided, we need to devise the best strategy to
 select the button. # The action button can be identified using the class name
 "action-btn" action_button = driver.find_element(By.XPATH, "//*[@class='action-
 btn']") # Then we can click on it action_button.click() ``` --- HTML:
 {context_str} Query: {query_str} Completion: ```python # Let's proceed step by
-step. '''
+step. ''' PLAYWRIGHT_PROMPT = ''' Your goal is to write Playwright Python code
+to answer queries. Your answer must be a Python markdown only. You can have
+access to external websites and libraries. You can assume the following code
+has been executed: ```python from playwright.sync_api import sync_playwright p
+= playwright().__enter__() browser = p.chromium.launch() page =
+browser.new_page() ``` --- HTML:
+************ SSeeaarrcchh PPaaggee EExxaammppllee ************
+[                    ]Search
+Query: Click on the search bar 'Type here to search...', type 'playwright', and
+press the 'Enter' key Completion: ```python # Let's proceed step by step. #
+First we need to identify the component first, then we can click on it. # Based
+on the HTML, the link can be uniquely identified using the ID "searchBar" #
+Click on the search bar search_bar = page.locator('#searchBar')
+search_bar.click() # Type 'playwright' into the search bar page.type
+('#searchBar', 'playwright') # Press the 'Enter' key page.keyboard.press
+('Enter') ``` --- HTML:
+************ WWeellccoommee ttoo tthhee MMoocckk PPaaggee ************
+_L_i_n_k_ _1
+_L_i_n_k_ _2
+Query: Click on the title Link 1 and then click on the title Link 2 Completion:
+```python # Let's proceed step by step. # First we need to identify the first
+component, then we can click on it. Then we can identify the second component
+and click on it. # Based on the HTML, the first link the link can be uniquely
+identified using the ID "link1" # Let's use this ID with playwright to identify
+the link link1 = page.locator('#link1') # Then we click on the link link1.click
+() # The other link can be uniquely identified using the class "link" # Let's
+use this class to identify the link link2 = page.locator('.link') # Click on
+the element found link2.click() ``` --- HTML:
+This is the first paragraph.
+This is the second paragraph.
+This is the third paragraph, which we will select and copy.
+This is the fourth paragraph.
+Query: Select the text inside the third paragraph Completion: ```python # Let's
+proceed step by step. # To select a paragraph, we can execute a JS script to
+select the text using the DOM # In the provided HTML, the third paragraph can
+be identified using the ID "para3" # We need to use getElementById to select
+the paragraph precisely js_script = """ // This part depends on the specific
+HTML, here is the identified ID "para3" var para = document.getElementById
+('para3'); // The rest is standard if (document.body.createTextRange) {{ var
+range = document.body.createTextRange(); range.moveToElementText(para);
+range.select(); }} else if (window.getSelection) {{ var selection =
+window.getSelection(); var range = document.createRange();
+range.selectNodeContents(para); selection.removeAllRanges(); selection.addRange
+(range); }} """ # Then we execute JavaScript page.evaluate(js_script) ``` --
+- HTML: Query: Scroll up a bit Completion: ```python # Let's proceed step by
+step. # We don't need to use the HTML data as this is a stateless operation. #
+200 pixels should be sufficient. Let's execute the JavaScript to scroll up.
+page.evaluate("window.scrollBy(0, 200)") ``` --- --- HTML:
+************ EEnnhhaanncceedd TTeesstt PPaaggee ffoorr PPllaayywwrriigghhtt ************
+First Button Action Button
+Test Button
+Hidden Button
+Query: Click on the Button 'Action Button' Completion: ```python # Let's
+proceed step by step. # First we need to identify the button first, then we can
+click on it. # Based on the HTML provided, we need to devise the best strategy
+to select the button. # The action button can be identified using the class
+name "action-btn" action_button = page.locator('.action-btn') # Then we can
+click on it await action_button.click() ``` --- HTML: {context_str} Query:
+{query_str} Completion: ```python # Let's proceed step by step. '''
```

### Comparing `lavague-1.0.5/src/lavague.egg-info/PKG-INFO` & `lavague-1.0.6/src/lavague.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.5
+Version: 1.0.6
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -243,23 +243,26 @@
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: gradio==4.21.0
+Requires-Dist: ipython
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: cuda
 Requires-Dist: accelerate==0.28.0; extra == "cuda"
 Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
 Provides-Extra: huggingface
 Requires-Dist: llama-index-embeddings-huggingface==0.1.4; extra == "huggingface"
 Requires-Dist: llama-index-llms-huggingface==0.1.4; extra == "huggingface"
+Provides-Extra: playwright
+Requires-Dist: playwright==1.42.0; extra == "playwright"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
   <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
@@ -278,19 +281,21 @@
 </h4>
   <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+LaVague is an **open-source** project designed to automate automation for devs! 
+
+We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
 
 ### LaVague in Action
 
-Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
+Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -305,20 +310,31 @@
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
 sudo bash setup.sh
 ```
 
 2. Run your LaVague command!
+
+You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+```
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+```
+
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
 ```
-lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
 ```
 
 For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
+## 🎭 Playwright integration
+
+If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
+
 ## 🙋 Contributing
 
 We would love your help in making La Vague a reality. 
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
@@ -328,23 +344,14 @@
 5) ⬆️ You should submit your work as a PR
 6) ✅ We will review & merge your code or request changes/give feedback
 
 Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
 If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-
-## ✨ Features
-
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
-
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
 This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.5/src/lavague.egg-info/requires.txt` & `lavague-1.0.6/src/lavague.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,23 @@
 tree-sitter==0.21.0
 tree-sitter-languages==1.10.2
 nest_asyncio==1.6.0
 selenium==4.18.1
 google-search-results==2.4.2
 python-dotenv==1.0.1
 gradio==4.21.0
+ipython
 
 [cuda]
 accelerate==0.28.0
 bitsandbytes==0.42.0
 
 [dev]
 ruff
 ipykernel
 
 [huggingface]
 llama-index-embeddings-huggingface==0.1.4
 llama-index-llms-huggingface==0.1.4
+
+[playwright]
+playwright==1.42.0
```


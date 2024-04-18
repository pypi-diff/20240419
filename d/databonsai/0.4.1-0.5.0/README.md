# Comparing `tmp/databonsai-0.4.1.tar.gz` & `tmp/databonsai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.4.1.tar", last modified: Wed Apr 17 06:25:30 2024, max compression
+gzip compressed data, was "databonsai-0.5.0.tar", last modified: Thu Apr 18 23:33:01 2024, max compression
```

## Comparing `databonsai-0.4.1.tar` & `databonsai-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.479673 databonsai-0.4.1/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     8261 2024-04-17 06:25:30.476498 databonsai-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     7405 2024-04-17 05:30:10.000000 databonsai-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.439505 databonsai-0.4.1/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.4.1/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.460499 databonsai-0.4.1/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.4.1/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     7516 2024-04-17 06:22:37.000000 databonsai-0.4.1/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     5634 2024-04-17 06:22:44.000000 databonsai-0.4.1/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.466500 databonsai-0.4.1/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      471 2024-04-07 00:16:34.000000 databonsai-0.4.1/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     5805 2024-04-17 05:14:05.000000 databonsai-0.4.1/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     2047 2024-04-07 20:19:59.000000 databonsai-0.4.1/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     5942 2024-04-17 06:22:58.000000 databonsai-0.4.1/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.469499 databonsai-0.4.1/databonsai/transform/
--rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.4.1/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     5564 2024-04-17 05:51:57.000000 databonsai-0.4.1/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     9886 2024-04-17 06:08:58.000000 databonsai-0.4.1/databonsai/transform/decompose_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.471500 databonsai-0.4.1/databonsai/utils/
--rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.4.1/databonsai/utils/__init__.py
--rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.4.1/databonsai/utils/apply.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.475499 databonsai-0.4.1/databonsai.egg-info/
--rw-rw-rw-   0        0        0     8261 2024-04-17 06:25:30.000000 databonsai-0.4.1/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-17 06:25:30.000000 databonsai-0.4.1/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:25:30.000000 databonsai-0.4.1/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-17 06:25:30.000000 databonsai-0.4.1/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 06:25:30.000000 databonsai-0.4.1/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2024-04-17 06:25:23.000000 databonsai-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 06:25:30.479673 databonsai-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-04-17 06:25:27.000000 databonsai-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:25:30.473502 databonsai-0.4.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.4.1/tests/__init__.py
--rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.4.1/tests/test_categorization.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.726221 databonsai-0.5.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     8368 2024-04-18 23:33:01.724211 databonsai-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7489 2024-04-18 21:28:28.000000 databonsai-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.632252 databonsai-0.5.0/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.5.0/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.681449 databonsai-0.5.0/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.5.0/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0     7771 2024-04-18 21:45:39.000000 databonsai-0.5.0/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     5634 2024-04-17 06:22:44.000000 databonsai-0.5.0/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.700304 databonsai-0.5.0/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.5.0/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.5.0/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.5.0/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.5.0/databonsai/llm_providers/ollama_provider.py
+-rw-rw-rw-   0        0        0     6266 2024-04-18 21:09:07.000000 databonsai-0.5.0/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.714712 databonsai-0.5.0/databonsai/transform/
+-rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.5.0/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     5564 2024-04-17 05:51:57.000000 databonsai-0.5.0/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     9886 2024-04-17 06:08:58.000000 databonsai-0.5.0/databonsai/transform/decompose_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/databonsai/utils/
+-rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.5.0/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.5.0/databonsai/utils/apply.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     8368 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      580 2024-04-18 23:32:31.000000 databonsai-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 23:33:01.726221 databonsai-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-18 23:32:21.000000 databonsai-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.5.0/tests/test_categorization.py
```

### Comparing `databonsai-0.4.1/LICENSE` & `databonsai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.4.1/PKG-INFO` & `databonsai-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.4.1
+Version: 0.5.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: anthropic
 Requires-Dist: tenacity
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: anthropic
+Requires-Dist: ollama
 
 # databonsai <img width="64" height="64" src="https://img.icons8.com/external-justicon-flat-justicon/64/external-bonsai-tree-justicon-flat-justicon.png" alt="external-bonsai-tree-justicon-flat-justicon"/>
 
 [![PyPI version](https://badge.fury.io/py/databonsai.svg)](https://badge.fury.io/py/databonsai)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/pypi/pyversions/databonsai.svg)](https://pypi.org/project/databonsai/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -75,15 +76,15 @@
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
 few_shot_examples = [
         {"example": "Big stormy skies over city", "response": "Weather"},
         {"example": "The team won the championship", "response": "Sports"},
         {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
-    ],
+    ]
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
@@ -200,15 +201,16 @@
 ```python
 print(categorizer.system_message)
 print(categorizer.system_message_batch)
 ```
 
 ### View token usage
 
-Token usage is recorded for each provider. Use these to estimate your costs!
+Token usage is recorded for OpenAI and Anthropic. Use these to estimate your
+costs!
 
 ```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
@@ -218,21 +220,23 @@
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
 -   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
     a structured format based on a schema
+-   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
--   CustomProvider (TBD)
+-   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
+-   .. more coming soon!
 
-### Examples (TBD)
+### Examples
 
 -   [Examples](./databonsai/examples/) (TBD)
 
 ### Acknowledgements
 
 Bonsai icon from icons8 https://icons8.com/icon/74uBtdDr5yFq/bonsai
```

### Comparing `databonsai-0.4.1/README.md` & `databonsai-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
 few_shot_examples = [
         {"example": "Big stormy skies over city", "response": "Weather"},
         {"example": "The team won the championship", "response": "Sports"},
         {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
-    ],
+    ]
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
@@ -176,15 +176,16 @@
 ```python
 print(categorizer.system_message)
 print(categorizer.system_message_batch)
 ```
 
 ### View token usage
 
-Token usage is recorded for each provider. Use these to estimate your costs!
+Token usage is recorded for OpenAI and Anthropic. Use these to estimate your
+costs!
 
 ```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
@@ -194,21 +195,23 @@
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
 -   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
     a structured format based on a schema
+-   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
--   CustomProvider (TBD)
+-   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
+-   .. more coming soon!
 
-### Examples (TBD)
+### Examples
 
 -   [Examples](./databonsai/examples/) (TBD)
 
 ### Acknowledgements
 
 Bonsai icon from icons8 https://icons8.com/icon/74uBtdDr5yFq/bonsai
```

### Comparing `databonsai-0.4.1/databonsai/categorize/base_categorizer.py` & `databonsai-0.5.0/databonsai/categorize/base_categorizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 raise ValueError("Each example must be a dictionary.")
             if "example" not in example or "response" not in example:
                 raise ValueError(
                     "Each example dictionary must have 'example' and 'response' keys."
                 )
         return v
 
-    @model_validator(mode='after')
+    @model_validator(mode="after")
     def validate_examples_responses(self):
         """
         Validates that the "response" values in the examples are within the categories keys.
         """
 
         if self.examples:
             category_keys = set(self.categories.keys())
@@ -100,15 +100,15 @@
         # Add in fewshot examples
         if self.examples:
             for example in self.examples:
                 system_message += (
                     f"\nEXAMPLE: {example['example']}  RESPONSE: {example['response']}"
                 )
         return system_message
-    
+
     @computed_field
     @property
     def system_message_batch(self) -> str:
         system_message = f"""
         Each category is formatted as <category>: <description of data that fits the category>
         {str(self.categories)}
         Classify each given text snippet into one of the following categories:
@@ -119,19 +119,19 @@
         Only reply with the categories. Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             system_message += "\n EXAMPLE:"
             for idx, example in enumerate(self.examples):
-                system_message += (
-                    f"Content {idx+1}: {example['example']}, ")
-            system_message += f"\n RESPONSE: {",".join([example['response'] for example in self.examples])}"
+                system_message += f"Content {idx+1}: {example['example']}, "
+            system_message += f"\n RESPONSE: {','.join([example['response'] for example in self.examples])}"
 
         return system_message
+
     def categorize(self, input_data: str) -> str:
         """
         Categorizes the input data using the specified LLM provider.
 
         Args:
             input_data (str): The text data to be categorized.
 
@@ -162,24 +162,34 @@
 
         Returns:
             List[str]: A list of predicted categories for the input data.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
-        
+
         # Call the LLM provider to get the predicted category
-        response = self.llm_provider.generate_batch(self.system_message_batch, input_data)
+        response = self.llm_provider.generate_batch(
+            self.system_message_batch, input_data
+        )
         predicted_categories = [category.strip() for category in response.split("||")]
         if len(predicted_categories) != len(input_data):
             raise ValueError(
                 f"Number of predicted categories ({len(predicted_categories)}) does not match the number of input data ({len(input_data)})."
             )
         return self.validate_predicted_categories(predicted_categories)
 
-    def validate_predicted_categories(self, predicted_categories: List[str]):
-        for predicted_category in predicted_categories:
+    def validate_predicted_categories(
+        self, predicted_categories: List[str]
+    ) -> List[str]:
+        # Filter out empty strings from the predicted categories
+        filtered_categories = [
+            category for category in predicted_categories if category
+        ]
+
+        # Validate each category in the filtered list
+        for predicted_category in filtered_categories:
             if predicted_category not in self.categories:
                 raise ValueError(
                     f"Predicted category '{predicted_category}' is not one of the provided categories."
                 )
-        return predicted_categories
+        return filtered_categories
```

### Comparing `databonsai-0.4.1/databonsai/categorize/multi_categorizer.py` & `databonsai-0.5.0/databonsai/categorize/multi_categorizer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.4.1/databonsai/llm_providers/anthropic_provider.py` & `databonsai-0.5.0/databonsai/llm_providers/anthropic_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
         Parameters:
         api_key (str): Anthropic API key.
         multiplier (int): The multiplier for the exponential backoff in retries.
         min_wait (int): The minimum wait time between retries.
         max_wait (int): The maximum wait time between retries.
         max_tries (int): The maximum number of attempts before giving up.
+        model (str): The default model to use for text generation.
         temperature (float): The temperature parameter for text generation.
         """
         super().__init__()
 
         # Provider related configs
         if api_key:
             self.api_key = api_key
@@ -72,24 +73,23 @@
                 stop=stop_after_attempt(self.max_tries),
             )
             return retry_decorator(method)(self, *args, **kwargs)
 
         return wrapper
 
     @retry_with_exponential_backoff
-    def generate(
-        self, system_prompt: str, user_prompt: str, max_tokens=1000, json=False
-    ) -> str:
+    def generate(self, system_prompt: str, user_prompt: str, max_tokens=1000) -> str:
         """
         Generates a text completion using Anthropic's Claude API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
+        max_tokens (int): The maximum number of tokens to generate in the response.
 
         Returns:
         str: The generated text completion.
         """
         if not system_prompt:
             raise ValueError("System prompt is required.")
         if not user_prompt:
@@ -113,23 +113,24 @@
         )
         self.input_tokens += response.usage.input_tokens
         self.output_tokens += response.usage.output_tokens
         return response.content[0].text
 
     # @retry_with_exponential_backoff
     def generate_batch(
-        self, system_prompt: str, user_prompts: List[str], max_tokens=1000, json=False
+        self, system_prompt: str, user_prompts: List[str], max_tokens=1000
     ) -> str:
         """
         Generates a text completion using OpenAI's API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
+        max_tokens (int): The maximum number of tokens to generate in the response.
 
         Returns:
         str: The generated text completion.
         """
         if not system_prompt:
             raise ValueError("System prompt is required.")
         if len(user_prompts) == 0:
```

### Comparing `databonsai-0.4.1/databonsai/llm_providers/openai_provider.py` & `databonsai-0.5.0/databonsai/llm_providers/openai_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
         Parameters:
         api_key (str): OpenAI API key.
         multiplier (int): The multiplier for the exponential backoff in retries.
         min_wait (int): The minimum wait time between retries.
         max_wait (int): The maximum wait time between retries.
         max_tries (int): The maximum number of attempts before giving up.
+        model (str): The default model to use for text generation.
         temperature (float): The temperature parameter for text generation.
         """
         super().__init__()
 
         # Provider related configs
         if api_key:
             self.api_key = api_key
@@ -86,14 +87,16 @@
         """
         Generates a text completion using OpenAI's API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
+        max_tokens (int): The maximum number of tokens to generate in the response.
+        json (bool): Whether to use OpenAI's JSON response format.
 
         Returns:
         str: The generated text completion.
         """
         if not system_prompt:
             raise ValueError("System prompt is required.")
         if not user_prompt:
@@ -102,34 +105,35 @@
             model=self.model,
             messages=[
                 {"role": "system", "content": system_prompt},
                 {"role": "user", "content": f"{user_prompt}"},
             ],
             temperature=self.temperature,
             max_tokens=max_tokens,
-            top_p=0.1,
             frequency_penalty=0,
             presence_penalty=0,
             response_format={"type": "json_object"} if json else {"type": "text"},
         )
         self.input_tokens += response.usage.prompt_tokens
         self.output_tokens += response.usage.completion_tokens
         return response.choices[0].message.content
 
-    # @retry_with_exponential_backoff
+    @retry_with_exponential_backoff
     def generate_batch(
         self, system_prompt: str, user_prompts: List[str], max_tokens=1000, json=False
     ) -> str:
         """
         Generates a text completion using OpenAI's API, with a given system and user prompt.
         This method is decorated with retry logic to handle temporary failures.
 
         Parameters:
         system_prompt (str): The system prompt to provide context or instructions for the generation.
         user_prompt (str): The user's prompt, based on which the text completion is generated.
+        max_tokens (int): The maximum number of tokens to generate in the response.
+        json (bool): Whether to use OpenAI's JSON response format.
 
         Returns:
         str: The generated text completion.
         """
         if not system_prompt:
             raise ValueError("System prompt is required.")
         if len(user_prompts) == 0:
@@ -142,15 +146,14 @@
             {"role": "user", "content": input_data_prompt},
         ]
         response = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             temperature=self.temperature,
             max_tokens=max_tokens,
-            top_p=0.1,
             frequency_penalty=0,
             presence_penalty=0,
             response_format={"type": "json_object"} if json else {"type": "text"},
         )
         self.input_tokens += response.usage.prompt_tokens
         self.output_tokens += response.usage.completion_tokens
         return response.choices[0].message.content
```

### Comparing `databonsai-0.4.1/databonsai/transform/base_transformer.py` & `databonsai-0.5.0/databonsai/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.4.1/databonsai/transform/decompose_transformer.py` & `databonsai-0.5.0/databonsai/transform/decompose_transformer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.4.1/databonsai/utils/apply.py` & `databonsai-0.5.0/databonsai/utils/apply.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.4.1/databonsai.egg-info/PKG-INFO` & `databonsai-0.5.0/databonsai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.4.1
+Version: 0.5.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: anthropic
 Requires-Dist: tenacity
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: anthropic
+Requires-Dist: ollama
 
 # databonsai <img width="64" height="64" src="https://img.icons8.com/external-justicon-flat-justicon/64/external-bonsai-tree-justicon-flat-justicon.png" alt="external-bonsai-tree-justicon-flat-justicon"/>
 
 [![PyPI version](https://badge.fury.io/py/databonsai.svg)](https://badge.fury.io/py/databonsai)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/pypi/pyversions/databonsai.svg)](https://pypi.org/project/databonsai/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -75,15 +76,15 @@
     "Others": "Comments do not fit into any of the above categories",
     "Anomaly": "Data that does not look like comments or natural language",
 }
 few_shot_examples = [
         {"example": "Big stormy skies over city", "response": "Weather"},
         {"example": "The team won the championship", "response": "Sports"},
         {"example": "I saw a famous rapper at the mall", "response": "Celebrities"},
-    ],
+    ]
 ```
 
 Categorize your data:
 
 ```python
 categorizer = BaseCategorizer(
     categories=categories,
@@ -200,15 +201,16 @@
 ```python
 print(categorizer.system_message)
 print(categorizer.system_message_batch)
 ```
 
 ### View token usage
 
-Token usage is recorded for each provider. Use these to estimate your costs!
+Token usage is recorded for OpenAI and Anthropic. Use these to estimate your
+costs!
 
 ```python
 print(provder.input_tokens)
 print(provder.output_tokens)
 ```
 
 ## [Docs](./docs/)
@@ -218,21 +220,23 @@
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
 -   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
     a structured format based on a schema
+-   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
--   CustomProvider (TBD)
+-   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
+-   .. more coming soon!
 
-### Examples (TBD)
+### Examples
 
 -   [Examples](./databonsai/examples/) (TBD)
 
 ### Acknowledgements
 
 Bonsai icon from icons8 https://icons8.com/icon/74uBtdDr5yFq/bonsai
```

### Comparing `databonsai-0.4.1/databonsai.egg-info/SOURCES.txt` & `databonsai-0.5.0/databonsai.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 databonsai.egg-info/top_level.txt
 databonsai/categorize/__init__.py
 databonsai/categorize/base_categorizer.py
 databonsai/categorize/multi_categorizer.py
 databonsai/llm_providers/__init__.py
 databonsai/llm_providers/anthropic_provider.py
 databonsai/llm_providers/llm_provider.py
+databonsai/llm_providers/ollama_provider.py
 databonsai/llm_providers/openai_provider.py
 databonsai/transform/__init__.py
 databonsai/transform/base_transformer.py
 databonsai/transform/decompose_transformer.py
 databonsai/utils/__init__.py
 databonsai/utils/apply.py
 tests/__init__.py
```

### Comparing `databonsai-0.4.1/pyproject.toml` & `databonsai-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.4.1"
+version = "0.5.0"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
 anthropic = "^0.23.1"
 tenacity = "^8.2.3"
 python-dotenv = "^1.0.1"
 pydantic = "^2.6.4"
 pydantic_core = "^2.16.3"
+ollama = "^0.1.0"
 
 [tool.poetry.dev-dependencies]
 # Add development dependencies here (if any)
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `databonsai-0.4.1/setup.py` & `databonsai-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.4.1",
+    version="0.5.0",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
     install_requires=[
         "openai",
         "anthropic",
         "tenacity",
         "python-dotenv",
         "pydantic",
         "anthropic",
+        "ollama",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `databonsai-0.4.1/tests/test_categorization.py` & `databonsai-0.5.0/tests/test_categorization.py`

 * *Files identical despite different names*


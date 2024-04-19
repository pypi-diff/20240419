# Comparing `tmp/prompt_learner-0.1.7.tar.gz` & `tmp/prompt_learner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.1.7.tar", max compression
+gzip compressed data, was "prompt_learner-0.1.8.tar", max compression
```

## Comparing `prompt_learner-0.1.7.tar` & `prompt_learner-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.1.7/README.md
--rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.1.7/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.1.7/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      240 2024-04-11 03:34:45.465265 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2024-04-11 03:18:16.055309 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc
--rw-r--r--   0        0        0     1470 2024-04-11 03:12:44.449954 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.1.7/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1261 2024-04-11 03:18:09.033090 prompt_learner-0.1.7/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      597 2024-04-11 03:12:12.072973 prompt_learner-0.1.7/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.1.7/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.1.7/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.1.7/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.1.7/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.1.7/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.1.7/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.1.7/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.1.7/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.1.7/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.1.7/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.1.7/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      623 2024-04-11 03:17:38.543493 prompt_learner-0.1.7/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1009 2024-04-18 07:04:18.022386 prompt_learner-0.1.7/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.1.7/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      614 2024-04-18 01:51:33.806026 prompt_learner-0.1.7/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.1.7/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.1.7/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.1.7/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.1.7/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     3104 2024-04-18 06:59:46.552014 prompt_learner-0.1.7/prompt_learner/templates/anthropic_template.py
--rw-r--r--   0        0        0     2746 2024-04-18 07:20:36.951484 prompt_learner-0.1.7/prompt_learner/templates/openai_template.py
--rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.1.7/prompt_learner/templates/template.py
--rw-r--r--   0        0        0      428 2024-04-18 07:50:09.607958 prompt_learner-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 prompt_learner-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.1.8/README.md
+-rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.1.8/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.1.8/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-11 03:34:45.465265 prompt_learner-0.1.8/prompt_learner/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2024-04-11 03:18:16.055309 prompt_learner-0.1.8/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc
+-rw-r--r--   0        0        0     1470 2024-04-11 03:12:44.449954 prompt_learner-0.1.8/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.1.8/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0     1261 2024-04-11 03:18:09.033090 prompt_learner-0.1.8/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      597 2024-04-11 03:12:12.072973 prompt_learner-0.1.8/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.1.8/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.1.8/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.1.8/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.1.8/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.1.8/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.1.8/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.1.8/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.1.8/prompt_learner/optimizers/descriptors/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.1.8/prompt_learner/optimizers/descriptors/descriptor.py
+-rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.1.8/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.1.8/prompt_learner/optimizers/selectors/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.1.8/prompt_learner/optimizers/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.1.8/prompt_learner/optimizers/selectors/random_sampler.py
+-rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.1.8/prompt_learner/optimizers/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.1.8/prompt_learner/optimizers/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.1.8/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-18 08:15:47.085207 prompt_learner-0.1.8/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1005 2024-04-18 08:13:03.030889 prompt_learner-0.1.8/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.1.8/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-18 01:51:33.806026 prompt_learner-0.1.8/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.1.8/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.1.8/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.1.8/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.1.8/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2844 2024-04-18 08:23:15.734126 prompt_learner-0.1.8/prompt_learner/templates/anthropic_template.py
+-rw-r--r--   0        0        0     2562 2024-04-18 08:31:06.348404 prompt_learner-0.1.8/prompt_learner/templates/openai_template.py
+-rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.1.8/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0      428 2024-04-18 08:32:56.461647 prompt_learner-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 prompt_learner-0.1.8/PKG-INFO
```

### Comparing `prompt_learner-0.1.7/README.md` & `prompt_learner-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/.DS_Store` & `prompt_learner-0.1.8/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc` & `prompt_learner-0.1.8/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc` & `prompt_learner-0.1.8/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.1.8/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/adapters/openai.py` & `prompt_learner-0.1.8/prompt_learner/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.1.8/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.1.8/prompt_learner/optimizers/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.1.8/prompt_learner/optimizers/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.1.8/prompt_learner/optimizers/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.1.8/prompt_learner/optimizers/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/prompts/cot.py` & `prompt_learner-0.1.8/prompt_learner/prompts/cot.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,12 @@
 from .prompt import Prompt
 
 
 class CoT(Prompt):
     """Think step by step"""
     custom_intructions: str = Field(description="""Custom intructions for Chain
                                  of Thought Prompting""",
-                                 default="Think step by step.")
+                                 default="Think step by step.\n")
     
     def assemble_prompt(self):
         """Assemble the prompt."""
-        self.prompt = f"""{self.template.descriptor}\n
-        {self.template.examples_preamble}
-        \n{self.template.format_examples(self.selector.selected_examples)}
-        \n{self.custom_intructions}"""
+        self.prompt = f"""{self.template.descriptor}{self.template.examples_preamble}{self.template.format_examples(self.selector.selected_examples)}{self.custom_intructions}"""
```

### Comparing `prompt_learner-0.1.7/prompt_learner/prompts/prompt.py` & `prompt_learner-0.1.8/prompt_learner/prompts/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     prompt: str = Field(description="Final prompt string.", default="")
 
     def select_examples(self):
         """Select examples for the task."""
     
     def assemble_prompt(self):
         """Assemble the prompt."""
-        self.prompt = f"""{self.template.descriptor}\n{self.template.examples_preamble}
-        \n{self.template.format_examples(self.selector.selected_examples)}"""
+        self.prompt = f"""{self.template.descriptor}{self.template.examples_preamble}
+        {self.template.format_examples(self.selector.selected_examples)}"""
 
     def add_inference(self, text: str, context: str = ""):
         """Add inference sample"""
         self.prompt = self.prompt + self.template.add_prediction_sample(text,context)
```

### Comparing `prompt_learner-0.1.7/prompt_learner/tasks/classification.py` & `prompt_learner-0.1.8/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/tasks/tagging.py` & `prompt_learner-0.1.8/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/tasks/task.py` & `prompt_learner-0.1.8/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/prompt_learner/templates/anthropic_template.py` & `prompt_learner-0.1.8/prompt_learner/templates/openai_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,46 @@
-"""This module contains the AnthropicCompletionTemplate class"""
+"""This module contains the OpenAICompletionTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class AnthropicCompletionTemplate(Template):
-    """This class generates a template for Anthropic completions"""
+class OpenAICompletionTemplate(Template):
+    """This class generates a template for OpenAI completions"""
+    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
-        self.descriptor = f"""You are a helpful AI assistant.
-        You are helping a user with a {self.task_type} task.
-        You have to perform the following task.
-        <task_description>{self.task_description}</task_description>"""
+        self.descriptor = f"""You are a helpful AI assistant.\nYou are helping a user with a {self.task_type} task.\nThe user gives you the following task description.\n{self.task_description}\n"""
         if self.allowed_labels:
-            self.descriptor += """You have to select from the following labels.
-        <allowed_labels>{self.allowed_labels}</allowed_labels>"""
+            self.descriptor += f"""You have to select from the following labels.\n{self.allowed_labels}."""
         if self.task_type in tasks_with_labels:
-            self.prediction_preamble = f"""Given the text, you have
-        to now predict the labels from
-        list of allowed labels - {self.allowed_labels}
-        Output only the label(s) and close the <label> tag."""
+            self.prediction_preamble = f"""Given the text, you have to now predict the labels from the list of allowed labels - {self.allowed_labels}."""
         elif self.task_type == "SQLGeneration":
-            self.prediction_preamble = """Given the text, you have
-        to now generate a SQL query. Only the SQL query is expected."""
+            self.prediction_preamble = """Given the text, you have to now generate a SQL query."""
         else:  #generic preamble for prediction
             self.prediction_preamble = """Given the text, you have to now predict."""
-        self.examples_preamble = """ Here are a few examples to
-        help you understand the task better."""
-    
+        self.examples_preamble = """Here are a few examples to help you understand the task better.\n"""
+       
     def format_examples(self, examples: List[Example]):
         """Formats the task examples into a string."""
         tasks_with_labels = ["Classification", "Tagging"]
         examples_str = ""
         for example in examples:
             if self.task_type in tasks_with_labels:
-                examples_str += f"""
-                <example>
-                <text> {example.text}</text>\n
-                <label> {example.label}</label>\n
-                </example>"""
+                examples_str += f"""text: {example.text}\nlabel: {example.label}\n"""
             elif self.task_type == "SQLGeneration":
+                examples_str += f"""schema: {example.context}\ntext: {example.text}\nSQL: {example.label}\n"""
+            else: #generic example format
                 examples_str += f"""
-                <example>
-                <schema> {example.context}</schema>\n
-                <text> {example.text}</text>\n
-                <SQL> {example.label}</SQL>\n
-                </example>"""
-            else:
-                examples_str += f"""
-                <example>
-                <text> {example.text}</text>\n
-                <output> {example.label}</output>\n
-                </example>"""
+                text: {example.text}\noutput: {example.label}\n"""
         return examples_str
-    
-    def add_prediction_sample(self, text: str, context: str):
+
+    def add_prediction_sample(self, text: str, context: str = None):
         """Add prediction sample to task."""
         tasks_with_labels = ["Classification", "Tagging"]
-        prediction_preamble = self.prediction_preamble + f"""\n <text> {text} <text>"""
         if self.task_type in tasks_with_labels:
-            return prediction_preamble + "<label>"
+            return self.prediction_preamble + f"""\ntext: {text}"""+ "\nlabel:"
         elif self.task_type == "SQLGeneration":
-            return prediction_preamble + f"""\n <schema>{context} <\schema>\m <SQL>"""
+            return self.prediction_preamble + f"""\nschema: {context}\ntext: {text}\nSQL: """
         else:
-            return prediction_preamble + "<output>"
+            return self.prediction_preamble + "\noutput:"
```

### Comparing `prompt_learner-0.1.7/prompt_learner/templates/openai_template.py` & `prompt_learner-0.1.8/prompt_learner/templates/anthropic_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,45 @@
-"""This module contains the OpenAICompletionTemplate class"""
+"""This module contains the AnthropicCompletionTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class OpenAICompletionTemplate(Template):
-    """This class generates a template for OpenAI completions"""
-    
+class AnthropicCompletionTemplate(Template):
+    """This class generates a template for Anthropic completions"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
-        self.descriptor = f"""You are a helpful AI assistant.
-        You are helping a user with a {self.task_type} task.
-        The user asks you to {self.task_description}."""
+        self.descriptor = f"""You are a helpful AI assistant.\nYou are helping a user with a {self.task_type} task.\nThe user gives you the following task description.\n<task_description>{self.task_description}</task_description>\n"""
         if self.allowed_labels:
-            self.descriptor += """You have to select from the following labels.
-            {self.allowed_labels}."""
+            self.descriptor += """You have to select from the following labels.\n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
         if self.task_type in tasks_with_labels:
-            self.prediction_preamble = f"""Given the text, 
-            you have to now predict the labels from the 
-            list of allowed labels - {self.allowed_labels}."""
+            self.prediction_preamble = f"""Given the text, you have to now predict the labels from list of allowed labels - {self.allowed_labels}.\nOutput only the label(s) and close the <label> tag."""
         elif self.task_type == "SQLGeneration":
-            self.prediction_preamble = """Given the text, 
-            you have to now generate a SQL query."""
+            self.prediction_preamble = """Given the text, you have to now generate a SQL query.\nOnly the SQL query is expected."""
         else:  #generic preamble for prediction
-            self.prediction_preamble = """Given the text, 
-            you have to now predict."""
-        self.examples_preamble = """Here are a few examples to help you
-        understand the task better."""
-       
+            self.prediction_preamble = """Given the text, you have to now predict."""
+        self.examples_preamble = """Here are a few examples to help you understand the task better.\n"""
+    
     def format_examples(self, examples: List[Example]):
         """Formats the task examples into a string."""
         tasks_with_labels = ["Classification", "Tagging"]
         examples_str = ""
         for example in examples:
             if self.task_type in tasks_with_labels:
-                examples_str += f"""
-                text: {example.text}\n
-                label: {example.label}\n"""
+                examples_str += f"""<example>\n<text> {example.text}</text>\n<label> {example.label}</label>\n</example>\n"""
             elif self.task_type == "SQLGeneration":
-                examples_str += f"""
-                schema: {example.context}\n
-                text: {example.text}\n
-                SQL: {example.label}\n"""
-            else: #generic example format
-                examples_str += f"""
-                text: {example.text}\n
-                output: {example.label}\n"""
+                examples_str += f"""<example>\n<schema> {example.context}</schema>\n<text> {example.text}</text>\n<SQL> {example.label}</SQL>\n</example>\n"""
+            else:
+                examples_str += f"""<example>\n<text> {example.text}</text>\n<output> {example.label}</output>\n</example>\n"""
         return examples_str
-
-    def add_prediction_sample(self, text: str, context: str = None):
+    
+    def add_prediction_sample(self, text: str, context: str):
         """Add prediction sample to task."""
         tasks_with_labels = ["Classification", "Tagging"]
-        prediction_preamble = self.prediction_preamble + f"""\n text: {text}"""
+        prediction_preamble = self.prediction_preamble + f"""\n <text> {text} <text>"""
         if self.task_type in tasks_with_labels:
-            return prediction_preamble + "\n label:"
+            return prediction_preamble + "<label>"
         elif self.task_type == "SQLGeneration":
-            return prediction_preamble + f"""\n schema: {context}\n SQL: """
+            return prediction_preamble + f"""\n <schema>{context} <\schema>\m <SQL>"""
         else:
-            return prediction_preamble + "\n output:"
+            return prediction_preamble + "<output>"
```

### Comparing `prompt_learner-0.1.7/prompt_learner/templates/template.py` & `prompt_learner-0.1.8/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.7/PKG-INFO` & `prompt_learner-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


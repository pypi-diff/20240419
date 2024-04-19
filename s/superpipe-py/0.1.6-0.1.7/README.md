# Comparing `tmp/superpipe_py-0.1.6.tar.gz` & `tmp/superpipe_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpipe_py-0.1.6.tar", max compression
+gzip compressed data, was "superpipe_py-0.1.7.tar", max compression
```

## Comparing `superpipe_py-0.1.6.tar` & `superpipe_py-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     8241 2024-03-26 02:12:03.580726 superpipe_py-0.1.6/README.md
--rw-r--r--   0        0        0      830 2024-03-29 17:34:38.528274 superpipe_py-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      153 2024-03-25 15:10:35.189973 superpipe_py-0.1.6/superpipe/__init__.py
--rw-r--r--   0        0        0     2286 2024-03-29 17:34:38.528585 superpipe_py-0.1.6/superpipe/clients.py
--rw-r--r--   0        0        0       84 2024-03-07 18:22:24.180551 superpipe_py-0.1.6/superpipe/config.py
--rw-r--r--   0        0        0     6112 2024-03-25 20:28:08.394089 superpipe_py-0.1.6/superpipe/grid_search.py
--rw-r--r--   0        0        0     7311 2024-03-29 17:34:38.528991 superpipe_py-0.1.6/superpipe/llm.py
--rw-r--r--   0        0        0     1363 2024-03-28 23:49:05.058152 superpipe_py-0.1.6/superpipe/models.py
--rw-r--r--   0        0        0     6270 2024-03-29 17:34:38.529294 superpipe_py-0.1.6/superpipe/pipeline.py
--rw-r--r--   0        0        0     2505 2024-03-07 18:22:24.182418 superpipe_py-0.1.6/superpipe/pydantic.py
--rw-r--r--   0        0        0      188 2024-03-25 15:10:35.191485 superpipe_py-0.1.6/superpipe/steps/__init__.py
--rw-r--r--   0        0        0     2198 2024-03-19 19:49:12.348695 superpipe_py-0.1.6/superpipe/steps/custom.py
--rw-r--r--   0        0        0     4861 2024-03-19 19:49:12.349044 superpipe_py-0.1.6/superpipe/steps/embedding_search.py
--rw-r--r--   0        0        0     3290 2024-03-29 17:34:38.529583 superpipe_py-0.1.6/superpipe/steps/llm_step.py
--rw-r--r--   0        0        0     4256 2024-03-29 17:34:38.530014 superpipe_py-0.1.6/superpipe/steps/llm_structured.py
--rw-r--r--   0        0        0     4478 2024-03-29 17:34:38.530223 superpipe_py-0.1.6/superpipe/steps/llm_structured_composite.py
--rw-r--r--   0        0        0     3314 2024-03-21 18:44:40.347252 superpipe_py-0.1.6/superpipe/steps/serp.py
--rw-r--r--   0        0        0     4923 2024-03-19 19:49:12.350964 superpipe_py-0.1.6/superpipe/steps/step.py
--rw-r--r--   0        0        0     2173 2024-03-25 20:28:08.395135 superpipe_py-0.1.6/superpipe/steps/utils.py
--rw-r--r--   0        0        0     1854 2024-03-20 15:30:05.901744 superpipe_py-0.1.6/superpipe/util.py
--rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 superpipe_py-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     8241 2024-03-26 02:12:03.580726 superpipe_py-0.1.7/README.md
+-rw-r--r--   0        0        0      830 2024-04-19 17:21:07.867395 superpipe_py-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-03-25 15:10:35.189973 superpipe_py-0.1.7/superpipe/__init__.py
+-rw-r--r--   0        0        0     2286 2024-03-29 17:34:38.528585 superpipe_py-0.1.7/superpipe/clients.py
+-rw-r--r--   0        0        0      466 2024-04-19 17:21:07.867817 superpipe_py-0.1.7/superpipe/config.py
+-rw-r--r--   0        0        0     6112 2024-03-25 20:28:08.394089 superpipe_py-0.1.7/superpipe/grid_search.py
+-rw-r--r--   0        0        0     7311 2024-03-29 17:34:38.528991 superpipe_py-0.1.7/superpipe/llm.py
+-rw-r--r--   0        0        0     1363 2024-03-28 23:49:05.058152 superpipe_py-0.1.7/superpipe/models.py
+-rw-r--r--   0        0        0     7274 2024-04-19 17:21:07.868179 superpipe_py-0.1.7/superpipe/pipeline.py
+-rw-r--r--   0        0        0     2505 2024-03-07 18:22:24.182418 superpipe_py-0.1.7/superpipe/pydantic.py
+-rw-r--r--   0        0        0      188 2024-03-25 15:10:35.191485 superpipe_py-0.1.7/superpipe/steps/__init__.py
+-rw-r--r--   0        0        0     2480 2024-04-19 17:21:07.868423 superpipe_py-0.1.7/superpipe/steps/custom.py
+-rw-r--r--   0        0        0     5397 2024-04-19 17:21:07.868646 superpipe_py-0.1.7/superpipe/steps/embedding_search.py
+-rw-r--r--   0        0        0     3582 2024-04-19 17:21:07.868811 superpipe_py-0.1.7/superpipe/steps/llm_step.py
+-rw-r--r--   0        0        0     4489 2024-04-19 17:21:07.869026 superpipe_py-0.1.7/superpipe/steps/llm_structured.py
+-rw-r--r--   0        0        0     4627 2024-04-19 17:21:07.869241 superpipe_py-0.1.7/superpipe/steps/llm_structured_composite.py
+-rw-r--r--   0        0        0     3721 2024-04-19 17:21:07.869411 superpipe_py-0.1.7/superpipe/steps/serp.py
+-rw-r--r--   0        0        0     6283 2024-04-19 17:21:07.869666 superpipe_py-0.1.7/superpipe/steps/step.py
+-rw-r--r--   0        0        0     2173 2024-03-25 20:28:08.395135 superpipe_py-0.1.7/superpipe/steps/utils.py
+-rw-r--r--   0        0        0     1854 2024-03-20 15:30:05.901744 superpipe_py-0.1.7/superpipe/util.py
+-rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 superpipe_py-0.1.7/PKG-INFO
```

### Comparing `superpipe_py-0.1.6/README.md` & `superpipe_py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/pyproject.toml` & `superpipe_py-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superpipe-py"
-version = "0.1.6"
+version = "0.1.7"
 description = "build unstructured to structured data transformation pipelines"
 authors = ["Aman Dhesi <aman@stelolabs.com>"]
 license = "MIT"
 packages = [{ include = "superpipe" }]
 readme = "README.md"
 repository = "https://github.com/villagecomputing/superpipe"
```

### Comparing `superpipe_py-0.1.6/superpipe/clients.py` & `superpipe_py-0.1.7/superpipe/clients.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/grid_search.py` & `superpipe_py-0.1.7/superpipe/grid_search.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/llm.py` & `superpipe_py-0.1.7/superpipe/llm.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/models.py` & `superpipe_py-0.1.7/superpipe/models.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/pipeline.py` & `superpipe_py-0.1.7/superpipe/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import pickle
+import hashlib
 from typing import List, Callable, Union, Dict, Optional
 from collections import defaultdict
 from dataclasses import dataclass, field
 import pandas as pd
 from prettytable import PrettyTable
 from superpipe.steps import Step, LLMStep, LLMStructuredStep, LLMStructuredCompositeStep
-from superpipe.config import is_dev
+from superpipe.config import is_dev, studio_enabled
 
 
 @dataclass
 class PipelineStatistics:
     score: Optional[float] = None
     input_tokens: dict = field(default_factory=lambda: defaultdict(int))
     output_tokens: dict = field(default_factory=lambda: defaultdict(int))
@@ -52,45 +54,72 @@
         update_params(params): Updates the parameters of the pipeline steps.
         evaluate(evaluation_fn=None): Evaluates the processed data using an evaluation function.
         _aggregate_statistics(data): Aggregates statistics from the pipeline steps.
     """
 
     def __init__(self,
                  steps: List[Step],
-                 evaluation_fn: Callable[[any], Union[bool, float]] = None):
+                 evaluation_fn: Callable[[any], Union[bool, float]] = None,
+                 name: str = None):
         self.steps = steps
         self.evaluation_fn = evaluation_fn
         self.data = None
         self.score = None
+        self.name = name or self.__class__.__name__
         self.statistics = PipelineStatistics()
 
-    def run(self, data: Union[pd.DataFrame, Dict], row_wise=False, verbose=True):
+    def run(self, data: Union[pd.DataFrame, Dict], enable_logging=False, row_wise=True, verbose=True):
+        def run_steps(row):
+            for step in self.steps:
+                step.run(row, verbose)
+            return row
+
         # Note: currently running row-wise is ~40% slower than step-wise (because of memory overhead?)
-        if row_wise and isinstance(data, pd.DataFrame):
-            def fn(row):
-                for step in self.steps:
-                    step.run(row, verbose)
-                return row
-            if verbose and is_dev:
-                from tqdm import tqdm
-                tqdm.pandas(desc=f"Running pipeline row-wise")
-                results = data.progress_apply(fn, axis=1)
+        if row_wise:
+            if enable_logging and studio_enabled():
+                from studio import run_pipeline_with_log
+                run_steps = run_pipeline_with_log(run_steps, self)
+            if isinstance(data, pd.DataFrame):
+                if verbose and is_dev:
+                    from tqdm import tqdm
+                    tqdm.pandas(desc=f"Running pipeline row-wise")
+                    results = data.progress_apply(run_steps, axis=1)
+                else:
+                    results = data.apply(run_steps, axis=1)
+                data[results.columns] = results
             else:
-                results = data.apply(fn, axis=1)
-            data[results.columns] = results
+                run_steps(data)
         else:
+            # logging not supported for step-wise execution
             for step in self.steps:
                 step.run(data, verbose)
         if isinstance(data, pd.DataFrame):
             self.data = data
             if self.evaluation_fn is not None:
                 self.evaluate()
         self._aggregate_statistics(data)
         return data
 
+    def fingerprint(self, deep=False):
+        fingerprint_obj = {
+            "name": self.name,
+            "steps": [step.fingerprint(deep) for step in self.steps]
+        }
+        object_bytes = pickle.dumps(fingerprint_obj)
+        hash_object = hashlib.sha256()
+        hash_object.update(object_bytes)
+        return hash_object.hexdigest()
+
+    def get_params(self):
+        return {
+            k: v for k, v in [
+                (step.name, step.get_params()) for step in self.steps
+            ]
+        }
+
     # TODO: only include params relevant for each step, raise if param is not found in any step
     def update_params(self, params: Dict):
         for step in self.steps:
             global_params = params.get('global', {})
             step_params = params.get(step.name, {})
             step.update_params({**global_params, **step_params})
```

### Comparing `superpipe_py-0.1.6/superpipe/pydantic.py` & `superpipe_py-0.1.7/superpipe/pydantic.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/steps/custom.py` & `superpipe_py-0.1.7/superpipe/steps/custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,26 @@
             out_schema (T): A Pydantic model that the output of the transform function should conform to.
 
             name (str, optional): An optional name for the step. Defaults to None.
         """
         super().__init__(name)
         self.transform = transform
 
+    def get_params(self):
+        """
+        Returns the parameters of the step.
+
+        Returns:
+            Dict: A dictionary of the step's parameters.
+        """
+        return {
+            **super().get_params(),
+            "transform": self.transform.__name__
+        }
+
     def _run(self, row: Union[pd.Series, Dict]) -> Dict:
         """
         Applies the transformation function to a single row of data.
 
         This method ensures that the output of the transformation matches the fields defined in the Pydantic model specified by `out_schema`.
 
         Args:
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/embedding_search.py` & `superpipe_py-0.1.7/superpipe/steps/embedding_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,30 @@
             self.index = self._create_index(candidates)
         elif self.candidates_fn:
             self.index = None
         else:
             raise ValueError(
                 "Either candidates or candidates_fn must be provided")
 
+    def get_params(self):
+        """
+        Returns the parameters of the step.
+
+        Returns:
+            Dict: A dictionary of the step's parameters.
+        """
+        return {
+            **super().get_params(),
+            "search_prompt": self.search_prompt.__name__,
+            "embed_fn": self.embed_fn.__name__,
+            "candidates": self.candidates.__hash__() if self.candidates else None,
+            "candidates_fn": self.candidates_fn.__name__ if self.candidates_fn else None,
+            "k": self.k
+        }
+
     def update_params(self, params: Dict):
         """
         Updates the parameters of the step and rebuilds the index if embed_fn or candidates are updated.
 
         Parameters:
             params (Dict): A dictionary of parameters to update.
         """
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/llm_step.py` & `superpipe_py-0.1.7/superpipe/steps/llm_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,28 @@
             name (str, optional): The name of the step. Defaults to None.
         """
         super().__init__(name)
         self.model = model
         self.prompt = prompt
         self.openai_args = openai_args
 
+    def get_params(self):
+        """
+        Returns the parameters of the step.
+
+        Returns:
+            Dict: A dictionary of the step's parameters.
+        """
+        return {
+            **super().get_params(),
+            "model": self.model,
+            "prompt": self.prompt.__name__,
+            "openai_args": self.openai_args
+        }
+
     def _get_row_statistics(self, response: LLMResponse):
         """
         Create a StepRowStatistics object based on the response from the LLM.
 
         Args:
             response (LLMResponse): The response from the LLM.
         """
@@ -71,15 +85,12 @@
         try:
             response = get_llm_response(compiled_prompt, model, openai_args)
         except Exception as e:
             # TODO: need better error logging here include stacktrace
             response = LLMResponse(
                 success=False, error=str(e), latency=0)
         statistics = self._get_row_statistics(response)
-        result = {f"__{self.name}__": {
-            **statistics.model_dump(),
-            "error": response.error,
-        }}
+        result = {}
         # TODO: how should we handle failure cases?
         if response.success:
             result[f"{self.name}"] = response.content
-        return StepResult(fields=result, statistics=statistics)
+        return StepResult(fields=result, statistics=statistics, error=response.error, input=compiled_prompt)
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/llm_structured.py` & `superpipe_py-0.1.7/superpipe/steps/llm_structured.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,14 +47,26 @@
             prompt (Callable[[Union[Dict, pd.Series]], str]): A function that takes input data and returns a prompt string.
             out_schema (T): The Pydantic model that defines the expected structure of the LLM's response.
             name (str, optional): The name of the step. Defaults to None.
         """
         super().__init__(model, prompt, openai_args, name)
         self.out_schema = out_schema
 
+    def get_params(self):
+        """
+        Returns the parameters of the step.
+
+        Returns:
+            Dict: A dictionary of the step's parameters.
+        """
+        return {
+            **super().get_params(),
+            "out_schema": self.out_schema.model_json_schema()
+        }
+
     def _compile_structured_prompt(self, input: dict):
         """
         Compiles a structured prompt from the input data.
 
         Args:
             input (dict): The input data for the prompt.
 
@@ -86,22 +98,19 @@
             response = get_structured_llm_response(
                 compiled_prompt, model, openai_args)
         except Exception as e:
             # TODO: need better error logging here include stacktrace
             response = StructuredLLMResponse(
                 success=False, error=str(e), latency=0)
         statistics = self._get_row_statistics(response)
-        result = {f"__{self.name}__": {
-            **statistics.model_dump(),
-            "error": response.error,
-        }}
+        result = {}
         # TODO: how should we handle failure cases
         if response.success:
             content = response.content
             for field in fields:
                 # TODO: handle missing fields instead of printing
                 if field not in content:
                     print(
                         f"Step {self.name}: Missing field {field} in response {content}")
                 val = content.get(field)
                 result[field] = val if val is not None else ""
-        return StepResult(fields=result, statistics=statistics)
+        return StepResult(fields=result, statistics=statistics, error=response.error, input=compiled_prompt)
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/llm_structured_composite.py` & `superpipe_py-0.1.7/superpipe/steps/llm_structured_composite.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,21 @@
             structured_model (str): Identifier for the structured LLM. Defaults to gpt35.
             name (str, optional): Name of the step.
         """
         super().__init__(model, prompt, openai_args, name)
         self.structured_model = structured_model
         self.out_schema = out_schema
 
+    def get_params(self):
+        return {
+            **super().get_params(),
+            "structured_model": self.structured_model,
+            "out_schema": self.out_schema.model_json_schema()
+        }
+
     def _compile_structured_prompt(self, unstructured: str):
         prompt_main = f"""
         You are a helpful assistant designed to output JSON. Turn the following unstructured data into a structured JSON object.
         
         {unstructured}
         """
         output_schema = describe_pydantic_model(self.out_schema)
@@ -71,37 +78,34 @@
         openai_args = self.openai_args
         fields = self.out_schema.model_fields.keys()
         compiled_prompt = prompt(row)
         try:
             response = get_llm_response(compiled_prompt, model, openai_args)
             statistics_first = self._get_row_statistics(response)
             if response.success:
-                compiled_prompt = self._compile_structured_prompt(
+                structured_prompt = self._compile_structured_prompt(
                     response.content)
                 response = get_structured_llm_response(
-                    compiled_prompt, structured_model, openai_args)
+                    structured_prompt, structured_model, openai_args)
             else:
                 response = StructuredLLMResponse(
                     success=False, error=response.error, latency=0)
         except Exception as e:
             # TODO: need better error logging here include stacktrace
             response = StructuredLLMResponse(
                 success=False, error=str(e), latency=0)
         # TODO: combine model dumps of both LLM calls
         statistics_second = self._get_row_statistics(response)
         statistics = combine_step_row_statistics(
             [statistics_first, statistics_second])
-        result = {f"__{self.name}__": {
-            **statistics.model_dump(),
-            "error": response.error,
-        }}
+        result = {}
         # TODO: how should we handle failure cases
         if response.success:
             content = response.content
             for field in fields:
                 # TODO: handle missing fields instead of printing
                 if field not in content:
                     print(
                         f"Step {self.name}: Missing field {field} in response {content}")
                 val = content.get(field)
                 result[field] = val if val is not None else ""
-        return StepResult(fields=result, statistics=statistics)
+        return StepResult(fields=result, statistics=statistics, error=response.error, input=compiled_prompt)
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/serp.py` & `superpipe_py-0.1.7/superpipe/steps/serp.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,27 @@
             postprocess (Optional[Callable[[str], str]]): An optional callable for post-processing the search results.
             name (Optional[str]): An optional name for the step.
         """
         super().__init__(name)
         self.prompt = prompt
         self.postprocess = postprocess
 
+    def get_params(self):
+        """
+        Returns the parameters of the step.
+
+        Returns:
+            Dict: A dictionary of the step's parameters.
+        """
+        return {
+            **super().get_params(),
+            "prompt": self.prompt.__name__,
+            "postprocess": self.postprocess.__name__ if self.postprocess is not None else None
+        }
+
     def _get_search_results(self, q):
         """
         Fetches search results for a given query string.
 
         Args:
             q (str): The search query string.
 
@@ -70,12 +83,12 @@
 
         Args:
             row (Union[pd.Series, Dict]): A single row of data, either as a pandas Series or a dictionary.
 
         Returns:
             Dict: A dictionary containing the enriched data.
         """
-        prompt = self.prompt
+        search_prompt = self.prompt(row)
         postprocess = self.postprocess if self.postprocess is not None else lambda x: x
-        def fn(x): return postprocess(self._get_search_results(prompt(x)))
-        result, statistics = with_statistics(fn)(row)
-        return StepResult(fields={self.name: result}, statistics=statistics)
+        def fn(x): return postprocess(self._get_search_results(x))
+        result, statistics = with_statistics(fn)(search_prompt)
+        return StepResult(fields={self.name: result}, statistics=statistics, input=search_prompt)
```

### Comparing `superpipe_py-0.1.6/superpipe/steps/utils.py` & `superpipe_py-0.1.7/superpipe/steps/utils.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/superpipe/util.py` & `superpipe_py-0.1.7/superpipe/util.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.6/PKG-INFO` & `superpipe_py-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpipe-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: build unstructured to structured data transformation pipelines
 Home-page: https://github.com/villagecomputing/superpipe
 License: MIT
 Author: Aman Dhesi
 Author-email: aman@stelolabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


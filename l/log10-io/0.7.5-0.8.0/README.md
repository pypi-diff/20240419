# Comparing `tmp/log10_io-0.7.5.tar.gz` & `tmp/log10_io-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.7.5.tar", max compression
+gzip compressed data, was "log10_io-0.8.0.tar", max compression
```

## Comparing `log10_io-0.7.5.tar` & `log10_io-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2024-04-10 04:30:32.129246 log10_io-0.7.5/LICENSE
--rw-r--r--   0        0        0     8934 2024-04-10 04:30:32.129246 log10_io-0.7.5/README.md
--rw-r--r--   0        0        0        0 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/__init__.py
--rw-r--r--   0        0        0     1470 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/__main__.py
--rw-r--r--   0        0        0    10132 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/bigquery.py
--rw-r--r--   0        0        0     9532 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/evals.py
--rw-r--r--   0        0        0     5399 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4153 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/langchain.py
--rw-r--r--   0        0        0     4296 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/llm.py
--rw-r--r--   0        0        0    34743 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/openai.py
--rw-r--r--   0        0        0     5343 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/utils.py
--rw-r--r--   0        0        0     2180 2024-04-10 04:30:32.133246 log10_io-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 log10_io-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-18 22:15:06.477241 log10_io-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8934 2024-04-18 22:15:06.481241 log10_io-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/__main__.py
+-rw-r--r--   0        0        0    10132 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/bigquery.py
+-rw-r--r--   0        0        0    22333 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/evals.py
+-rw-r--r--   0        0        0     5459 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4487 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     4880 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/langchain.py
+-rw-r--r--   0        0        0     4432 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/llm.py
+-rw-r--r--   0        0        0    35998 2024-04-18 22:15:06.481241 log10_io-0.8.0/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/openai.py
+-rw-r--r--   0        0        0     6915 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/tools.py
+-rw-r--r--   0        0        0     1931 2024-04-18 22:15:06.485241 log10_io-0.8.0/log10/utils.py
+-rw-r--r--   0        0        0     2242 2024-04-18 22:15:06.485241 log10_io-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 log10_io-0.8.0/PKG-INFO
```

### Comparing `log10_io-0.7.5/LICENSE` & `log10_io-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/README.md` & `log10_io-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/__main__.py` & `log10_io-0.8.0/log10/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from log10.completions.completions import download_completions, get_completion, list_completions
+from log10.completions.completions import benchmark_models, download_completions, get_completion, list_completions
 from log10.feedback.autofeedback import auto_feedback_icl
 from log10.feedback.feedback import create_feedback, download_feedback, get_feedback, list_feedback
 from log10.feedback.feedback_task import create_feedback_task, get_feedback_task, list_feedback_task
 
 
 @click.group()
 def cli():
@@ -35,14 +35,15 @@
     pass
 
 
 cli.add_command(completions)
 completions.add_command(list_completions, "list")
 completions.add_command(get_completion, "get")
 completions.add_command(download_completions, "download")
+completions.add_command(benchmark_models, "benchmark_models")
 
 cli.add_command(feedback)
 feedback.add_command(create_feedback, "create")
 feedback.add_command(list_feedback, "list")
 feedback.add_command(get_feedback, "get")
 feedback.add_command(download_feedback, "download")
 feedback.add_command(auto_feedback_icl, "predict")
```

### Comparing `log10_io-0.7.5/log10/_httpx_utils.py` & `log10_io-0.8.0/log10/_httpx_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/agents/camel.py` & `log10_io-0.8.0/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/agents/scrape_summarizer.py` & `log10_io-0.8.0/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/anthropic.py` & `log10_io-0.8.0/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/bigquery.py` & `log10_io-0.8.0/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/evals.py` & `log10_io-0.8.0/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.8.0/log10/feedback/_summary_feedback_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 import sys
 
+import openai
+
+from log10.load import log10
+
+
+log10(openai)
 
 if sys.version_info < (3, 10):
     raise RuntimeError("Python 3.10 or higher is required to run summary feedback llm call.")
 
 try:
     from magentic import SystemMessage, UserMessage, chatprompt
     from magentic.chat_model.openai_chat_model import OpenaiChatModel
```

### Comparing `log10_io-0.7.5/log10/feedback/autofeedback.py` & `log10_io-0.8.0/log10/feedback/autofeedback.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import json
 import logging
 import random
 from types import FunctionType
 
 import click
-import openai
 from rich.console import Console
 
 from log10.completions.completions import _get_completion
-from log10.feedback._summary_feedback_utils import flatten_messages, summary_feedback_llm_call
 from log10.feedback.feedback import _get_feedback_list
-from log10.load import log10, log10_session
+from log10.load import log10_session
 
 
-log10(openai)
+try:
+    from log10.feedback._summary_feedback_utils import flatten_messages, summary_feedback_llm_call
+
+    Magentic_imported = True
+except ImportError:
+    Magentic_imported = False
+
 
 logger = logging.getLogger("LOG10")
 logger.setLevel(logging.INFO)
 
 
 class AutoFeedbackICL:
     """
     Generate feedback with in context learning (ICL) based on existing feedback.
     """
 
     _examples: list[dict] = []
     _predict_func: FunctionType = None
 
-    def __init__(self, task_id: str, num_samples: int = 5, predict_func: FunctionType = summary_feedback_llm_call):
+    def __init__(
+        self,
+        task_id: str,
+        num_samples: int = 5,
+        predict_func: FunctionType = summary_feedback_llm_call if Magentic_imported else None,
+    ):
+        if not Magentic_imported:
+            raise ImportError(
+                "Log10 feedback predict requires magentic package. Please install using 'pip install log10-io[autofeedback_icl]'"
+            )
         self.num_samples = num_samples
         self.task_id = task_id
         self._predict_func = predict_func
 
     def _get_examples(self):
         logger.info(f"Getting {self.num_samples} feedback for task {self.task_id}")
         feedback_data = _get_feedback_list(offset=0, limit="", task_id=self.task_id)
```

### Comparing `log10_io-0.7.5/log10/feedback/feedback.py` & `log10_io-0.8.0/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/feedback/feedback_task.py` & `log10_io-0.8.0/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/langchain.py` & `log10_io-0.8.0/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/litellm.py` & `log10_io-0.8.0/log10/litellm.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,20 @@
 
     #### ASYNC #### - for acompletion/aembeddings
 
     async def async_log_stream_event(self, kwargs, response_obj, start_time, end_time):
         pass
 
     async def async_log_success_event(self, kwargs, response_obj, start_time, end_time):
+        if kwargs["call_type"] == "completion":
+            return
+
         logger.debug(
             f"**\n**async_log_success_event**\n**\n: kwargs:\n {kwargs} response_obj:\n {response_obj} \n\n {start_time} \n\n duration: {end_time - start_time}"
         )
         self.log_success_event(kwargs, response_obj, start_time, end_time)
 
     async def async_log_failure_event(self, kwargs, response_obj, start_time, end_time):
+        if kwargs["call_type"] == "completion":
+            return
+
         self.log_failure_event(kwargs, response_obj, start_time, end_time)
```

### Comparing `log10_io-0.7.5/log10/llm.py` & `log10_io-0.8.0/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/load.py` & `log10_io-0.8.0/log10/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
             "lineno": frame.lineno,
             "name": frame.name,
         }
         for frame in current_stack_frame
     ]
 
 
-def _init_log_row(func, **kwargs):
+def _init_log_row(func, *args, **kwargs):
     kwargs_copy = deepcopy(kwargs)
 
     log_row = {
         "status": "started",
         "orig_module": func.__module__,
         "orig_qualname": func.__qualname__,
         "stacktrace": json.dumps(_get_stack_trace()),
@@ -493,14 +493,19 @@
             if kwargs_copy.get("generation_config"):
                 for key, value in kwargs_copy["generation_config"].to_dict().items():
                     if key == "max_output_tokens":
                         kwargs_copy["max_tokens"] = value
                     else:
                         kwargs_copy[key] = value
                 kwargs_copy.pop("generation_config")
+    elif "lamini" in func.__module__:
+        log_row["kind"] = "chat"
+        kwargs_copy.update(
+            {"model": args[1]["model_name"], "messages": [{"role": "user", "content": args[1]["prompt"]}]}
+        )
     elif "mistralai" in func.__module__:
         log_row["kind"] = "chat"
     elif "openai" in func.__module__:
         kind = "chat" if "chat" in func.__module__ else "completion"
         log_row["kind"] = kind
 
     log_row["request"] = json.dumps(kwargs_copy)
@@ -512,15 +517,15 @@
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         completion_url = url + "/api/completions"
         output = None
         result_queue = queue.Queue()
 
         try:
-            log_row = _init_log_row(func, **kwargs)
+            log_row = _init_log_row(func, *args, **kwargs)
 
             with timed_block(sync_log_text + " call duration"):
                 if USE_ASYNC:
                     threading.Thread(
                         target=run_async_in_thread,
                         kwargs={
                             "completion_url": completion_url,
@@ -589,19 +594,17 @@
                         )
                     from log10.anthropic import Anthropic
 
                     response = Anthropic.prepare_response(output, input_prompt=kwargs.get("prompt", ""))
                 elif "vertexai" in func.__module__:
                     response = output
                     reason = response.candidates[0].finish_reason.name
-                    import uuid
-
                     ret_response = {
                         "id": str(uuid.uuid4()),
-                        "object": "completion",
+                        "object": "chat.completion",
                         "choices": [
                             {
                                 "index": 0,
                                 "finish_reason": str(reason).lower(),
                                 "message": {"role": "assistant", "content": response.text},
                             }
                         ],
@@ -624,14 +627,27 @@
                             response=response,
                             partial_log_row=log_row,
                         )
                     response = output.copy()
 
                     if "choices" in response:
                         response = flatten_response(response)
+                elif "lamini" in func.__module__:
+                    response = {
+                        "id": str(uuid.uuid4()),
+                        "object": "chat.completion",
+                        "choices": [
+                            {
+                                "index": 0,
+                                "finish_reason": "stop",
+                                "message": {"role": "assistant", "content": output["output"]},
+                            }
+                        ],
+                        "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0},
+                    }
                 elif "mistralai" in func.__module__:
                     if "stream" in func.__qualname__:
                         log_row["response"] = response
                         log_row["status"] = "finished"
                         return StreamingResponseWrapper(
                             completion_url=completion_url,
                             completionID=completionID,
@@ -785,24 +801,32 @@
     #             setattr(cls, method_name, classmethod(decorated_method))
     #         elif isinstance(method, (types.FunctionType, types.MethodType)):
     #             print(f"method:{method}")
     #             setattr(cls, method_name, intercepting_decorator(method))
     #         elif inspect.isclass(method):  # Handle nested classes
     #             intercept_class_methods(method)
 
+    if getattr(module, "_log10_patched", False):
+        logger.warning(f"{module.__name__} already patched. Skipping.")
+        return
+
     if module.__name__ == "anthropic":
         attr = module.resources.completions.Completions
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
 
         # anthropic Messages completion
         attr = module.resources.messages.Messages
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
-    if module.__name__ == "mistralai":
+    elif module.__name__ == "lamini":
+        attr = module.api.utils.completion.Completion
+        method = getattr(attr, "generate")
+        setattr(attr, "generate", intercepting_decorator(method))
+    elif module.__name__ == "mistralai" and getattr(module, "_log10_patched", False) is False:
         attr = module.client.MistralClient
         method = getattr(attr, "chat")
         setattr(attr, "chat", intercepting_decorator(method))
 
         method = getattr(attr, "chat_stream")
         setattr(attr, "chat_stream", intercepting_decorator(method))
     elif module.__name__ == "openai":
@@ -865,14 +889,16 @@
         #     print(f"attr:{attr}")
         #     setattr(module, name, intercepting_decorator(attr))
         # elif inspect.isclass(attr):  # Check if attribute is a class
         #     intercept_class_methods(attr)
         # # else: # uncomment if we want to include nested function support
         # #     intercept_nested_functions(attr)
 
+    module._log10_patched = True
+
 
 if is_openai_v1():
     import openai
     from openai import OpenAI
 
     class OpenAI(OpenAI):
         """
```

### Comparing `log10_io-0.7.5/log10/mosaicml.py` & `log10_io-0.8.0/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/openai.py` & `log10_io-0.8.0/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/schemas/bigquery.json` & `log10_io-0.8.0/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/together.py` & `log10_io-0.8.0/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/log10/tools.py` & `log10_io-0.8.0/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.5/pyproject.toml` & `log10_io-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.7.5"
+version = "0.8.0"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -47,17 +47,19 @@
 faker = "^19.2.0"
 backoff = "^2.2.1"
 anthropic = "<1"
 mosaicml-cli = "^0.5.30"
 together = "^0.2.7"
 google-cloud-aiplatform = ">=1.44.0"
 mistralai = "^0.1.5"
+pandas = ">=2"
 
 magentic = {version = ">=0.17.0", optional = true, markers = "python_version >= '3.10'"}
 litellm = {version = "^1.34.18", optional = true}
+lamini = {version = "^2.1.8", optional = true}
 
 [tool.poetry.extras]
 autofeedback_icl = ["magentic"]
 litellm = ["litellm"]
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
```

### Comparing `log10_io-0.7.5/PKG-INFO` & `log10_io-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.7.5
+Version: 0.8.0
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -17,20 +17,22 @@
 Requires-Dist: anthropic (<1)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: faker (>=19.2.0,<20.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.44.0)
 Requires-Dist: google-cloud-bigquery (>=3.11.4,<4.0.0)
 Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
+Requires-Dist: lamini (>=2.1.8,<3.0.0)
 Requires-Dist: langchain (<0.2.0)
 Requires-Dist: litellm (>=1.34.18,<2.0.0) ; extra == "litellm"
 Requires-Dist: magentic (>=0.17.0) ; (python_version >= "3.10") and (extra == "autofeedback-icl")
 Requires-Dist: mistralai (>=0.1.5,<0.2.0)
 Requires-Dist: mosaicml-cli (>=0.5.30,<0.6.0)
 Requires-Dist: openai (<2)
+Requires-Dist: pandas (>=2)
 Requires-Dist: pexpect (>=4.8.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: together (>=0.2.7,<0.3.0)
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
```


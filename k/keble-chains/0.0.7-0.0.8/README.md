# Comparing `tmp/keble_chains-0.0.7.tar.gz` & `tmp/keble_chains-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keble_chains-0.0.7.tar", max compression
+gzip compressed data, was "keble_chains-0.0.8.tar", max compression
```

## Comparing `keble_chains-0.0.7.tar` & `keble_chains-0.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1067 2024-03-05 11:27:13.622616 keble_chains-0.0.7/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 11:27:13.623628 keble_chains-0.0.7/README.md
--rw-r--r--   0        0        0      373 2024-03-05 11:27:13.615707 keble_chains-0.0.7/keble_chains/__init__.py
--rw-r--r--   0        0        0       65 2024-03-05 11:27:13.615841 keble_chains-0.0.7/keble_chains/chainables/__init__.py
--rw-r--r--   0        0        0       28 2024-03-05 11:27:13.615961 keble_chains-0.0.7/keble_chains/chainables/chunk/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616078 keble_chains-0.0.7/keble_chains/chainables/chunk/chainable.py
--rw-r--r--   0        0        0       31 2024-03-05 11:27:13.616191 keble_chains-0.0.7/keble_chains/chainables/metadata/__init__.py
--rw-r--r--   0        0        0      283 2024-03-05 11:27:13.616344 keble_chains-0.0.7/keble_chains/chainables/metadata/chainable.py
--rw-r--r--   0        0        0       28 2024-03-05 11:27:13.616582 keble_chains-0.0.7/keble_chains/chainables/prune/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616892 keble_chains-0.0.7/keble_chains/chainables/prune/chainable.py
--rw-r--r--   0        0        0    12082 2024-03-05 11:27:13.617158 keble_chains-0.0.7/keble_chains/chains.py
--rw-r--r--   0        0        0      215 2024-03-05 11:27:13.617420 keble_chains-0.0.7/keble_chains/exceptions/__init__.py
--rw-r--r--   0        0        0     1632 2024-03-05 11:27:13.617747 keble_chains-0.0.7/keble_chains/exceptions/openai.py
--rw-r--r--   0        0        0       57 2024-03-05 11:27:13.617856 keble_chains-0.0.7/keble_chains/export/__init__.py
--rw-r--r--   0        0        0     7777 2024-03-05 11:27:13.617971 keble_chains-0.0.7/keble_chains/export/export.py
--rw-r--r--   0        0        0       36 2024-03-05 11:27:13.618077 keble_chains-0.0.7/keble_chains/interact/__init__.py
--rw-r--r--   0        0        0      135 2024-03-05 11:27:13.618190 keble_chains-0.0.7/keble_chains/interact/ai/__init__.py
--rw-r--r--   0        0        0     6762 2024-04-03 11:17:00.551407 keble_chains-0.0.7/keble_chains/interact/ai/azure.py
--rw-r--r--   0        0        0     1286 2024-03-05 11:27:13.618440 keble_chains-0.0.7/keble_chains/interact/ai/fake.py
--rw-r--r--   0        0        0     1387 2024-03-05 11:27:13.618658 keble_chains-0.0.7/keble_chains/interact/ai/session.py
--rw-r--r--   0        0        0     4017 2024-03-05 11:27:13.618771 keble_chains-0.0.7/keble_chains/interact/ai/token_manager.py
--rw-r--r--   0        0        0      120 2024-03-05 11:27:13.618873 keble_chains-0.0.7/keble_chains/interact/m14/__init__.py
--rw-r--r--   0        0        0     5717 2024-03-05 11:27:13.618981 keble_chains-0.0.7/keble_chains/interact/m14/m14_compressors.py
--rw-r--r--   0        0        0     1457 2024-03-05 11:27:13.619082 keble_chains-0.0.7/keble_chains/interact/m14/m14_session.py
--rw-r--r--   0        0        0      232 2024-03-05 11:27:13.619198 keble_chains-0.0.7/keble_chains/template/__init__.py
--rw-r--r--   0        0        0       46 2024-03-05 11:27:13.619315 keble_chains-0.0.7/keble_chains/template/base.py
--rw-r--r--   0        0        0     8179 2024-03-05 11:27:13.619488 keble_chains-0.0.7/keble_chains/template/chat.py
--rw-r--r--   0        0        0     2632 2024-03-05 11:27:13.619602 keble_chains-0.0.7/keble_chains/template/email.py
--rw-r--r--   0        0        0      460 2024-03-05 11:27:13.619706 keble_chains-0.0.7/keble_chains/template/openai.py
--rw-r--r--   0        0        0       63 2024-03-05 11:27:13.619811 keble_chains-0.0.7/keble_chains/tuning/__init__.py
--rw-r--r--   0        0        0    16219 2024-03-05 11:27:13.620867 keble_chains-0.0.7/keble_chains/tuning/datasets.py
--rw-r--r--   0        0        0      562 2024-03-05 11:27:13.621013 keble_chains-0.0.7/keble_chains/typings/__init__.py
--rw-r--r--   0        0        0    11627 2024-03-05 11:27:13.621272 keble_chains-0.0.7/keble_chains/typings/abc.py
--rw-r--r--   0        0        0     9513 2024-03-12 14:33:49.625950 keble_chains-0.0.7/keble_chains/typings/ai.py
--rw-r--r--   0        0        0      321 2024-03-05 11:27:13.621784 keble_chains-0.0.7/keble_chains/typings/collected.py
--rw-r--r--   0        0        0     1865 2024-03-05 11:27:13.621905 keble_chains-0.0.7/keble_chains/typings/dataset.py
--rw-r--r--   0        0        0     1922 2024-03-05 11:27:13.622026 keble_chains-0.0.7/keble_chains/typings/export.py
--rw-r--r--   0        0        0      419 2024-03-05 11:27:13.622152 keble_chains-0.0.7/keble_chains/typings/main.py
--rw-r--r--   0        0        0      122 2024-03-05 11:27:13.622281 keble_chains-0.0.7/keble_chains/typings/valid.py
--rw-r--r--   0        0        0       84 2024-03-05 11:27:13.622403 keble_chains-0.0.7/keble_chains/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-03-05 11:27:13.622508 keble_chains-0.0.7/keble_chains/utils/main.py
--rw-r--r--   0        0        0      588 2024-04-03 11:17:07.055304 keble_chains-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 keble_chains-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-05 11:27:13.622616 keble_chains-0.0.8/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 11:27:13.623628 keble_chains-0.0.8/README.md
+-rw-r--r--   0        0        0      373 2024-03-05 11:27:13.615707 keble_chains-0.0.8/keble_chains/__init__.py
+-rw-r--r--   0        0        0       65 2024-03-05 11:27:13.615841 keble_chains-0.0.8/keble_chains/chainables/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-05 11:27:13.615961 keble_chains-0.0.8/keble_chains/chainables/chunk/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616078 keble_chains-0.0.8/keble_chains/chainables/chunk/chainable.py
+-rw-r--r--   0        0        0       31 2024-03-05 11:27:13.616191 keble_chains-0.0.8/keble_chains/chainables/metadata/__init__.py
+-rw-r--r--   0        0        0      283 2024-03-05 11:27:13.616344 keble_chains-0.0.8/keble_chains/chainables/metadata/chainable.py
+-rw-r--r--   0        0        0       28 2024-03-05 11:27:13.616582 keble_chains-0.0.8/keble_chains/chainables/prune/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 11:27:13.616892 keble_chains-0.0.8/keble_chains/chainables/prune/chainable.py
+-rw-r--r--   0        0        0    12082 2024-03-05 11:27:13.617158 keble_chains-0.0.8/keble_chains/chains.py
+-rw-r--r--   0        0        0      215 2024-03-05 11:27:13.617420 keble_chains-0.0.8/keble_chains/exceptions/__init__.py
+-rw-r--r--   0        0        0     1632 2024-03-05 11:27:13.617747 keble_chains-0.0.8/keble_chains/exceptions/openai.py
+-rw-r--r--   0        0        0       57 2024-03-05 11:27:13.617856 keble_chains-0.0.8/keble_chains/export/__init__.py
+-rw-r--r--   0        0        0     7777 2024-03-05 11:27:13.617971 keble_chains-0.0.8/keble_chains/export/export.py
+-rw-r--r--   0        0        0       36 2024-03-05 11:27:13.618077 keble_chains-0.0.8/keble_chains/interact/__init__.py
+-rw-r--r--   0        0        0      135 2024-03-05 11:27:13.618190 keble_chains-0.0.8/keble_chains/interact/ai/__init__.py
+-rw-r--r--   0        0        0     6762 2024-04-03 11:17:00.551407 keble_chains-0.0.8/keble_chains/interact/ai/azure.py
+-rw-r--r--   0        0        0     1286 2024-03-05 11:27:13.618440 keble_chains-0.0.8/keble_chains/interact/ai/fake.py
+-rw-r--r--   0        0        0     1387 2024-03-05 11:27:13.618658 keble_chains-0.0.8/keble_chains/interact/ai/session.py
+-rw-r--r--   0        0        0     4017 2024-03-05 11:27:13.618771 keble_chains-0.0.8/keble_chains/interact/ai/token_manager.py
+-rw-r--r--   0        0        0      120 2024-03-05 11:27:13.618873 keble_chains-0.0.8/keble_chains/interact/m14/__init__.py
+-rw-r--r--   0        0        0     5717 2024-03-05 11:27:13.618981 keble_chains-0.0.8/keble_chains/interact/m14/m14_compressors.py
+-rw-r--r--   0        0        0     1457 2024-03-05 11:27:13.619082 keble_chains-0.0.8/keble_chains/interact/m14/m14_session.py
+-rw-r--r--   0        0        0      232 2024-03-05 11:27:13.619198 keble_chains-0.0.8/keble_chains/template/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-05 11:27:13.619315 keble_chains-0.0.8/keble_chains/template/base.py
+-rw-r--r--   0        0        0     8179 2024-03-05 11:27:13.619488 keble_chains-0.0.8/keble_chains/template/chat.py
+-rw-r--r--   0        0        0     2632 2024-03-05 11:27:13.619602 keble_chains-0.0.8/keble_chains/template/email.py
+-rw-r--r--   0        0        0      460 2024-03-05 11:27:13.619706 keble_chains-0.0.8/keble_chains/template/openai.py
+-rw-r--r--   0        0        0       63 2024-03-05 11:27:13.619811 keble_chains-0.0.8/keble_chains/tuning/__init__.py
+-rw-r--r--   0        0        0    16219 2024-03-05 11:27:13.620867 keble_chains-0.0.8/keble_chains/tuning/datasets.py
+-rw-r--r--   0        0        0      562 2024-03-05 11:27:13.621013 keble_chains-0.0.8/keble_chains/typings/__init__.py
+-rw-r--r--   0        0        0    11627 2024-03-05 11:27:13.621272 keble_chains-0.0.8/keble_chains/typings/abc.py
+-rw-r--r--   0        0        0    10698 2024-04-19 03:51:19.840264 keble_chains-0.0.8/keble_chains/typings/ai.py
+-rw-r--r--   0        0        0      321 2024-03-05 11:27:13.621784 keble_chains-0.0.8/keble_chains/typings/collected.py
+-rw-r--r--   0        0        0     1865 2024-03-05 11:27:13.621905 keble_chains-0.0.8/keble_chains/typings/dataset.py
+-rw-r--r--   0        0        0     1922 2024-03-05 11:27:13.622026 keble_chains-0.0.8/keble_chains/typings/export.py
+-rw-r--r--   0        0        0      419 2024-03-05 11:27:13.622152 keble_chains-0.0.8/keble_chains/typings/main.py
+-rw-r--r--   0        0        0      122 2024-03-05 11:27:13.622281 keble_chains-0.0.8/keble_chains/typings/valid.py
+-rw-r--r--   0        0        0       84 2024-03-05 11:27:13.622403 keble_chains-0.0.8/keble_chains/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-03-05 11:27:13.622508 keble_chains-0.0.8/keble_chains/utils/main.py
+-rw-r--r--   0        0        0      588 2024-04-19 03:51:23.639839 keble_chains-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 keble_chains-0.0.8/PKG-INFO
```

### Comparing `keble_chains-0.0.7/LICENSE` & `keble_chains-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/chains.py` & `keble_chains-0.0.8/keble_chains/chains.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/exceptions/openai.py` & `keble_chains-0.0.8/keble_chains/exceptions/openai.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/export/export.py` & `keble_chains-0.0.8/keble_chains/export/export.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/ai/azure.py` & `keble_chains-0.0.8/keble_chains/interact/ai/azure.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/ai/fake.py` & `keble_chains-0.0.8/keble_chains/interact/ai/fake.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/ai/session.py` & `keble_chains-0.0.8/keble_chains/interact/ai/session.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/ai/token_manager.py` & `keble_chains-0.0.8/keble_chains/interact/ai/token_manager.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/m14/m14_compressors.py` & `keble_chains-0.0.8/keble_chains/interact/m14/m14_compressors.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/interact/m14/m14_session.py` & `keble_chains-0.0.8/keble_chains/interact/m14/m14_session.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/template/chat.py` & `keble_chains-0.0.8/keble_chains/template/chat.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/template/email.py` & `keble_chains-0.0.8/keble_chains/template/email.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/tuning/datasets.py` & `keble_chains-0.0.8/keble_chains/tuning/datasets.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/typings/__init__.py` & `keble_chains-0.0.8/keble_chains/typings/__init__.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/typings/abc.py` & `keble_chains-0.0.8/keble_chains/typings/abc.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/typings/ai.py` & `keble_chains-0.0.8/keble_chains/typings/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from typing import List, Tuple, Type, Any, Dict, Iterator, Optional
+import json
 from abc import ABC, abstractmethod
 from enum import Enum
+from typing import List, Tuple, Type, Any, Dict, Iterator
+
+from langchain_core.messages import HumanMessage, SystemMessage, AIMessage
 from pydantic import BaseModel
+
 from ..utils import get_string_tokens
-import json
 
 
 class AiMessageRole(str, Enum):
     system = 'system'
     user = 'user'
     assistant = 'assistant'
 
@@ -69,14 +72,44 @@
         for prompt in prompts:
             if prompt.role == AiMessageRole.user:
                 assert len(replacements) > 0, f"Insufficient user message for replacement in the prompts list"
                 replacement = replacements.pop(0)
                 prompt.content = replacement
         return prompts
 
+    def to_langchain_message(self) -> HumanMessage | SystemMessage | AIMessage:
+        if self.role == AiMessageRole.assistant:
+            return AIMessage(self.content)
+        elif self.role == AiMessageRole.user:
+            return HumanMessage(self.content)
+        elif self.role == AiMessageRole.system:
+            return SystemMessage(self.content)
+        else:
+            raise ValueError(f"Unhandled role type: {self.role}")
+
+    @classmethod
+    def from_langchain_message(cls, message: HumanMessage | SystemMessage | AIMessage) -> "AiPrompt":
+        if message.type == "human":
+            return cls(
+                role=AiMessageRole.user,
+                content=message.content
+            )
+        elif message.type == "system":
+            return cls(
+                role=AiMessageRole.system,
+                content=message.content
+            )
+        elif message.type == "ai":
+            return cls(
+                role=AiMessageRole.assistant,
+                content=message.content
+            )
+        else:
+            raise ValueError(f"Unhandled message type: {message.type}")
+
 
 AiMessage = AiPrompt | Tuple[str, str] | AiMessageObject | str
 
 Vector = List[float]
 
 
 def is_ai_prompt(maybe_prompt: Any) -> bool:
@@ -280,9 +313,7 @@
     def prompts(self) -> List[AiPrompt]:
         """Get its entire prompt in this session"""
 
     @prompts.setter
     @abstractmethod
     def prompts(self, messages: List[AiMessage]):
         """Set its entire prompt in this session"""
-
-
```

### Comparing `keble_chains-0.0.7/keble_chains/typings/dataset.py` & `keble_chains-0.0.8/keble_chains/typings/dataset.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/typings/export.py` & `keble_chains-0.0.8/keble_chains/typings/export.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/keble_chains/utils/main.py` & `keble_chains-0.0.8/keble_chains/utils/main.py`

 * *Files identical despite different names*

### Comparing `keble_chains-0.0.7/pyproject.toml` & `keble_chains-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keble-chains"
-version = "0.0.7"
+version = "0.0.8"
 description = "Keble ai model toolkit"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 packages = [{include = "keble_chains"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `keble_chains-0.0.7/PKG-INFO` & `keble_chains-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keble-chains
-Version: 0.0.7
+Version: 0.0.8
 Summary: Keble ai model toolkit
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


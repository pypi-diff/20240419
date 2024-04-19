# Comparing `tmp/grayswan_api-0.1.0a6.tar.gz` & `tmp/grayswan_api-0.1.0a7.tar.gz`

## Comparing `grayswan_api-0.1.0a6.tar` & `grayswan_api-0.1.0a7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/__init__.py
--rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_base_client.py
--rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_compat.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_constants.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_qs.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_resource.py
--rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_response.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_streaming.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_types.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/chat.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/completion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/grayswan/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/__init__.py
+-rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_base_client.py
+-rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_compat.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_constants.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_qs.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_resource.py
+-rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_response.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_streaming.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_types.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/resources/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/chat.py
+-rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/completion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/types/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/types/chat/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/gray_swan_security/types/chat/completion_create_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/src/grayswan/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a7/PKG-INFO
```

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/__init__.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_base_client.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_base_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_client.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_compat.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_compat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_exceptions.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_exceptions.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_files.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_files.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_models.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_models.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_qs.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_qs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_resource.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_resource.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_response.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_streaming.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_streaming.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_types.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_types.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/__init__.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_logs.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_proxy.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_sync.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_transform.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_typing.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_utils.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/__init__.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/chat.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/completion.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/resources/chat/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Iterable, Optional
+from typing import Any, Iterable, Optional, cast
 from typing_extensions import Literal
 
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
@@ -65,35 +65,40 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return self._post(
-            "/chat/completion",
-            body=maybe_transform(
-                {
-                    "messages": messages,
-                    "model": model,
-                    "frequency_penalty": frequency_penalty,
-                    "max_tokens": max_tokens,
-                    "n": n,
-                    "stream": stream,
-                    "temperature": temperature,
-                    "tool_choice": tool_choice,
-                    "tools": tools,
-                    "top_p": top_p,
-                },
-                completion_create_params.CompletionCreateParams,
+        return cast(
+            CompletionCreateResponse,
+            self._post(
+                "/chat/completion",
+                body=maybe_transform(
+                    {
+                        "messages": messages,
+                        "model": model,
+                        "frequency_penalty": frequency_penalty,
+                        "max_tokens": max_tokens,
+                        "n": n,
+                        "stream": stream,
+                        "temperature": temperature,
+                        "tool_choice": tool_choice,
+                        "tools": tools,
+                        "top_p": top_p,
+                    },
+                    completion_create_params.CompletionCreateParams,
+                ),
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, CompletionCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=CompletionCreateResponse,
         )
 
 
 class AsyncCompletion(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncCompletionWithRawResponse:
         return AsyncCompletionWithRawResponse(self)
@@ -130,35 +135,40 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return await self._post(
-            "/chat/completion",
-            body=await async_maybe_transform(
-                {
-                    "messages": messages,
-                    "model": model,
-                    "frequency_penalty": frequency_penalty,
-                    "max_tokens": max_tokens,
-                    "n": n,
-                    "stream": stream,
-                    "temperature": temperature,
-                    "tool_choice": tool_choice,
-                    "tools": tools,
-                    "top_p": top_p,
-                },
-                completion_create_params.CompletionCreateParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+        return cast(
+            CompletionCreateResponse,
+            await self._post(
+                "/chat/completion",
+                body=await async_maybe_transform(
+                    {
+                        "messages": messages,
+                        "model": model,
+                        "frequency_penalty": frequency_penalty,
+                        "max_tokens": max_tokens,
+                        "n": n,
+                        "stream": stream,
+                        "temperature": temperature,
+                        "tool_choice": tool_choice,
+                        "tools": tools,
+                        "top_p": top_p,
+                    },
+                    completion_create_params.CompletionCreateParams,
+                ),
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, CompletionCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            cast_to=CompletionCreateResponse,
         )
 
 
 class CompletionWithRawResponse:
     def __init__(self, completion: Completion) -> None:
         self._completion = completion
```

### Comparing `grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_params.py` & `grayswan_api-0.1.0a7/src/gray_swan_security/types/chat/completion_create_params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Dict, List, Union, Iterable, Optional
+from typing import Dict, Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = [
     "CompletionCreateParams",
     "Message",
     "ToolChoice",
     "ToolChoiceToolChoice",
     "ToolChoiceToolChoiceFunction",
     "Tool",
     "ToolFunction",
-    "ToolFunctionParameters",
-    "ToolFunctionParametersProperties",
 ]
 
 
 class CompletionCreateParams(TypedDict, total=False):
     messages: Required[Iterable[Message]]
 
     model: Required[Literal["cygnet-v0.2"]]
@@ -55,35 +53,19 @@
 
     type: Required[str]
 
 
 ToolChoice = Union[Literal["none", "auto"], ToolChoiceToolChoice]
 
 
-class ToolFunctionParametersProperties(TypedDict, total=False):
-    description: Required[str]
-
-    enum: Required[object]
-
-    type: Required[str]
-
-
-class ToolFunctionParameters(TypedDict, total=False):
-    properties: Required[Dict[str, ToolFunctionParametersProperties]]
-
-    required: Required[List[str]]
-
-    type: Required[str]
-
-
 class ToolFunction(TypedDict, total=False):
     description: Required[str]
 
     name: Required[str]
 
-    parameters: Required[ToolFunctionParameters]
+    parameters: Required[Dict[str, object]]
 
 
 class Tool(TypedDict, total=False):
     function: Required[ToolFunction]
 
     type: Required[str]
```

### Comparing `grayswan_api-0.1.0a6/LICENSE` & `grayswan_api-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a6/pyproject.toml` & `grayswan_api-0.1.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grayswan-api"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = "The official Python library for the Gray Swan Security API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Gray Swan Security", email = "dev-feedback@grayswan.ai" },
 ]
 dependencies = [
```

### Comparing `grayswan_api-0.1.0a6/PKG-INFO` & `grayswan_api-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grayswan-api
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: The official Python library for the Gray Swan Security API
 Project-URL: Homepage, https://github.com/grayswansecurity/grayswan-python
 Project-URL: Repository, https://github.com/grayswansecurity/grayswan-python
 Author-email: Gray Swan Security <dev-feedback@grayswan.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -66,15 +66,14 @@
     api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
 )
 
 completion_create_response = client.chat.completion.create(
     messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
     model="cygnet-v0.2",
 )
-print(completion_create_response.id)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `GRAYSWAN_BEARER_TOKEN="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
@@ -94,15 +93,14 @@
 
 
 async def main() -> None:
     completion_create_response = await client.chat.completion.create(
         messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
         model="cygnet-v0.2",
     )
-    print(completion_create_response.id)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -254,15 +252,15 @@
         "role": "system"
     }],
     model="cygnet-v0.2",
 )
 print(response.headers.get('X-My-Header'))
 
 completion = response.parse()  # get the object that `chat.completion.create()` would have returned
-print(completion.id)
+print(completion)
 ```
 
 These methods return an [`APIResponse`](https://github.com/grayswansecurity/grayswan-python/tree/main/src/gray_swan_security/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/grayswansecurity/grayswan-python/tree/main/src/gray_swan_security/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
```


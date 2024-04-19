# Comparing `tmp/grayswan_api-0.1.0a3.tar.gz` & `tmp/grayswan_api-0.1.0a4.tar.gz`

## Comparing `grayswan_api-0.1.0a3.tar` & `grayswan_api-0.1.0a4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/__init__.py
--rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_base_client.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_compat.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_constants.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_qs.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_resource.py
--rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_response.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_streaming.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_types.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/resources/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/chat.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/completion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/types/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/types/chat/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/gray_swan_security/types/chat/completion_create_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/src/grayswan/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/__init__.py
+-rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_base_client.py
+-rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_compat.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_constants.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_qs.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_resource.py
+-rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_response.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_streaming.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_types.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/resources/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/chat.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/completion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/types/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/types/chat/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/gray_swan_security/types/chat/completion_create_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/src/grayswan/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a4/PKG-INFO
```

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/__init__.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_base_client.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_base_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_client.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous Gray Swan Security client instance.
 
-        This automatically infers the `api_key` argument from the `GRAYSWAN_API_KEY` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `GRAYSWAN_BEARER_TOKEN` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("GRAYSWAN_API_KEY")
+            api_key = os.environ.get("GRAYSWAN_BEARER_TOKEN")
         if api_key is None:
             raise GraySwanSecurityError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_API_KEY environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_BEARER_TOKEN environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("GRAY_SWAN_SECURITY_BASE_URL")
         if base_url is None:
             base_url = f"https://api.grayswan.ai"
@@ -242,21 +242,21 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async Gray Swan Security client instance.
 
-        This automatically infers the `api_key` argument from the `GRAYSWAN_API_KEY` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `GRAYSWAN_BEARER_TOKEN` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("GRAYSWAN_API_KEY")
+            api_key = os.environ.get("GRAYSWAN_BEARER_TOKEN")
         if api_key is None:
             raise GraySwanSecurityError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_API_KEY environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_BEARER_TOKEN environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("GRAY_SWAN_SECURITY_BASE_URL")
         if base_url is None:
             base_url = f"https://api.grayswan.ai"
```

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_compat.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_compat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_exceptions.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_exceptions.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_files.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_files.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_models.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_models.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_qs.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_qs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_resource.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_resource.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_response.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_streaming.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_streaming.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_types.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_types.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/__init__.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_logs.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_proxy.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_sync.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_transform.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_typing.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/_utils/_utils.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/__init__.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/chat.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/resources/chat/completion.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/resources/chat/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Any, Iterable, Optional, cast
+from typing import Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
@@ -65,40 +65,35 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return cast(
-            CompletionCreateResponse,
-            self._post(
-                "/chat/completion/",
-                body=maybe_transform(
-                    {
-                        "messages": messages,
-                        "model": model,
-                        "frequency_penalty": frequency_penalty,
-                        "max_tokens": max_tokens,
-                        "n": n,
-                        "stream": stream,
-                        "temperature": temperature,
-                        "tool_choice": tool_choice,
-                        "tools": tools,
-                        "top_p": top_p,
-                    },
-                    completion_create_params.CompletionCreateParams,
-                ),
-                options=make_request_options(
-                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-                ),
-                cast_to=cast(
-                    Any, CompletionCreateResponse
-                ),  # Union types cannot be passed in as arguments in the type system
+        return self._post(
+            "/chat/completion/",
+            body=maybe_transform(
+                {
+                    "messages": messages,
+                    "model": model,
+                    "frequency_penalty": frequency_penalty,
+                    "max_tokens": max_tokens,
+                    "n": n,
+                    "stream": stream,
+                    "temperature": temperature,
+                    "tool_choice": tool_choice,
+                    "tools": tools,
+                    "top_p": top_p,
+                },
+                completion_create_params.CompletionCreateParams,
             ),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=CompletionCreateResponse,
         )
 
 
 class AsyncCompletion(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncCompletionWithRawResponse:
         return AsyncCompletionWithRawResponse(self)
@@ -135,40 +130,35 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return cast(
-            CompletionCreateResponse,
-            await self._post(
-                "/chat/completion/",
-                body=await async_maybe_transform(
-                    {
-                        "messages": messages,
-                        "model": model,
-                        "frequency_penalty": frequency_penalty,
-                        "max_tokens": max_tokens,
-                        "n": n,
-                        "stream": stream,
-                        "temperature": temperature,
-                        "tool_choice": tool_choice,
-                        "tools": tools,
-                        "top_p": top_p,
-                    },
-                    completion_create_params.CompletionCreateParams,
-                ),
-                options=make_request_options(
-                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-                ),
-                cast_to=cast(
-                    Any, CompletionCreateResponse
-                ),  # Union types cannot be passed in as arguments in the type system
+        return await self._post(
+            "/chat/completion/",
+            body=await async_maybe_transform(
+                {
+                    "messages": messages,
+                    "model": model,
+                    "frequency_penalty": frequency_penalty,
+                    "max_tokens": max_tokens,
+                    "n": n,
+                    "stream": stream,
+                    "temperature": temperature,
+                    "tool_choice": tool_choice,
+                    "tools": tools,
+                    "top_p": top_p,
+                },
+                completion_create_params.CompletionCreateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
+            cast_to=CompletionCreateResponse,
         )
 
 
 class CompletionWithRawResponse:
     def __init__(self, completion: Completion) -> None:
         self._completion = completion
```

### Comparing `grayswan_api-0.1.0a3/src/gray_swan_security/types/chat/completion_create_params.py` & `grayswan_api-0.1.0a4/src/gray_swan_security/types/chat/completion_create_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ToolChoice = Union[Literal["none", "auto"], ToolChoiceToolChoice]
 
 
 class ToolFunctionParametersProperties(TypedDict, total=False):
     description: Required[str]
 
-    enum: Required[Optional[Iterable[object]]]
+    enum: Required[object]
 
     type: Required[str]
 
 
 class ToolFunctionParameters(TypedDict, total=False):
     properties: Required[Dict[str, ToolFunctionParametersProperties]]
```

### Comparing `grayswan_api-0.1.0a3/LICENSE` & `grayswan_api-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a3/pyproject.toml` & `grayswan_api-0.1.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grayswan-api"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = "The official Python library for the Gray Swan Security API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Gray Swan Security", email = "dev-feedback@grayswan.ai" },
 ]
 dependencies = [
```

### Comparing `grayswan_api-0.1.0a3/PKG-INFO` & `grayswan_api-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grayswan-api
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: The official Python library for the Gray Swan Security API
 Project-URL: Homepage, https://github.com/grayswansecurity/grayswan-python
 Project-URL: Repository, https://github.com/grayswansecurity/grayswan-python
 Author-email: Gray Swan Security <dev-feedback@grayswan.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -59,48 +59,50 @@
 
 ```python
 import os
 from gray_swan_security import GraySwanSecurity
 
 client = GraySwanSecurity(
     # This is the default and can be omitted
-    api_key=os.environ.get("GRAYSWAN_API_KEY"),
+    api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
 )
 
 completion_create_response = client.chat.completion.create(
     messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
     model="cygnet-v0.2",
 )
+print(completion_create_response.id)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
-to add `GRAYSWAN_API_KEY="My API Key"` to your `.env` file
+to add `GRAYSWAN_BEARER_TOKEN="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
 ## Async usage
 
 Simply import `AsyncGraySwanSecurity` instead of `GraySwanSecurity` and use `await` with each API call:
 
 ```python
 import os
 import asyncio
 from gray_swan_security import AsyncGraySwanSecurity
 
 client = AsyncGraySwanSecurity(
     # This is the default and can be omitted
-    api_key=os.environ.get("GRAYSWAN_API_KEY"),
+    api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
 )
 
 
 async def main() -> None:
     completion_create_response = await client.chat.completion.create(
         messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
         model="cygnet-v0.2",
     )
+    print(completion_create_response.id)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -252,15 +254,15 @@
         "role": "system"
     }],
     model="cygnet-v0.2",
 )
 print(response.headers.get('X-My-Header'))
 
 completion = response.parse()  # get the object that `chat.completion.create()` would have returned
-print(completion)
+print(completion.id)
 ```
 
 These methods return an [`APIResponse`](https://github.com/grayswansecurity/grayswan-python/tree/main/src/gray_swan_security/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/grayswansecurity/grayswan-python/tree/main/src/gray_swan_security/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
```


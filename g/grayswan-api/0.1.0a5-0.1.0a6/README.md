# Comparing `tmp/grayswan_api-0.1.0a5.tar.gz` & `tmp/grayswan_api-0.1.0a6.tar.gz`

## Comparing `grayswan_api-0.1.0a5.tar` & `grayswan_api-0.1.0a6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/__init__.py
--rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_base_client.py
--rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_compat.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_constants.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_qs.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_resource.py
--rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_response.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_streaming.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_types.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/resources/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/chat.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/completion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/types/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/types/chat/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/gray_swan_security/types/chat/completion_create_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/src/grayswan/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/__init__.py
+-rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_base_client.py
+-rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_compat.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_constants.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_qs.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_resource.py
+-rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_response.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_streaming.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_types.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/chat.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/completion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/src/grayswan/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a6/PKG-INFO
```

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/__init__.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_base_client.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_base_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_client.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_compat.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_compat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_exceptions.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_exceptions.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_files.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_files.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_models.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_models.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_qs.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_qs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_resource.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_resource.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_response.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_streaming.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_streaming.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_types.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_types.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/__init__.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_logs.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_proxy.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_sync.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_transform.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_typing.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/_utils/_utils.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/__init__.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/chat.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/resources/chat/completion.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/resources/chat/completion.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/types/chat/completion_create_params.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/src/gray_swan_security/types/chat/completion_create_response.py` & `grayswan_api-0.1.0a6/src/gray_swan_security/types/chat/completion_create_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from typing import List, Optional
+from typing import List, Union, Optional
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
 __all__ = [
     "CompletionCreateResponse",
     "Choice",
@@ -40,15 +40,15 @@
 class Choice(BaseModel):
     finish_reason: Literal["stop", "length", "content_filter", "tool_calls"]
 
     index: int
 
     message: ChoiceMessage
 
-    logprobs: Optional[object] = None
+    logprobs: Union[str, object, None] = None
 
 
 class Usage(BaseModel):
     completion_tokens: int
 
     prompt_tokens: int
```

### Comparing `grayswan_api-0.1.0a5/LICENSE` & `grayswan_api-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a5/pyproject.toml` & `grayswan_api-0.1.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grayswan-api"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "The official Python library for the Gray Swan Security API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Gray Swan Security", email = "dev-feedback@grayswan.ai" },
 ]
 dependencies = [
```

### Comparing `grayswan_api-0.1.0a5/PKG-INFO` & `grayswan_api-0.1.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grayswan-api
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: The official Python library for the Gray Swan Security API
 Project-URL: Homepage, https://github.com/grayswansecurity/grayswan-python
 Project-URL: Repository, https://github.com/grayswansecurity/grayswan-python
 Author-email: Gray Swan Security <dev-feedback@grayswan.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```


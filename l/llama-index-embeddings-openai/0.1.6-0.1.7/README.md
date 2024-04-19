# Comparing `tmp/llama_index_embeddings_openai-0.1.6.tar.gz` & `tmp/llama_index_embeddings_openai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_openai-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_embeddings_openai-0.1.7.tar", max compression
```

## Comparing `llama_index_embeddings_openai-0.1.6.tar` & `llama_index_embeddings_openai-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2024-02-13 13:53:01.629184 llama_index_embeddings_openai-0.1.6/README.md
--rw-r--r--   0        0        0      286 2024-02-13 13:53:01.629432 llama_index_embeddings_openai-0.1.6/llama_index/embeddings/openai/__init__.py
--rw-r--r--   0        0        0    14610 2024-02-20 18:45:10.219685 llama_index_embeddings_openai-0.1.6/llama_index/embeddings/openai/base.py
--rw-r--r--   0        0        0     3267 2024-02-20 22:37:41.285953 llama_index_embeddings_openai-0.1.6/llama_index/embeddings/openai/utils.py
--rw-r--r--   0        0        0     1566 2024-02-21 16:33:57.223128 llama_index_embeddings_openai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 llama_index_embeddings_openai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-03-19 20:18:32.214671 llama_index_embeddings_openai-0.1.7/README.md
+-rw-r--r--   0        0        0      286 2024-03-19 20:18:32.214671 llama_index_embeddings_openai-0.1.7/llama_index/embeddings/openai/__init__.py
+-rw-r--r--   0        0        0    14911 2024-03-19 20:18:32.214671 llama_index_embeddings_openai-0.1.7/llama_index/embeddings/openai/base.py
+-rw-r--r--   0        0        0     3267 2024-03-19 20:18:32.214671 llama_index_embeddings_openai-0.1.7/llama_index/embeddings/openai/utils.py
+-rw-r--r--   0        0        0     1448 2024-03-19 20:18:32.214671 llama_index_embeddings_openai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_openai-0.1.7/PKG-INFO
```

### Comparing `llama_index_embeddings_openai-0.1.6/llama_index/embeddings/openai/base.py` & `llama_index_embeddings_openai-0.1.7/llama_index/embeddings/openai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,18 +242,18 @@
     """
 
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the OpenAI API."
     )
 
     api_key: str = Field(description="The OpenAI API key.")
-    api_base: str = Field(
+    api_base: Optional[str] = Field(
         default=DEFAULT_OPENAI_API_BASE, description="The base URL for OpenAI API."
     )
-    api_version: str = Field(
+    api_version: Optional[str] = Field(
         default=DEFAULT_OPENAI_API_VERSION, description="The version for OpenAI API."
     )
 
     max_retries: int = Field(
         default=10, description="Maximum number of retries.", gte=0
     )
     timeout: float = Field(default=60.0, description="Timeout for each request.", gte=0)
@@ -299,15 +299,15 @@
         http_client: Optional[httpx.Client] = None,
         **kwargs: Any,
     ) -> None:
         additional_kwargs = additional_kwargs or {}
         if dimensions is not None:
             additional_kwargs["dimensions"] = dimensions
 
-        api_key, api_base, api_version = resolve_openai_credentials(
+        api_key, api_base, api_version = self._resolve_credentials(
             api_key=api_key,
             api_base=api_base,
             api_version=api_version,
         )
 
         self._query_engine = get_engine(mode, model, _QUERY_MODE_MODEL_DICT)
         self._text_engine = get_engine(mode, model, _TEXT_MODE_MODEL_DICT)
@@ -334,14 +334,22 @@
             **kwargs,
         )
 
         self._client = None
         self._aclient = None
         self._http_client = http_client
 
+    def _resolve_credentials(
+        self,
+        api_key: Optional[str] = None,
+        api_base: Optional[str] = None,
+        api_version: Optional[str] = None,
+    ) -> Tuple[Optional[str], str, str]:
+        return resolve_openai_credentials(api_key, api_base, api_version)
+
     def _get_client(self) -> OpenAI:
         if not self.reuse_client:
             return OpenAI(**self._get_credential_kwargs())
 
         if self._client is None:
             self._client = OpenAI(**self._get_credential_kwargs())
         return self._client
```

### Comparing `llama_index_embeddings_openai-0.1.6/llama_index/embeddings/openai/utils.py` & `llama_index_embeddings_openai-0.1.7/llama_index/embeddings/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_openai-0.1.6/pyproject.toml` & `llama_index_embeddings_openai-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.embeddings.openai"
 
 [tool.llamahub.class_authors]
 OpenAIEmbedding = "llama-index"
-OpenAIEmbeddingMode = "llama-index"
-OpenAIEmbeddingModeModel = "llama-index"
-OpenAIEmbeddingModelType = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-openai"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_embeddings_openai-0.1.6/PKG-INFO` & `llama_index_embeddings_openai-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-openai
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index embeddings openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Openai
```


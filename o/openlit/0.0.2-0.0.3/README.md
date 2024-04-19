# Comparing `tmp/openlit-0.0.2.tar.gz` & `tmp/openlit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-0.0.2.tar", max compression
+gzip compressed data, was "openlit-0.0.3.tar", max compression
```

## Comparing `openlit-0.0.2.tar` & `openlit-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2024-04-18 10:18:44.839351 openlit-0.0.2/LICENSE
--rw-r--r--   0        0        0     5294 2024-04-18 10:18:44.839351 openlit-0.0.2/README.md
--rw-r--r--   0        0        0      929 2024-04-18 10:18:44.839351 openlit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4649 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/__helpers.py
--rw-r--r--   0        0        0     8795 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     3253 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     4293 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5686 2024-04-18 10:18:44.839351 openlit-0.0.2/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 openlit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 15:03:28.223177 openlit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9238 2024-04-19 15:03:28.223177 openlit-0.0.3/README.md
+-rw-r--r--   0        0        0      927 2024-04-19 15:03:28.223177 openlit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     8795 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    15993 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16035 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     3253 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10374 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20348 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     2531 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7609 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     3156 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21328 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21179 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8732 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     4293 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5686 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    10457 1970-01-01 00:00:00.000000 openlit-0.0.3/PKG-INFO
```

### Comparing `openlit-0.0.2/LICENSE` & `openlit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/pyproject.toml` & `openlit-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "openlit"
-version = "0.0.2"
+version = "0.0.3"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
-repository = "https://github.com/open-lit/openlit/tree/main/openlit/python"
+repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
-homepage = "https://github.com/open-lit/openlit/tree/main/openlit/python"
+homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 requests = "^2.26.0"
 tiktoken = "^0.1.1"
 opentelemetry-api = "^1.24.0"
```

### Comparing `openlit-0.0.2/src/openlit/__helpers.py` & `openlit-0.0.3/src/openlit/__helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         cost = (len(prompt) / 1000) * pricing_info["audio"][model]
     except:
         cost = 0
     return cost
 
 def fetch_pricing_info():
     """Fetches pricing information from a specified URL."""
-    pricing_url = "https://raw.githubusercontent.com/dokulabs/doku/main/assets/pricing.json"
+    pricing_url = "https://raw.githubusercontent.com/openlit/openlit/main/assets/pricing.json"
     try:
          # Set a timeout of 10 seconds for both the connection and the read
         response = requests.get(pricing_url, timeout=20)
         response.raise_for_status()
         return response.json()
     except requests.HTTPError as http_err:
         logger.error("HTTP error occured while fetching pricing info: %s", http_err)
```

### Comparing `openlit-0.0.2/src/openlit/__init__.py` & `openlit-0.0.3/src/openlit/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-0.0.3/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-0.0.3/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/chroma/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/chroma/chroma.py` & `openlit-0.0.3/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/cohere/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/cohere/cohere.py` & `openlit-0.0.3/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/langchain/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/langchain/langchain.py` & `openlit-0.0.3/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/mistral/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-0.0.3/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/mistral/mistral.py` & `openlit-0.0.3/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/openai/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-0.0.3/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/openai/async_openai.py` & `openlit-0.0.3/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-0.0.3/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/openai/openai.py` & `openlit-0.0.3/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-0.0.3/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/transformers/__init__.py` & `openlit-0.0.3/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/instrumentation/transformers/transformers.py` & `openlit-0.0.3/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/otel/metrics.py` & `openlit-0.0.3/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/otel/tracing.py` & `openlit-0.0.3/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.2/src/openlit/semcov/__init__.py` & `openlit-0.0.3/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*


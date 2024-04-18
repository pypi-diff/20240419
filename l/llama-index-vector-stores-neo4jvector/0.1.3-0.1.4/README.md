# Comparing `tmp/llama_index_vector_stores_neo4jvector-0.1.3.tar.gz` & `tmp/llama_index_vector_stores_neo4jvector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_neo4jvector-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_neo4jvector-0.1.4.tar", max compression
```

## Comparing `llama_index_vector_stores_neo4jvector-0.1.3.tar` & `llama_index_vector_stores_neo4jvector-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2024-02-13 13:53:02.013361 llama_index_vector_stores_neo4jvector-0.1.3/README.md
--rw-r--r--   0        0        0      104 2024-02-13 13:53:02.013599 llama_index_vector_stores_neo4jvector-0.1.3/llama_index/vector_stores/neo4jvector/__init__.py
--rw-r--r--   0        0        0    14236 2024-02-20 18:45:10.366517 llama_index_vector_stores_neo4jvector-0.1.3/llama_index/vector_stores/neo4jvector/base.py
--rw-r--r--   0        0        0     1491 2024-02-21 23:33:17.868849 llama_index_vector_stores_neo4jvector-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 llama_index_vector_stores_neo4jvector-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-04-18 22:07:35.441385 llama_index_vector_stores_neo4jvector-0.1.4/README.md
+-rw-r--r--   0        0        0      104 2024-04-18 22:07:35.441385 llama_index_vector_stores_neo4jvector-0.1.4/llama_index/vector_stores/neo4jvector/__init__.py
+-rw-r--r--   0        0        0    18948 2024-04-18 22:07:35.445385 llama_index_vector_stores_neo4jvector-0.1.4/llama_index/vector_stores/neo4jvector/base.py
+-rw-r--r--   0        0        0     1491 2024-04-18 22:07:35.445385 llama_index_vector_stores_neo4jvector-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_vector_stores_neo4jvector-0.1.4/PKG-INFO
```

### Comparing `llama_index_vector_stores_neo4jvector-0.1.3/pyproject.toml` & `llama_index_vector_stores_neo4jvector-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores neo4jvector integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-neo4jvector"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 neo4j = "^5.16.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_neo4jvector-0.1.3/PKG-INFO` & `llama_index_vector_stores_neo4jvector-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-neo4jvector
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index vector_stores neo4jvector integration
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
 Requires-Dist: neo4j (>=5.16.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Neo4Jvector
```


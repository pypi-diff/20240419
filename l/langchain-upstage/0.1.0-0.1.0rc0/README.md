# Comparing `tmp/langchain_upstage-0.1.0.tar.gz` & `tmp/langchain_upstage-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.0.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.0rc0.tar", max compression
```

## Comparing `langchain_upstage-0.1.0.tar` & `langchain_upstage-0.1.0rc0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/LICENSE
--rw-r--r--   0        0        0      979 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/README.md
--rw-r--r--   0        0        0      161 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/langchain_upstage/py.typed
--rw-r--r--   0        0        0     2658 2024-04-19 02:03:25.906135 langchain_upstage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 langchain_upstage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0      979 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/README.md
+-rw-r--r--   0        0        0      161 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9097 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     2661 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 langchain_upstage-0.1.0rc0/PKG-INFO
```

### Comparing `langchain_upstage-0.1.0/LICENSE` & `langchain_upstage-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0/README.md` & `langchain_upstage-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.0rc0/langchain_upstage/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.0rc0/langchain_upstage/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0/pyproject.toml` & `langchain_upstage-0.1.0rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.0"
+version = "0.1.0rc0"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_upstage-0.1.0/PKG-INFO` & `langchain_upstage-0.1.0rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


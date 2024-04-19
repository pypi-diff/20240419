# Comparing `tmp/gptify-0.3.0.tar.gz` & `tmp/gptify-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptify-0.3.0.tar", max compression
+gzip compressed data, was "gptify-0.3.1.tar", max compression
```

## Comparing `gptify-0.3.0.tar` & `gptify-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1234 2024-04-13 04:51:55.154941 gptify-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-13 04:51:55.154941 gptify-0.3.0/gptify/__init__.py
--rw-r--r--   0        0        0      201 2024-04-13 04:51:55.154941 gptify-0.3.0/gptify/cli.py
--rw-r--r--   0        0        0     4665 2024-04-13 04:51:55.154941 gptify-0.3.0/gptify/gpt_repository_loader.py
--rw-r--r--   0        0        0      465 2024-04-13 04:51:55.154941 gptify-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1234 2024-04-19 05:06:48.947055 gptify-0.3.1/README.md
+-rw-r--r--   0        0        0      248 2024-04-19 05:06:48.947055 gptify-0.3.1/gptify/.gptignore
+-rw-r--r--   0        0        0        0 2024-04-19 05:06:48.947055 gptify-0.3.1/gptify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-19 05:06:48.947055 gptify-0.3.1/gptify/cli.py
+-rw-r--r--   0        0        0     4665 2024-04-19 05:06:48.947055 gptify-0.3.1/gptify/gpt_repository_loader.py
+-rw-r--r--   0        0        0      465 2024-04-19 05:06:48.947055 gptify-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.1/PKG-INFO
```

### Comparing `gptify-0.3.0/README.md` & `gptify-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gptify-0.3.0/gptify/gpt_repository_loader.py` & `gptify-0.3.1/gptify/gpt_repository_loader.py`

 * *Files identical despite different names*

### Comparing `gptify-0.3.0/PKG-INFO` & `gptify-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptify
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convert code repos into an LLM prompt-friendly format. Forked from https://github.com/zackees/gptrepo
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


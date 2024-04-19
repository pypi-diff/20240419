# Comparing `tmp/goose_checker-0.0.7.tar.gz` & `tmp/goose_checker-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goose_checker-0.0.7.tar", max compression
+gzip compressed data, was "goose_checker-0.0.8.tar", max compression
```

## Comparing `goose_checker-0.0.7.tar` & `goose_checker-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-19 02:33:05.163103 goose_checker-0.0.7/LICENSE
--rw-r--r--   0        0        0     1448 2024-04-19 02:33:05.163103 goose_checker-0.0.7/README.md
--rw-r--r--   0        0        0     5553 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/chains.py
--rw-r--r--   0        0        0     4131 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/cli.py
--rw-r--r--   0        0        0      779 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/context.py
--rw-r--r--   0        0        0     1390 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/diff.py
--rw-r--r--   0        0        0     2776 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/goose_ascii.py
--rw-r--r--   0        0        0     2386 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/models.py
--rw-r--r--   0        0        0     1164 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/prompts.py
--rw-r--r--   0        0        0      924 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/response_schema.py
--rw-r--r--   0        0        0      573 2024-04-19 02:33:05.163103 goose_checker-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 02:46:29.815952 goose_checker-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-19 02:46:29.815952 goose_checker-0.0.8/README.md
+-rw-r--r--   0        0        0     5553 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/chains.py
+-rw-r--r--   0        0        0     4394 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/cli.py
+-rw-r--r--   0        0        0      779 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/context.py
+-rw-r--r--   0        0        0     1390 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/diff.py
+-rw-r--r--   0        0        0     2776 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/goose_ascii.py
+-rw-r--r--   0        0        0     2386 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/models.py
+-rw-r--r--   0        0        0     1164 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/prompts.py
+-rw-r--r--   0        0        0      924 2024-04-19 02:46:29.815952 goose_checker-0.0.8/goose_checker/response_schema.py
+-rw-r--r--   0        0        0      573 2024-04-19 02:46:29.815952 goose_checker-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.8/PKG-INFO
```

### Comparing `goose_checker-0.0.7/LICENSE` & `goose_checker-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/README.md` & `goose_checker-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/chains.py` & `goose_checker-0.0.8/goose_checker/chains.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/cli.py` & `goose_checker-0.0.8/goose_checker/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import warnings
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from dotenv import load_dotenv
 from pydantic import BaseModel
 
 from goose_checker.chains import (approve_or_deny, base_checker,
@@ -57,14 +58,16 @@
         help=f"The cloud provider to use, choices are: {supported_providers}"
     )
 
     args = parser.parse_args()
     return AppConfig(**vars(args))
 
 def main(config: AppConfig):
+    
+    warnings.filterwarnings("ignore", message="Importing verbose from langchain root module is no longer supported")
     print(f"Checking for geese by comparing to {config.branch}")
     print(f"Using model: {config.model} provided by {config.provider}")
 
     if config.provider == "azure":
         goose_checker = AzureGooseChecker(
             with_respect_to=config.branch, deployment_name=config.model
         )
@@ -72,14 +75,18 @@
         goose_checker = OpenAIGooseChecker(
             with_respect_to=config.branch, model=config.model
         )
     else:
         raise ValueError(f"Provider specified not supported: {config.provider}")
 
     diffs = get_git_diffs(with_respect_to=config.branch)
+    
+    print("Checking these files for geese-like behaviour...")
+    for diff in diffs:
+        print(f"{diff.file_name}")
 
     if len(diffs) == 0:
         print(
             f"Compared your current checked out branch to {config.branch} and found nothing to check"
         )
         return False
```

### Comparing `goose_checker-0.0.7/goose_checker/context.py` & `goose_checker-0.0.8/goose_checker/context.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/diff.py` & `goose_checker-0.0.8/goose_checker/diff.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/goose_ascii.py` & `goose_checker-0.0.8/goose_checker/goose_ascii.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/models.py` & `goose_checker-0.0.8/goose_checker/models.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/prompts.py` & `goose_checker-0.0.8/goose_checker/prompts.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/goose_checker/response_schema.py` & `goose_checker-0.0.8/goose_checker/response_schema.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.7/pyproject.toml` & `goose_checker-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goose-checker"
-version = "0.0.7"
+version = "0.0.8"
 description = "State of the Art Silly Goose Detection Technology"
 authors = ["AdamPaslawski <adampaslawski@gmail.com>"]
 readme = "README.md"
 packages = [{include = "goose_checker"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `goose_checker-0.0.7/PKG-INFO` & `goose_checker-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goose-checker
-Version: 0.0.7
+Version: 0.0.8
 Summary: State of the Art Silly Goose Detection Technology
 Author: AdamPaslawski
 Author-email: adampaslawski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/goose_checker-0.0.6.tar.gz` & `tmp/goose_checker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goose_checker-0.0.6.tar", max compression
+gzip compressed data, was "goose_checker-0.0.7.tar", max compression
```

## Comparing `goose_checker-0.0.6.tar` & `goose_checker-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-19 02:24:08.391046 goose_checker-0.0.6/LICENSE
--rw-r--r--   0        0        0     1448 2024-04-19 02:24:08.391046 goose_checker-0.0.6/README.md
--rw-r--r--   0        0        0     5553 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/chains.py
--rw-r--r--   0        0        0     3952 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/cli.py
--rw-r--r--   0        0        0      779 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/context.py
--rw-r--r--   0        0        0     1390 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/diff.py
--rw-r--r--   0        0        0     2776 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/goose_ascii.py
--rw-r--r--   0        0        0     2386 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/models.py
--rw-r--r--   0        0        0     1164 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/prompts.py
--rw-r--r--   0        0        0      924 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/response_schema.py
--rw-r--r--   0        0        0      573 2024-04-19 02:24:08.395046 goose_checker-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 02:33:05.163103 goose_checker-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-19 02:33:05.163103 goose_checker-0.0.7/README.md
+-rw-r--r--   0        0        0     5553 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/chains.py
+-rw-r--r--   0        0        0     4131 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/cli.py
+-rw-r--r--   0        0        0      779 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/context.py
+-rw-r--r--   0        0        0     1390 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/diff.py
+-rw-r--r--   0        0        0     2776 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/goose_ascii.py
+-rw-r--r--   0        0        0     2386 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/models.py
+-rw-r--r--   0        0        0     1164 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/prompts.py
+-rw-r--r--   0        0        0      924 2024-04-19 02:33:05.163103 goose_checker-0.0.7/goose_checker/response_schema.py
+-rw-r--r--   0        0        0      573 2024-04-19 02:33:05.163103 goose_checker-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.7/PKG-INFO
```

### Comparing `goose_checker-0.0.6/LICENSE` & `goose_checker-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/README.md` & `goose_checker-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/chains.py` & `goose_checker-0.0.7/goose_checker/chains.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/cli.py` & `goose_checker-0.0.7/goose_checker/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from goose_checker.diff import get_git_diffs
 from goose_checker.goose_ascii import detected_ascii, goose_ascii
 from goose_checker.models import (AzureGooseChecker, GooseChecker,
                                   GooseCheckerResponse, OpenAIGooseChecker)
 
 
 class AppConfig(BaseModel):
-    branch: str = os.environ.get("GOOSE_CHECKER_BRANCH_NAME", "main")
-    model: str = os.environ.get("GOOSE_CHECKER_MODEL_NAME", "gpt-3.5-turbo")
-    provider: str = os.environ.get("GOOSE_CHECKER_PROVIDER", "openai")
+    branch: str
+    model: str
+    provider: str
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
 def run_checker(diff, goose_checker: GooseChecker):
@@ -39,32 +39,30 @@
             print(f"Other Issues: {response.other_issues}")
             print("\n")
 
 
 def parse_args() -> AppConfig:
     parser = argparse.ArgumentParser(description="Checks if you goofed")
     parser.add_argument(
-        "--branch", nargs="?", help="The branch or commit to compare against"
+        "--branch", nargs="?", default=os.environ.get("GOOSE_CHECKER_BRANCH_NAME", "main"),
+        help="The branch or commit to compare against"
     )
     parser.add_argument(
-        "--model",
-        nargs="?",
-        help="LLM model to use, for Azure instances this is the deployment ID.",
+        "--model", nargs="?", default=os.environ.get("GOOSE_CHECKER_MODEL_NAME", "gpt-3.5-turbo"),
+        help="LLM model to use, for Azure instances this is the deployment ID."
     )
     supported_providers = ["azure", "openai"]
     parser.add_argument(
-        "--provider",
-        nargs="?",
-        choices=supported_providers,
-        help=f"The cloud provider to use, choices are: {supported_providers}",
+        "--provider", nargs="?", choices=supported_providers,
+        default=os.environ.get("GOOSE_CHECKER_PROVIDER", "openai"),
+        help=f"The cloud provider to use, choices are: {supported_providers}"
     )
 
     args = parser.parse_args()
-    return AppConfig(branch=args.branch, model=args.model, provider=args.provider)
-
+    return AppConfig(**vars(args))
 
 def main(config: AppConfig):
     print(f"Checking for geese by comparing to {config.branch}")
     print(f"Using model: {config.model} provided by {config.provider}")
 
     if config.provider == "azure":
         goose_checker = AzureGooseChecker(
@@ -114,9 +112,13 @@
 def cli_main():
     config = parse_args()
     main(config)
 
 
 if __name__ == "__main__":
     load_dotenv()
-    config = AppConfig()
+    config = AppConfig(
+        branch=os.environ.get("GOOSE_CHECKER_BRANCH_NAME", "main"),
+        model=os.environ.get("GOOSE_CHECKER_MODEL_NAME", "gpt-3.5-turbo"),
+        provider=os.environ.get("GOOSE_CHECKER_PROVIDER", "openai"),
+    )
     main(config)
```

### Comparing `goose_checker-0.0.6/goose_checker/context.py` & `goose_checker-0.0.7/goose_checker/context.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/diff.py` & `goose_checker-0.0.7/goose_checker/diff.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/goose_ascii.py` & `goose_checker-0.0.7/goose_checker/goose_ascii.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/models.py` & `goose_checker-0.0.7/goose_checker/models.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/prompts.py` & `goose_checker-0.0.7/goose_checker/prompts.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/goose_checker/response_schema.py` & `goose_checker-0.0.7/goose_checker/response_schema.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.6/pyproject.toml` & `goose_checker-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goose-checker"
-version = "0.0.6"
+version = "0.0.7"
 description = "State of the Art Silly Goose Detection Technology"
 authors = ["AdamPaslawski <adampaslawski@gmail.com>"]
 readme = "README.md"
 packages = [{include = "goose_checker"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `goose_checker-0.0.6/PKG-INFO` & `goose_checker-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goose-checker
-Version: 0.0.6
+Version: 0.0.7
 Summary: State of the Art Silly Goose Detection Technology
 Author: AdamPaslawski
 Author-email: adampaslawski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


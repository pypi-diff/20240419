# Comparing `tmp/goose_checker-0.0.5.tar.gz` & `tmp/goose_checker-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goose_checker-0.0.5.tar", max compression
+gzip compressed data, was "goose_checker-0.0.6.tar", max compression
```

## Comparing `goose_checker-0.0.5.tar` & `goose_checker-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-11 14:18:08.881893 goose_checker-0.0.5/LICENSE
--rw-r--r--   0        0        0     1321 2024-04-11 14:18:08.881893 goose_checker-0.0.5/README.md
--rw-r--r--   0        0        0     5553 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/chains.py
--rw-r--r--   0        0        0     3558 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/cli.py
--rw-r--r--   0        0        0      779 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/context.py
--rw-r--r--   0        0        0     1254 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/diff.py
--rw-r--r--   0        0        0     2776 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/goose_ascii.py
--rw-r--r--   0        0        0     2386 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/models.py
--rw-r--r--   0        0        0     1164 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/prompts.py
--rw-r--r--   0        0        0      924 2024-04-11 14:18:08.881893 goose_checker-0.0.5/goose_checker/response_schema.py
--rw-r--r--   0        0        0      573 2024-04-11 14:18:08.881893 goose_checker-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 goose_checker-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 02:24:08.391046 goose_checker-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-19 02:24:08.391046 goose_checker-0.0.6/README.md
+-rw-r--r--   0        0        0     5553 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/chains.py
+-rw-r--r--   0        0        0     3952 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/cli.py
+-rw-r--r--   0        0        0      779 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/context.py
+-rw-r--r--   0        0        0     1390 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/diff.py
+-rw-r--r--   0        0        0     2776 2024-04-19 02:24:08.391046 goose_checker-0.0.6/goose_checker/goose_ascii.py
+-rw-r--r--   0        0        0     2386 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/models.py
+-rw-r--r--   0        0        0     1164 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/prompts.py
+-rw-r--r--   0        0        0      924 2024-04-19 02:24:08.395046 goose_checker-0.0.6/goose_checker/response_schema.py
+-rw-r--r--   0        0        0      573 2024-04-19 02:24:08.395046 goose_checker-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 goose_checker-0.0.6/PKG-INFO
```

### Comparing `goose_checker-0.0.5/LICENSE` & `goose_checker-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/README.md` & `goose_checker-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 ![goose checker logo](https://raw.githubusercontent.com/AdamPaslawski/goose-checker/main/assets/goose_checker.svg)
 
 # goose-checker
 Military Grade Silly Goose Detection
 
+# Quick Start
+Navigate to a git repository on your machine
+```
+export OPENAI_API_KEY=your-api-key-goes-here
+goose-checker
+```
+
 
 # Setup
 
 ## 1. Installation
 
 via pipx
```

### Comparing `goose_checker-0.0.5/goose_checker/chains.py` & `goose_checker-0.0.6/goose_checker/chains.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         other_issues=output["other_issues_explanation"],
     )
 
 
 def approve_or_deny(
     responses: list[GooseCheckerResponse], goose_checker: GooseChecker
 ) -> tuple[bool, str]:
-    response_schemas = [approve_or_deny_schema, silly_mistakes_aggregation_schema]
+    response_schemas = [silly_mistakes_aggregation_schema, approve_or_deny_schema]
     output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
     format_instructions = output_parser.get_format_instructions()
     model = goose_checker._get_model()
 
     evaluations_subprompt = ""
 
     for response in responses:
```

### Comparing `goose_checker-0.0.5/goose_checker/cli.py` & `goose_checker-0.0.6/goose_checker/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import argparse
-from concurrent.futures import ThreadPoolExecutor, as_completed
 import os
+from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from dotenv import load_dotenv
+from pydantic import BaseModel
 
-from goose_checker.chains import (base_checker, approve_or_deny,
+from goose_checker.chains import (approve_or_deny, base_checker,
                                   terraform_checker)
 from goose_checker.diff import get_git_diffs
 from goose_checker.goose_ascii import detected_ascii, goose_ascii
-from goose_checker.models import (AzureGooseChecker, GooseCheckerResponse,
-                                  OpenAIGooseChecker)
+from goose_checker.models import (AzureGooseChecker, GooseChecker,
+                                  GooseCheckerResponse, OpenAIGooseChecker)
+
+
+class AppConfig(BaseModel):
+    branch: str = os.environ.get("GOOSE_CHECKER_BRANCH_NAME", "main")
+    model: str = os.environ.get("GOOSE_CHECKER_MODEL_NAME", "gpt-3.5-turbo")
+    provider: str = os.environ.get("GOOSE_CHECKER_PROVIDER", "openai")
 
+    class Config:
+        env_file = ".env"
+        env_file_encoding = "utf-8"
 
-def run_checker(diff, goose_checker):
+
+def run_checker(diff, goose_checker: GooseChecker):
     if diff.file_name.endswith(".tf"):
         return terraform_checker(diff=diff, goose_checker=goose_checker)
     else:
         return base_checker(diff=diff, goose_checker=goose_checker)
 
 
 def display_issues(responses: list[GooseCheckerResponse]):
@@ -25,85 +36,87 @@
             print("\n")
             print(f"File Name: {response.file_name}")
             print(f"Silly Mistakes: {response.silly_mistakes}")
             print(f"Other Issues: {response.other_issues}")
             print("\n")
 
 
-def cli_main():
+def parse_args() -> AppConfig:
     parser = argparse.ArgumentParser(description="Checks if you goofed")
     parser.add_argument(
-        "--branch",
-        nargs="?",
-        default=os.environ.get("GOOSE_CHECKER_BRANCH_NAME", "main"),
-        help="The branch or commit to compare against",
+        "--branch", nargs="?", help="The branch or commit to compare against"
     )
     parser.add_argument(
         "--model",
         nargs="?",
-        default=os.environ.get("GOOSE_CHECKER_MODEL_NAME", "gpt-3.5-turbo"),
         help="LLM model to use, for Azure instances this is the deployment ID.",
     )
-
     supported_providers = ["azure", "openai"]
     parser.add_argument(
         "--provider",
         nargs="?",
-        default=os.environ.get("GOOSE_CHECKER_PROVIDER","openai"),
         choices=supported_providers,
         help=f"The cloud provider to use, choices are: {supported_providers}",
     )
 
     args = parser.parse_args()
+    return AppConfig(branch=args.branch, model=args.model, provider=args.provider)
 
-    print(f"Checking for geese by comparing to {args.branch}")
-    print(f"Using model: {args.model} provided by {args.provider}")
 
-    if args.provider == "azure":
+def main(config: AppConfig):
+    print(f"Checking for geese by comparing to {config.branch}")
+    print(f"Using model: {config.model} provided by {config.provider}")
+
+    if config.provider == "azure":
         goose_checker = AzureGooseChecker(
-            with_respect_to=args.branch, deployment_name=args.model
+            with_respect_to=config.branch, deployment_name=config.model
         )
-    elif args.provider == "openai":
+    elif config.provider == "openai":
         goose_checker = OpenAIGooseChecker(
-            with_respect_to=args.branch, model=args.model
+            with_respect_to=config.branch, model=config.model
         )
     else:
-        raise ValueError(f"Provider specified not supported: {args.provider}")
+        raise ValueError(f"Provider specified not supported: {config.provider}")
 
-    # Lets Cook
+    diffs = get_git_diffs(with_respect_to=config.branch)
 
-    diffs = get_git_diffs(with_respect_to=args.branch)
+    if len(diffs) == 0:
+        print(
+            f"Compared your current checked out branch to {config.branch} and found nothing to check"
+        )
+        return False
 
     all_responses = []
-    # Initialize ThreadPoolExecutor
     with ThreadPoolExecutor(max_workers=4) as executor:
-        # Submit tasks to the executor
         future_to_diff = {
             executor.submit(run_checker, diff, goose_checker): diff for diff in diffs
         }
-        # Retrieve and store results as they complete
         for future in as_completed(future_to_diff):
             diff = future_to_diff[future]
             try:
                 resp = future.result()
                 all_responses.append(resp)
             except Exception as exc:
                 print(f"Failed to analyze {diff.file_name} due to {exc}")
-    if not all_responses:
-        return False
 
     approved, explanation = approve_or_deny(all_responses, goose_checker)
 
     if not approved:
         print(goose_ascii)
         print(detected_ascii)
         print(explanation)
-    
+        return approved
     else:
         print("Approved! No Geese detected.")
 
     return approved
 
 
+def cli_main():
+    config = parse_args()
+    main(config)
+
+
 if __name__ == "__main__":
     load_dotenv()
-    cli_main()
+    config = AppConfig()
+    main(config)
```

### Comparing `goose_checker-0.0.5/goose_checker/context.py` & `goose_checker-0.0.6/goose_checker/context.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/goose_checker/diff.py` & `goose_checker-0.0.6/goose_checker/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,14 @@
 
 
 def get_git_diffs(with_respect_to: str) -> list[GitDiff]:
     """Get all files with a diff compared to the given branch or commit."""
     files_with_diff = get_all_files_with_diff(with_respect_to)
     diffs = []
     for file in files_with_diff:
-        diff = _get_diff_for_file(file, with_respect_to)
+        try:
+            diff = _get_diff_for_file(file, with_respect_to)
+        except subprocess.CalledProcessError:
+            print(f"Failed to get diff for {file}")
+            continue
         diffs.append(GitDiff(file_name=file, diff=diff))
     return diffs
```

### Comparing `goose_checker-0.0.5/goose_checker/goose_ascii.py` & `goose_checker-0.0.6/goose_checker/goose_ascii.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/goose_checker/models.py` & `goose_checker-0.0.6/goose_checker/models.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/goose_checker/prompts.py` & `goose_checker-0.0.6/goose_checker/prompts.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/goose_checker/response_schema.py` & `goose_checker-0.0.6/goose_checker/response_schema.py`

 * *Files identical despite different names*

### Comparing `goose_checker-0.0.5/pyproject.toml` & `goose_checker-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goose-checker"
-version = "0.0.5"
+version = "0.0.6"
 description = "State of the Art Silly Goose Detection Technology"
 authors = ["AdamPaslawski <adampaslawski@gmail.com>"]
 readme = "README.md"
 packages = [{include = "goose_checker"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `goose_checker-0.0.5/PKG-INFO` & `goose_checker-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goose-checker
-Version: 0.0.5
+Version: 0.0.6
 Summary: State of the Art Silly Goose Detection Technology
 Author: AdamPaslawski
 Author-email: adampaslawski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,14 +18,21 @@
 Description-Content-Type: text/markdown
 
 ![goose checker logo](https://raw.githubusercontent.com/AdamPaslawski/goose-checker/main/assets/goose_checker.svg)
 
 # goose-checker
 Military Grade Silly Goose Detection
 
+# Quick Start
+Navigate to a git repository on your machine
+```
+export OPENAI_API_KEY=your-api-key-goes-here
+goose-checker
+```
+
 
 # Setup
 
 ## 1. Installation
 
 via pipx
```


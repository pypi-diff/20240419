# Comparing `tmp/commitcrafter-0.1.4.tar.gz` & `tmp/commitcrafter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcrafter-0.1.4.tar", max compression
+gzip compressed data, was "commitcrafter-0.1.5.tar", max compression
```

## Comparing `commitcrafter-0.1.4.tar` & `commitcrafter-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.4/commitcrafter/__init__.py
--rw-r--r--   0        0        0     1010 2024-04-19 15:24:21.810829 commitcrafter-0.1.4/commitcrafter/cli.py
--rw-r--r--   0        0        0     1691 2024-04-19 15:23:24.364456 commitcrafter-0.1.4/commitcrafter/commitcrafter.py
--rw-r--r--   0        0        0       42 2024-04-19 14:52:43.909465 commitcrafter-0.1.4/commitcrafter/exceptions.py
--rw-r--r--   0        0        0      544 2024-04-19 14:23:56.857977 commitcrafter-0.1.4/commitcrafter/git_tools.py
--rw-r--r--   0        0        0     1010 2024-04-19 14:55:53.329167 commitcrafter-0.1.4/commitcrafter/gpt_integration.py
--rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.4/commitcrafter/prompt.txt
--rw-r--r--   0        0        0      444 2024-04-19 15:25:01.148243 commitcrafter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 commitcrafter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.5/commitcrafter/__init__.py
+-rw-r--r--   0        0        0      972 2024-04-19 15:26:15.446622 commitcrafter-0.1.5/commitcrafter/cli.py
+-rw-r--r--   0        0        0     1691 2024-04-19 15:23:24.364456 commitcrafter-0.1.5/commitcrafter/commitcrafter.py
+-rw-r--r--   0        0        0       42 2024-04-19 14:52:43.909465 commitcrafter-0.1.5/commitcrafter/exceptions.py
+-rw-r--r--   0        0        0      544 2024-04-19 14:23:56.857977 commitcrafter-0.1.5/commitcrafter/git_tools.py
+-rw-r--r--   0        0        0     1010 2024-04-19 14:55:53.329167 commitcrafter-0.1.5/commitcrafter/gpt_integration.py
+-rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.5/commitcrafter/prompt.txt
+-rw-r--r--   0        0        0      444 2024-04-19 15:26:20.734621 commitcrafter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 commitcrafter-0.1.5/PKG-INFO
```

### Comparing `commitcrafter-0.1.4/commitcrafter/cli.py` & `commitcrafter-0.1.5/commitcrafter/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,12 @@
         print(
             f"[bold red]{e}[/bold red] : Please set the COMMITCRAFT_OPENAI_API_KEY environment variable.\n\n"
             f"=> export COMMITCRAFT_OPENAI_API_KEY='your-api-key' <="
         )
     except EmptyDiffError:
         print(":man_facepalming: [bold]No changes found in the latest commit[/bold] :man_facepalming: ")
     except InvalidGitRepositoryError:
-        print(f":neutral_face:\n"
-              f"[bold]No git repository found at {os.getcwd()}[bold]\n"
-              f":neutral_face:")
+        print(f":neutral_face: [bold]No git repository found at {os.getcwd()}[bold] :neutral_face:")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `commitcrafter-0.1.4/commitcrafter/commitcrafter.py` & `commitcrafter-0.1.5/commitcrafter/commitcrafter.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.4/commitcrafter/git_tools.py` & `commitcrafter-0.1.5/commitcrafter/git_tools.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.4/commitcrafter/gpt_integration.py` & `commitcrafter-0.1.5/commitcrafter/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.4/commitcrafter/prompt.txt` & `commitcrafter-0.1.5/commitcrafter/prompt.txt`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.4/PKG-INFO` & `commitcrafter-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcrafter
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: mpruvot
 Author-email: marius.pruvot@outlook.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
```


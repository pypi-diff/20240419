# Comparing `tmp/commitcrafter-0.1.1.tar.gz` & `tmp/commitcrafter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcrafter-0.1.1.tar", max compression
+gzip compressed data, was "commitcrafter-0.1.2.tar", max compression
```

## Comparing `commitcrafter-0.1.1.tar` & `commitcrafter-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.1/commitcrafter/__init__.py
--rw-r--r--   0        0        0      523 2024-04-19 13:41:17.502609 commitcrafter-0.1.1/commitcrafter/cli.py
--rw-r--r--   0        0        0      544 2024-04-19 14:04:56.564239 commitcrafter-0.1.1/commitcrafter/git_tools.py
--rw-r--r--   0        0        0     1104 2024-04-19 14:04:56.564241 commitcrafter-0.1.1/commitcrafter/gpt_integration.py
--rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.1/commitcrafter/prompt.txt
--rw-r--r--   0        0        0      427 2024-04-19 14:06:18.635225 commitcrafter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 commitcrafter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.2/commitcrafter/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-19 14:07:25.263294 commitcrafter-0.1.2/commitcrafter/cli.py
+-rw-r--r--   0        0        0      544 2024-04-19 14:04:56.564239 commitcrafter-0.1.2/commitcrafter/git_tools.py
+-rw-r--r--   0        0        0     1104 2024-04-19 14:04:56.564241 commitcrafter-0.1.2/commitcrafter/gpt_integration.py
+-rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.2/commitcrafter/prompt.txt
+-rw-r--r--   0        0        0      427 2024-04-19 14:07:48.804228 commitcrafter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 commitcrafter-0.1.2/PKG-INFO
```

### Comparing `commitcrafter-0.1.1/commitcrafter/cli.py` & `commitcrafter-0.1.2/commitcrafter/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 
 
 @app.command()
 def generate():
     """Generate commit names based on the latest git diff."""
     diff = get_latest_diff(os.getcwd())
     if diff:
-        commit_names = generate_commit_names_using_chat(diff)
-        for name in commit_names:
-            typer.echo(name)
+        try:
+            commit_names = generate_commit_names_using_chat(diff)
+            for name in commit_names:
+                typer.echo(name)
+        except ValueError as e:
+            typer.echo(str(e))
     else:
         typer.echo("No diff found or diff is empty.")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `commitcrafter-0.1.1/commitcrafter/git_tools.py` & `commitcrafter-0.1.2/commitcrafter/git_tools.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.1/commitcrafter/gpt_integration.py` & `commitcrafter-0.1.2/commitcrafter/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.1/commitcrafter/prompt.txt` & `commitcrafter-0.1.2/commitcrafter/prompt.txt`

 * *Files identical despite different names*


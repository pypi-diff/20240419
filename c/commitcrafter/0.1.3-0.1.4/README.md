# Comparing `tmp/commitcrafter-0.1.3.tar.gz` & `tmp/commitcrafter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcrafter-0.1.3.tar", max compression
+gzip compressed data, was "commitcrafter-0.1.4.tar", max compression
```

## Comparing `commitcrafter-0.1.3.tar` & `commitcrafter-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.3/commitcrafter/__init__.py
--rw-r--r--   0        0        0      780 2024-04-19 15:11:09.409768 commitcrafter-0.1.3/commitcrafter/cli.py
--rw-r--r--   0        0        0     1747 2024-04-19 15:10:31.464108 commitcrafter-0.1.3/commitcrafter/commitcrafter.py
--rw-r--r--   0        0        0       42 2024-04-19 14:52:43.909465 commitcrafter-0.1.3/commitcrafter/exceptions.py
--rw-r--r--   0        0        0      544 2024-04-19 14:23:56.857977 commitcrafter-0.1.3/commitcrafter/git_tools.py
--rw-r--r--   0        0        0     1010 2024-04-19 14:55:53.329167 commitcrafter-0.1.3/commitcrafter/gpt_integration.py
--rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.3/commitcrafter/prompt.txt
--rw-r--r--   0        0        0      444 2024-04-19 15:12:14.838943 commitcrafter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 commitcrafter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 12:44:56.515352 commitcrafter-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 08:49:42.134232 commitcrafter-0.1.4/commitcrafter/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-19 15:24:21.810829 commitcrafter-0.1.4/commitcrafter/cli.py
+-rw-r--r--   0        0        0     1691 2024-04-19 15:23:24.364456 commitcrafter-0.1.4/commitcrafter/commitcrafter.py
+-rw-r--r--   0        0        0       42 2024-04-19 14:52:43.909465 commitcrafter-0.1.4/commitcrafter/exceptions.py
+-rw-r--r--   0        0        0      544 2024-04-19 14:23:56.857977 commitcrafter-0.1.4/commitcrafter/git_tools.py
+-rw-r--r--   0        0        0     1010 2024-04-19 14:55:53.329167 commitcrafter-0.1.4/commitcrafter/gpt_integration.py
+-rw-r--r--   0        0        0     1670 2024-04-19 09:24:12.850668 commitcrafter-0.1.4/commitcrafter/prompt.txt
+-rw-r--r--   0        0        0      444 2024-04-19 15:25:01.148243 commitcrafter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 commitcrafter-0.1.4/PKG-INFO
```

### Comparing `commitcrafter-0.1.3/commitcrafter/commitcrafter.py` & `commitcrafter-0.1.4/commitcrafter/commitcrafter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         Get the latest diff from the git repository at the given path.
         Args:
         repo_path (str): The path to the git repository.
         compare_to (str): The commit to compare the latest commit to.
         """
         try:
             repo = Repo(self.path, search_parent_directories=True)
-        except InvalidGitRepositoryError:
-            raise ValueError(f" :x: No git repository found at {self.path} :x:")
+        except InvalidGitRepositoryError as e:
+            raise e
         hcommit = repo.head.commit
         diff = hcommit.diff(self.compare_to, create_patch=True)
         diff_text = "".join([d.diff.decode() if d.diff else "" for d in diff])
         return diff_text
 
     def generate(self) -> list[str] | str:
         """
```

### Comparing `commitcrafter-0.1.3/commitcrafter/git_tools.py` & `commitcrafter-0.1.4/commitcrafter/git_tools.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.3/commitcrafter/gpt_integration.py` & `commitcrafter-0.1.4/commitcrafter/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.3/commitcrafter/prompt.txt` & `commitcrafter-0.1.4/commitcrafter/prompt.txt`

 * *Files identical despite different names*

### Comparing `commitcrafter-0.1.3/PKG-INFO` & `commitcrafter-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcrafter
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: mpruvot
 Author-email: marius.pruvot@outlook.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
```


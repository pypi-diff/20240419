# Comparing `tmp/pyaction-0.5.6.tar.gz` & `tmp/pyaction-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.5.6.tar", last modified: Wed Apr 17 19:31:41 2024, max compression
+gzip compressed data, was "pyaction-0.5.7.tar", last modified: Fri Apr 19 14:54:07 2024, max compression
```

## Comparing `pyaction-0.5.6.tar` & `pyaction-0.5.7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 19:31:34.000000 pyaction-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 19:31:34.000000 pyaction-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-17 19:31:41.917925 pyaction-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 19:31:34.000000 pyaction-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.913925 pyaction-0.5.6/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/issues/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.913925 pyaction-0.5.6/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:31:41.917925 pyaction-0.5.6/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 19:31:41.000000 pyaction-0.5.6/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-17 19:31:34.000000 pyaction-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:31:41.917925 pyaction-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.970106 pyaction-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 14:54:03.000000 pyaction-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 14:54:03.000000 pyaction-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 14:54:07.970106 pyaction-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-19 14:54:03.000000 pyaction-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.962106 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.970106 pyaction-0.5.7/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:54:07.970106 pyaction-0.5.7/setup.cfg
```

### Comparing `pyaction-0.5.6/LICENSE` & `pyaction-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.6/PKG-INFO` & `pyaction-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.6
+Version: 0.5.7
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.5.6/README.md` & `pyaction-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.6/pyaction/cli.py` & `pyaction-0.5.7/pyaction/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import os
 import subprocess
 
 import click
 from copier import run_copy
 
 from pyaction import __version__
-
-TEMPLATE_PATH = os.path.join(os.path.dirname(__file__), "template")
+from pyaction.consts import TEMPLATE_PATH, PROJECT_NAME
 
 
 @click.version_option(
     __version__,
-    prog_name="PyAction",
-    message="%(prog)s ~ version %(version)s",
+    prog_name=PROJECT_NAME,
+    message="%(prog)s - v%(version)s",
 )
 @click.group()
 def cli():
+    """Create GitHub Actions Using Python"""
     pass
 
 
 @cli.command("init", help="creates a basic action template (recommended for starting)")
 @click.argument("path", default=".")
 def init(path: str = ".") -> None:
     run_copy(TEMPLATE_PATH, path)
 
 
 @cli.command("run", help="uses .env to run the action locally")
 def run() -> None:
-    try:
-        subprocess.check_call(
-            "env $(cat .env | xargs) python main.py",
-            shell=True,
-            stderr=subprocess.DEVNULL,
-        )
-    except subprocess.CalledProcessError:
-        click.echo(
-            "Make sure the `.env` file is properly configured based on `action.yml`.",
-            err=True,
+    if not os.path.isfile(".env"):
+        raise FileNotFoundError(
+            "Make sure you have the `.env` file inside the root path of your action directory."
         )
+
+    subprocess.check_call("env $(cat .env | xargs) python main.py", shell=True)
```

### Comparing `pyaction-0.5.6/pyaction/io.py` & `pyaction-0.5.7/pyaction/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import os
 from typing import Dict
 
+from pyaction.consts import GITHUB_OUTPUT
 from pyaction.exceptions import WorkflowParameterNotFound
 
-BUFFER_PATH = os.environ.get("GITHUB_OUTPUT", os.devnull)
-
 
 def write(context: Dict[str, str]) -> None:
-    """writes the key(s) (as variables) and value(s) (as values) to the output buffer
+    """writes the key(s) (as variables) and value(s) (as values) to the output env variable
 
     Args:
         context: variables and values
 
     Examples:
         In your project, use this function like:
 
         >>> write({"name": "John", "age": 20, ...})
 
         `name` will be the variable name and `John` is the value.
     """
 
-    with open(BUFFER_PATH, "a") as _buffer:
+    with open(GITHUB_OUTPUT, "a") as _env:
         for var, val in context.items():
-            _buffer.write(f"{var}={val}\r\n")
+            _env.write(f"{var}={val}\r\n")
 
 
 def read(param: str) -> str | int | bool | None:
     """reads a parameter from the inputs
 
     Args:
         param (str): parameter name
 
     Returns:
         str | int | bool: value of `param`
     """
 
     prefix = "INPUT_"
+    var_name = prefix + param.upper()
 
     try:
-        value = os.environ[prefix + param.upper()]
+        value = os.environ[var_name]
     except KeyError:
         raise WorkflowParameterNotFound(
-            f"Couldn't read the `{param}` input parameter from your pipeline. "
+            f"Couldn't read the `{var_name}` input parameter from your pipeline. "
             "Make sure it's declared properly."
         )
 
     return value
```

### Comparing `pyaction-0.5.6/pyaction/issues/connector.py` & `pyaction-0.5.7/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.6/pyaction/template/copier.yml` & `pyaction-0.5.7/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.6/pyaction.egg-info/PKG-INFO` & `pyaction-0.5.7/pyaction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.6
+Version: 0.5.7
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.5.6/pyaction.egg-info/SOURCES.txt` & `pyaction-0.5.7/pyaction.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 pyaction/__init__.py
 pyaction/auth.py
 pyaction/cli.py
+pyaction/consts.py
 pyaction/exceptions.py
 pyaction/io.py
 pyaction.egg-info/PKG-INFO
 pyaction.egg-info/SOURCES.txt
 pyaction.egg-info/dependency_links.txt
 pyaction.egg-info/entry_points.txt
 pyaction.egg-info/requires.txt
```

### Comparing `pyaction-0.5.6/pyproject.toml` & `pyaction-0.5.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.5.6"
+version = "0.5.7"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
     "pygithub >= 2.3.0",
@@ -35,15 +35,15 @@
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
 [tool.bumpversion]
-current_version = "0.5.6"
+current_version = "0.5.7"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```


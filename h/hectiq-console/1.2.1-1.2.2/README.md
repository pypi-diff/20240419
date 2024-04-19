# Comparing `tmp/hectiq_console-1.2.1.tar.gz` & `tmp/hectiq_console-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-9_9n33pn/hectiq_console-1.2.1.tar", last modified: Wed Apr 17 13:24:41 2024, max compression
+gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-2lq6l6d3/hectiq_console-1.2.2.tar", last modified: Fri Apr 19 13:06:35 2024, max compression
```

## Comparing `hectiq_console-1.2.1.tar` & `hectiq_console-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/starlette/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/batch_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:24:33.000000 hectiq_console-1.2.1/hectiq_console.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/starlette/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/batch_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:28.000000 hectiq_console-1.2.2/hectiq_console.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/setup.py
```

### Comparing `hectiq_console-1.2.1/LICENSE` & `hectiq_console-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/PKG-INFO` & `hectiq_console-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq_console
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.1/README.md` & `hectiq_console-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console/cli/__init__.py` & `hectiq_console-1.2.2/hectiq_console/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 import logging
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 
 @click.group()
 def base():
     pass
 
-
 @base.command("version")
 def version():
     from hectiq_console import __version__, __path__
     click.echo(f"Version: {__version__}")
     click.echo(f"Located: {__path__}")
 
-
 @base.command("download-model", help="Download a model from the Hectiq API.")
 @click.option("--name", "-n", type=click.STRING, help="Name of the model.")
 @click.option("--version", "-v", type=click.STRING, help="Version of the model.")
 @click.option("--organization", "-o", type=click.STRING, help="Organization to download the model from.")
 @click.option("--savepath", "-s", type=click.Path(), help="Path to save the model.", default=".")
 def download_model(name:str, version: str, savepath: str, organization: str):
```

### Comparing `hectiq_console-1.2.1/hectiq_console/cli/auth.py` & `hectiq_console-1.2.2/hectiq_console/cli/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,35 @@
 
 
 @click.group()
 def auth_group():
     pass
 
 @auth_group.command("authenticate")
-@click.option("--replace", is_flag=True, default=False, help="If the key already exists, replace it.")
-def cli_authenticate(replace: bool):
+@click.option("--replace", 
+              is_flag=True, 
+              default=False, help="If the key already exists, replace it.")
+@click.option("--generate", '-g', 'only_generate', 
+              is_flag=True, 
+              default=False, 
+              help="If True, the key is only generated and not saved on your computer. Use this option if you want to use the key on another device.")
+def cli_authenticate(replace: bool, only_generate: bool):
     """Authenticate to the Hectiq Console."""
     from hectiq_console.functional import authenticate
     from hectiq_console import CONSOLE_APP_URL
     from pathlib import Path
     import requests
     import os
     import toml
+
+    if only_generate:
+        click.secho("🚨 Mode is set to generate only. The key will not be saved on your computer.", fg="cyan")
     is_logged = authenticate()
     
-    if is_logged:
+    if is_logged and not only_generate:
         # Ask if the user wants to add a new key
         click.secho("You are already logged in.", fg="green")
         should_continue = click.prompt("Do you still want to continue and create a new API key?",
                                         default="y", 
                                         show_default=True, 
                                         type=click.Choice(["y", "n"]))
         if should_continue=="n":
@@ -52,41 +61,48 @@
     click.echo("Select an organization:")
     for i, org in enumerate(user.get("organizations")):
         click.echo(f"[{i}] - {org.get('name')}")
     index = click.prompt("Enter the index of the organization:", 
                  type=click.Choice([str(i) for i in range(len(user.get("organizations")))]))
     organization_slug = user.get("organizations")[int(index)]["slug"]
 
-    path = os.getenv("HECTIQ_CONSOLE_CREDENTIALS_FILE", 
-                         os.path.join(Path.home(),".hectiq-console", "credentials.toml"))
-    
-    os.makedirs(os.path.dirname(path), exist_ok=True)
-
-    # Load the existing keys
-    if os.path.exists(path):
-        with open(path, "r") as f:
-            current_auth_data = toml.load(f)
-    else:
-        current_auth_data = {}
-
-    should_replace = True
-    if organization_slug in current_auth_data:
-        if not replace:
-            click.secho(f"⚠️ A key for {organization_slug} already exists. Use --replace to replace it.", err=True, fg="red")
-            return
+    if not only_generate:
+        path = os.getenv("HECTIQ_CONSOLE_CREDENTIALS_FILE", 
+                            os.path.join(Path.home(),".hectiq-console", "credentials.toml"))
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+
+        # Load the existing keys
+        if os.path.exists(path):
+            with open(path, "r") as f:
+                current_auth_data = toml.load(f)
         else:
-            should_replace = True
+            current_auth_data = {}
+
+        should_replace = True
+        if organization_slug in current_auth_data:
+            if not replace:
+                click.secho(f"⚠️ A key for {organization_slug} already exists. Use --replace to replace it.", err=True, fg="red")
+                return
+            else:
+                should_replace = True
 
     # Get the API key
     res = requests.post(f"{CONSOLE_APP_URL}/app/auth/api-keys", 
                   json={"email": email, "password": password, "name": name, "organization": organization_slug})
     if res.status_code!=200:
         click.echo("Authentication failed.")
         return
     api_key = res.json()
+
+    if only_generate:
+        click.secho(f"Your API key:")
+        click.secho(f"{api_key['value']}", bold=True)
+        click.secho(f"⚠️ The value above is your API key for {organization_slug}. It won't be show again and the key has not been saved on your computer.", bg="red", fg="white", bold=True)
+        click.echo(f"Use HECTIQ_CONSOLE_API_KEY to authenticate or visit https://hectiq-console.surge.sh/authenticate.html to learn how to use the key.")
+        return
     
     if should_replace:
         api_key["email"] = email
         current_auth_data[organization_slug] = api_key
         with open(path, "w") as f:
             toml.dump(current_auth_data, f)
         click.echo(f"The API key for {organization_slug} has been replaced at {path}.")
@@ -97,8 +113,8 @@
             data = {}
             api_key["email"] = email
             data[organization_slug] = api_key
             toml.dump(data, f)
             f.write("\n")
 
         click.echo(f"A new API key has been added to {path}.")
-    click.secho("You are now logged in.", fg="green")
+    click.secho("You are now logged in.", fg="green")
```

### Comparing `hectiq_console-1.2.1/hectiq_console/functional.py` & `hectiq_console-1.2.2/hectiq_console/functional.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console/starlette/middleware.py` & `hectiq_console-1.2.2/hectiq_console/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console/upload.py` & `hectiq_console-1.2.2/hectiq_console/upload.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console/utils/batch_fetch.py` & `hectiq_console-1.2.2/hectiq_console/utils/batch_fetch.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console/utils/log_handler.py` & `hectiq_console-1.2.2/hectiq_console/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/hectiq_console.egg-info/PKG-INFO` & `hectiq_console-1.2.2/hectiq_console.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq-console
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.1/hectiq_console.egg-info/SOURCES.txt` & `hectiq_console-1.2.2/hectiq_console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.1/setup.py` & `hectiq_console-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
     "requests",
     "toml",
```


# Comparing `tmp/integrate-ai-9.8.0.tar.gz` & `tmp/integrate-ai-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integrate-ai-9.8.0.tar", last modified: Tue Mar 19 19:10:05 2024, max compression
+gzip compressed data, was "integrate-ai-9.9.0.tar", last modified: Fri Apr 19 16:56:37 2024, max compression
```

## Comparing `integrate-ai-9.8.0.tar` & `integrate-ai-9.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.922165 integrate-ai-9.8.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-03-19 19:10:05.922165 integrate-ai-9.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/backend_shim.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.918165 integrate-ai-9.8.0/integrate_ai/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21146 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/sdk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.922165 integrate-ai-9.8.0/integrate_ai/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/docker_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/error_handling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/path_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/rest_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai/utils/typer_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-19 19:10:05.922165 integrate-ai-9.8.0/integrate_ai.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/integrate_ai.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-19 19:10:05.922165 integrate-ai-9.8.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2024-03-19 19:10:05.000000 integrate-ai-9.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/backend_shim.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.365031 integrate-ai-9.9.0/integrate_ai/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21141 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/sdk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/integrate_ai/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/docker_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/error_handling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/path_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/rest_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/typer_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.365031 integrate-ai-9.9.0/integrate_ai.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/setup.py
```

### Comparing `integrate-ai-9.8.0/PKG-INFO` & `integrate-ai-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.8.0
+Version: 9.9.0
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.8.0/backend_shim.py` & `integrate-ai-9.9.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/cli.py` & `integrate-ai-9.9.0/integrate_ai/cli.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/client.py` & `integrate-ai-9.9.0/integrate_ai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
             raise typer.Exit(1)
         token = input("Please provide your IAI token: ")
         # sanitize token
         token = "".join(filter(lambda c: c.isalnum() or c in (".", "-", "_"), token))
 
     # start progress bar
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
-
         # connect to docker
         p = progress.add_task(description="Connecting to docker...", total=1)
         docker_client = DockerClient(token, gpu=GPU)
         progress.update(task_id=p, completed=True)
 
         # check if any existing docker images on system
         p = progress.add_task(description="Searching for existing client images...", total=1)
@@ -62,26 +61,24 @@
         latest_available_version = docker_client.get_latest_available_version()
         progress.update(task_id=p, completed=True)
 
     version_to_pull = latest_available_version if version == "latest" else version
     if len(current_images) == 0:
         rprint("No existing client version found on system.")
     else:
-
         # if images exist on system, check the latest version that is installed
         latest_version = docker_client.get_latest_version_of_image(current_images) or "`latest`"
         if not GPU and "-cpu" not in version_to_pull:
             version_to_pull += "-cpu"
 
         rprint(
             f"Latest version of docker image found on system is {latest_version}. Most recent version is {latest_available_version}."
         )
 
         if latest_version == version_to_pull:
-
             # no point installing if they already have the latest image
             rprint("The requested version of the client image is already on your system. Exiting...")
             raise typer.Exit(0)
         else:
             prompt_msg = f"A newer version {latest_available_version} was found. The current version of the client image will be deleted from your system. Do you want to proceed?"
             # confirm that they are ok with deleting current client images on system
             prompt_msg = "Installing this client image will delete any current version of this image on your system. Do you want to proceed?"
@@ -521,15 +518,15 @@
         exec_id = container.client.api.exec_create(container.id, cmd, stdout=verbose, environment=environment)
         response = container.client.api.exec_start(
             exec_id,
             stream=True,
             demux=True,
         )
         if response:
-            for (output, error) in response:  # type: ignore
+            for output, error in response:  # type: ignore
                 if error:
                     progress.console.print(error.decode("utf-8"))
                 else:
                     progress.console.print(output.decode("utf-8"))
 
         progress.update(task_id=task, completed=True)
```

### Comparing `integrate-ai-9.8.0/integrate_ai/main.py` & `integrate-ai-9.9.0/integrate_ai/main.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/sdk.py` & `integrate-ai-9.9.0/integrate_ai/sdk.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/server.py` & `integrate-ai-9.9.0/integrate_ai/server.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/docker_client.py` & `integrate-ai-9.9.0/integrate_ai/utils/docker_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/error_handling.py` & `integrate-ai-9.9.0/integrate_ai/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/logger.py` & `integrate-ai-9.9.0/integrate_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/path_utils.py` & `integrate-ai-9.9.0/integrate_ai/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/rest_client.py` & `integrate-ai-9.9.0/integrate_ai/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai/utils/typer_utils.py` & `integrate-ai-9.9.0/integrate_ai/utils/typer_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/integrate_ai.egg-info/PKG-INFO` & `integrate-ai-9.9.0/integrate_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.8.0
+Version: 9.9.0
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.8.0/integrate_ai.egg-info/SOURCES.txt` & `integrate-ai-9.9.0/integrate_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.8.0/setup.py` & `integrate-ai-9.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
     'package_data': {
     },
     'packages': (
         'integrate_ai',
         'integrate_ai.utils',
     ),
     'python_requires': '>=3.7.5',
-    'version': '9.8.0',
+    'version': '9.9.0',
 })
```


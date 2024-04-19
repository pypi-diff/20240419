# Comparing `tmp/sinaraml-2024.3.20.tar.gz` & `tmp/sinaraml-2024.4.19.tar.gz`

## Comparing `sinaraml-2024.3.20.tar` & `sinaraml-2024.4.19.tar`

### file list

```diff
@@ -1,16 +1,9 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/__init__.py
--rwxr-xr-x   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/_version.py
--rwxr-xr-x   0        0        0     5487 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/common_utils.py
--rwxr-xr-x   0        0        0     2507 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/config_manager.py
--rwxr-xr-x   0        0        0     8302 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/docker_utils.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/infra.py
--rwxr-xr-x   0        0        0    10170 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/model.py
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/platform.py
--rwxr-xr-x   0        0        0      788 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/plugin_loader.py
--rwxr-xr-x   0        0        0    31033 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/server.py
--rwxr-xr-x   0        0        0     4420 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/sinaraml/sinaraml.py
--rwxr-xr-x   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/LICENSE
--rwxr-xr-x   0        0        0     3336 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/README.md
--rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/pyproject.toml
--rw-r--r--   0        0        0    17285 2020-02-02 00:00:00.000000 sinaraml-2024.3.20/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/_version.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/org_manager.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/sinaraml.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/pyproject.toml
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/PKG-INFO
```

### Comparing `sinaraml-2024.3.20/sinaraml/sinaraml.py` & `sinaraml-2024.4.19/sinaraml/sinaraml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
 import platform
 import sys
-from .server import SinaraServer
-from .model import SinaraModel
-from .common_utils import get_cli_version
-
-from .plugin_loader import SinaraPluginLoader
-from docker import errors
-
-def init_cli(root_parser, subject_parser):
-    overloaded_modules = []
-    for infra_plugin in SinaraPluginLoader.get_infra_plugins():
-        module = SinaraPluginLoader.get_infra_plugin(infra_plugin)
-        for plugin_class in module.get_plugin_classes():
-            for base in plugin_class.__bases__:
-                overloaded_modules.append(base.__name__)
-            plugin_class.add_command_handlers(subject_parser)
-
-    if not 'SinaraServer' in overloaded_modules:
-        SinaraServer.add_command_handlers(root_parser, subject_parser)
-    if not 'SinaraModel' in overloaded_modules:
-        SinaraModel.add_command_handlers(subject_parser)
+from dataclasses import dataclass
+from .org_manager import SinaraOrgManager
+
+
+@dataclass
+class Gitref:
+    gitref: str
+
+def check_any_cli_exists():
+    if not SinaraOrgManager.check_last_update():
+        args = Gitref(gitref = "https://github.com/4-DS/mlops_organization.git")
+        SinaraOrgManager.install_from_git(args)
+    
+def init_cli(root_parser, subject_parser, platform=None):
+
+    root_parser.subjects = []
+
+    SinaraOrgManager.add_command_handlers(root_parser, subject_parser)
+
+    org_name = 'personal'
+    if platform and '_' in platform:
+        org_name = platform.split('_')[0]
+    org = SinaraOrgManager.load_organization(org_name)
+    if org:
+        org.add_command_handlers(root_parser, subject_parser)
+    
+def update_orgs():
+    for org in SinaraOrgManager.get_orgs():
+        from collections import namedtuple
+        Args = namedtuple('Args', ['name', 'internal'])
+        args = Args(name=org["name"], internal=True)
+        SinaraOrgManager.update_org(args)
+
 
 def setup_logging(use_vebose=False):
     logging.basicConfig(format="%(levelname)s: %(message)s")
     if use_vebose:
         logging.getLogger().setLevel(logging.DEBUG)
 
 def platform_is_supported():
@@ -39,28 +52,40 @@
     exit_code = -1
 
     if not platform_is_supported():
         print(f'Your OS "{platform.system()}" is not supported. Check https://github.com/4-DS/sinara-tutorials/wiki/SinaraML-Known-issues#error-message-your-os-is-not-supported')
         return exit_code
 
     # add root parser and root subcommand parser (subject)
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(add_help=True)
     subject_subparser = parser.add_subparsers(title='subject', dest='subject', help=f"subject to use")
     parser.add_argument('-v', '--verbose', action='store_true', help="display verbose logs")
-    parser.add_argument('--version', action='version', version=f"SinaraML CLI {get_cli_version()}")
+    parser.add_argument('-p', '--platform', help="choose SinaraML platform")
+    #parser.add_argument('--version', action='version', version=f"SinaraML CLI {get_cli_version()}")
 
+    sinara_platform = None
+    for i in range(1, len(sys.argv)):
+        a = sys.argv[i]
+        if a.startswith('--platform'):
+            sinara_platform = a.split('=')[1] if "=" in a else sys.argv[i+1]
+            break
+    
+    if not sinara_platform:
+        check_any_cli_exists()
+    update_orgs()
     # each cli plugin adds and manages subcommand handlers (starting from subject handler) to root parser
-    init_cli(parser, subject_subparser)
+    init_cli(parser, subject_subparser, platform=sinara_platform)
+    
 
     # parse the command line and get all arguments
     args = parser.parse_known_args()[0]
 
     # Setup logs format and verbosity level
     setup_logging(args.verbose)
-    
+
     # display help if required arguments are missing
     if not args.subject:
         parser.print_help()
     elif not args.action:
         subparsers_actions = [
             action for action in parser._actions 
             if isinstance(action, argparse._SubParsersAction)]
@@ -71,31 +96,30 @@
 
     # call appropriate handler for the whole command line from a cli plugin if installed
     if hasattr(args, 'func'):
         try:
             args.func(args)
             exit_code = 0
         except Exception as e:
-            from requests.exceptions import ConnectionError
-
-            if isinstance(e.__cause__, ConnectionError):
+            #from requests.exceptions import ConnectionError
+            if e.__cause__.__class__.__name__ == "ConnectionError":
                 logging.error("Docker daemon is not available, make sure docker is running and you have permissions to access it. Run CLI with sinara --verbose flag to see details")
 
-            elif isinstance(e, errors.APIError):
+            elif e.__class__.__name__ == "APIError":
                 if e.is_client_error():
                     if e.status_code == 404:
                         logging.error(f"Docker image or container not found. Run CLI with sinara --verbose flag to see details")
                     elif e.status_code == 401 or e.status_code == 403:
                         logging.error(f"Make sure you have permissions to access requested resource. Run CLI with sinara --verbose flag to see details")                        
                     else:
                         logging.error("Docker client has failed, Run CLI with sinara --verbose flag to see details")
                 else:
                     logging.error("Docker daemon failed, Run CLI with sinara --verbose flag to see details")
 
-            elif isinstance(e, errors.DockerException):
+            elif e.__class__.__name__ == "DockerException":
                 logging.error("Docker client has failed, Run CLI with sinara --verbose flag to see details")
 
             logging.error(e, exc_info=args.verbose)
                 
     return exit_code
 
 if __name__ == "__main__":
```

### Comparing `sinaraml-2024.3.20/.gitignore` & `sinaraml-2024.4.19/.gitignore`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.3.20/pyproject.toml` & `sinaraml-2024.4.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 ]
 description = "SinaraML"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["cli", "sinaraml"]
 license = { file="LICENSE" }
 classifiers = [
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 dependencies = [
-    "docker>=4.3.1",
     "tqdm",
     "requests",
     'importlib-metadata; python_version>="3.6"'
 ]
 dynamic = ["version"]
 
 [project.urls]
```


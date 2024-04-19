# Comparing `tmp/envoy.base.utils-0.5.0.tar.gz` & `tmp/envoy.base.utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.5.0.tar", last modified: Fri Oct 27 09:15:57 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.5.1.tar", last modified: Fri Apr 19 10:15:43 2024, max compression
```

## Comparing `envoy.base.utils-0.5.0.tar` & `envoy.base.utils-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.137051 envoy.base.utils-0.5.0/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.137051 envoy.base.utils-0.5.0/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-27 09:15:57.000000 envoy.base.utils-0.5.0/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 09:15:57.141051 envoy.base.utils-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-10-27 09:15:56.000000 envoy.base.utils-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.661622 envoy.base.utils-0.5.1/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.661622 envoy.base.utils-0.5.1/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:43.661622 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:15:43.665622 envoy.base.utils-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-19 10:15:43.000000 envoy.base.utils-0.5.1/setup.py
```

### Comparing `envoy.base.utils-0.5.0/backend_shim.py` & `envoy.base.utils-0.5.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/__init__.py` & `envoy.base.utils-0.5.1/envoy/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from envoy.base.utils import interface, typing
 
 
 INVENTORY_PATH_GLOB = "docs/inventories/v*.*/objects.inv"
 INVENTORY_PATH_FMT = "docs/inventories/v{minor_version}/objects.inv"
 INVENTORY_VERSIONS_PATH = "docs/versions.yaml"
 INVENTORY_URL_FMT = (
-    "https://www.envoyproxy.io/docs/envoy/v{version}/objects.inv")
+    "https://github.com/envoyproxy/archive/raw/main/"
+    "docs/envoy/v{version}/objects.inv")
 
 
 @abstracts.implementer(interface.IInventories)
 class AInventories(metaclass=abstracts.Abstraction):
 
     def __init__(self, project: interface.IProject) -> None:
         self.project = project
```

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.5.1/envoy/base/utils/abstract/project/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.5.1/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/data_env.py` & `envoy.base.utils-0.5.1/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/interface.py` & `envoy.base.utils-0.5.1/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.5.1/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.5.1/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/project.py` & `envoy.base.utils-0.5.1/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.5.1/envoy/base/utils/project_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/tar.py` & `envoy.base.utils-0.5.1/envoy/base/utils/tar.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/typing.py` & `envoy.base.utils-0.5.1/envoy/base/utils/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/utils.py` & `envoy.base.utils-0.5.1/envoy/base/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,24 +44,28 @@
     with tempfile.TemporaryDirectory() as tmpdir:
         tmprc = os.path.join(tmpdir, ".coveragerc")
         with open(tmprc, "w") as f:
             parser.write(f)
         yield tmprc
 
 
-def from_json(path: Union[pathlib.Path, str], type: Type = None) -> Any:
+def from_json(
+        path: Union[pathlib.Path, str],
+        type: Optional[Type] = None) -> Any:
     """Returns the loaded python object from a JSON file given by `path`"""
     data = json.loads(pathlib.Path(path).read_text())
     return (
         data
         if type is None
         else typed(type, data))
 
 
-def from_yaml(path: Union[pathlib.Path, str], type: Type = None) -> Any:
+def from_yaml(
+        path: Union[pathlib.Path, str],
+        type: Optional[Type] = None) -> Any:
     """Returns the loaded python object from a yaml file given by `path`"""
     data = yaml.safe_load(pathlib.Path(path).read_text())
     return (
         data
         if type is None
         else typed(type, data))
```

### Comparing `envoy.base.utils-0.5.0/envoy/base/utils/yaml.py` & `envoy.base.utils-0.5.1/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.5.1/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.5.0/setup.py` & `envoy.base.utils-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             'envoy.project=envoy.base.utils:project_cmd',
             'envoy.project_data=envoy.base.utils:project_data_cmd',
         ],
     },
     'install_requires': (
         'abstracts>=0.0.12',
         'aio.api.github>=0.2.5',
-        'aio.core>=0.10.0',
+        'aio.core>=0.10.1',
         'aio.run.runner>=0.3.3',
         'aiohttp>=3.8.1',
         'frozendict',
         'jinja2',
         'orjson',
         'packaging>=23.0',
         'protobuf',
@@ -53,9 +53,9 @@
     'packages': (
         'envoy.base.utils',
         'envoy.base.utils.abstract',
         'envoy.base.utils.abstract.project',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.base.utils',
-    'version': '0.5.0',
+    'version': '0.5.1',
 })
```


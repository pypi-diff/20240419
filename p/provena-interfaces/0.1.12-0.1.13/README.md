# Comparing `tmp/provena-interfaces-0.1.12.tar.gz` & `tmp/provena-interfaces-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provena-interfaces-0.1.12.tar", last modified: Fri Apr 19 03:56:16 2024, max compression
+gzip compressed data, was "provena-interfaces-0.1.13.tar", last modified: Fri Apr 19 04:18:58 2024, max compression
```

## Comparing `provena-interfaces-0.1.12.tar` & `provena-interfaces-0.1.13.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/ProvenaInterfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/APIResponses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/AsyncJobAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/AsyncJobModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/AuthAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/DataStoreAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/HandleAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/HandleModels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/ProvenanceAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/ProvenanceModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/RegistryAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    64215 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/RegistryModels.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/SearchAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/SharedTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/ProvenaInterfaces/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/helpers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/ProvenaInterfaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/provena_interfaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 03:56:16.000000 provena-interfaces-0.1.12/provena_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 03:56:16.000000 provena-interfaces-0.1.12/provena_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:56:16.000000 provena-interfaces-0.1.12/provena_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 03:56:16.000000 provena-interfaces-0.1.12/provena_interfaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 03:56:16.000000 provena-interfaces-0.1.12/provena_interfaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:56:16.848954 provena-interfaces-0.1.12/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/tests/test_registry_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-19 03:55:44.000000 provena-interfaces-0.1.12/tests/test_registry_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:58.167419 provena-interfaces-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 04:18:58.167419 provena-interfaces-0.1.13/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:58.163419 provena-interfaces-0.1.13/ProvenaInterfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/APIResponses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/AsyncJobAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/AsyncJobModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/AuthAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/DataStoreAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/HandleAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/HandleModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/ProvenanceAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/ProvenanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/RegistryAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64215 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/RegistryModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/SearchAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/SharedTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:58.163419 provena-interfaces-0.1.13/ProvenaInterfaces/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/helpers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/ProvenaInterfaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:58.163419 provena-interfaces-0.1.13/provena_interfaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 04:18:58.000000 provena-interfaces-0.1.13/provena_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 04:18:58.000000 provena-interfaces-0.1.13/provena_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:18:58.000000 provena-interfaces-0.1.13/provena_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 04:18:58.000000 provena-interfaces-0.1.13/provena_interfaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 04:18:58.000000 provena-interfaces-0.1.13/provena_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:18:58.167419 provena-interfaces-0.1.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:18:58.163419 provena-interfaces-0.1.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/tests/test_registry_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-19 04:18:22.000000 provena-interfaces-0.1.13/tests/test_registry_models.py
```

### Comparing `provena-interfaces-0.1.12/PKG-INFO` & `provena-interfaces-0.1.13/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provena-interfaces
-Version: 0.1.12
+Version: 0.1.13
 Summary: Interfaces for Provena Application (see https://provena.io)
 Home-page: https://provena.io
 Maintainer-email: rrap-mds-is-support@csiro.au
 Description-Content-Type: text/markdown
 
 
 Provena-Interfaces is a Python package that provides interfaces for the Provena Application. It includes a set of interfaces that are used to interact with the Provena system. The interfaces are especially useful for parsing response payloads from the API, and for creating requests to the API. The interfaces will sit adjacent to (and be consumed by) a ProvenaClient library which is a work in progress.
```

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/AsyncJobAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/AsyncJobAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/AsyncJobModels.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/AsyncJobModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/AuthAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/AuthAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/DataStoreAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/DataStoreAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/HandleAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/HandleAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/ProvenanceAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/ProvenanceAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/ProvenanceModels.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/ProvenanceModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/RegistryAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/RegistryAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/RegistryModels.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/RegistryModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/SearchAPI.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/SearchAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/SharedTypes.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/SharedTypes.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/ProvenaInterfaces/helpers/types.py` & `provena-interfaces-0.1.13/ProvenaInterfaces/helpers/types.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/README.md` & `provena-interfaces-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/provena_interfaces.egg-info/PKG-INFO` & `provena-interfaces-0.1.13/provena_interfaces.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provena-interfaces
-Version: 0.1.12
+Version: 0.1.13
 Summary: Interfaces for Provena Application (see https://provena.io)
 Home-page: https://provena.io
 Maintainer-email: rrap-mds-is-support@csiro.au
 Description-Content-Type: text/markdown
 
 
 Provena-Interfaces is a Python package that provides interfaces for the Provena Application. It includes a set of interfaces that are used to interact with the Provena system. The interfaces are especially useful for parsing response payloads from the API, and for creating requests to the API. The interfaces will sit adjacent to (and be consumed by) a ProvenaClient library which is a work in progress.
```

### Comparing `provena-interfaces-0.1.12/provena_interfaces.egg-info/SOURCES.txt` & `provena-interfaces-0.1.13/provena_interfaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/setup.py` & `provena-interfaces-0.1.13/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from setuptools import setup, find_packages  # type: ignore
 import os
 from package_readme import long_description
 import re
 
 # 0.1.0 is the 'version' installs from this directory from other components in repo will use
-version = os.getenv('PACKAGE_VERSION', 'refs/tags/v0.1.0')
-
-if re.match(r'refs/tags/.*', version):
-    version = version.replace('refs/tags/', '')
-else:
-    raise ValueError("PACKAGE_VERSION environment variable is not set correctly. Expecting 'refs/tags/*'. Got " + version + " instead")
+version = os.getenv('TAG_NAME', 'v0.1.0')
 
 setup(
     name='provena-interfaces',
     # format acceptably as 'v0.0.1' or '0.0.1',
     version=version,
     description='Interfaces for Provena Application (see https://provena.io)',
     long_description=long_description,
```

### Comparing `provena-interfaces-0.1.12/tests/test_registry_api_models.py` & `provena-interfaces-0.1.13/tests/test_registry_api_models.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.12/tests/test_registry_models.py` & `provena-interfaces-0.1.13/tests/test_registry_models.py`

 * *Files identical despite different names*


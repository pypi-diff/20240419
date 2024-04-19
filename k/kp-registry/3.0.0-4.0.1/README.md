# Comparing `tmp/kp-registry-3.0.0.tar.gz` & `tmp/kp-registry-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kp-registry-3.0.0.tar", last modified: Mon Dec 19 17:03:19 2022, max compression
+gzip compressed data, was "kp-registry-4.0.1.tar", last modified: Fri Apr 19 16:54:14 2024, max compression
```

## Comparing `kp-registry-3.0.0.tar` & `kp-registry-4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:03:19.868407 kp-registry-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)      221 2022-12-19 17:03:19.868407 kp-registry-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      642 2022-12-19 17:03:14.000000 kp-registry-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:03:19.868407 kp-registry-3.0.0/kp_registry/
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-12-19 17:03:14.000000 kp-registry-3.0.0/kp_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10817 2022-12-19 17:03:14.000000 kp-registry-3.0.0/kp_registry/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:03:19.868407 kp-registry-3.0.0/kp_registry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      221 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      270 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-12-19 17:03:19.000000 kp-registry-3.0.0/kp_registry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-19 17:03:19.868407 kp-registry-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      449 2022-12-19 17:03:14.000000 kp-registry-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:54:14.806913 kp-registry-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 16:54:14.806913 kp-registry-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-19 16:54:12.000000 kp-registry-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:54:14.806913 kp-registry-4.0.1/kp_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 16:54:12.000000 kp-registry-4.0.1/kp_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-19 16:54:12.000000 kp-registry-4.0.1/kp_registry/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:54:14.806913 kp-registry-4.0.1/kp_registry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 16:54:14.000000 kp-registry-4.0.1/kp_registry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:54:14.806913 kp-registry-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-19 16:54:12.000000 kp-registry-4.0.1/setup.py
```

### Comparing `kp-registry-3.0.0/README.md` & `kp-registry-4.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 To install:
 ```bash
 pip install kp-registry
 ```
 
 KP Registry will also use an environment variable:
 ```
-KP_TRAPI_VERSION=1.3.0
+KP_TRAPI_VERSION=1.5.0
 ```
 
 ## Usage:
 ```python
 from kp_registry import Registry
 
 # Initialize the registry
```

### Comparing `kp-registry-3.0.0/kp_registry/main.py` & `kp-registry-4.0.1/kp_registry/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """KP registry."""
+
 import asyncio
 import httpx
 import json
 import logging
 import os
 import pydantic
 import re
@@ -201,15 +202,15 @@
                 LOGGER.warning(
                     "No x-trapi.version for %s (https://smart-api.info/registry?q=%s)",
                     title,
                     _id,
                 )
                 continue
             regex = re.compile("[0-9]\.[0-9]")
-            target_trapi_version = os.getenv("KP_TRAPI_VERSION", "1.3.0")
+            target_trapi_version = os.getenv("KP_TRAPI_VERSION", "1.5.0")
             trapi_version = regex.match(target_trapi_version)
             if not version.startswith(trapi_version.group() + "."):
                 LOGGER.info(
                     f"TRAPI version != {trapi_version.group()}.x for %s (https://smart-api.info/registry?q=%s)",
                     title,
                     _id,
                 )
@@ -261,16 +262,25 @@
                             "infores": infores,
                             "url": url,
                             "maturity": maturity,
                             "operations": operations,
                             "version": version,
                         }
                     )
-            except (KeyError):
+            except KeyError:
                 LOGGER.warning(
                     "No servers for %s (https://smart-api.info/registry?q=%s)",
                     title,
                     _id,
                 )
                 continue
 
         return endpoints
+
+
+async def main():
+    registry = Registry()
+    await registry.retrieve_kps()
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
```

